<!-- THIS FILE IS GENERATED VIA './update-remote.sh' -->

# Tags of `xwiki`

-	[`xwiki:14`](#xwiki14)
-	[`xwiki:14-mariadb-tomcat`](#xwiki14-mariadb-tomcat)
-	[`xwiki:14-mysql-tomcat`](#xwiki14-mysql-tomcat)
-	[`xwiki:14-postgres-tomcat`](#xwiki14-postgres-tomcat)
-	[`xwiki:14.10`](#xwiki1410)
-	[`xwiki:14.10-mariadb-tomcat`](#xwiki1410-mariadb-tomcat)
-	[`xwiki:14.10-mysql-tomcat`](#xwiki1410-mysql-tomcat)
-	[`xwiki:14.10-postgres-tomcat`](#xwiki1410-postgres-tomcat)
-	[`xwiki:14.10.5`](#xwiki14105)
-	[`xwiki:14.10.5-mariadb-tomcat`](#xwiki14105-mariadb-tomcat)
-	[`xwiki:14.10.5-mysql-tomcat`](#xwiki14105-mysql-tomcat)
-	[`xwiki:14.10.5-postgres-tomcat`](#xwiki14105-postgres-tomcat)
-	[`xwiki:15`](#xwiki15)
-	[`xwiki:15-mariadb-tomcat`](#xwiki15-mariadb-tomcat)
-	[`xwiki:15-mysql-tomcat`](#xwiki15-mysql-tomcat)
-	[`xwiki:15-postgres-tomcat`](#xwiki15-postgres-tomcat)
-	[`xwiki:15.0`](#xwiki150)
-	[`xwiki:15.0-mariadb-tomcat`](#xwiki150-mariadb-tomcat)
-	[`xwiki:15.0-mysql-tomcat`](#xwiki150-mysql-tomcat)
-	[`xwiki:15.0-postgres-tomcat`](#xwiki150-postgres-tomcat)
-	[`xwiki:15.0.0`](#xwiki1500)
-	[`xwiki:15.0.0-mariadb-tomcat`](#xwiki1500-mariadb-tomcat)
-	[`xwiki:15.0.0-mysql-tomcat`](#xwiki1500-mysql-tomcat)
-	[`xwiki:15.0.0-postgres-tomcat`](#xwiki1500-postgres-tomcat)
-	[`xwiki:latest`](#xwikilatest)
-	[`xwiki:lts`](#xwikilts)
-	[`xwiki:lts-mariadb`](#xwikilts-mariadb)
-	[`xwiki:lts-mariadb-tomcat`](#xwikilts-mariadb-tomcat)
-	[`xwiki:lts-mysql`](#xwikilts-mysql)
-	[`xwiki:lts-mysql-tomcat`](#xwikilts-mysql-tomcat)
-	[`xwiki:lts-postgres`](#xwikilts-postgres)
-	[`xwiki:lts-postgres-tomcat`](#xwikilts-postgres-tomcat)
-	[`xwiki:mariadb-tomcat`](#xwikimariadb-tomcat)
-	[`xwiki:mysql-tomcat`](#xwikimysql-tomcat)
-	[`xwiki:postgres-tomcat`](#xwikipostgres-tomcat)
-	[`xwiki:stable`](#xwikistable)
-	[`xwiki:stable-mariadb`](#xwikistable-mariadb)
-	[`xwiki:stable-mariadb-tomcat`](#xwikistable-mariadb-tomcat)
-	[`xwiki:stable-mysql`](#xwikistable-mysql)
-	[`xwiki:stable-mysql-tomcat`](#xwikistable-mysql-tomcat)
-	[`xwiki:stable-postgres`](#xwikistable-postgres)
-	[`xwiki:stable-postgres-tomcat`](#xwikistable-postgres-tomcat)

## `xwiki:14`

```console
$ docker pull xwiki@sha256:32e51c9775fda50082b0f02856f2af444a67284446679c9a3a13a78c02ec0c4b
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `xwiki:14` - linux; amd64

```console
$ docker pull xwiki@sha256:a2e996a399fc68cbccfe11eaeb0115a15314bd69f06c483fef3cba244fa07cbf
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **590.4 MB (590449604 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:6b73fd725d5c1dd8044289fdb0e76f973e7e1d4a64e1efc44428235a718b550a`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["xwiki"]`

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
# Wed, 02 Nov 2022 18:44:10 GMT
RUN apt-get update     && DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends tzdata curl wget ca-certificates fontconfig locales     && echo "en_US.UTF-8 UTF-8" >> /etc/locale.gen     && locale-gen en_US.UTF-8     && rm -rf /var/lib/apt/lists/*
# Fri, 04 Nov 2022 23:21:41 GMT
ENV JAVA_VERSION=jdk-11.0.17+8
# Fri, 04 Nov 2022 23:22:31 GMT
RUN set -eux;     ARCH="$(dpkg --print-architecture)";     case "${ARCH}" in        aarch64|arm64)          ESUM='bd6efe3290c8b5a42f695a55a26f3e3c9c284288574879d4b7089f31f5114177';          BINARY_URL='https://github.com/adoptium/temurin11-binaries/releases/download/jdk-11.0.17%2B8/OpenJDK11U-jre_aarch64_linux_hotspot_11.0.17_8.tar.gz';          ;;        armhf|arm)          ESUM='8cf113d3d7fa808895c8d2e41bb890af21c47e38c2460e0588147a4bb8fc658d';          BINARY_URL='https://github.com/adoptium/temurin11-binaries/releases/download/jdk-11.0.17%2B8/OpenJDK11U-jre_arm_linux_hotspot_11.0.17_8.tar.gz';          ;;        ppc64el|powerpc:common64)          ESUM='0ca3d806131ab5834c501f9c625bb0248cd528af361c704503348e9c9605bedf';          BINARY_URL='https://github.com/adoptium/temurin11-binaries/releases/download/jdk-11.0.17%2B8/OpenJDK11U-jre_ppc64le_linux_hotspot_11.0.17_8.tar.gz';          ;;        s390x|s390:64-bit)          ESUM='dd3b159a374086e65cb07c4ccb226c90f9c02ef929cba6f0b642171d7ed97fa4';          BINARY_URL='https://github.com/adoptium/temurin11-binaries/releases/download/jdk-11.0.17%2B8/OpenJDK11U-jre_s390x_linux_hotspot_11.0.17_8.tar.gz';          ;;        amd64|i386:x86-64)          ESUM='752616097e09d7f60a3ad8bd312f90eaf50ac72577e55df229fe6e8091148f79';          BINARY_URL='https://github.com/adoptium/temurin11-binaries/releases/download/jdk-11.0.17%2B8/OpenJDK11U-jre_x64_linux_hotspot_11.0.17_8.tar.gz';          ;;        *)          echo "Unsupported arch: ${ARCH}";          exit 1;          ;;     esac; 	  wget -O /tmp/openjdk.tar.gz ${BINARY_URL}; 	  echo "${ESUM} */tmp/openjdk.tar.gz" | sha256sum -c -; 	  mkdir -p "$JAVA_HOME"; 	  tar --extract 	      --file /tmp/openjdk.tar.gz 	      --directory "$JAVA_HOME" 	      --strip-components 1 	      --no-same-owner 	  ;     rm /tmp/openjdk.tar.gz;     find "$JAVA_HOME/lib" -name '*.so' -exec dirname '{}' ';' | sort -u > /etc/ld.so.conf.d/docker-openjdk.conf;     ldconfig;     java -Xshare:dump;
# Fri, 04 Nov 2022 23:22:32 GMT
RUN echo Verifying install ...     && fileEncoding="$(echo 'System.out.println(System.getProperty("file.encoding"))' | jshell -s -)"; [ "$fileEncoding" = 'UTF-8' ]; rm -rf ~/.java     && echo java --version && java --version     && echo Complete.
# Sat, 05 Nov 2022 01:35:16 GMT
ENV CATALINA_HOME=/usr/local/tomcat
# Sat, 05 Nov 2022 01:35:16 GMT
ENV PATH=/usr/local/tomcat/bin:/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Sat, 05 Nov 2022 01:35:17 GMT
RUN mkdir -p "$CATALINA_HOME"
# Sat, 05 Nov 2022 01:35:17 GMT
WORKDIR /usr/local/tomcat
# Sat, 05 Nov 2022 01:35:17 GMT
ENV TOMCAT_NATIVE_LIBDIR=/usr/local/tomcat/native-jni-lib
# Sat, 05 Nov 2022 01:35:17 GMT
ENV LD_LIBRARY_PATH=/usr/local/tomcat/native-jni-lib
# Sat, 05 Nov 2022 01:39:54 GMT
ENV GPG_KEYS=48F8E69F6390C9F25CFEDCD268248959359E722B A9C5DF4D22E99998D9875A5110C01C5A2F6059E7 DCFD35E0BF8CA7344752DE8B6FB21E8933C60243
# Sat, 05 Nov 2022 01:39:54 GMT
ENV TOMCAT_MAJOR=9
# Tue, 15 Nov 2022 03:06:43 GMT
ENV TOMCAT_VERSION=9.0.69
# Tue, 15 Nov 2022 03:06:43 GMT
ENV TOMCAT_SHA512=8c883c54ce9ce43eba37756a6404cdf3477879883a3e6d146dc8a7aa5e0425f487466afe6b6da4a895927cb7cb59177b9379cec18000f2de12785be57408c779
# Tue, 15 Nov 2022 03:06:44 GMT
COPY dir:b1a33aa3993dbbfbebb33bd9aa546b60c2f2191abf1227f453d4e830f6deb35f in /usr/local/tomcat 
# Tue, 15 Nov 2022 03:06:48 GMT
RUN set -eux; 	apt-get update; 	xargs -rt apt-get install -y --no-install-recommends < "$TOMCAT_NATIVE_LIBDIR/.dependencies.txt"; 	rm -rf /var/lib/apt/lists/*
# Tue, 15 Nov 2022 03:06:49 GMT
RUN set -eux; 	nativeLines="$(catalina.sh configtest 2>&1)"; 	nativeLines="$(echo "$nativeLines" | grep 'Apache Tomcat Native')"; 	nativeLines="$(echo "$nativeLines" | sort -u)"; 	if ! echo "$nativeLines" | grep -E 'INFO: Loaded( APR based)? Apache Tomcat Native library' >&2; then 		echo >&2 "$nativeLines"; 		exit 1; 	fi
# Tue, 15 Nov 2022 03:06:49 GMT
EXPOSE 8080
# Tue, 15 Nov 2022 03:06:49 GMT
CMD ["catalina.sh" "run"]
# Wed, 11 Jan 2023 02:47:03 GMT
LABEL org.opencontainers.image.authors=XWiki Development Team <committers@xwiki.org>
# Wed, 11 Jan 2023 02:47:03 GMT
LABEL org.opencontainers.image.url=https://hub.docker.com/_/xwiki
# Wed, 11 Jan 2023 02:47:03 GMT
LABEL org.opencontainers.image.documentation=https://hub.docker.com/_/xwiki
# Wed, 11 Jan 2023 02:47:03 GMT
LABEL org.opencontainers.image.source=https://github.com/xwiki/xwiki-docker.git
# Wed, 11 Jan 2023 02:47:04 GMT
LABEL org.opencontainers.image.vendor=xwiki.org
# Wed, 11 Jan 2023 02:47:04 GMT
LABEL org.opencontainers.image.licenses=LGPL-2.1
# Wed, 11 Jan 2023 02:49:03 GMT
RUN apt-get update &&   apt-get --no-install-recommends -y install     curl     libreoffice     unzip     procps &&   rm -rf /var/lib/apt/lists/*
# Wed, 22 Feb 2023 18:39:36 GMT
ENV XWIKI_VERSION=14.10.5
# Wed, 22 Feb 2023 18:39:36 GMT
ENV XWIKI_URL_PREFIX=https://maven.xwiki.org/releases/org/xwiki/platform/xwiki-platform-distribution-war/14.10.5
# Wed, 22 Feb 2023 18:39:36 GMT
ENV XWIKI_DOWNLOAD_SHA256=f58465d0869e4c5605ae8375a09c79399d1149c7131fed3cf9959918267eb6a8
# Wed, 22 Feb 2023 18:40:15 GMT
RUN rm -rf /usr/local/tomcat/webapps/* &&   mkdir -p /usr/local/tomcat/temp &&   mkdir -p /usr/local/xwiki/data &&   curl -fSL "${XWIKI_URL_PREFIX}/xwiki-platform-distribution-war-${XWIKI_VERSION}.war" -o xwiki.war &&   echo "$XWIKI_DOWNLOAD_SHA256 xwiki.war" | sha256sum -c - &&   unzip -d /usr/local/tomcat/webapps/ROOT xwiki.war &&   rm -f xwiki.war
# Wed, 22 Feb 2023 18:40:17 GMT
ENV MYSQL_JDBC_VERSION=8.0.32
# Wed, 22 Feb 2023 18:40:17 GMT
ENV MYSQL_JDBC_SHA256=522329fe925980f02e5eb89b59d227245d345415ff0c08932a68c9765c13acc5
# Wed, 22 Feb 2023 18:40:17 GMT
ENV MYSQL_JDBC_PREFIX=https://repo1.maven.org/maven2/com/mysql/mysql-connector-j/8.0.32
# Wed, 22 Feb 2023 18:40:17 GMT
ENV MYSQL_JDBC_ARTIFACT=mysql-connector-j-8.0.32.jar
# Wed, 22 Feb 2023 18:40:17 GMT
ENV MYSQL_JDBC_TARGET=/usr/local/tomcat/webapps/ROOT/WEB-INF/lib/mysql-connector-j-8.0.32.jar
# Wed, 22 Feb 2023 18:40:18 GMT
RUN curl -fSL "${MYSQL_JDBC_PREFIX}/${MYSQL_JDBC_ARTIFACT}" -o $MYSQL_JDBC_TARGET &&   echo "$MYSQL_JDBC_SHA256 $MYSQL_JDBC_TARGET" | sha256sum -c -
# Wed, 22 Feb 2023 18:40:18 GMT
COPY file:0a1be11e2eb610a1dbcd415404e3a592641110b93090030cb831e3a19a163017 in /usr/local/tomcat/bin/ 
# Wed, 22 Feb 2023 18:40:18 GMT
COPY file:1b8409986f3e4eb79a7a0b18472cb2692a61d504fb5ef34292bc997b79fd760d in /usr/local/tomcat/webapps/ROOT/WEB-INF/hibernate.cfg.xml 
# Wed, 22 Feb 2023 18:40:19 GMT
RUN sed -i 's/<id>org.xwiki.platform:xwiki-platform-distribution-war/<id>org.xwiki.platform:xwiki-platform-distribution-docker/'   /usr/local/tomcat/webapps/ROOT/META-INF/extension.xed
# Wed, 22 Feb 2023 18:40:19 GMT
COPY file:a47c4dcd87c9dad97aff38c49188357e6193bcad50757e516cfb08a60d4de611 in /usr/local/bin/docker-entrypoint.sh 
# Wed, 22 Feb 2023 18:40:19 GMT
VOLUME [/usr/local/xwiki]
# Wed, 22 Feb 2023 18:40:19 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 22 Feb 2023 18:40:19 GMT
CMD ["xwiki"]
```

-	Layers:
	-	`sha256:e96e057aae67380a4ddb16c337c5c3669d97fdff69ec537f02aa2cc30d814281`  
		Last Modified: Wed, 02 Nov 2022 03:03:36 GMT  
		Size: 30.4 MB (30425607 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4ced2591451da3a02e2b6bb44752b9e3f00d77789921be4df5082fb9f9880ad0`  
		Last Modified: Wed, 02 Nov 2022 18:48:43 GMT  
		Size: 12.4 MB (12439006 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:df8f874ae8c08a9e69e5fbe6c5a64200a45386132a3203d1a9a7f1146d94cfbc`  
		Last Modified: Fri, 04 Nov 2022 23:29:33 GMT  
		Size: 46.6 MB (46629936 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:111b6c7486426c4b6989102c2ee5be856e8a58e20ab0a350b24a905d536e8e7f`  
		Last Modified: Fri, 04 Nov 2022 23:29:26 GMT  
		Size: 161.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e6f84dce457c6d4f7b7291fce05f8e77998a3a7722a54125a1f1d52ca83043b4`  
		Last Modified: Sat, 05 Nov 2022 01:50:51 GMT  
		Size: 173.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a6c26749ee782392e38845ee2ba79b0da586ef6a45d8e7f29c7af14612278547`  
		Last Modified: Tue, 15 Nov 2022 03:19:57 GMT  
		Size: 12.2 MB (12200249 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4dddc6d9fa6024025b3fcfe729cab2dc544fb25476eca6e80b1af8e8d93bb0ee`  
		Last Modified: Tue, 15 Nov 2022 03:19:56 GMT  
		Size: 452.7 KB (452680 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:06637eebe5e72c8ad9019ad4eb4cdde1f11f7d4c24c7ed7374cf8966343aa2fb`  
		Last Modified: Tue, 15 Nov 2022 03:19:56 GMT  
		Size: 131.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b276fb8390410a8208724033e325715ea26000d5a1a762d4c3699b927884fbfe`  
		Last Modified: Wed, 11 Jan 2023 02:52:45 GMT  
		Size: 178.8 MB (178805608 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:89de9d9e2c09cd5b84430562516cbcd5695a0a3b2347b451e157bde75c2b5619`  
		Last Modified: Wed, 22 Feb 2023 18:42:21 GMT  
		Size: 307.1 MB (307141303 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4a2089179b7c1db514d0502e476e09b8f9313d08d4c4e4f3981be456288fe507`  
		Last Modified: Wed, 22 Feb 2023 18:42:04 GMT  
		Size: 2.3 MB (2342572 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e7c4ef360ff3673244adb3dfc4769b5710fa68fcc1fbe1c08b2f5fa32dbd4976`  
		Last Modified: Wed, 22 Feb 2023 18:42:04 GMT  
		Size: 1.3 KB (1348 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:08441c368d4b01e361491d7fbf1ac579fcc303b8484123c309a8d5a3b6657c46`  
		Last Modified: Wed, 22 Feb 2023 18:42:04 GMT  
		Size: 2.3 KB (2311 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:542b4bb846d438395e458c08de292f72d14d289fae6ffe7eba6fec1cd8518475`  
		Last Modified: Wed, 22 Feb 2023 18:42:04 GMT  
		Size: 6.0 KB (6013 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:039c0305df9e64c69bb546e64f0658dba6e728eee13022cfd682aa1ee76b8b7f`  
		Last Modified: Wed, 22 Feb 2023 18:42:04 GMT  
		Size: 2.5 KB (2506 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `xwiki:14` - linux; arm64 variant v8

```console
$ docker pull xwiki@sha256:33e36167828fe9bae944e7d4cbbe3b69dd2415595d40610ac2ebcd73f2c2fa7f
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **581.7 MB (581697690 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:44013daf43fd09deb7221eef006c4d30d484a03c433118e5b59da0a44b573f06`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["xwiki"]`

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
# Wed, 02 Nov 2022 19:44:32 GMT
RUN apt-get update     && DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends tzdata curl wget ca-certificates fontconfig locales     && echo "en_US.UTF-8 UTF-8" >> /etc/locale.gen     && locale-gen en_US.UTF-8     && rm -rf /var/lib/apt/lists/*
# Fri, 04 Nov 2022 22:40:54 GMT
ENV JAVA_VERSION=jdk-11.0.17+8
# Fri, 04 Nov 2022 22:41:33 GMT
RUN set -eux;     ARCH="$(dpkg --print-architecture)";     case "${ARCH}" in        aarch64|arm64)          ESUM='bd6efe3290c8b5a42f695a55a26f3e3c9c284288574879d4b7089f31f5114177';          BINARY_URL='https://github.com/adoptium/temurin11-binaries/releases/download/jdk-11.0.17%2B8/OpenJDK11U-jre_aarch64_linux_hotspot_11.0.17_8.tar.gz';          ;;        armhf|arm)          ESUM='8cf113d3d7fa808895c8d2e41bb890af21c47e38c2460e0588147a4bb8fc658d';          BINARY_URL='https://github.com/adoptium/temurin11-binaries/releases/download/jdk-11.0.17%2B8/OpenJDK11U-jre_arm_linux_hotspot_11.0.17_8.tar.gz';          ;;        ppc64el|powerpc:common64)          ESUM='0ca3d806131ab5834c501f9c625bb0248cd528af361c704503348e9c9605bedf';          BINARY_URL='https://github.com/adoptium/temurin11-binaries/releases/download/jdk-11.0.17%2B8/OpenJDK11U-jre_ppc64le_linux_hotspot_11.0.17_8.tar.gz';          ;;        s390x|s390:64-bit)          ESUM='dd3b159a374086e65cb07c4ccb226c90f9c02ef929cba6f0b642171d7ed97fa4';          BINARY_URL='https://github.com/adoptium/temurin11-binaries/releases/download/jdk-11.0.17%2B8/OpenJDK11U-jre_s390x_linux_hotspot_11.0.17_8.tar.gz';          ;;        amd64|i386:x86-64)          ESUM='752616097e09d7f60a3ad8bd312f90eaf50ac72577e55df229fe6e8091148f79';          BINARY_URL='https://github.com/adoptium/temurin11-binaries/releases/download/jdk-11.0.17%2B8/OpenJDK11U-jre_x64_linux_hotspot_11.0.17_8.tar.gz';          ;;        *)          echo "Unsupported arch: ${ARCH}";          exit 1;          ;;     esac; 	  wget -O /tmp/openjdk.tar.gz ${BINARY_URL}; 	  echo "${ESUM} */tmp/openjdk.tar.gz" | sha256sum -c -; 	  mkdir -p "$JAVA_HOME"; 	  tar --extract 	      --file /tmp/openjdk.tar.gz 	      --directory "$JAVA_HOME" 	      --strip-components 1 	      --no-same-owner 	  ;     rm /tmp/openjdk.tar.gz;     find "$JAVA_HOME/lib" -name '*.so' -exec dirname '{}' ';' | sort -u > /etc/ld.so.conf.d/docker-openjdk.conf;     ldconfig;     java -Xshare:dump;
# Fri, 04 Nov 2022 22:41:34 GMT
RUN echo Verifying install ...     && fileEncoding="$(echo 'System.out.println(System.getProperty("file.encoding"))' | jshell -s -)"; [ "$fileEncoding" = 'UTF-8' ]; rm -rf ~/.java     && echo java --version && java --version     && echo Complete.
# Fri, 04 Nov 2022 23:48:38 GMT
ENV CATALINA_HOME=/usr/local/tomcat
# Fri, 04 Nov 2022 23:48:38 GMT
ENV PATH=/usr/local/tomcat/bin:/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Fri, 04 Nov 2022 23:48:38 GMT
RUN mkdir -p "$CATALINA_HOME"
# Fri, 04 Nov 2022 23:48:39 GMT
WORKDIR /usr/local/tomcat
# Fri, 04 Nov 2022 23:48:39 GMT
ENV TOMCAT_NATIVE_LIBDIR=/usr/local/tomcat/native-jni-lib
# Fri, 04 Nov 2022 23:48:39 GMT
ENV LD_LIBRARY_PATH=/usr/local/tomcat/native-jni-lib
# Fri, 04 Nov 2022 23:53:12 GMT
ENV GPG_KEYS=48F8E69F6390C9F25CFEDCD268248959359E722B A9C5DF4D22E99998D9875A5110C01C5A2F6059E7 DCFD35E0BF8CA7344752DE8B6FB21E8933C60243
# Fri, 04 Nov 2022 23:53:12 GMT
ENV TOMCAT_MAJOR=9
# Tue, 15 Nov 2022 04:57:22 GMT
ENV TOMCAT_VERSION=9.0.69
# Tue, 15 Nov 2022 04:57:22 GMT
ENV TOMCAT_SHA512=8c883c54ce9ce43eba37756a6404cdf3477879883a3e6d146dc8a7aa5e0425f487466afe6b6da4a895927cb7cb59177b9379cec18000f2de12785be57408c779
# Tue, 15 Nov 2022 04:57:22 GMT
COPY dir:096b403a5f78b17e6b4bff63128a9c93941b97f22470991610dd641633d977f1 in /usr/local/tomcat 
# Tue, 15 Nov 2022 04:57:25 GMT
RUN set -eux; 	apt-get update; 	xargs -rt apt-get install -y --no-install-recommends < "$TOMCAT_NATIVE_LIBDIR/.dependencies.txt"; 	rm -rf /var/lib/apt/lists/*
# Tue, 15 Nov 2022 04:57:26 GMT
RUN set -eux; 	nativeLines="$(catalina.sh configtest 2>&1)"; 	nativeLines="$(echo "$nativeLines" | grep 'Apache Tomcat Native')"; 	nativeLines="$(echo "$nativeLines" | sort -u)"; 	if ! echo "$nativeLines" | grep -E 'INFO: Loaded( APR based)? Apache Tomcat Native library' >&2; then 		echo >&2 "$nativeLines"; 		exit 1; 	fi
# Tue, 15 Nov 2022 04:57:26 GMT
EXPOSE 8080
# Tue, 15 Nov 2022 04:57:27 GMT
CMD ["catalina.sh" "run"]
# Wed, 11 Jan 2023 03:05:10 GMT
LABEL org.opencontainers.image.authors=XWiki Development Team <committers@xwiki.org>
# Wed, 11 Jan 2023 03:05:10 GMT
LABEL org.opencontainers.image.url=https://hub.docker.com/_/xwiki
# Wed, 11 Jan 2023 03:05:10 GMT
LABEL org.opencontainers.image.documentation=https://hub.docker.com/_/xwiki
# Wed, 11 Jan 2023 03:05:10 GMT
LABEL org.opencontainers.image.source=https://github.com/xwiki/xwiki-docker.git
# Wed, 11 Jan 2023 03:05:11 GMT
LABEL org.opencontainers.image.vendor=xwiki.org
# Wed, 11 Jan 2023 03:05:11 GMT
LABEL org.opencontainers.image.licenses=LGPL-2.1
# Wed, 11 Jan 2023 03:07:37 GMT
RUN apt-get update &&   apt-get --no-install-recommends -y install     curl     libreoffice     unzip     procps &&   rm -rf /var/lib/apt/lists/*
# Wed, 01 Feb 2023 22:26:19 GMT
ENV XWIKI_VERSION=14.10.4
# Wed, 01 Feb 2023 22:26:19 GMT
ENV XWIKI_URL_PREFIX=https://maven.xwiki.org/releases/org/xwiki/platform/xwiki-platform-distribution-war/14.10.4
# Wed, 01 Feb 2023 22:26:19 GMT
ENV XWIKI_DOWNLOAD_SHA256=2fcfb622319172c2e424b9c11848ebfabe27cf8ef69cba39ceb5d124b7ebe713
# Wed, 01 Feb 2023 22:27:00 GMT
RUN rm -rf /usr/local/tomcat/webapps/* &&   mkdir -p /usr/local/tomcat/temp &&   mkdir -p /usr/local/xwiki/data &&   curl -fSL "${XWIKI_URL_PREFIX}/xwiki-platform-distribution-war-${XWIKI_VERSION}.war" -o xwiki.war &&   echo "$XWIKI_DOWNLOAD_SHA256 xwiki.war" | sha256sum -c - &&   unzip -d /usr/local/tomcat/webapps/ROOT xwiki.war &&   rm -f xwiki.war
# Wed, 01 Feb 2023 22:27:03 GMT
ENV MYSQL_JDBC_VERSION=8.0.31
# Wed, 01 Feb 2023 22:27:03 GMT
ENV MYSQL_JDBC_SHA256=5249e3dc6d6531b37790e3f61845b96db5e41e891d3d8edb0e2e3a1b53ca2f4f
# Wed, 01 Feb 2023 22:27:03 GMT
ENV MYSQL_JDBC_PREFIX=https://repo1.maven.org/maven2/com/mysql/mysql-connector-j/8.0.31
# Wed, 01 Feb 2023 22:27:03 GMT
ENV MYSQL_JDBC_ARTIFACT=mysql-connector-j-8.0.31.jar
# Wed, 01 Feb 2023 22:27:03 GMT
ENV MYSQL_JDBC_TARGET=/usr/local/tomcat/webapps/ROOT/WEB-INF/lib/mysql-connector-j-8.0.31.jar
# Wed, 01 Feb 2023 22:27:04 GMT
RUN curl -fSL "${MYSQL_JDBC_PREFIX}/${MYSQL_JDBC_ARTIFACT}" -o $MYSQL_JDBC_TARGET &&   echo "$MYSQL_JDBC_SHA256 $MYSQL_JDBC_TARGET" | sha256sum -c -
# Wed, 01 Feb 2023 22:27:04 GMT
COPY file:0a1be11e2eb610a1dbcd415404e3a592641110b93090030cb831e3a19a163017 in /usr/local/tomcat/bin/ 
# Wed, 01 Feb 2023 22:27:04 GMT
COPY file:1b8409986f3e4eb79a7a0b18472cb2692a61d504fb5ef34292bc997b79fd760d in /usr/local/tomcat/webapps/ROOT/WEB-INF/hibernate.cfg.xml 
# Wed, 01 Feb 2023 22:27:05 GMT
RUN sed -i 's/<id>org.xwiki.platform:xwiki-platform-distribution-war/<id>org.xwiki.platform:xwiki-platform-distribution-docker/'   /usr/local/tomcat/webapps/ROOT/META-INF/extension.xed
# Wed, 01 Feb 2023 22:27:05 GMT
COPY file:a47c4dcd87c9dad97aff38c49188357e6193bcad50757e516cfb08a60d4de611 in /usr/local/bin/docker-entrypoint.sh 
# Wed, 01 Feb 2023 22:27:05 GMT
VOLUME [/usr/local/xwiki]
# Wed, 01 Feb 2023 22:27:05 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 01 Feb 2023 22:27:05 GMT
CMD ["xwiki"]
```

-	Layers:
	-	`sha256:0509fae36eb0656f8bdb23f8ae64100d893bcea2563e97468d337e04d2d0410b`  
		Last Modified: Wed, 02 Nov 2022 18:50:21 GMT  
		Size: 28.4 MB (28382154 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e502a1af2bcd98f5f0d2f5e4da1a0e7bbe07a2c548e2662f7d37dce5ae1df46c`  
		Last Modified: Wed, 02 Nov 2022 19:48:28 GMT  
		Size: 12.4 MB (12396330 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bc4598c07dd818f03a0378b0341a4a8e80f0152fbb3e7d5246ca4f466f42e611`  
		Last Modified: Fri, 04 Nov 2022 22:46:46 GMT  
		Size: 45.0 MB (44958470 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:715a937a1066f998b331fcd62256ad01a5571bdf46804e97825afc64f9ebb427`  
		Last Modified: Fri, 04 Nov 2022 22:46:41 GMT  
		Size: 160.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5fb623f082f74b2fa9fc2c4e3f3a4802875cb9753cfa26ed940201ce72bb56cb`  
		Last Modified: Sat, 05 Nov 2022 00:03:40 GMT  
		Size: 172.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:33260b83200262bbd546be371ad3c1f50f5ae7228afb87982d6fa9d6b11bf26f`  
		Last Modified: Tue, 15 Nov 2022 05:10:19 GMT  
		Size: 12.2 MB (12207235 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0955fb697ea9b30a1b4f95385464f646aa1525cb6efba648e22df84ebef6b2ee`  
		Last Modified: Tue, 15 Nov 2022 05:10:18 GMT  
		Size: 452.0 KB (452021 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6eddcf66f2083b1487296a0308e0b058917c97f614f12428d82d89662038dc2e`  
		Last Modified: Tue, 15 Nov 2022 05:10:18 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ae5f60bb64f3fa11da3d15a9639f886186b4c2c021455c3f9db22e0cfe1b1311`  
		Last Modified: Wed, 11 Jan 2023 03:11:14 GMT  
		Size: 173.8 MB (173806827 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:13334e257ce7313ca9d6028534e3ec6c7858c374c4afedea7f96c51da716806e`  
		Last Modified: Wed, 01 Feb 2023 22:29:16 GMT  
		Size: 307.1 MB (307104849 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ccb59878c7670194b75b6af22dd3908f9ae1a12dc1074f0b5ed156a5e3afdf0a`  
		Last Modified: Wed, 01 Feb 2023 22:29:02 GMT  
		Size: 2.4 MB (2377177 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d3946fb25102529cda96bcad4925905c9b997e442b447675d89066505cbe1026`  
		Last Modified: Wed, 01 Feb 2023 22:29:02 GMT  
		Size: 1.3 KB (1344 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1ba832da71f2ed07bae5269bb37e7ea79724a069ad63032f2af14996893baa37`  
		Last Modified: Wed, 01 Feb 2023 22:29:02 GMT  
		Size: 2.3 KB (2307 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6616193191331001a42a5d452ea69a215bbc414eca5cb00914c359665be5817f`  
		Last Modified: Wed, 01 Feb 2023 22:29:02 GMT  
		Size: 6.0 KB (6009 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6de4b8ce214cd9b76eda5b4955e5abb249a0b0292e8a38d39683e3002d6534bf`  
		Last Modified: Wed, 01 Feb 2023 22:29:03 GMT  
		Size: 2.5 KB (2506 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `xwiki:14-mariadb-tomcat`

```console
$ docker pull xwiki@sha256:016ba45d303064d25d04a705c1a307612a6383139366413fb169f42acc0419ee
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `xwiki:14-mariadb-tomcat` - linux; amd64

```console
$ docker pull xwiki@sha256:4aec14b2a2ae95584b839238412bbe33a7314bf32edc3e05f34f532d07fdedce
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **588.7 MB (588696916 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f5fbe86c66c7ac80e07663234a80353ce71d1847f409e2e2a603e0eb2a3342bc`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["xwiki"]`

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
# Wed, 02 Nov 2022 18:44:10 GMT
RUN apt-get update     && DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends tzdata curl wget ca-certificates fontconfig locales     && echo "en_US.UTF-8 UTF-8" >> /etc/locale.gen     && locale-gen en_US.UTF-8     && rm -rf /var/lib/apt/lists/*
# Fri, 04 Nov 2022 23:21:41 GMT
ENV JAVA_VERSION=jdk-11.0.17+8
# Fri, 04 Nov 2022 23:22:31 GMT
RUN set -eux;     ARCH="$(dpkg --print-architecture)";     case "${ARCH}" in        aarch64|arm64)          ESUM='bd6efe3290c8b5a42f695a55a26f3e3c9c284288574879d4b7089f31f5114177';          BINARY_URL='https://github.com/adoptium/temurin11-binaries/releases/download/jdk-11.0.17%2B8/OpenJDK11U-jre_aarch64_linux_hotspot_11.0.17_8.tar.gz';          ;;        armhf|arm)          ESUM='8cf113d3d7fa808895c8d2e41bb890af21c47e38c2460e0588147a4bb8fc658d';          BINARY_URL='https://github.com/adoptium/temurin11-binaries/releases/download/jdk-11.0.17%2B8/OpenJDK11U-jre_arm_linux_hotspot_11.0.17_8.tar.gz';          ;;        ppc64el|powerpc:common64)          ESUM='0ca3d806131ab5834c501f9c625bb0248cd528af361c704503348e9c9605bedf';          BINARY_URL='https://github.com/adoptium/temurin11-binaries/releases/download/jdk-11.0.17%2B8/OpenJDK11U-jre_ppc64le_linux_hotspot_11.0.17_8.tar.gz';          ;;        s390x|s390:64-bit)          ESUM='dd3b159a374086e65cb07c4ccb226c90f9c02ef929cba6f0b642171d7ed97fa4';          BINARY_URL='https://github.com/adoptium/temurin11-binaries/releases/download/jdk-11.0.17%2B8/OpenJDK11U-jre_s390x_linux_hotspot_11.0.17_8.tar.gz';          ;;        amd64|i386:x86-64)          ESUM='752616097e09d7f60a3ad8bd312f90eaf50ac72577e55df229fe6e8091148f79';          BINARY_URL='https://github.com/adoptium/temurin11-binaries/releases/download/jdk-11.0.17%2B8/OpenJDK11U-jre_x64_linux_hotspot_11.0.17_8.tar.gz';          ;;        *)          echo "Unsupported arch: ${ARCH}";          exit 1;          ;;     esac; 	  wget -O /tmp/openjdk.tar.gz ${BINARY_URL}; 	  echo "${ESUM} */tmp/openjdk.tar.gz" | sha256sum -c -; 	  mkdir -p "$JAVA_HOME"; 	  tar --extract 	      --file /tmp/openjdk.tar.gz 	      --directory "$JAVA_HOME" 	      --strip-components 1 	      --no-same-owner 	  ;     rm /tmp/openjdk.tar.gz;     find "$JAVA_HOME/lib" -name '*.so' -exec dirname '{}' ';' | sort -u > /etc/ld.so.conf.d/docker-openjdk.conf;     ldconfig;     java -Xshare:dump;
# Fri, 04 Nov 2022 23:22:32 GMT
RUN echo Verifying install ...     && fileEncoding="$(echo 'System.out.println(System.getProperty("file.encoding"))' | jshell -s -)"; [ "$fileEncoding" = 'UTF-8' ]; rm -rf ~/.java     && echo java --version && java --version     && echo Complete.
# Sat, 05 Nov 2022 01:35:16 GMT
ENV CATALINA_HOME=/usr/local/tomcat
# Sat, 05 Nov 2022 01:35:16 GMT
ENV PATH=/usr/local/tomcat/bin:/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Sat, 05 Nov 2022 01:35:17 GMT
RUN mkdir -p "$CATALINA_HOME"
# Sat, 05 Nov 2022 01:35:17 GMT
WORKDIR /usr/local/tomcat
# Sat, 05 Nov 2022 01:35:17 GMT
ENV TOMCAT_NATIVE_LIBDIR=/usr/local/tomcat/native-jni-lib
# Sat, 05 Nov 2022 01:35:17 GMT
ENV LD_LIBRARY_PATH=/usr/local/tomcat/native-jni-lib
# Sat, 05 Nov 2022 01:39:54 GMT
ENV GPG_KEYS=48F8E69F6390C9F25CFEDCD268248959359E722B A9C5DF4D22E99998D9875A5110C01C5A2F6059E7 DCFD35E0BF8CA7344752DE8B6FB21E8933C60243
# Sat, 05 Nov 2022 01:39:54 GMT
ENV TOMCAT_MAJOR=9
# Tue, 15 Nov 2022 03:06:43 GMT
ENV TOMCAT_VERSION=9.0.69
# Tue, 15 Nov 2022 03:06:43 GMT
ENV TOMCAT_SHA512=8c883c54ce9ce43eba37756a6404cdf3477879883a3e6d146dc8a7aa5e0425f487466afe6b6da4a895927cb7cb59177b9379cec18000f2de12785be57408c779
# Tue, 15 Nov 2022 03:06:44 GMT
COPY dir:b1a33aa3993dbbfbebb33bd9aa546b60c2f2191abf1227f453d4e830f6deb35f in /usr/local/tomcat 
# Tue, 15 Nov 2022 03:06:48 GMT
RUN set -eux; 	apt-get update; 	xargs -rt apt-get install -y --no-install-recommends < "$TOMCAT_NATIVE_LIBDIR/.dependencies.txt"; 	rm -rf /var/lib/apt/lists/*
# Tue, 15 Nov 2022 03:06:49 GMT
RUN set -eux; 	nativeLines="$(catalina.sh configtest 2>&1)"; 	nativeLines="$(echo "$nativeLines" | grep 'Apache Tomcat Native')"; 	nativeLines="$(echo "$nativeLines" | sort -u)"; 	if ! echo "$nativeLines" | grep -E 'INFO: Loaded( APR based)? Apache Tomcat Native library' >&2; then 		echo >&2 "$nativeLines"; 		exit 1; 	fi
# Tue, 15 Nov 2022 03:06:49 GMT
EXPOSE 8080
# Tue, 15 Nov 2022 03:06:49 GMT
CMD ["catalina.sh" "run"]
# Wed, 11 Jan 2023 02:47:03 GMT
LABEL org.opencontainers.image.authors=XWiki Development Team <committers@xwiki.org>
# Wed, 11 Jan 2023 02:47:03 GMT
LABEL org.opencontainers.image.url=https://hub.docker.com/_/xwiki
# Wed, 11 Jan 2023 02:47:03 GMT
LABEL org.opencontainers.image.documentation=https://hub.docker.com/_/xwiki
# Wed, 11 Jan 2023 02:47:03 GMT
LABEL org.opencontainers.image.source=https://github.com/xwiki/xwiki-docker.git
# Wed, 11 Jan 2023 02:47:04 GMT
LABEL org.opencontainers.image.vendor=xwiki.org
# Wed, 11 Jan 2023 02:47:04 GMT
LABEL org.opencontainers.image.licenses=LGPL-2.1
# Wed, 11 Jan 2023 02:49:03 GMT
RUN apt-get update &&   apt-get --no-install-recommends -y install     curl     libreoffice     unzip     procps &&   rm -rf /var/lib/apt/lists/*
# Wed, 22 Feb 2023 18:39:36 GMT
ENV XWIKI_VERSION=14.10.5
# Wed, 22 Feb 2023 18:39:36 GMT
ENV XWIKI_URL_PREFIX=https://maven.xwiki.org/releases/org/xwiki/platform/xwiki-platform-distribution-war/14.10.5
# Wed, 22 Feb 2023 18:39:36 GMT
ENV XWIKI_DOWNLOAD_SHA256=f58465d0869e4c5605ae8375a09c79399d1149c7131fed3cf9959918267eb6a8
# Wed, 22 Feb 2023 18:40:15 GMT
RUN rm -rf /usr/local/tomcat/webapps/* &&   mkdir -p /usr/local/tomcat/temp &&   mkdir -p /usr/local/xwiki/data &&   curl -fSL "${XWIKI_URL_PREFIX}/xwiki-platform-distribution-war-${XWIKI_VERSION}.war" -o xwiki.war &&   echo "$XWIKI_DOWNLOAD_SHA256 xwiki.war" | sha256sum -c - &&   unzip -d /usr/local/tomcat/webapps/ROOT xwiki.war &&   rm -f xwiki.war
# Wed, 22 Feb 2023 18:41:14 GMT
ENV MARIADB_JDBC_VERSION=3.1.2
# Wed, 22 Feb 2023 18:41:14 GMT
ENV MARIADB_JDBC_SHA256=aaec1ad348d030a65b25c93c65cdaf472bf8b4b6b314b965e5ba13aec81bc622
# Wed, 22 Feb 2023 18:41:14 GMT
ENV MARIADB_JDBC_PREFIX=https://repo1.maven.org/maven2/org/mariadb/jdbc/mariadb-java-client/3.1.2
# Wed, 22 Feb 2023 18:41:14 GMT
ENV MARIADB_JDBC_ARTIFACT=mariadb-java-client-3.1.2.jar
# Wed, 22 Feb 2023 18:41:14 GMT
ENV MARIADB_JDBC_TARGET=/usr/local/tomcat/webapps/ROOT/WEB-INF/lib/mariadb-java-client-3.1.2.jar
# Wed, 22 Feb 2023 18:41:15 GMT
RUN curl -fSL "${MARIADB_JDBC_PREFIX}/${MARIADB_JDBC_ARTIFACT}" -o $MARIADB_JDBC_TARGET &&   echo "$MARIADB_JDBC_SHA256 $MARIADB_JDBC_TARGET" | sha256sum -c -
# Wed, 22 Feb 2023 18:41:15 GMT
COPY file:0a1be11e2eb610a1dbcd415404e3a592641110b93090030cb831e3a19a163017 in /usr/local/tomcat/bin/ 
# Wed, 22 Feb 2023 18:41:15 GMT
COPY file:0e237c3876eeb3b5f3473a064d3e507da2df6c228ca714687930b34e3b687601 in /usr/local/tomcat/webapps/ROOT/WEB-INF/hibernate.cfg.xml 
# Wed, 22 Feb 2023 18:41:15 GMT
RUN sed -i 's/<id>org.xwiki.platform:xwiki-platform-distribution-war/<id>org.xwiki.platform:xwiki-platform-distribution-docker/'   /usr/local/tomcat/webapps/ROOT/META-INF/extension.xed
# Wed, 22 Feb 2023 18:41:16 GMT
COPY file:a47c4dcd87c9dad97aff38c49188357e6193bcad50757e516cfb08a60d4de611 in /usr/local/bin/docker-entrypoint.sh 
# Wed, 22 Feb 2023 18:41:16 GMT
VOLUME [/usr/local/xwiki]
# Wed, 22 Feb 2023 18:41:16 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 22 Feb 2023 18:41:16 GMT
CMD ["xwiki"]
```

-	Layers:
	-	`sha256:e96e057aae67380a4ddb16c337c5c3669d97fdff69ec537f02aa2cc30d814281`  
		Last Modified: Wed, 02 Nov 2022 03:03:36 GMT  
		Size: 30.4 MB (30425607 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4ced2591451da3a02e2b6bb44752b9e3f00d77789921be4df5082fb9f9880ad0`  
		Last Modified: Wed, 02 Nov 2022 18:48:43 GMT  
		Size: 12.4 MB (12439006 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:df8f874ae8c08a9e69e5fbe6c5a64200a45386132a3203d1a9a7f1146d94cfbc`  
		Last Modified: Fri, 04 Nov 2022 23:29:33 GMT  
		Size: 46.6 MB (46629936 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:111b6c7486426c4b6989102c2ee5be856e8a58e20ab0a350b24a905d536e8e7f`  
		Last Modified: Fri, 04 Nov 2022 23:29:26 GMT  
		Size: 161.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e6f84dce457c6d4f7b7291fce05f8e77998a3a7722a54125a1f1d52ca83043b4`  
		Last Modified: Sat, 05 Nov 2022 01:50:51 GMT  
		Size: 173.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a6c26749ee782392e38845ee2ba79b0da586ef6a45d8e7f29c7af14612278547`  
		Last Modified: Tue, 15 Nov 2022 03:19:57 GMT  
		Size: 12.2 MB (12200249 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4dddc6d9fa6024025b3fcfe729cab2dc544fb25476eca6e80b1af8e8d93bb0ee`  
		Last Modified: Tue, 15 Nov 2022 03:19:56 GMT  
		Size: 452.7 KB (452680 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:06637eebe5e72c8ad9019ad4eb4cdde1f11f7d4c24c7ed7374cf8966343aa2fb`  
		Last Modified: Tue, 15 Nov 2022 03:19:56 GMT  
		Size: 131.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b276fb8390410a8208724033e325715ea26000d5a1a762d4c3699b927884fbfe`  
		Last Modified: Wed, 11 Jan 2023 02:52:45 GMT  
		Size: 178.8 MB (178805608 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:89de9d9e2c09cd5b84430562516cbcd5695a0a3b2347b451e157bde75c2b5619`  
		Last Modified: Wed, 22 Feb 2023 18:42:21 GMT  
		Size: 307.1 MB (307141303 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c34f6e86e4b4ce021fdc5c26a390f8682b638ef5b002596f5d85721a5b4f8b78`  
		Last Modified: Wed, 22 Feb 2023 18:43:25 GMT  
		Size: 589.9 KB (589888 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7c59af828719a4990baaba43861a4b7dfcf7c9301bc8c1c17b1977363ae47d8f`  
		Last Modified: Wed, 22 Feb 2023 18:43:25 GMT  
		Size: 1.3 KB (1345 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a1ce8abe653003fb1cf66551dd2e3daf88c2ec88e42e874179577314bcb129d7`  
		Last Modified: Wed, 22 Feb 2023 18:43:25 GMT  
		Size: 2.3 KB (2312 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:68e8b10875b16f8254c97d2580791e4ed6c27787f670ac843c0508addb3b38b3`  
		Last Modified: Wed, 22 Feb 2023 18:43:25 GMT  
		Size: 6.0 KB (6013 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ed46c896037147ae7b8029b5b7e890b7930132f0eec078e1211ccb92ff45c89e`  
		Last Modified: Wed, 22 Feb 2023 18:43:25 GMT  
		Size: 2.5 KB (2504 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `xwiki:14-mariadb-tomcat` - linux; arm64 variant v8

```console
$ docker pull xwiki@sha256:7325fc8b1c018497044befd011b0c006d687105f4227efb007aa304e9a7aae36
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **579.9 MB (579910180 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e16df67b6f15552144570116827b8b364c740abb52e9ca29c35e0c5ed526fe1b`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["xwiki"]`

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
# Wed, 02 Nov 2022 19:44:32 GMT
RUN apt-get update     && DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends tzdata curl wget ca-certificates fontconfig locales     && echo "en_US.UTF-8 UTF-8" >> /etc/locale.gen     && locale-gen en_US.UTF-8     && rm -rf /var/lib/apt/lists/*
# Fri, 04 Nov 2022 22:40:54 GMT
ENV JAVA_VERSION=jdk-11.0.17+8
# Fri, 04 Nov 2022 22:41:33 GMT
RUN set -eux;     ARCH="$(dpkg --print-architecture)";     case "${ARCH}" in        aarch64|arm64)          ESUM='bd6efe3290c8b5a42f695a55a26f3e3c9c284288574879d4b7089f31f5114177';          BINARY_URL='https://github.com/adoptium/temurin11-binaries/releases/download/jdk-11.0.17%2B8/OpenJDK11U-jre_aarch64_linux_hotspot_11.0.17_8.tar.gz';          ;;        armhf|arm)          ESUM='8cf113d3d7fa808895c8d2e41bb890af21c47e38c2460e0588147a4bb8fc658d';          BINARY_URL='https://github.com/adoptium/temurin11-binaries/releases/download/jdk-11.0.17%2B8/OpenJDK11U-jre_arm_linux_hotspot_11.0.17_8.tar.gz';          ;;        ppc64el|powerpc:common64)          ESUM='0ca3d806131ab5834c501f9c625bb0248cd528af361c704503348e9c9605bedf';          BINARY_URL='https://github.com/adoptium/temurin11-binaries/releases/download/jdk-11.0.17%2B8/OpenJDK11U-jre_ppc64le_linux_hotspot_11.0.17_8.tar.gz';          ;;        s390x|s390:64-bit)          ESUM='dd3b159a374086e65cb07c4ccb226c90f9c02ef929cba6f0b642171d7ed97fa4';          BINARY_URL='https://github.com/adoptium/temurin11-binaries/releases/download/jdk-11.0.17%2B8/OpenJDK11U-jre_s390x_linux_hotspot_11.0.17_8.tar.gz';          ;;        amd64|i386:x86-64)          ESUM='752616097e09d7f60a3ad8bd312f90eaf50ac72577e55df229fe6e8091148f79';          BINARY_URL='https://github.com/adoptium/temurin11-binaries/releases/download/jdk-11.0.17%2B8/OpenJDK11U-jre_x64_linux_hotspot_11.0.17_8.tar.gz';          ;;        *)          echo "Unsupported arch: ${ARCH}";          exit 1;          ;;     esac; 	  wget -O /tmp/openjdk.tar.gz ${BINARY_URL}; 	  echo "${ESUM} */tmp/openjdk.tar.gz" | sha256sum -c -; 	  mkdir -p "$JAVA_HOME"; 	  tar --extract 	      --file /tmp/openjdk.tar.gz 	      --directory "$JAVA_HOME" 	      --strip-components 1 	      --no-same-owner 	  ;     rm /tmp/openjdk.tar.gz;     find "$JAVA_HOME/lib" -name '*.so' -exec dirname '{}' ';' | sort -u > /etc/ld.so.conf.d/docker-openjdk.conf;     ldconfig;     java -Xshare:dump;
# Fri, 04 Nov 2022 22:41:34 GMT
RUN echo Verifying install ...     && fileEncoding="$(echo 'System.out.println(System.getProperty("file.encoding"))' | jshell -s -)"; [ "$fileEncoding" = 'UTF-8' ]; rm -rf ~/.java     && echo java --version && java --version     && echo Complete.
# Fri, 04 Nov 2022 23:48:38 GMT
ENV CATALINA_HOME=/usr/local/tomcat
# Fri, 04 Nov 2022 23:48:38 GMT
ENV PATH=/usr/local/tomcat/bin:/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Fri, 04 Nov 2022 23:48:38 GMT
RUN mkdir -p "$CATALINA_HOME"
# Fri, 04 Nov 2022 23:48:39 GMT
WORKDIR /usr/local/tomcat
# Fri, 04 Nov 2022 23:48:39 GMT
ENV TOMCAT_NATIVE_LIBDIR=/usr/local/tomcat/native-jni-lib
# Fri, 04 Nov 2022 23:48:39 GMT
ENV LD_LIBRARY_PATH=/usr/local/tomcat/native-jni-lib
# Fri, 04 Nov 2022 23:53:12 GMT
ENV GPG_KEYS=48F8E69F6390C9F25CFEDCD268248959359E722B A9C5DF4D22E99998D9875A5110C01C5A2F6059E7 DCFD35E0BF8CA7344752DE8B6FB21E8933C60243
# Fri, 04 Nov 2022 23:53:12 GMT
ENV TOMCAT_MAJOR=9
# Tue, 15 Nov 2022 04:57:22 GMT
ENV TOMCAT_VERSION=9.0.69
# Tue, 15 Nov 2022 04:57:22 GMT
ENV TOMCAT_SHA512=8c883c54ce9ce43eba37756a6404cdf3477879883a3e6d146dc8a7aa5e0425f487466afe6b6da4a895927cb7cb59177b9379cec18000f2de12785be57408c779
# Tue, 15 Nov 2022 04:57:22 GMT
COPY dir:096b403a5f78b17e6b4bff63128a9c93941b97f22470991610dd641633d977f1 in /usr/local/tomcat 
# Tue, 15 Nov 2022 04:57:25 GMT
RUN set -eux; 	apt-get update; 	xargs -rt apt-get install -y --no-install-recommends < "$TOMCAT_NATIVE_LIBDIR/.dependencies.txt"; 	rm -rf /var/lib/apt/lists/*
# Tue, 15 Nov 2022 04:57:26 GMT
RUN set -eux; 	nativeLines="$(catalina.sh configtest 2>&1)"; 	nativeLines="$(echo "$nativeLines" | grep 'Apache Tomcat Native')"; 	nativeLines="$(echo "$nativeLines" | sort -u)"; 	if ! echo "$nativeLines" | grep -E 'INFO: Loaded( APR based)? Apache Tomcat Native library' >&2; then 		echo >&2 "$nativeLines"; 		exit 1; 	fi
# Tue, 15 Nov 2022 04:57:26 GMT
EXPOSE 8080
# Tue, 15 Nov 2022 04:57:27 GMT
CMD ["catalina.sh" "run"]
# Wed, 11 Jan 2023 03:05:10 GMT
LABEL org.opencontainers.image.authors=XWiki Development Team <committers@xwiki.org>
# Wed, 11 Jan 2023 03:05:10 GMT
LABEL org.opencontainers.image.url=https://hub.docker.com/_/xwiki
# Wed, 11 Jan 2023 03:05:10 GMT
LABEL org.opencontainers.image.documentation=https://hub.docker.com/_/xwiki
# Wed, 11 Jan 2023 03:05:10 GMT
LABEL org.opencontainers.image.source=https://github.com/xwiki/xwiki-docker.git
# Wed, 11 Jan 2023 03:05:11 GMT
LABEL org.opencontainers.image.vendor=xwiki.org
# Wed, 11 Jan 2023 03:05:11 GMT
LABEL org.opencontainers.image.licenses=LGPL-2.1
# Wed, 11 Jan 2023 03:07:37 GMT
RUN apt-get update &&   apt-get --no-install-recommends -y install     curl     libreoffice     unzip     procps &&   rm -rf /var/lib/apt/lists/*
# Wed, 01 Feb 2023 22:26:19 GMT
ENV XWIKI_VERSION=14.10.4
# Wed, 01 Feb 2023 22:26:19 GMT
ENV XWIKI_URL_PREFIX=https://maven.xwiki.org/releases/org/xwiki/platform/xwiki-platform-distribution-war/14.10.4
# Wed, 01 Feb 2023 22:26:19 GMT
ENV XWIKI_DOWNLOAD_SHA256=2fcfb622319172c2e424b9c11848ebfabe27cf8ef69cba39ceb5d124b7ebe713
# Wed, 01 Feb 2023 22:27:00 GMT
RUN rm -rf /usr/local/tomcat/webapps/* &&   mkdir -p /usr/local/tomcat/temp &&   mkdir -p /usr/local/xwiki/data &&   curl -fSL "${XWIKI_URL_PREFIX}/xwiki-platform-distribution-war-${XWIKI_VERSION}.war" -o xwiki.war &&   echo "$XWIKI_DOWNLOAD_SHA256 xwiki.war" | sha256sum -c - &&   unzip -d /usr/local/tomcat/webapps/ROOT xwiki.war &&   rm -f xwiki.war
# Wed, 01 Feb 2023 22:27:55 GMT
ENV MARIADB_JDBC_VERSION=3.1.1
# Wed, 01 Feb 2023 22:27:55 GMT
ENV MARIADB_JDBC_SHA256=a554541fd88047905fb0c4c10e1d85295f5e38c7bb5fb408b425392a79fc26e3
# Wed, 01 Feb 2023 22:27:55 GMT
ENV MARIADB_JDBC_PREFIX=https://repo1.maven.org/maven2/org/mariadb/jdbc/mariadb-java-client/3.1.1
# Wed, 01 Feb 2023 22:27:55 GMT
ENV MARIADB_JDBC_ARTIFACT=mariadb-java-client-3.1.1.jar
# Wed, 01 Feb 2023 22:27:55 GMT
ENV MARIADB_JDBC_TARGET=/usr/local/tomcat/webapps/ROOT/WEB-INF/lib/mariadb-java-client-3.1.1.jar
# Wed, 01 Feb 2023 22:27:56 GMT
RUN curl -fSL "${MARIADB_JDBC_PREFIX}/${MARIADB_JDBC_ARTIFACT}" -o $MARIADB_JDBC_TARGET &&   echo "$MARIADB_JDBC_SHA256 $MARIADB_JDBC_TARGET" | sha256sum -c -
# Wed, 01 Feb 2023 22:27:56 GMT
COPY file:0a1be11e2eb610a1dbcd415404e3a592641110b93090030cb831e3a19a163017 in /usr/local/tomcat/bin/ 
# Wed, 01 Feb 2023 22:27:56 GMT
COPY file:0e237c3876eeb3b5f3473a064d3e507da2df6c228ca714687930b34e3b687601 in /usr/local/tomcat/webapps/ROOT/WEB-INF/hibernate.cfg.xml 
# Wed, 01 Feb 2023 22:27:57 GMT
RUN sed -i 's/<id>org.xwiki.platform:xwiki-platform-distribution-war/<id>org.xwiki.platform:xwiki-platform-distribution-docker/'   /usr/local/tomcat/webapps/ROOT/META-INF/extension.xed
# Wed, 01 Feb 2023 22:27:57 GMT
COPY file:a47c4dcd87c9dad97aff38c49188357e6193bcad50757e516cfb08a60d4de611 in /usr/local/bin/docker-entrypoint.sh 
# Wed, 01 Feb 2023 22:27:57 GMT
VOLUME [/usr/local/xwiki]
# Wed, 01 Feb 2023 22:27:57 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 01 Feb 2023 22:27:57 GMT
CMD ["xwiki"]
```

-	Layers:
	-	`sha256:0509fae36eb0656f8bdb23f8ae64100d893bcea2563e97468d337e04d2d0410b`  
		Last Modified: Wed, 02 Nov 2022 18:50:21 GMT  
		Size: 28.4 MB (28382154 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e502a1af2bcd98f5f0d2f5e4da1a0e7bbe07a2c548e2662f7d37dce5ae1df46c`  
		Last Modified: Wed, 02 Nov 2022 19:48:28 GMT  
		Size: 12.4 MB (12396330 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bc4598c07dd818f03a0378b0341a4a8e80f0152fbb3e7d5246ca4f466f42e611`  
		Last Modified: Fri, 04 Nov 2022 22:46:46 GMT  
		Size: 45.0 MB (44958470 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:715a937a1066f998b331fcd62256ad01a5571bdf46804e97825afc64f9ebb427`  
		Last Modified: Fri, 04 Nov 2022 22:46:41 GMT  
		Size: 160.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5fb623f082f74b2fa9fc2c4e3f3a4802875cb9753cfa26ed940201ce72bb56cb`  
		Last Modified: Sat, 05 Nov 2022 00:03:40 GMT  
		Size: 172.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:33260b83200262bbd546be371ad3c1f50f5ae7228afb87982d6fa9d6b11bf26f`  
		Last Modified: Tue, 15 Nov 2022 05:10:19 GMT  
		Size: 12.2 MB (12207235 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0955fb697ea9b30a1b4f95385464f646aa1525cb6efba648e22df84ebef6b2ee`  
		Last Modified: Tue, 15 Nov 2022 05:10:18 GMT  
		Size: 452.0 KB (452021 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6eddcf66f2083b1487296a0308e0b058917c97f614f12428d82d89662038dc2e`  
		Last Modified: Tue, 15 Nov 2022 05:10:18 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ae5f60bb64f3fa11da3d15a9639f886186b4c2c021455c3f9db22e0cfe1b1311`  
		Last Modified: Wed, 11 Jan 2023 03:11:14 GMT  
		Size: 173.8 MB (173806827 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:13334e257ce7313ca9d6028534e3ec6c7858c374c4afedea7f96c51da716806e`  
		Last Modified: Wed, 01 Feb 2023 22:29:16 GMT  
		Size: 307.1 MB (307104849 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a825dc0bda4f4de7842c41ce3db12885844733a8717fc3072c599678278e4b9b`  
		Last Modified: Wed, 01 Feb 2023 22:30:19 GMT  
		Size: 589.7 KB (589668 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0d3b831d82d4e981ad4dd1f4ef4cb7a5b16e7e27fff8121997366b1c93b836b7`  
		Last Modified: Wed, 01 Feb 2023 22:30:19 GMT  
		Size: 1.3 KB (1343 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b4b1db4f27135bc027a5f8478949b1118838f79760f5c779a18756553b080ac0`  
		Last Modified: Wed, 01 Feb 2023 22:30:19 GMT  
		Size: 2.3 KB (2309 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7f634a749b61f1dc714bb14b2b20c7fedd422c285161bdce24613edffc1feaca`  
		Last Modified: Wed, 01 Feb 2023 22:30:19 GMT  
		Size: 6.0 KB (6007 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f68b784196e13fd8e6790aa86b2f5a906f53094387165b175a9b981413e22fe1`  
		Last Modified: Wed, 01 Feb 2023 22:30:20 GMT  
		Size: 2.5 KB (2506 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `xwiki:14-mysql-tomcat`

```console
$ docker pull xwiki@sha256:32e51c9775fda50082b0f02856f2af444a67284446679c9a3a13a78c02ec0c4b
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `xwiki:14-mysql-tomcat` - linux; amd64

```console
$ docker pull xwiki@sha256:a2e996a399fc68cbccfe11eaeb0115a15314bd69f06c483fef3cba244fa07cbf
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **590.4 MB (590449604 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:6b73fd725d5c1dd8044289fdb0e76f973e7e1d4a64e1efc44428235a718b550a`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["xwiki"]`

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
# Wed, 02 Nov 2022 18:44:10 GMT
RUN apt-get update     && DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends tzdata curl wget ca-certificates fontconfig locales     && echo "en_US.UTF-8 UTF-8" >> /etc/locale.gen     && locale-gen en_US.UTF-8     && rm -rf /var/lib/apt/lists/*
# Fri, 04 Nov 2022 23:21:41 GMT
ENV JAVA_VERSION=jdk-11.0.17+8
# Fri, 04 Nov 2022 23:22:31 GMT
RUN set -eux;     ARCH="$(dpkg --print-architecture)";     case "${ARCH}" in        aarch64|arm64)          ESUM='bd6efe3290c8b5a42f695a55a26f3e3c9c284288574879d4b7089f31f5114177';          BINARY_URL='https://github.com/adoptium/temurin11-binaries/releases/download/jdk-11.0.17%2B8/OpenJDK11U-jre_aarch64_linux_hotspot_11.0.17_8.tar.gz';          ;;        armhf|arm)          ESUM='8cf113d3d7fa808895c8d2e41bb890af21c47e38c2460e0588147a4bb8fc658d';          BINARY_URL='https://github.com/adoptium/temurin11-binaries/releases/download/jdk-11.0.17%2B8/OpenJDK11U-jre_arm_linux_hotspot_11.0.17_8.tar.gz';          ;;        ppc64el|powerpc:common64)          ESUM='0ca3d806131ab5834c501f9c625bb0248cd528af361c704503348e9c9605bedf';          BINARY_URL='https://github.com/adoptium/temurin11-binaries/releases/download/jdk-11.0.17%2B8/OpenJDK11U-jre_ppc64le_linux_hotspot_11.0.17_8.tar.gz';          ;;        s390x|s390:64-bit)          ESUM='dd3b159a374086e65cb07c4ccb226c90f9c02ef929cba6f0b642171d7ed97fa4';          BINARY_URL='https://github.com/adoptium/temurin11-binaries/releases/download/jdk-11.0.17%2B8/OpenJDK11U-jre_s390x_linux_hotspot_11.0.17_8.tar.gz';          ;;        amd64|i386:x86-64)          ESUM='752616097e09d7f60a3ad8bd312f90eaf50ac72577e55df229fe6e8091148f79';          BINARY_URL='https://github.com/adoptium/temurin11-binaries/releases/download/jdk-11.0.17%2B8/OpenJDK11U-jre_x64_linux_hotspot_11.0.17_8.tar.gz';          ;;        *)          echo "Unsupported arch: ${ARCH}";          exit 1;          ;;     esac; 	  wget -O /tmp/openjdk.tar.gz ${BINARY_URL}; 	  echo "${ESUM} */tmp/openjdk.tar.gz" | sha256sum -c -; 	  mkdir -p "$JAVA_HOME"; 	  tar --extract 	      --file /tmp/openjdk.tar.gz 	      --directory "$JAVA_HOME" 	      --strip-components 1 	      --no-same-owner 	  ;     rm /tmp/openjdk.tar.gz;     find "$JAVA_HOME/lib" -name '*.so' -exec dirname '{}' ';' | sort -u > /etc/ld.so.conf.d/docker-openjdk.conf;     ldconfig;     java -Xshare:dump;
# Fri, 04 Nov 2022 23:22:32 GMT
RUN echo Verifying install ...     && fileEncoding="$(echo 'System.out.println(System.getProperty("file.encoding"))' | jshell -s -)"; [ "$fileEncoding" = 'UTF-8' ]; rm -rf ~/.java     && echo java --version && java --version     && echo Complete.
# Sat, 05 Nov 2022 01:35:16 GMT
ENV CATALINA_HOME=/usr/local/tomcat
# Sat, 05 Nov 2022 01:35:16 GMT
ENV PATH=/usr/local/tomcat/bin:/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Sat, 05 Nov 2022 01:35:17 GMT
RUN mkdir -p "$CATALINA_HOME"
# Sat, 05 Nov 2022 01:35:17 GMT
WORKDIR /usr/local/tomcat
# Sat, 05 Nov 2022 01:35:17 GMT
ENV TOMCAT_NATIVE_LIBDIR=/usr/local/tomcat/native-jni-lib
# Sat, 05 Nov 2022 01:35:17 GMT
ENV LD_LIBRARY_PATH=/usr/local/tomcat/native-jni-lib
# Sat, 05 Nov 2022 01:39:54 GMT
ENV GPG_KEYS=48F8E69F6390C9F25CFEDCD268248959359E722B A9C5DF4D22E99998D9875A5110C01C5A2F6059E7 DCFD35E0BF8CA7344752DE8B6FB21E8933C60243
# Sat, 05 Nov 2022 01:39:54 GMT
ENV TOMCAT_MAJOR=9
# Tue, 15 Nov 2022 03:06:43 GMT
ENV TOMCAT_VERSION=9.0.69
# Tue, 15 Nov 2022 03:06:43 GMT
ENV TOMCAT_SHA512=8c883c54ce9ce43eba37756a6404cdf3477879883a3e6d146dc8a7aa5e0425f487466afe6b6da4a895927cb7cb59177b9379cec18000f2de12785be57408c779
# Tue, 15 Nov 2022 03:06:44 GMT
COPY dir:b1a33aa3993dbbfbebb33bd9aa546b60c2f2191abf1227f453d4e830f6deb35f in /usr/local/tomcat 
# Tue, 15 Nov 2022 03:06:48 GMT
RUN set -eux; 	apt-get update; 	xargs -rt apt-get install -y --no-install-recommends < "$TOMCAT_NATIVE_LIBDIR/.dependencies.txt"; 	rm -rf /var/lib/apt/lists/*
# Tue, 15 Nov 2022 03:06:49 GMT
RUN set -eux; 	nativeLines="$(catalina.sh configtest 2>&1)"; 	nativeLines="$(echo "$nativeLines" | grep 'Apache Tomcat Native')"; 	nativeLines="$(echo "$nativeLines" | sort -u)"; 	if ! echo "$nativeLines" | grep -E 'INFO: Loaded( APR based)? Apache Tomcat Native library' >&2; then 		echo >&2 "$nativeLines"; 		exit 1; 	fi
# Tue, 15 Nov 2022 03:06:49 GMT
EXPOSE 8080
# Tue, 15 Nov 2022 03:06:49 GMT
CMD ["catalina.sh" "run"]
# Wed, 11 Jan 2023 02:47:03 GMT
LABEL org.opencontainers.image.authors=XWiki Development Team <committers@xwiki.org>
# Wed, 11 Jan 2023 02:47:03 GMT
LABEL org.opencontainers.image.url=https://hub.docker.com/_/xwiki
# Wed, 11 Jan 2023 02:47:03 GMT
LABEL org.opencontainers.image.documentation=https://hub.docker.com/_/xwiki
# Wed, 11 Jan 2023 02:47:03 GMT
LABEL org.opencontainers.image.source=https://github.com/xwiki/xwiki-docker.git
# Wed, 11 Jan 2023 02:47:04 GMT
LABEL org.opencontainers.image.vendor=xwiki.org
# Wed, 11 Jan 2023 02:47:04 GMT
LABEL org.opencontainers.image.licenses=LGPL-2.1
# Wed, 11 Jan 2023 02:49:03 GMT
RUN apt-get update &&   apt-get --no-install-recommends -y install     curl     libreoffice     unzip     procps &&   rm -rf /var/lib/apt/lists/*
# Wed, 22 Feb 2023 18:39:36 GMT
ENV XWIKI_VERSION=14.10.5
# Wed, 22 Feb 2023 18:39:36 GMT
ENV XWIKI_URL_PREFIX=https://maven.xwiki.org/releases/org/xwiki/platform/xwiki-platform-distribution-war/14.10.5
# Wed, 22 Feb 2023 18:39:36 GMT
ENV XWIKI_DOWNLOAD_SHA256=f58465d0869e4c5605ae8375a09c79399d1149c7131fed3cf9959918267eb6a8
# Wed, 22 Feb 2023 18:40:15 GMT
RUN rm -rf /usr/local/tomcat/webapps/* &&   mkdir -p /usr/local/tomcat/temp &&   mkdir -p /usr/local/xwiki/data &&   curl -fSL "${XWIKI_URL_PREFIX}/xwiki-platform-distribution-war-${XWIKI_VERSION}.war" -o xwiki.war &&   echo "$XWIKI_DOWNLOAD_SHA256 xwiki.war" | sha256sum -c - &&   unzip -d /usr/local/tomcat/webapps/ROOT xwiki.war &&   rm -f xwiki.war
# Wed, 22 Feb 2023 18:40:17 GMT
ENV MYSQL_JDBC_VERSION=8.0.32
# Wed, 22 Feb 2023 18:40:17 GMT
ENV MYSQL_JDBC_SHA256=522329fe925980f02e5eb89b59d227245d345415ff0c08932a68c9765c13acc5
# Wed, 22 Feb 2023 18:40:17 GMT
ENV MYSQL_JDBC_PREFIX=https://repo1.maven.org/maven2/com/mysql/mysql-connector-j/8.0.32
# Wed, 22 Feb 2023 18:40:17 GMT
ENV MYSQL_JDBC_ARTIFACT=mysql-connector-j-8.0.32.jar
# Wed, 22 Feb 2023 18:40:17 GMT
ENV MYSQL_JDBC_TARGET=/usr/local/tomcat/webapps/ROOT/WEB-INF/lib/mysql-connector-j-8.0.32.jar
# Wed, 22 Feb 2023 18:40:18 GMT
RUN curl -fSL "${MYSQL_JDBC_PREFIX}/${MYSQL_JDBC_ARTIFACT}" -o $MYSQL_JDBC_TARGET &&   echo "$MYSQL_JDBC_SHA256 $MYSQL_JDBC_TARGET" | sha256sum -c -
# Wed, 22 Feb 2023 18:40:18 GMT
COPY file:0a1be11e2eb610a1dbcd415404e3a592641110b93090030cb831e3a19a163017 in /usr/local/tomcat/bin/ 
# Wed, 22 Feb 2023 18:40:18 GMT
COPY file:1b8409986f3e4eb79a7a0b18472cb2692a61d504fb5ef34292bc997b79fd760d in /usr/local/tomcat/webapps/ROOT/WEB-INF/hibernate.cfg.xml 
# Wed, 22 Feb 2023 18:40:19 GMT
RUN sed -i 's/<id>org.xwiki.platform:xwiki-platform-distribution-war/<id>org.xwiki.platform:xwiki-platform-distribution-docker/'   /usr/local/tomcat/webapps/ROOT/META-INF/extension.xed
# Wed, 22 Feb 2023 18:40:19 GMT
COPY file:a47c4dcd87c9dad97aff38c49188357e6193bcad50757e516cfb08a60d4de611 in /usr/local/bin/docker-entrypoint.sh 
# Wed, 22 Feb 2023 18:40:19 GMT
VOLUME [/usr/local/xwiki]
# Wed, 22 Feb 2023 18:40:19 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 22 Feb 2023 18:40:19 GMT
CMD ["xwiki"]
```

-	Layers:
	-	`sha256:e96e057aae67380a4ddb16c337c5c3669d97fdff69ec537f02aa2cc30d814281`  
		Last Modified: Wed, 02 Nov 2022 03:03:36 GMT  
		Size: 30.4 MB (30425607 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4ced2591451da3a02e2b6bb44752b9e3f00d77789921be4df5082fb9f9880ad0`  
		Last Modified: Wed, 02 Nov 2022 18:48:43 GMT  
		Size: 12.4 MB (12439006 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:df8f874ae8c08a9e69e5fbe6c5a64200a45386132a3203d1a9a7f1146d94cfbc`  
		Last Modified: Fri, 04 Nov 2022 23:29:33 GMT  
		Size: 46.6 MB (46629936 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:111b6c7486426c4b6989102c2ee5be856e8a58e20ab0a350b24a905d536e8e7f`  
		Last Modified: Fri, 04 Nov 2022 23:29:26 GMT  
		Size: 161.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e6f84dce457c6d4f7b7291fce05f8e77998a3a7722a54125a1f1d52ca83043b4`  
		Last Modified: Sat, 05 Nov 2022 01:50:51 GMT  
		Size: 173.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a6c26749ee782392e38845ee2ba79b0da586ef6a45d8e7f29c7af14612278547`  
		Last Modified: Tue, 15 Nov 2022 03:19:57 GMT  
		Size: 12.2 MB (12200249 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4dddc6d9fa6024025b3fcfe729cab2dc544fb25476eca6e80b1af8e8d93bb0ee`  
		Last Modified: Tue, 15 Nov 2022 03:19:56 GMT  
		Size: 452.7 KB (452680 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:06637eebe5e72c8ad9019ad4eb4cdde1f11f7d4c24c7ed7374cf8966343aa2fb`  
		Last Modified: Tue, 15 Nov 2022 03:19:56 GMT  
		Size: 131.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b276fb8390410a8208724033e325715ea26000d5a1a762d4c3699b927884fbfe`  
		Last Modified: Wed, 11 Jan 2023 02:52:45 GMT  
		Size: 178.8 MB (178805608 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:89de9d9e2c09cd5b84430562516cbcd5695a0a3b2347b451e157bde75c2b5619`  
		Last Modified: Wed, 22 Feb 2023 18:42:21 GMT  
		Size: 307.1 MB (307141303 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4a2089179b7c1db514d0502e476e09b8f9313d08d4c4e4f3981be456288fe507`  
		Last Modified: Wed, 22 Feb 2023 18:42:04 GMT  
		Size: 2.3 MB (2342572 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e7c4ef360ff3673244adb3dfc4769b5710fa68fcc1fbe1c08b2f5fa32dbd4976`  
		Last Modified: Wed, 22 Feb 2023 18:42:04 GMT  
		Size: 1.3 KB (1348 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:08441c368d4b01e361491d7fbf1ac579fcc303b8484123c309a8d5a3b6657c46`  
		Last Modified: Wed, 22 Feb 2023 18:42:04 GMT  
		Size: 2.3 KB (2311 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:542b4bb846d438395e458c08de292f72d14d289fae6ffe7eba6fec1cd8518475`  
		Last Modified: Wed, 22 Feb 2023 18:42:04 GMT  
		Size: 6.0 KB (6013 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:039c0305df9e64c69bb546e64f0658dba6e728eee13022cfd682aa1ee76b8b7f`  
		Last Modified: Wed, 22 Feb 2023 18:42:04 GMT  
		Size: 2.5 KB (2506 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `xwiki:14-mysql-tomcat` - linux; arm64 variant v8

```console
$ docker pull xwiki@sha256:33e36167828fe9bae944e7d4cbbe3b69dd2415595d40610ac2ebcd73f2c2fa7f
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **581.7 MB (581697690 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:44013daf43fd09deb7221eef006c4d30d484a03c433118e5b59da0a44b573f06`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["xwiki"]`

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
# Wed, 02 Nov 2022 19:44:32 GMT
RUN apt-get update     && DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends tzdata curl wget ca-certificates fontconfig locales     && echo "en_US.UTF-8 UTF-8" >> /etc/locale.gen     && locale-gen en_US.UTF-8     && rm -rf /var/lib/apt/lists/*
# Fri, 04 Nov 2022 22:40:54 GMT
ENV JAVA_VERSION=jdk-11.0.17+8
# Fri, 04 Nov 2022 22:41:33 GMT
RUN set -eux;     ARCH="$(dpkg --print-architecture)";     case "${ARCH}" in        aarch64|arm64)          ESUM='bd6efe3290c8b5a42f695a55a26f3e3c9c284288574879d4b7089f31f5114177';          BINARY_URL='https://github.com/adoptium/temurin11-binaries/releases/download/jdk-11.0.17%2B8/OpenJDK11U-jre_aarch64_linux_hotspot_11.0.17_8.tar.gz';          ;;        armhf|arm)          ESUM='8cf113d3d7fa808895c8d2e41bb890af21c47e38c2460e0588147a4bb8fc658d';          BINARY_URL='https://github.com/adoptium/temurin11-binaries/releases/download/jdk-11.0.17%2B8/OpenJDK11U-jre_arm_linux_hotspot_11.0.17_8.tar.gz';          ;;        ppc64el|powerpc:common64)          ESUM='0ca3d806131ab5834c501f9c625bb0248cd528af361c704503348e9c9605bedf';          BINARY_URL='https://github.com/adoptium/temurin11-binaries/releases/download/jdk-11.0.17%2B8/OpenJDK11U-jre_ppc64le_linux_hotspot_11.0.17_8.tar.gz';          ;;        s390x|s390:64-bit)          ESUM='dd3b159a374086e65cb07c4ccb226c90f9c02ef929cba6f0b642171d7ed97fa4';          BINARY_URL='https://github.com/adoptium/temurin11-binaries/releases/download/jdk-11.0.17%2B8/OpenJDK11U-jre_s390x_linux_hotspot_11.0.17_8.tar.gz';          ;;        amd64|i386:x86-64)          ESUM='752616097e09d7f60a3ad8bd312f90eaf50ac72577e55df229fe6e8091148f79';          BINARY_URL='https://github.com/adoptium/temurin11-binaries/releases/download/jdk-11.0.17%2B8/OpenJDK11U-jre_x64_linux_hotspot_11.0.17_8.tar.gz';          ;;        *)          echo "Unsupported arch: ${ARCH}";          exit 1;          ;;     esac; 	  wget -O /tmp/openjdk.tar.gz ${BINARY_URL}; 	  echo "${ESUM} */tmp/openjdk.tar.gz" | sha256sum -c -; 	  mkdir -p "$JAVA_HOME"; 	  tar --extract 	      --file /tmp/openjdk.tar.gz 	      --directory "$JAVA_HOME" 	      --strip-components 1 	      --no-same-owner 	  ;     rm /tmp/openjdk.tar.gz;     find "$JAVA_HOME/lib" -name '*.so' -exec dirname '{}' ';' | sort -u > /etc/ld.so.conf.d/docker-openjdk.conf;     ldconfig;     java -Xshare:dump;
# Fri, 04 Nov 2022 22:41:34 GMT
RUN echo Verifying install ...     && fileEncoding="$(echo 'System.out.println(System.getProperty("file.encoding"))' | jshell -s -)"; [ "$fileEncoding" = 'UTF-8' ]; rm -rf ~/.java     && echo java --version && java --version     && echo Complete.
# Fri, 04 Nov 2022 23:48:38 GMT
ENV CATALINA_HOME=/usr/local/tomcat
# Fri, 04 Nov 2022 23:48:38 GMT
ENV PATH=/usr/local/tomcat/bin:/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Fri, 04 Nov 2022 23:48:38 GMT
RUN mkdir -p "$CATALINA_HOME"
# Fri, 04 Nov 2022 23:48:39 GMT
WORKDIR /usr/local/tomcat
# Fri, 04 Nov 2022 23:48:39 GMT
ENV TOMCAT_NATIVE_LIBDIR=/usr/local/tomcat/native-jni-lib
# Fri, 04 Nov 2022 23:48:39 GMT
ENV LD_LIBRARY_PATH=/usr/local/tomcat/native-jni-lib
# Fri, 04 Nov 2022 23:53:12 GMT
ENV GPG_KEYS=48F8E69F6390C9F25CFEDCD268248959359E722B A9C5DF4D22E99998D9875A5110C01C5A2F6059E7 DCFD35E0BF8CA7344752DE8B6FB21E8933C60243
# Fri, 04 Nov 2022 23:53:12 GMT
ENV TOMCAT_MAJOR=9
# Tue, 15 Nov 2022 04:57:22 GMT
ENV TOMCAT_VERSION=9.0.69
# Tue, 15 Nov 2022 04:57:22 GMT
ENV TOMCAT_SHA512=8c883c54ce9ce43eba37756a6404cdf3477879883a3e6d146dc8a7aa5e0425f487466afe6b6da4a895927cb7cb59177b9379cec18000f2de12785be57408c779
# Tue, 15 Nov 2022 04:57:22 GMT
COPY dir:096b403a5f78b17e6b4bff63128a9c93941b97f22470991610dd641633d977f1 in /usr/local/tomcat 
# Tue, 15 Nov 2022 04:57:25 GMT
RUN set -eux; 	apt-get update; 	xargs -rt apt-get install -y --no-install-recommends < "$TOMCAT_NATIVE_LIBDIR/.dependencies.txt"; 	rm -rf /var/lib/apt/lists/*
# Tue, 15 Nov 2022 04:57:26 GMT
RUN set -eux; 	nativeLines="$(catalina.sh configtest 2>&1)"; 	nativeLines="$(echo "$nativeLines" | grep 'Apache Tomcat Native')"; 	nativeLines="$(echo "$nativeLines" | sort -u)"; 	if ! echo "$nativeLines" | grep -E 'INFO: Loaded( APR based)? Apache Tomcat Native library' >&2; then 		echo >&2 "$nativeLines"; 		exit 1; 	fi
# Tue, 15 Nov 2022 04:57:26 GMT
EXPOSE 8080
# Tue, 15 Nov 2022 04:57:27 GMT
CMD ["catalina.sh" "run"]
# Wed, 11 Jan 2023 03:05:10 GMT
LABEL org.opencontainers.image.authors=XWiki Development Team <committers@xwiki.org>
# Wed, 11 Jan 2023 03:05:10 GMT
LABEL org.opencontainers.image.url=https://hub.docker.com/_/xwiki
# Wed, 11 Jan 2023 03:05:10 GMT
LABEL org.opencontainers.image.documentation=https://hub.docker.com/_/xwiki
# Wed, 11 Jan 2023 03:05:10 GMT
LABEL org.opencontainers.image.source=https://github.com/xwiki/xwiki-docker.git
# Wed, 11 Jan 2023 03:05:11 GMT
LABEL org.opencontainers.image.vendor=xwiki.org
# Wed, 11 Jan 2023 03:05:11 GMT
LABEL org.opencontainers.image.licenses=LGPL-2.1
# Wed, 11 Jan 2023 03:07:37 GMT
RUN apt-get update &&   apt-get --no-install-recommends -y install     curl     libreoffice     unzip     procps &&   rm -rf /var/lib/apt/lists/*
# Wed, 01 Feb 2023 22:26:19 GMT
ENV XWIKI_VERSION=14.10.4
# Wed, 01 Feb 2023 22:26:19 GMT
ENV XWIKI_URL_PREFIX=https://maven.xwiki.org/releases/org/xwiki/platform/xwiki-platform-distribution-war/14.10.4
# Wed, 01 Feb 2023 22:26:19 GMT
ENV XWIKI_DOWNLOAD_SHA256=2fcfb622319172c2e424b9c11848ebfabe27cf8ef69cba39ceb5d124b7ebe713
# Wed, 01 Feb 2023 22:27:00 GMT
RUN rm -rf /usr/local/tomcat/webapps/* &&   mkdir -p /usr/local/tomcat/temp &&   mkdir -p /usr/local/xwiki/data &&   curl -fSL "${XWIKI_URL_PREFIX}/xwiki-platform-distribution-war-${XWIKI_VERSION}.war" -o xwiki.war &&   echo "$XWIKI_DOWNLOAD_SHA256 xwiki.war" | sha256sum -c - &&   unzip -d /usr/local/tomcat/webapps/ROOT xwiki.war &&   rm -f xwiki.war
# Wed, 01 Feb 2023 22:27:03 GMT
ENV MYSQL_JDBC_VERSION=8.0.31
# Wed, 01 Feb 2023 22:27:03 GMT
ENV MYSQL_JDBC_SHA256=5249e3dc6d6531b37790e3f61845b96db5e41e891d3d8edb0e2e3a1b53ca2f4f
# Wed, 01 Feb 2023 22:27:03 GMT
ENV MYSQL_JDBC_PREFIX=https://repo1.maven.org/maven2/com/mysql/mysql-connector-j/8.0.31
# Wed, 01 Feb 2023 22:27:03 GMT
ENV MYSQL_JDBC_ARTIFACT=mysql-connector-j-8.0.31.jar
# Wed, 01 Feb 2023 22:27:03 GMT
ENV MYSQL_JDBC_TARGET=/usr/local/tomcat/webapps/ROOT/WEB-INF/lib/mysql-connector-j-8.0.31.jar
# Wed, 01 Feb 2023 22:27:04 GMT
RUN curl -fSL "${MYSQL_JDBC_PREFIX}/${MYSQL_JDBC_ARTIFACT}" -o $MYSQL_JDBC_TARGET &&   echo "$MYSQL_JDBC_SHA256 $MYSQL_JDBC_TARGET" | sha256sum -c -
# Wed, 01 Feb 2023 22:27:04 GMT
COPY file:0a1be11e2eb610a1dbcd415404e3a592641110b93090030cb831e3a19a163017 in /usr/local/tomcat/bin/ 
# Wed, 01 Feb 2023 22:27:04 GMT
COPY file:1b8409986f3e4eb79a7a0b18472cb2692a61d504fb5ef34292bc997b79fd760d in /usr/local/tomcat/webapps/ROOT/WEB-INF/hibernate.cfg.xml 
# Wed, 01 Feb 2023 22:27:05 GMT
RUN sed -i 's/<id>org.xwiki.platform:xwiki-platform-distribution-war/<id>org.xwiki.platform:xwiki-platform-distribution-docker/'   /usr/local/tomcat/webapps/ROOT/META-INF/extension.xed
# Wed, 01 Feb 2023 22:27:05 GMT
COPY file:a47c4dcd87c9dad97aff38c49188357e6193bcad50757e516cfb08a60d4de611 in /usr/local/bin/docker-entrypoint.sh 
# Wed, 01 Feb 2023 22:27:05 GMT
VOLUME [/usr/local/xwiki]
# Wed, 01 Feb 2023 22:27:05 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 01 Feb 2023 22:27:05 GMT
CMD ["xwiki"]
```

-	Layers:
	-	`sha256:0509fae36eb0656f8bdb23f8ae64100d893bcea2563e97468d337e04d2d0410b`  
		Last Modified: Wed, 02 Nov 2022 18:50:21 GMT  
		Size: 28.4 MB (28382154 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e502a1af2bcd98f5f0d2f5e4da1a0e7bbe07a2c548e2662f7d37dce5ae1df46c`  
		Last Modified: Wed, 02 Nov 2022 19:48:28 GMT  
		Size: 12.4 MB (12396330 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bc4598c07dd818f03a0378b0341a4a8e80f0152fbb3e7d5246ca4f466f42e611`  
		Last Modified: Fri, 04 Nov 2022 22:46:46 GMT  
		Size: 45.0 MB (44958470 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:715a937a1066f998b331fcd62256ad01a5571bdf46804e97825afc64f9ebb427`  
		Last Modified: Fri, 04 Nov 2022 22:46:41 GMT  
		Size: 160.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5fb623f082f74b2fa9fc2c4e3f3a4802875cb9753cfa26ed940201ce72bb56cb`  
		Last Modified: Sat, 05 Nov 2022 00:03:40 GMT  
		Size: 172.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:33260b83200262bbd546be371ad3c1f50f5ae7228afb87982d6fa9d6b11bf26f`  
		Last Modified: Tue, 15 Nov 2022 05:10:19 GMT  
		Size: 12.2 MB (12207235 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0955fb697ea9b30a1b4f95385464f646aa1525cb6efba648e22df84ebef6b2ee`  
		Last Modified: Tue, 15 Nov 2022 05:10:18 GMT  
		Size: 452.0 KB (452021 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6eddcf66f2083b1487296a0308e0b058917c97f614f12428d82d89662038dc2e`  
		Last Modified: Tue, 15 Nov 2022 05:10:18 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ae5f60bb64f3fa11da3d15a9639f886186b4c2c021455c3f9db22e0cfe1b1311`  
		Last Modified: Wed, 11 Jan 2023 03:11:14 GMT  
		Size: 173.8 MB (173806827 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:13334e257ce7313ca9d6028534e3ec6c7858c374c4afedea7f96c51da716806e`  
		Last Modified: Wed, 01 Feb 2023 22:29:16 GMT  
		Size: 307.1 MB (307104849 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ccb59878c7670194b75b6af22dd3908f9ae1a12dc1074f0b5ed156a5e3afdf0a`  
		Last Modified: Wed, 01 Feb 2023 22:29:02 GMT  
		Size: 2.4 MB (2377177 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d3946fb25102529cda96bcad4925905c9b997e442b447675d89066505cbe1026`  
		Last Modified: Wed, 01 Feb 2023 22:29:02 GMT  
		Size: 1.3 KB (1344 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1ba832da71f2ed07bae5269bb37e7ea79724a069ad63032f2af14996893baa37`  
		Last Modified: Wed, 01 Feb 2023 22:29:02 GMT  
		Size: 2.3 KB (2307 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6616193191331001a42a5d452ea69a215bbc414eca5cb00914c359665be5817f`  
		Last Modified: Wed, 01 Feb 2023 22:29:02 GMT  
		Size: 6.0 KB (6009 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6de4b8ce214cd9b76eda5b4955e5abb249a0b0292e8a38d39683e3002d6534bf`  
		Last Modified: Wed, 01 Feb 2023 22:29:03 GMT  
		Size: 2.5 KB (2506 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `xwiki:14-postgres-tomcat`

```console
$ docker pull xwiki@sha256:48a8c82a2dcfa36f6d55a5f3e75d3e2b3aca3f80de56276b35838dc7bcb6a4a6
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `xwiki:14-postgres-tomcat` - linux; amd64

```console
$ docker pull xwiki@sha256:5cd23e4200b4eed664a61d05e3d436d0e372a3e4e985e29cb866dd9dbb573713
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **590.0 MB (589983532 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ab0dc70572c5101e5837a6281e7cb29a2b4dbf26ad0b9c91860a748aeb3360e1`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["xwiki"]`

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
# Wed, 02 Nov 2022 18:44:10 GMT
RUN apt-get update     && DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends tzdata curl wget ca-certificates fontconfig locales     && echo "en_US.UTF-8 UTF-8" >> /etc/locale.gen     && locale-gen en_US.UTF-8     && rm -rf /var/lib/apt/lists/*
# Fri, 04 Nov 2022 23:21:41 GMT
ENV JAVA_VERSION=jdk-11.0.17+8
# Fri, 04 Nov 2022 23:22:31 GMT
RUN set -eux;     ARCH="$(dpkg --print-architecture)";     case "${ARCH}" in        aarch64|arm64)          ESUM='bd6efe3290c8b5a42f695a55a26f3e3c9c284288574879d4b7089f31f5114177';          BINARY_URL='https://github.com/adoptium/temurin11-binaries/releases/download/jdk-11.0.17%2B8/OpenJDK11U-jre_aarch64_linux_hotspot_11.0.17_8.tar.gz';          ;;        armhf|arm)          ESUM='8cf113d3d7fa808895c8d2e41bb890af21c47e38c2460e0588147a4bb8fc658d';          BINARY_URL='https://github.com/adoptium/temurin11-binaries/releases/download/jdk-11.0.17%2B8/OpenJDK11U-jre_arm_linux_hotspot_11.0.17_8.tar.gz';          ;;        ppc64el|powerpc:common64)          ESUM='0ca3d806131ab5834c501f9c625bb0248cd528af361c704503348e9c9605bedf';          BINARY_URL='https://github.com/adoptium/temurin11-binaries/releases/download/jdk-11.0.17%2B8/OpenJDK11U-jre_ppc64le_linux_hotspot_11.0.17_8.tar.gz';          ;;        s390x|s390:64-bit)          ESUM='dd3b159a374086e65cb07c4ccb226c90f9c02ef929cba6f0b642171d7ed97fa4';          BINARY_URL='https://github.com/adoptium/temurin11-binaries/releases/download/jdk-11.0.17%2B8/OpenJDK11U-jre_s390x_linux_hotspot_11.0.17_8.tar.gz';          ;;        amd64|i386:x86-64)          ESUM='752616097e09d7f60a3ad8bd312f90eaf50ac72577e55df229fe6e8091148f79';          BINARY_URL='https://github.com/adoptium/temurin11-binaries/releases/download/jdk-11.0.17%2B8/OpenJDK11U-jre_x64_linux_hotspot_11.0.17_8.tar.gz';          ;;        *)          echo "Unsupported arch: ${ARCH}";          exit 1;          ;;     esac; 	  wget -O /tmp/openjdk.tar.gz ${BINARY_URL}; 	  echo "${ESUM} */tmp/openjdk.tar.gz" | sha256sum -c -; 	  mkdir -p "$JAVA_HOME"; 	  tar --extract 	      --file /tmp/openjdk.tar.gz 	      --directory "$JAVA_HOME" 	      --strip-components 1 	      --no-same-owner 	  ;     rm /tmp/openjdk.tar.gz;     find "$JAVA_HOME/lib" -name '*.so' -exec dirname '{}' ';' | sort -u > /etc/ld.so.conf.d/docker-openjdk.conf;     ldconfig;     java -Xshare:dump;
# Fri, 04 Nov 2022 23:22:32 GMT
RUN echo Verifying install ...     && fileEncoding="$(echo 'System.out.println(System.getProperty("file.encoding"))' | jshell -s -)"; [ "$fileEncoding" = 'UTF-8' ]; rm -rf ~/.java     && echo java --version && java --version     && echo Complete.
# Sat, 05 Nov 2022 01:35:16 GMT
ENV CATALINA_HOME=/usr/local/tomcat
# Sat, 05 Nov 2022 01:35:16 GMT
ENV PATH=/usr/local/tomcat/bin:/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Sat, 05 Nov 2022 01:35:17 GMT
RUN mkdir -p "$CATALINA_HOME"
# Sat, 05 Nov 2022 01:35:17 GMT
WORKDIR /usr/local/tomcat
# Sat, 05 Nov 2022 01:35:17 GMT
ENV TOMCAT_NATIVE_LIBDIR=/usr/local/tomcat/native-jni-lib
# Sat, 05 Nov 2022 01:35:17 GMT
ENV LD_LIBRARY_PATH=/usr/local/tomcat/native-jni-lib
# Sat, 05 Nov 2022 01:39:54 GMT
ENV GPG_KEYS=48F8E69F6390C9F25CFEDCD268248959359E722B A9C5DF4D22E99998D9875A5110C01C5A2F6059E7 DCFD35E0BF8CA7344752DE8B6FB21E8933C60243
# Sat, 05 Nov 2022 01:39:54 GMT
ENV TOMCAT_MAJOR=9
# Tue, 15 Nov 2022 03:06:43 GMT
ENV TOMCAT_VERSION=9.0.69
# Tue, 15 Nov 2022 03:06:43 GMT
ENV TOMCAT_SHA512=8c883c54ce9ce43eba37756a6404cdf3477879883a3e6d146dc8a7aa5e0425f487466afe6b6da4a895927cb7cb59177b9379cec18000f2de12785be57408c779
# Tue, 15 Nov 2022 03:06:44 GMT
COPY dir:b1a33aa3993dbbfbebb33bd9aa546b60c2f2191abf1227f453d4e830f6deb35f in /usr/local/tomcat 
# Tue, 15 Nov 2022 03:06:48 GMT
RUN set -eux; 	apt-get update; 	xargs -rt apt-get install -y --no-install-recommends < "$TOMCAT_NATIVE_LIBDIR/.dependencies.txt"; 	rm -rf /var/lib/apt/lists/*
# Tue, 15 Nov 2022 03:06:49 GMT
RUN set -eux; 	nativeLines="$(catalina.sh configtest 2>&1)"; 	nativeLines="$(echo "$nativeLines" | grep 'Apache Tomcat Native')"; 	nativeLines="$(echo "$nativeLines" | sort -u)"; 	if ! echo "$nativeLines" | grep -E 'INFO: Loaded( APR based)? Apache Tomcat Native library' >&2; then 		echo >&2 "$nativeLines"; 		exit 1; 	fi
# Tue, 15 Nov 2022 03:06:49 GMT
EXPOSE 8080
# Tue, 15 Nov 2022 03:06:49 GMT
CMD ["catalina.sh" "run"]
# Wed, 11 Jan 2023 02:47:03 GMT
LABEL org.opencontainers.image.authors=XWiki Development Team <committers@xwiki.org>
# Wed, 11 Jan 2023 02:47:03 GMT
LABEL org.opencontainers.image.url=https://hub.docker.com/_/xwiki
# Wed, 11 Jan 2023 02:47:03 GMT
LABEL org.opencontainers.image.documentation=https://hub.docker.com/_/xwiki
# Wed, 11 Jan 2023 02:47:03 GMT
LABEL org.opencontainers.image.source=https://github.com/xwiki/xwiki-docker.git
# Wed, 11 Jan 2023 02:47:04 GMT
LABEL org.opencontainers.image.vendor=xwiki.org
# Wed, 11 Jan 2023 02:47:04 GMT
LABEL org.opencontainers.image.licenses=LGPL-2.1
# Wed, 11 Jan 2023 02:50:25 GMT
RUN apt-get update &&   apt-get --no-install-recommends -y install     curl     libreoffice     unzip     procps     libpostgresql-jdbc-java &&   rm -rf /var/lib/apt/lists/*
# Wed, 22 Feb 2023 18:40:25 GMT
ENV XWIKI_VERSION=14.10.5
# Wed, 22 Feb 2023 18:40:25 GMT
ENV XWIKI_URL_PREFIX=https://maven.xwiki.org/releases/org/xwiki/platform/xwiki-platform-distribution-war/14.10.5
# Wed, 22 Feb 2023 18:40:25 GMT
ENV XWIKI_DOWNLOAD_SHA256=f58465d0869e4c5605ae8375a09c79399d1149c7131fed3cf9959918267eb6a8
# Wed, 22 Feb 2023 18:41:04 GMT
RUN rm -rf /usr/local/tomcat/webapps/* &&   mkdir -p /usr/local/tomcat/temp &&   mkdir -p /usr/local/xwiki/data &&   curl -fSL "${XWIKI_URL_PREFIX}/xwiki-platform-distribution-war-${XWIKI_VERSION}.war" -o xwiki.war &&   echo "$XWIKI_DOWNLOAD_SHA256 xwiki.war" | sha256sum -c - &&   unzip -d /usr/local/tomcat/webapps/ROOT xwiki.war &&   rm -f xwiki.war
# Wed, 22 Feb 2023 18:41:05 GMT
RUN cp /usr/share/java/postgresql-jdbc4.jar /usr/local/tomcat/webapps/ROOT/WEB-INF/lib/
# Wed, 22 Feb 2023 18:41:05 GMT
COPY file:0a1be11e2eb610a1dbcd415404e3a592641110b93090030cb831e3a19a163017 in /usr/local/tomcat/bin/ 
# Wed, 22 Feb 2023 18:41:05 GMT
COPY file:4a923f484bb29a26630c19e1d617d3bf6aa6ae7c6c4a5561e97b037bcde0847c in /usr/local/tomcat/webapps/ROOT/WEB-INF/hibernate.cfg.xml 
# Wed, 22 Feb 2023 18:41:06 GMT
RUN sed -i 's/<id>org.xwiki.platform:xwiki-platform-distribution-war/<id>org.xwiki.platform:xwiki-platform-distribution-docker/'   /usr/local/tomcat/webapps/ROOT/META-INF/extension.xed
# Wed, 22 Feb 2023 18:41:06 GMT
COPY file:a47c4dcd87c9dad97aff38c49188357e6193bcad50757e516cfb08a60d4de611 in /usr/local/bin/docker-entrypoint.sh 
# Wed, 22 Feb 2023 18:41:06 GMT
VOLUME [/usr/local/xwiki]
# Wed, 22 Feb 2023 18:41:06 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 22 Feb 2023 18:41:06 GMT
CMD ["xwiki"]
```

-	Layers:
	-	`sha256:e96e057aae67380a4ddb16c337c5c3669d97fdff69ec537f02aa2cc30d814281`  
		Last Modified: Wed, 02 Nov 2022 03:03:36 GMT  
		Size: 30.4 MB (30425607 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4ced2591451da3a02e2b6bb44752b9e3f00d77789921be4df5082fb9f9880ad0`  
		Last Modified: Wed, 02 Nov 2022 18:48:43 GMT  
		Size: 12.4 MB (12439006 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:df8f874ae8c08a9e69e5fbe6c5a64200a45386132a3203d1a9a7f1146d94cfbc`  
		Last Modified: Fri, 04 Nov 2022 23:29:33 GMT  
		Size: 46.6 MB (46629936 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:111b6c7486426c4b6989102c2ee5be856e8a58e20ab0a350b24a905d536e8e7f`  
		Last Modified: Fri, 04 Nov 2022 23:29:26 GMT  
		Size: 161.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e6f84dce457c6d4f7b7291fce05f8e77998a3a7722a54125a1f1d52ca83043b4`  
		Last Modified: Sat, 05 Nov 2022 01:50:51 GMT  
		Size: 173.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a6c26749ee782392e38845ee2ba79b0da586ef6a45d8e7f29c7af14612278547`  
		Last Modified: Tue, 15 Nov 2022 03:19:57 GMT  
		Size: 12.2 MB (12200249 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4dddc6d9fa6024025b3fcfe729cab2dc544fb25476eca6e80b1af8e8d93bb0ee`  
		Last Modified: Tue, 15 Nov 2022 03:19:56 GMT  
		Size: 452.7 KB (452680 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:06637eebe5e72c8ad9019ad4eb4cdde1f11f7d4c24c7ed7374cf8966343aa2fb`  
		Last Modified: Tue, 15 Nov 2022 03:19:56 GMT  
		Size: 131.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b57f6f8bcfb0d93b8e21d3068d1f65d3f08dba05c5fab7d4c36e2359317b18c7`  
		Last Modified: Wed, 11 Jan 2023 02:53:53 GMT  
		Size: 179.7 MB (179745182 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b26b00a2f6717a934b9a1b08bac612aaaf57a4cfb4d82db521e7d36755621933`  
		Last Modified: Wed, 22 Feb 2023 18:43:06 GMT  
		Size: 307.1 MB (307141251 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:11801aa48fd913e3278b4d0a512df366a8ef26c1cc3e95a8439a1be90aadfd5a`  
		Last Modified: Wed, 22 Feb 2023 18:42:50 GMT  
		Size: 936.9 KB (936850 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fb4e8755162307a316ff405759f2417dc77e746651f89c83a0477ab19dc7da5d`  
		Last Modified: Wed, 22 Feb 2023 18:42:50 GMT  
		Size: 1.3 KB (1342 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2ba124a3d49367a8e2f46fc2043189f91e2dd282d40a301d9c1f79a705d35e66`  
		Last Modified: Wed, 22 Feb 2023 18:42:50 GMT  
		Size: 2.5 KB (2450 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8f421201132c3966dbb37a473df5922718780304fa03993ef75bb78522d5cafd`  
		Last Modified: Wed, 22 Feb 2023 18:42:50 GMT  
		Size: 6.0 KB (6012 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1b5dc6b32b3d1d9a80058f5ffc684363a0cfadf60ade5875fa37854ec7b46fff`  
		Last Modified: Wed, 22 Feb 2023 18:42:50 GMT  
		Size: 2.5 KB (2502 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `xwiki:14-postgres-tomcat` - linux; arm64 variant v8

```console
$ docker pull xwiki@sha256:e04b6d052b479b648834e5d960deff2f28274834a9dc812b628ccb9a624c53ef
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **581.2 MB (581199952 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:4693188024e4d84ad63e783e3377e2d600a040c344f7f36ab1bff14f5630ffe7`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["xwiki"]`

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
# Wed, 02 Nov 2022 19:44:32 GMT
RUN apt-get update     && DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends tzdata curl wget ca-certificates fontconfig locales     && echo "en_US.UTF-8 UTF-8" >> /etc/locale.gen     && locale-gen en_US.UTF-8     && rm -rf /var/lib/apt/lists/*
# Fri, 04 Nov 2022 22:40:54 GMT
ENV JAVA_VERSION=jdk-11.0.17+8
# Fri, 04 Nov 2022 22:41:33 GMT
RUN set -eux;     ARCH="$(dpkg --print-architecture)";     case "${ARCH}" in        aarch64|arm64)          ESUM='bd6efe3290c8b5a42f695a55a26f3e3c9c284288574879d4b7089f31f5114177';          BINARY_URL='https://github.com/adoptium/temurin11-binaries/releases/download/jdk-11.0.17%2B8/OpenJDK11U-jre_aarch64_linux_hotspot_11.0.17_8.tar.gz';          ;;        armhf|arm)          ESUM='8cf113d3d7fa808895c8d2e41bb890af21c47e38c2460e0588147a4bb8fc658d';          BINARY_URL='https://github.com/adoptium/temurin11-binaries/releases/download/jdk-11.0.17%2B8/OpenJDK11U-jre_arm_linux_hotspot_11.0.17_8.tar.gz';          ;;        ppc64el|powerpc:common64)          ESUM='0ca3d806131ab5834c501f9c625bb0248cd528af361c704503348e9c9605bedf';          BINARY_URL='https://github.com/adoptium/temurin11-binaries/releases/download/jdk-11.0.17%2B8/OpenJDK11U-jre_ppc64le_linux_hotspot_11.0.17_8.tar.gz';          ;;        s390x|s390:64-bit)          ESUM='dd3b159a374086e65cb07c4ccb226c90f9c02ef929cba6f0b642171d7ed97fa4';          BINARY_URL='https://github.com/adoptium/temurin11-binaries/releases/download/jdk-11.0.17%2B8/OpenJDK11U-jre_s390x_linux_hotspot_11.0.17_8.tar.gz';          ;;        amd64|i386:x86-64)          ESUM='752616097e09d7f60a3ad8bd312f90eaf50ac72577e55df229fe6e8091148f79';          BINARY_URL='https://github.com/adoptium/temurin11-binaries/releases/download/jdk-11.0.17%2B8/OpenJDK11U-jre_x64_linux_hotspot_11.0.17_8.tar.gz';          ;;        *)          echo "Unsupported arch: ${ARCH}";          exit 1;          ;;     esac; 	  wget -O /tmp/openjdk.tar.gz ${BINARY_URL}; 	  echo "${ESUM} */tmp/openjdk.tar.gz" | sha256sum -c -; 	  mkdir -p "$JAVA_HOME"; 	  tar --extract 	      --file /tmp/openjdk.tar.gz 	      --directory "$JAVA_HOME" 	      --strip-components 1 	      --no-same-owner 	  ;     rm /tmp/openjdk.tar.gz;     find "$JAVA_HOME/lib" -name '*.so' -exec dirname '{}' ';' | sort -u > /etc/ld.so.conf.d/docker-openjdk.conf;     ldconfig;     java -Xshare:dump;
# Fri, 04 Nov 2022 22:41:34 GMT
RUN echo Verifying install ...     && fileEncoding="$(echo 'System.out.println(System.getProperty("file.encoding"))' | jshell -s -)"; [ "$fileEncoding" = 'UTF-8' ]; rm -rf ~/.java     && echo java --version && java --version     && echo Complete.
# Fri, 04 Nov 2022 23:48:38 GMT
ENV CATALINA_HOME=/usr/local/tomcat
# Fri, 04 Nov 2022 23:48:38 GMT
ENV PATH=/usr/local/tomcat/bin:/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Fri, 04 Nov 2022 23:48:38 GMT
RUN mkdir -p "$CATALINA_HOME"
# Fri, 04 Nov 2022 23:48:39 GMT
WORKDIR /usr/local/tomcat
# Fri, 04 Nov 2022 23:48:39 GMT
ENV TOMCAT_NATIVE_LIBDIR=/usr/local/tomcat/native-jni-lib
# Fri, 04 Nov 2022 23:48:39 GMT
ENV LD_LIBRARY_PATH=/usr/local/tomcat/native-jni-lib
# Fri, 04 Nov 2022 23:53:12 GMT
ENV GPG_KEYS=48F8E69F6390C9F25CFEDCD268248959359E722B A9C5DF4D22E99998D9875A5110C01C5A2F6059E7 DCFD35E0BF8CA7344752DE8B6FB21E8933C60243
# Fri, 04 Nov 2022 23:53:12 GMT
ENV TOMCAT_MAJOR=9
# Tue, 15 Nov 2022 04:57:22 GMT
ENV TOMCAT_VERSION=9.0.69
# Tue, 15 Nov 2022 04:57:22 GMT
ENV TOMCAT_SHA512=8c883c54ce9ce43eba37756a6404cdf3477879883a3e6d146dc8a7aa5e0425f487466afe6b6da4a895927cb7cb59177b9379cec18000f2de12785be57408c779
# Tue, 15 Nov 2022 04:57:22 GMT
COPY dir:096b403a5f78b17e6b4bff63128a9c93941b97f22470991610dd641633d977f1 in /usr/local/tomcat 
# Tue, 15 Nov 2022 04:57:25 GMT
RUN set -eux; 	apt-get update; 	xargs -rt apt-get install -y --no-install-recommends < "$TOMCAT_NATIVE_LIBDIR/.dependencies.txt"; 	rm -rf /var/lib/apt/lists/*
# Tue, 15 Nov 2022 04:57:26 GMT
RUN set -eux; 	nativeLines="$(catalina.sh configtest 2>&1)"; 	nativeLines="$(echo "$nativeLines" | grep 'Apache Tomcat Native')"; 	nativeLines="$(echo "$nativeLines" | sort -u)"; 	if ! echo "$nativeLines" | grep -E 'INFO: Loaded( APR based)? Apache Tomcat Native library' >&2; then 		echo >&2 "$nativeLines"; 		exit 1; 	fi
# Tue, 15 Nov 2022 04:57:26 GMT
EXPOSE 8080
# Tue, 15 Nov 2022 04:57:27 GMT
CMD ["catalina.sh" "run"]
# Wed, 11 Jan 2023 03:05:10 GMT
LABEL org.opencontainers.image.authors=XWiki Development Team <committers@xwiki.org>
# Wed, 11 Jan 2023 03:05:10 GMT
LABEL org.opencontainers.image.url=https://hub.docker.com/_/xwiki
# Wed, 11 Jan 2023 03:05:10 GMT
LABEL org.opencontainers.image.documentation=https://hub.docker.com/_/xwiki
# Wed, 11 Jan 2023 03:05:10 GMT
LABEL org.opencontainers.image.source=https://github.com/xwiki/xwiki-docker.git
# Wed, 11 Jan 2023 03:05:11 GMT
LABEL org.opencontainers.image.vendor=xwiki.org
# Wed, 11 Jan 2023 03:05:11 GMT
LABEL org.opencontainers.image.licenses=LGPL-2.1
# Wed, 11 Jan 2023 03:08:55 GMT
RUN apt-get update &&   apt-get --no-install-recommends -y install     curl     libreoffice     unzip     procps     libpostgresql-jdbc-java &&   rm -rf /var/lib/apt/lists/*
# Wed, 01 Feb 2023 22:27:07 GMT
ENV XWIKI_VERSION=14.10.4
# Wed, 01 Feb 2023 22:27:07 GMT
ENV XWIKI_URL_PREFIX=https://maven.xwiki.org/releases/org/xwiki/platform/xwiki-platform-distribution-war/14.10.4
# Wed, 01 Feb 2023 22:27:07 GMT
ENV XWIKI_DOWNLOAD_SHA256=2fcfb622319172c2e424b9c11848ebfabe27cf8ef69cba39ceb5d124b7ebe713
# Wed, 01 Feb 2023 22:27:47 GMT
RUN rm -rf /usr/local/tomcat/webapps/* &&   mkdir -p /usr/local/tomcat/temp &&   mkdir -p /usr/local/xwiki/data &&   curl -fSL "${XWIKI_URL_PREFIX}/xwiki-platform-distribution-war-${XWIKI_VERSION}.war" -o xwiki.war &&   echo "$XWIKI_DOWNLOAD_SHA256 xwiki.war" | sha256sum -c - &&   unzip -d /usr/local/tomcat/webapps/ROOT xwiki.war &&   rm -f xwiki.war
# Wed, 01 Feb 2023 22:27:50 GMT
RUN cp /usr/share/java/postgresql-jdbc4.jar /usr/local/tomcat/webapps/ROOT/WEB-INF/lib/
# Wed, 01 Feb 2023 22:27:50 GMT
COPY file:0a1be11e2eb610a1dbcd415404e3a592641110b93090030cb831e3a19a163017 in /usr/local/tomcat/bin/ 
# Wed, 01 Feb 2023 22:27:50 GMT
COPY file:4a923f484bb29a26630c19e1d617d3bf6aa6ae7c6c4a5561e97b037bcde0847c in /usr/local/tomcat/webapps/ROOT/WEB-INF/hibernate.cfg.xml 
# Wed, 01 Feb 2023 22:27:50 GMT
RUN sed -i 's/<id>org.xwiki.platform:xwiki-platform-distribution-war/<id>org.xwiki.platform:xwiki-platform-distribution-docker/'   /usr/local/tomcat/webapps/ROOT/META-INF/extension.xed
# Wed, 01 Feb 2023 22:27:50 GMT
COPY file:a47c4dcd87c9dad97aff38c49188357e6193bcad50757e516cfb08a60d4de611 in /usr/local/bin/docker-entrypoint.sh 
# Wed, 01 Feb 2023 22:27:50 GMT
VOLUME [/usr/local/xwiki]
# Wed, 01 Feb 2023 22:27:51 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 01 Feb 2023 22:27:51 GMT
CMD ["xwiki"]
```

-	Layers:
	-	`sha256:0509fae36eb0656f8bdb23f8ae64100d893bcea2563e97468d337e04d2d0410b`  
		Last Modified: Wed, 02 Nov 2022 18:50:21 GMT  
		Size: 28.4 MB (28382154 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e502a1af2bcd98f5f0d2f5e4da1a0e7bbe07a2c548e2662f7d37dce5ae1df46c`  
		Last Modified: Wed, 02 Nov 2022 19:48:28 GMT  
		Size: 12.4 MB (12396330 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bc4598c07dd818f03a0378b0341a4a8e80f0152fbb3e7d5246ca4f466f42e611`  
		Last Modified: Fri, 04 Nov 2022 22:46:46 GMT  
		Size: 45.0 MB (44958470 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:715a937a1066f998b331fcd62256ad01a5571bdf46804e97825afc64f9ebb427`  
		Last Modified: Fri, 04 Nov 2022 22:46:41 GMT  
		Size: 160.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5fb623f082f74b2fa9fc2c4e3f3a4802875cb9753cfa26ed940201ce72bb56cb`  
		Last Modified: Sat, 05 Nov 2022 00:03:40 GMT  
		Size: 172.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:33260b83200262bbd546be371ad3c1f50f5ae7228afb87982d6fa9d6b11bf26f`  
		Last Modified: Tue, 15 Nov 2022 05:10:19 GMT  
		Size: 12.2 MB (12207235 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0955fb697ea9b30a1b4f95385464f646aa1525cb6efba648e22df84ebef6b2ee`  
		Last Modified: Tue, 15 Nov 2022 05:10:18 GMT  
		Size: 452.0 KB (452021 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6eddcf66f2083b1487296a0308e0b058917c97f614f12428d82d89662038dc2e`  
		Last Modified: Tue, 15 Nov 2022 05:10:18 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1ae6a8fce0f2cd131007393c1a4eba9ce9d0501da8406af5c5ce9deb5dc187b8`  
		Last Modified: Wed, 11 Jan 2023 03:12:13 GMT  
		Size: 174.7 MB (174749274 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:64fdf9e1ef0289a65afb558897bc408557b353c604c9e3bd5dfe845ddc54ab93`  
		Last Modified: Wed, 01 Feb 2023 22:30:00 GMT  
		Size: 307.1 MB (307104835 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0eee07814c2c9ef72478213f8e0091378d617e777e157e5f5550dbf992e4a8bb`  
		Last Modified: Wed, 01 Feb 2023 22:29:45 GMT  
		Size: 936.9 KB (936853 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:889aa9ab03d69382e94096e25991f58b06afde5b4238b94ac1136db5337d1028`  
		Last Modified: Wed, 01 Feb 2023 22:29:45 GMT  
		Size: 1.3 KB (1347 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d0d21fec462339352953dc0188b312a1e80154e3e38402e546f0e4200627f5dc`  
		Last Modified: Wed, 01 Feb 2023 22:29:45 GMT  
		Size: 2.5 KB (2455 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9c6493af5a9b0ca2b189b7be35d0f796b0243ab70d7f92a34a7eae40d269c8f3`  
		Last Modified: Wed, 01 Feb 2023 22:29:45 GMT  
		Size: 6.0 KB (6011 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3a5f6da30b6a4dcd443e582890b4a323952b0320b4c3474d31c01236b8f4cf5e`  
		Last Modified: Wed, 01 Feb 2023 22:29:45 GMT  
		Size: 2.5 KB (2506 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `xwiki:14.10`

```console
$ docker pull xwiki@sha256:32e51c9775fda50082b0f02856f2af444a67284446679c9a3a13a78c02ec0c4b
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `xwiki:14.10` - linux; amd64

```console
$ docker pull xwiki@sha256:a2e996a399fc68cbccfe11eaeb0115a15314bd69f06c483fef3cba244fa07cbf
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **590.4 MB (590449604 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:6b73fd725d5c1dd8044289fdb0e76f973e7e1d4a64e1efc44428235a718b550a`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["xwiki"]`

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
# Wed, 02 Nov 2022 18:44:10 GMT
RUN apt-get update     && DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends tzdata curl wget ca-certificates fontconfig locales     && echo "en_US.UTF-8 UTF-8" >> /etc/locale.gen     && locale-gen en_US.UTF-8     && rm -rf /var/lib/apt/lists/*
# Fri, 04 Nov 2022 23:21:41 GMT
ENV JAVA_VERSION=jdk-11.0.17+8
# Fri, 04 Nov 2022 23:22:31 GMT
RUN set -eux;     ARCH="$(dpkg --print-architecture)";     case "${ARCH}" in        aarch64|arm64)          ESUM='bd6efe3290c8b5a42f695a55a26f3e3c9c284288574879d4b7089f31f5114177';          BINARY_URL='https://github.com/adoptium/temurin11-binaries/releases/download/jdk-11.0.17%2B8/OpenJDK11U-jre_aarch64_linux_hotspot_11.0.17_8.tar.gz';          ;;        armhf|arm)          ESUM='8cf113d3d7fa808895c8d2e41bb890af21c47e38c2460e0588147a4bb8fc658d';          BINARY_URL='https://github.com/adoptium/temurin11-binaries/releases/download/jdk-11.0.17%2B8/OpenJDK11U-jre_arm_linux_hotspot_11.0.17_8.tar.gz';          ;;        ppc64el|powerpc:common64)          ESUM='0ca3d806131ab5834c501f9c625bb0248cd528af361c704503348e9c9605bedf';          BINARY_URL='https://github.com/adoptium/temurin11-binaries/releases/download/jdk-11.0.17%2B8/OpenJDK11U-jre_ppc64le_linux_hotspot_11.0.17_8.tar.gz';          ;;        s390x|s390:64-bit)          ESUM='dd3b159a374086e65cb07c4ccb226c90f9c02ef929cba6f0b642171d7ed97fa4';          BINARY_URL='https://github.com/adoptium/temurin11-binaries/releases/download/jdk-11.0.17%2B8/OpenJDK11U-jre_s390x_linux_hotspot_11.0.17_8.tar.gz';          ;;        amd64|i386:x86-64)          ESUM='752616097e09d7f60a3ad8bd312f90eaf50ac72577e55df229fe6e8091148f79';          BINARY_URL='https://github.com/adoptium/temurin11-binaries/releases/download/jdk-11.0.17%2B8/OpenJDK11U-jre_x64_linux_hotspot_11.0.17_8.tar.gz';          ;;        *)          echo "Unsupported arch: ${ARCH}";          exit 1;          ;;     esac; 	  wget -O /tmp/openjdk.tar.gz ${BINARY_URL}; 	  echo "${ESUM} */tmp/openjdk.tar.gz" | sha256sum -c -; 	  mkdir -p "$JAVA_HOME"; 	  tar --extract 	      --file /tmp/openjdk.tar.gz 	      --directory "$JAVA_HOME" 	      --strip-components 1 	      --no-same-owner 	  ;     rm /tmp/openjdk.tar.gz;     find "$JAVA_HOME/lib" -name '*.so' -exec dirname '{}' ';' | sort -u > /etc/ld.so.conf.d/docker-openjdk.conf;     ldconfig;     java -Xshare:dump;
# Fri, 04 Nov 2022 23:22:32 GMT
RUN echo Verifying install ...     && fileEncoding="$(echo 'System.out.println(System.getProperty("file.encoding"))' | jshell -s -)"; [ "$fileEncoding" = 'UTF-8' ]; rm -rf ~/.java     && echo java --version && java --version     && echo Complete.
# Sat, 05 Nov 2022 01:35:16 GMT
ENV CATALINA_HOME=/usr/local/tomcat
# Sat, 05 Nov 2022 01:35:16 GMT
ENV PATH=/usr/local/tomcat/bin:/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Sat, 05 Nov 2022 01:35:17 GMT
RUN mkdir -p "$CATALINA_HOME"
# Sat, 05 Nov 2022 01:35:17 GMT
WORKDIR /usr/local/tomcat
# Sat, 05 Nov 2022 01:35:17 GMT
ENV TOMCAT_NATIVE_LIBDIR=/usr/local/tomcat/native-jni-lib
# Sat, 05 Nov 2022 01:35:17 GMT
ENV LD_LIBRARY_PATH=/usr/local/tomcat/native-jni-lib
# Sat, 05 Nov 2022 01:39:54 GMT
ENV GPG_KEYS=48F8E69F6390C9F25CFEDCD268248959359E722B A9C5DF4D22E99998D9875A5110C01C5A2F6059E7 DCFD35E0BF8CA7344752DE8B6FB21E8933C60243
# Sat, 05 Nov 2022 01:39:54 GMT
ENV TOMCAT_MAJOR=9
# Tue, 15 Nov 2022 03:06:43 GMT
ENV TOMCAT_VERSION=9.0.69
# Tue, 15 Nov 2022 03:06:43 GMT
ENV TOMCAT_SHA512=8c883c54ce9ce43eba37756a6404cdf3477879883a3e6d146dc8a7aa5e0425f487466afe6b6da4a895927cb7cb59177b9379cec18000f2de12785be57408c779
# Tue, 15 Nov 2022 03:06:44 GMT
COPY dir:b1a33aa3993dbbfbebb33bd9aa546b60c2f2191abf1227f453d4e830f6deb35f in /usr/local/tomcat 
# Tue, 15 Nov 2022 03:06:48 GMT
RUN set -eux; 	apt-get update; 	xargs -rt apt-get install -y --no-install-recommends < "$TOMCAT_NATIVE_LIBDIR/.dependencies.txt"; 	rm -rf /var/lib/apt/lists/*
# Tue, 15 Nov 2022 03:06:49 GMT
RUN set -eux; 	nativeLines="$(catalina.sh configtest 2>&1)"; 	nativeLines="$(echo "$nativeLines" | grep 'Apache Tomcat Native')"; 	nativeLines="$(echo "$nativeLines" | sort -u)"; 	if ! echo "$nativeLines" | grep -E 'INFO: Loaded( APR based)? Apache Tomcat Native library' >&2; then 		echo >&2 "$nativeLines"; 		exit 1; 	fi
# Tue, 15 Nov 2022 03:06:49 GMT
EXPOSE 8080
# Tue, 15 Nov 2022 03:06:49 GMT
CMD ["catalina.sh" "run"]
# Wed, 11 Jan 2023 02:47:03 GMT
LABEL org.opencontainers.image.authors=XWiki Development Team <committers@xwiki.org>
# Wed, 11 Jan 2023 02:47:03 GMT
LABEL org.opencontainers.image.url=https://hub.docker.com/_/xwiki
# Wed, 11 Jan 2023 02:47:03 GMT
LABEL org.opencontainers.image.documentation=https://hub.docker.com/_/xwiki
# Wed, 11 Jan 2023 02:47:03 GMT
LABEL org.opencontainers.image.source=https://github.com/xwiki/xwiki-docker.git
# Wed, 11 Jan 2023 02:47:04 GMT
LABEL org.opencontainers.image.vendor=xwiki.org
# Wed, 11 Jan 2023 02:47:04 GMT
LABEL org.opencontainers.image.licenses=LGPL-2.1
# Wed, 11 Jan 2023 02:49:03 GMT
RUN apt-get update &&   apt-get --no-install-recommends -y install     curl     libreoffice     unzip     procps &&   rm -rf /var/lib/apt/lists/*
# Wed, 22 Feb 2023 18:39:36 GMT
ENV XWIKI_VERSION=14.10.5
# Wed, 22 Feb 2023 18:39:36 GMT
ENV XWIKI_URL_PREFIX=https://maven.xwiki.org/releases/org/xwiki/platform/xwiki-platform-distribution-war/14.10.5
# Wed, 22 Feb 2023 18:39:36 GMT
ENV XWIKI_DOWNLOAD_SHA256=f58465d0869e4c5605ae8375a09c79399d1149c7131fed3cf9959918267eb6a8
# Wed, 22 Feb 2023 18:40:15 GMT
RUN rm -rf /usr/local/tomcat/webapps/* &&   mkdir -p /usr/local/tomcat/temp &&   mkdir -p /usr/local/xwiki/data &&   curl -fSL "${XWIKI_URL_PREFIX}/xwiki-platform-distribution-war-${XWIKI_VERSION}.war" -o xwiki.war &&   echo "$XWIKI_DOWNLOAD_SHA256 xwiki.war" | sha256sum -c - &&   unzip -d /usr/local/tomcat/webapps/ROOT xwiki.war &&   rm -f xwiki.war
# Wed, 22 Feb 2023 18:40:17 GMT
ENV MYSQL_JDBC_VERSION=8.0.32
# Wed, 22 Feb 2023 18:40:17 GMT
ENV MYSQL_JDBC_SHA256=522329fe925980f02e5eb89b59d227245d345415ff0c08932a68c9765c13acc5
# Wed, 22 Feb 2023 18:40:17 GMT
ENV MYSQL_JDBC_PREFIX=https://repo1.maven.org/maven2/com/mysql/mysql-connector-j/8.0.32
# Wed, 22 Feb 2023 18:40:17 GMT
ENV MYSQL_JDBC_ARTIFACT=mysql-connector-j-8.0.32.jar
# Wed, 22 Feb 2023 18:40:17 GMT
ENV MYSQL_JDBC_TARGET=/usr/local/tomcat/webapps/ROOT/WEB-INF/lib/mysql-connector-j-8.0.32.jar
# Wed, 22 Feb 2023 18:40:18 GMT
RUN curl -fSL "${MYSQL_JDBC_PREFIX}/${MYSQL_JDBC_ARTIFACT}" -o $MYSQL_JDBC_TARGET &&   echo "$MYSQL_JDBC_SHA256 $MYSQL_JDBC_TARGET" | sha256sum -c -
# Wed, 22 Feb 2023 18:40:18 GMT
COPY file:0a1be11e2eb610a1dbcd415404e3a592641110b93090030cb831e3a19a163017 in /usr/local/tomcat/bin/ 
# Wed, 22 Feb 2023 18:40:18 GMT
COPY file:1b8409986f3e4eb79a7a0b18472cb2692a61d504fb5ef34292bc997b79fd760d in /usr/local/tomcat/webapps/ROOT/WEB-INF/hibernate.cfg.xml 
# Wed, 22 Feb 2023 18:40:19 GMT
RUN sed -i 's/<id>org.xwiki.platform:xwiki-platform-distribution-war/<id>org.xwiki.platform:xwiki-platform-distribution-docker/'   /usr/local/tomcat/webapps/ROOT/META-INF/extension.xed
# Wed, 22 Feb 2023 18:40:19 GMT
COPY file:a47c4dcd87c9dad97aff38c49188357e6193bcad50757e516cfb08a60d4de611 in /usr/local/bin/docker-entrypoint.sh 
# Wed, 22 Feb 2023 18:40:19 GMT
VOLUME [/usr/local/xwiki]
# Wed, 22 Feb 2023 18:40:19 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 22 Feb 2023 18:40:19 GMT
CMD ["xwiki"]
```

-	Layers:
	-	`sha256:e96e057aae67380a4ddb16c337c5c3669d97fdff69ec537f02aa2cc30d814281`  
		Last Modified: Wed, 02 Nov 2022 03:03:36 GMT  
		Size: 30.4 MB (30425607 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4ced2591451da3a02e2b6bb44752b9e3f00d77789921be4df5082fb9f9880ad0`  
		Last Modified: Wed, 02 Nov 2022 18:48:43 GMT  
		Size: 12.4 MB (12439006 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:df8f874ae8c08a9e69e5fbe6c5a64200a45386132a3203d1a9a7f1146d94cfbc`  
		Last Modified: Fri, 04 Nov 2022 23:29:33 GMT  
		Size: 46.6 MB (46629936 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:111b6c7486426c4b6989102c2ee5be856e8a58e20ab0a350b24a905d536e8e7f`  
		Last Modified: Fri, 04 Nov 2022 23:29:26 GMT  
		Size: 161.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e6f84dce457c6d4f7b7291fce05f8e77998a3a7722a54125a1f1d52ca83043b4`  
		Last Modified: Sat, 05 Nov 2022 01:50:51 GMT  
		Size: 173.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a6c26749ee782392e38845ee2ba79b0da586ef6a45d8e7f29c7af14612278547`  
		Last Modified: Tue, 15 Nov 2022 03:19:57 GMT  
		Size: 12.2 MB (12200249 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4dddc6d9fa6024025b3fcfe729cab2dc544fb25476eca6e80b1af8e8d93bb0ee`  
		Last Modified: Tue, 15 Nov 2022 03:19:56 GMT  
		Size: 452.7 KB (452680 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:06637eebe5e72c8ad9019ad4eb4cdde1f11f7d4c24c7ed7374cf8966343aa2fb`  
		Last Modified: Tue, 15 Nov 2022 03:19:56 GMT  
		Size: 131.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b276fb8390410a8208724033e325715ea26000d5a1a762d4c3699b927884fbfe`  
		Last Modified: Wed, 11 Jan 2023 02:52:45 GMT  
		Size: 178.8 MB (178805608 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:89de9d9e2c09cd5b84430562516cbcd5695a0a3b2347b451e157bde75c2b5619`  
		Last Modified: Wed, 22 Feb 2023 18:42:21 GMT  
		Size: 307.1 MB (307141303 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4a2089179b7c1db514d0502e476e09b8f9313d08d4c4e4f3981be456288fe507`  
		Last Modified: Wed, 22 Feb 2023 18:42:04 GMT  
		Size: 2.3 MB (2342572 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e7c4ef360ff3673244adb3dfc4769b5710fa68fcc1fbe1c08b2f5fa32dbd4976`  
		Last Modified: Wed, 22 Feb 2023 18:42:04 GMT  
		Size: 1.3 KB (1348 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:08441c368d4b01e361491d7fbf1ac579fcc303b8484123c309a8d5a3b6657c46`  
		Last Modified: Wed, 22 Feb 2023 18:42:04 GMT  
		Size: 2.3 KB (2311 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:542b4bb846d438395e458c08de292f72d14d289fae6ffe7eba6fec1cd8518475`  
		Last Modified: Wed, 22 Feb 2023 18:42:04 GMT  
		Size: 6.0 KB (6013 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:039c0305df9e64c69bb546e64f0658dba6e728eee13022cfd682aa1ee76b8b7f`  
		Last Modified: Wed, 22 Feb 2023 18:42:04 GMT  
		Size: 2.5 KB (2506 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `xwiki:14.10` - linux; arm64 variant v8

```console
$ docker pull xwiki@sha256:33e36167828fe9bae944e7d4cbbe3b69dd2415595d40610ac2ebcd73f2c2fa7f
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **581.7 MB (581697690 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:44013daf43fd09deb7221eef006c4d30d484a03c433118e5b59da0a44b573f06`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["xwiki"]`

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
# Wed, 02 Nov 2022 19:44:32 GMT
RUN apt-get update     && DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends tzdata curl wget ca-certificates fontconfig locales     && echo "en_US.UTF-8 UTF-8" >> /etc/locale.gen     && locale-gen en_US.UTF-8     && rm -rf /var/lib/apt/lists/*
# Fri, 04 Nov 2022 22:40:54 GMT
ENV JAVA_VERSION=jdk-11.0.17+8
# Fri, 04 Nov 2022 22:41:33 GMT
RUN set -eux;     ARCH="$(dpkg --print-architecture)";     case "${ARCH}" in        aarch64|arm64)          ESUM='bd6efe3290c8b5a42f695a55a26f3e3c9c284288574879d4b7089f31f5114177';          BINARY_URL='https://github.com/adoptium/temurin11-binaries/releases/download/jdk-11.0.17%2B8/OpenJDK11U-jre_aarch64_linux_hotspot_11.0.17_8.tar.gz';          ;;        armhf|arm)          ESUM='8cf113d3d7fa808895c8d2e41bb890af21c47e38c2460e0588147a4bb8fc658d';          BINARY_URL='https://github.com/adoptium/temurin11-binaries/releases/download/jdk-11.0.17%2B8/OpenJDK11U-jre_arm_linux_hotspot_11.0.17_8.tar.gz';          ;;        ppc64el|powerpc:common64)          ESUM='0ca3d806131ab5834c501f9c625bb0248cd528af361c704503348e9c9605bedf';          BINARY_URL='https://github.com/adoptium/temurin11-binaries/releases/download/jdk-11.0.17%2B8/OpenJDK11U-jre_ppc64le_linux_hotspot_11.0.17_8.tar.gz';          ;;        s390x|s390:64-bit)          ESUM='dd3b159a374086e65cb07c4ccb226c90f9c02ef929cba6f0b642171d7ed97fa4';          BINARY_URL='https://github.com/adoptium/temurin11-binaries/releases/download/jdk-11.0.17%2B8/OpenJDK11U-jre_s390x_linux_hotspot_11.0.17_8.tar.gz';          ;;        amd64|i386:x86-64)          ESUM='752616097e09d7f60a3ad8bd312f90eaf50ac72577e55df229fe6e8091148f79';          BINARY_URL='https://github.com/adoptium/temurin11-binaries/releases/download/jdk-11.0.17%2B8/OpenJDK11U-jre_x64_linux_hotspot_11.0.17_8.tar.gz';          ;;        *)          echo "Unsupported arch: ${ARCH}";          exit 1;          ;;     esac; 	  wget -O /tmp/openjdk.tar.gz ${BINARY_URL}; 	  echo "${ESUM} */tmp/openjdk.tar.gz" | sha256sum -c -; 	  mkdir -p "$JAVA_HOME"; 	  tar --extract 	      --file /tmp/openjdk.tar.gz 	      --directory "$JAVA_HOME" 	      --strip-components 1 	      --no-same-owner 	  ;     rm /tmp/openjdk.tar.gz;     find "$JAVA_HOME/lib" -name '*.so' -exec dirname '{}' ';' | sort -u > /etc/ld.so.conf.d/docker-openjdk.conf;     ldconfig;     java -Xshare:dump;
# Fri, 04 Nov 2022 22:41:34 GMT
RUN echo Verifying install ...     && fileEncoding="$(echo 'System.out.println(System.getProperty("file.encoding"))' | jshell -s -)"; [ "$fileEncoding" = 'UTF-8' ]; rm -rf ~/.java     && echo java --version && java --version     && echo Complete.
# Fri, 04 Nov 2022 23:48:38 GMT
ENV CATALINA_HOME=/usr/local/tomcat
# Fri, 04 Nov 2022 23:48:38 GMT
ENV PATH=/usr/local/tomcat/bin:/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Fri, 04 Nov 2022 23:48:38 GMT
RUN mkdir -p "$CATALINA_HOME"
# Fri, 04 Nov 2022 23:48:39 GMT
WORKDIR /usr/local/tomcat
# Fri, 04 Nov 2022 23:48:39 GMT
ENV TOMCAT_NATIVE_LIBDIR=/usr/local/tomcat/native-jni-lib
# Fri, 04 Nov 2022 23:48:39 GMT
ENV LD_LIBRARY_PATH=/usr/local/tomcat/native-jni-lib
# Fri, 04 Nov 2022 23:53:12 GMT
ENV GPG_KEYS=48F8E69F6390C9F25CFEDCD268248959359E722B A9C5DF4D22E99998D9875A5110C01C5A2F6059E7 DCFD35E0BF8CA7344752DE8B6FB21E8933C60243
# Fri, 04 Nov 2022 23:53:12 GMT
ENV TOMCAT_MAJOR=9
# Tue, 15 Nov 2022 04:57:22 GMT
ENV TOMCAT_VERSION=9.0.69
# Tue, 15 Nov 2022 04:57:22 GMT
ENV TOMCAT_SHA512=8c883c54ce9ce43eba37756a6404cdf3477879883a3e6d146dc8a7aa5e0425f487466afe6b6da4a895927cb7cb59177b9379cec18000f2de12785be57408c779
# Tue, 15 Nov 2022 04:57:22 GMT
COPY dir:096b403a5f78b17e6b4bff63128a9c93941b97f22470991610dd641633d977f1 in /usr/local/tomcat 
# Tue, 15 Nov 2022 04:57:25 GMT
RUN set -eux; 	apt-get update; 	xargs -rt apt-get install -y --no-install-recommends < "$TOMCAT_NATIVE_LIBDIR/.dependencies.txt"; 	rm -rf /var/lib/apt/lists/*
# Tue, 15 Nov 2022 04:57:26 GMT
RUN set -eux; 	nativeLines="$(catalina.sh configtest 2>&1)"; 	nativeLines="$(echo "$nativeLines" | grep 'Apache Tomcat Native')"; 	nativeLines="$(echo "$nativeLines" | sort -u)"; 	if ! echo "$nativeLines" | grep -E 'INFO: Loaded( APR based)? Apache Tomcat Native library' >&2; then 		echo >&2 "$nativeLines"; 		exit 1; 	fi
# Tue, 15 Nov 2022 04:57:26 GMT
EXPOSE 8080
# Tue, 15 Nov 2022 04:57:27 GMT
CMD ["catalina.sh" "run"]
# Wed, 11 Jan 2023 03:05:10 GMT
LABEL org.opencontainers.image.authors=XWiki Development Team <committers@xwiki.org>
# Wed, 11 Jan 2023 03:05:10 GMT
LABEL org.opencontainers.image.url=https://hub.docker.com/_/xwiki
# Wed, 11 Jan 2023 03:05:10 GMT
LABEL org.opencontainers.image.documentation=https://hub.docker.com/_/xwiki
# Wed, 11 Jan 2023 03:05:10 GMT
LABEL org.opencontainers.image.source=https://github.com/xwiki/xwiki-docker.git
# Wed, 11 Jan 2023 03:05:11 GMT
LABEL org.opencontainers.image.vendor=xwiki.org
# Wed, 11 Jan 2023 03:05:11 GMT
LABEL org.opencontainers.image.licenses=LGPL-2.1
# Wed, 11 Jan 2023 03:07:37 GMT
RUN apt-get update &&   apt-get --no-install-recommends -y install     curl     libreoffice     unzip     procps &&   rm -rf /var/lib/apt/lists/*
# Wed, 01 Feb 2023 22:26:19 GMT
ENV XWIKI_VERSION=14.10.4
# Wed, 01 Feb 2023 22:26:19 GMT
ENV XWIKI_URL_PREFIX=https://maven.xwiki.org/releases/org/xwiki/platform/xwiki-platform-distribution-war/14.10.4
# Wed, 01 Feb 2023 22:26:19 GMT
ENV XWIKI_DOWNLOAD_SHA256=2fcfb622319172c2e424b9c11848ebfabe27cf8ef69cba39ceb5d124b7ebe713
# Wed, 01 Feb 2023 22:27:00 GMT
RUN rm -rf /usr/local/tomcat/webapps/* &&   mkdir -p /usr/local/tomcat/temp &&   mkdir -p /usr/local/xwiki/data &&   curl -fSL "${XWIKI_URL_PREFIX}/xwiki-platform-distribution-war-${XWIKI_VERSION}.war" -o xwiki.war &&   echo "$XWIKI_DOWNLOAD_SHA256 xwiki.war" | sha256sum -c - &&   unzip -d /usr/local/tomcat/webapps/ROOT xwiki.war &&   rm -f xwiki.war
# Wed, 01 Feb 2023 22:27:03 GMT
ENV MYSQL_JDBC_VERSION=8.0.31
# Wed, 01 Feb 2023 22:27:03 GMT
ENV MYSQL_JDBC_SHA256=5249e3dc6d6531b37790e3f61845b96db5e41e891d3d8edb0e2e3a1b53ca2f4f
# Wed, 01 Feb 2023 22:27:03 GMT
ENV MYSQL_JDBC_PREFIX=https://repo1.maven.org/maven2/com/mysql/mysql-connector-j/8.0.31
# Wed, 01 Feb 2023 22:27:03 GMT
ENV MYSQL_JDBC_ARTIFACT=mysql-connector-j-8.0.31.jar
# Wed, 01 Feb 2023 22:27:03 GMT
ENV MYSQL_JDBC_TARGET=/usr/local/tomcat/webapps/ROOT/WEB-INF/lib/mysql-connector-j-8.0.31.jar
# Wed, 01 Feb 2023 22:27:04 GMT
RUN curl -fSL "${MYSQL_JDBC_PREFIX}/${MYSQL_JDBC_ARTIFACT}" -o $MYSQL_JDBC_TARGET &&   echo "$MYSQL_JDBC_SHA256 $MYSQL_JDBC_TARGET" | sha256sum -c -
# Wed, 01 Feb 2023 22:27:04 GMT
COPY file:0a1be11e2eb610a1dbcd415404e3a592641110b93090030cb831e3a19a163017 in /usr/local/tomcat/bin/ 
# Wed, 01 Feb 2023 22:27:04 GMT
COPY file:1b8409986f3e4eb79a7a0b18472cb2692a61d504fb5ef34292bc997b79fd760d in /usr/local/tomcat/webapps/ROOT/WEB-INF/hibernate.cfg.xml 
# Wed, 01 Feb 2023 22:27:05 GMT
RUN sed -i 's/<id>org.xwiki.platform:xwiki-platform-distribution-war/<id>org.xwiki.platform:xwiki-platform-distribution-docker/'   /usr/local/tomcat/webapps/ROOT/META-INF/extension.xed
# Wed, 01 Feb 2023 22:27:05 GMT
COPY file:a47c4dcd87c9dad97aff38c49188357e6193bcad50757e516cfb08a60d4de611 in /usr/local/bin/docker-entrypoint.sh 
# Wed, 01 Feb 2023 22:27:05 GMT
VOLUME [/usr/local/xwiki]
# Wed, 01 Feb 2023 22:27:05 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 01 Feb 2023 22:27:05 GMT
CMD ["xwiki"]
```

-	Layers:
	-	`sha256:0509fae36eb0656f8bdb23f8ae64100d893bcea2563e97468d337e04d2d0410b`  
		Last Modified: Wed, 02 Nov 2022 18:50:21 GMT  
		Size: 28.4 MB (28382154 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e502a1af2bcd98f5f0d2f5e4da1a0e7bbe07a2c548e2662f7d37dce5ae1df46c`  
		Last Modified: Wed, 02 Nov 2022 19:48:28 GMT  
		Size: 12.4 MB (12396330 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bc4598c07dd818f03a0378b0341a4a8e80f0152fbb3e7d5246ca4f466f42e611`  
		Last Modified: Fri, 04 Nov 2022 22:46:46 GMT  
		Size: 45.0 MB (44958470 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:715a937a1066f998b331fcd62256ad01a5571bdf46804e97825afc64f9ebb427`  
		Last Modified: Fri, 04 Nov 2022 22:46:41 GMT  
		Size: 160.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5fb623f082f74b2fa9fc2c4e3f3a4802875cb9753cfa26ed940201ce72bb56cb`  
		Last Modified: Sat, 05 Nov 2022 00:03:40 GMT  
		Size: 172.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:33260b83200262bbd546be371ad3c1f50f5ae7228afb87982d6fa9d6b11bf26f`  
		Last Modified: Tue, 15 Nov 2022 05:10:19 GMT  
		Size: 12.2 MB (12207235 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0955fb697ea9b30a1b4f95385464f646aa1525cb6efba648e22df84ebef6b2ee`  
		Last Modified: Tue, 15 Nov 2022 05:10:18 GMT  
		Size: 452.0 KB (452021 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6eddcf66f2083b1487296a0308e0b058917c97f614f12428d82d89662038dc2e`  
		Last Modified: Tue, 15 Nov 2022 05:10:18 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ae5f60bb64f3fa11da3d15a9639f886186b4c2c021455c3f9db22e0cfe1b1311`  
		Last Modified: Wed, 11 Jan 2023 03:11:14 GMT  
		Size: 173.8 MB (173806827 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:13334e257ce7313ca9d6028534e3ec6c7858c374c4afedea7f96c51da716806e`  
		Last Modified: Wed, 01 Feb 2023 22:29:16 GMT  
		Size: 307.1 MB (307104849 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ccb59878c7670194b75b6af22dd3908f9ae1a12dc1074f0b5ed156a5e3afdf0a`  
		Last Modified: Wed, 01 Feb 2023 22:29:02 GMT  
		Size: 2.4 MB (2377177 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d3946fb25102529cda96bcad4925905c9b997e442b447675d89066505cbe1026`  
		Last Modified: Wed, 01 Feb 2023 22:29:02 GMT  
		Size: 1.3 KB (1344 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1ba832da71f2ed07bae5269bb37e7ea79724a069ad63032f2af14996893baa37`  
		Last Modified: Wed, 01 Feb 2023 22:29:02 GMT  
		Size: 2.3 KB (2307 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6616193191331001a42a5d452ea69a215bbc414eca5cb00914c359665be5817f`  
		Last Modified: Wed, 01 Feb 2023 22:29:02 GMT  
		Size: 6.0 KB (6009 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6de4b8ce214cd9b76eda5b4955e5abb249a0b0292e8a38d39683e3002d6534bf`  
		Last Modified: Wed, 01 Feb 2023 22:29:03 GMT  
		Size: 2.5 KB (2506 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `xwiki:14.10-mariadb-tomcat`

```console
$ docker pull xwiki@sha256:016ba45d303064d25d04a705c1a307612a6383139366413fb169f42acc0419ee
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `xwiki:14.10-mariadb-tomcat` - linux; amd64

```console
$ docker pull xwiki@sha256:4aec14b2a2ae95584b839238412bbe33a7314bf32edc3e05f34f532d07fdedce
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **588.7 MB (588696916 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f5fbe86c66c7ac80e07663234a80353ce71d1847f409e2e2a603e0eb2a3342bc`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["xwiki"]`

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
# Wed, 02 Nov 2022 18:44:10 GMT
RUN apt-get update     && DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends tzdata curl wget ca-certificates fontconfig locales     && echo "en_US.UTF-8 UTF-8" >> /etc/locale.gen     && locale-gen en_US.UTF-8     && rm -rf /var/lib/apt/lists/*
# Fri, 04 Nov 2022 23:21:41 GMT
ENV JAVA_VERSION=jdk-11.0.17+8
# Fri, 04 Nov 2022 23:22:31 GMT
RUN set -eux;     ARCH="$(dpkg --print-architecture)";     case "${ARCH}" in        aarch64|arm64)          ESUM='bd6efe3290c8b5a42f695a55a26f3e3c9c284288574879d4b7089f31f5114177';          BINARY_URL='https://github.com/adoptium/temurin11-binaries/releases/download/jdk-11.0.17%2B8/OpenJDK11U-jre_aarch64_linux_hotspot_11.0.17_8.tar.gz';          ;;        armhf|arm)          ESUM='8cf113d3d7fa808895c8d2e41bb890af21c47e38c2460e0588147a4bb8fc658d';          BINARY_URL='https://github.com/adoptium/temurin11-binaries/releases/download/jdk-11.0.17%2B8/OpenJDK11U-jre_arm_linux_hotspot_11.0.17_8.tar.gz';          ;;        ppc64el|powerpc:common64)          ESUM='0ca3d806131ab5834c501f9c625bb0248cd528af361c704503348e9c9605bedf';          BINARY_URL='https://github.com/adoptium/temurin11-binaries/releases/download/jdk-11.0.17%2B8/OpenJDK11U-jre_ppc64le_linux_hotspot_11.0.17_8.tar.gz';          ;;        s390x|s390:64-bit)          ESUM='dd3b159a374086e65cb07c4ccb226c90f9c02ef929cba6f0b642171d7ed97fa4';          BINARY_URL='https://github.com/adoptium/temurin11-binaries/releases/download/jdk-11.0.17%2B8/OpenJDK11U-jre_s390x_linux_hotspot_11.0.17_8.tar.gz';          ;;        amd64|i386:x86-64)          ESUM='752616097e09d7f60a3ad8bd312f90eaf50ac72577e55df229fe6e8091148f79';          BINARY_URL='https://github.com/adoptium/temurin11-binaries/releases/download/jdk-11.0.17%2B8/OpenJDK11U-jre_x64_linux_hotspot_11.0.17_8.tar.gz';          ;;        *)          echo "Unsupported arch: ${ARCH}";          exit 1;          ;;     esac; 	  wget -O /tmp/openjdk.tar.gz ${BINARY_URL}; 	  echo "${ESUM} */tmp/openjdk.tar.gz" | sha256sum -c -; 	  mkdir -p "$JAVA_HOME"; 	  tar --extract 	      --file /tmp/openjdk.tar.gz 	      --directory "$JAVA_HOME" 	      --strip-components 1 	      --no-same-owner 	  ;     rm /tmp/openjdk.tar.gz;     find "$JAVA_HOME/lib" -name '*.so' -exec dirname '{}' ';' | sort -u > /etc/ld.so.conf.d/docker-openjdk.conf;     ldconfig;     java -Xshare:dump;
# Fri, 04 Nov 2022 23:22:32 GMT
RUN echo Verifying install ...     && fileEncoding="$(echo 'System.out.println(System.getProperty("file.encoding"))' | jshell -s -)"; [ "$fileEncoding" = 'UTF-8' ]; rm -rf ~/.java     && echo java --version && java --version     && echo Complete.
# Sat, 05 Nov 2022 01:35:16 GMT
ENV CATALINA_HOME=/usr/local/tomcat
# Sat, 05 Nov 2022 01:35:16 GMT
ENV PATH=/usr/local/tomcat/bin:/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Sat, 05 Nov 2022 01:35:17 GMT
RUN mkdir -p "$CATALINA_HOME"
# Sat, 05 Nov 2022 01:35:17 GMT
WORKDIR /usr/local/tomcat
# Sat, 05 Nov 2022 01:35:17 GMT
ENV TOMCAT_NATIVE_LIBDIR=/usr/local/tomcat/native-jni-lib
# Sat, 05 Nov 2022 01:35:17 GMT
ENV LD_LIBRARY_PATH=/usr/local/tomcat/native-jni-lib
# Sat, 05 Nov 2022 01:39:54 GMT
ENV GPG_KEYS=48F8E69F6390C9F25CFEDCD268248959359E722B A9C5DF4D22E99998D9875A5110C01C5A2F6059E7 DCFD35E0BF8CA7344752DE8B6FB21E8933C60243
# Sat, 05 Nov 2022 01:39:54 GMT
ENV TOMCAT_MAJOR=9
# Tue, 15 Nov 2022 03:06:43 GMT
ENV TOMCAT_VERSION=9.0.69
# Tue, 15 Nov 2022 03:06:43 GMT
ENV TOMCAT_SHA512=8c883c54ce9ce43eba37756a6404cdf3477879883a3e6d146dc8a7aa5e0425f487466afe6b6da4a895927cb7cb59177b9379cec18000f2de12785be57408c779
# Tue, 15 Nov 2022 03:06:44 GMT
COPY dir:b1a33aa3993dbbfbebb33bd9aa546b60c2f2191abf1227f453d4e830f6deb35f in /usr/local/tomcat 
# Tue, 15 Nov 2022 03:06:48 GMT
RUN set -eux; 	apt-get update; 	xargs -rt apt-get install -y --no-install-recommends < "$TOMCAT_NATIVE_LIBDIR/.dependencies.txt"; 	rm -rf /var/lib/apt/lists/*
# Tue, 15 Nov 2022 03:06:49 GMT
RUN set -eux; 	nativeLines="$(catalina.sh configtest 2>&1)"; 	nativeLines="$(echo "$nativeLines" | grep 'Apache Tomcat Native')"; 	nativeLines="$(echo "$nativeLines" | sort -u)"; 	if ! echo "$nativeLines" | grep -E 'INFO: Loaded( APR based)? Apache Tomcat Native library' >&2; then 		echo >&2 "$nativeLines"; 		exit 1; 	fi
# Tue, 15 Nov 2022 03:06:49 GMT
EXPOSE 8080
# Tue, 15 Nov 2022 03:06:49 GMT
CMD ["catalina.sh" "run"]
# Wed, 11 Jan 2023 02:47:03 GMT
LABEL org.opencontainers.image.authors=XWiki Development Team <committers@xwiki.org>
# Wed, 11 Jan 2023 02:47:03 GMT
LABEL org.opencontainers.image.url=https://hub.docker.com/_/xwiki
# Wed, 11 Jan 2023 02:47:03 GMT
LABEL org.opencontainers.image.documentation=https://hub.docker.com/_/xwiki
# Wed, 11 Jan 2023 02:47:03 GMT
LABEL org.opencontainers.image.source=https://github.com/xwiki/xwiki-docker.git
# Wed, 11 Jan 2023 02:47:04 GMT
LABEL org.opencontainers.image.vendor=xwiki.org
# Wed, 11 Jan 2023 02:47:04 GMT
LABEL org.opencontainers.image.licenses=LGPL-2.1
# Wed, 11 Jan 2023 02:49:03 GMT
RUN apt-get update &&   apt-get --no-install-recommends -y install     curl     libreoffice     unzip     procps &&   rm -rf /var/lib/apt/lists/*
# Wed, 22 Feb 2023 18:39:36 GMT
ENV XWIKI_VERSION=14.10.5
# Wed, 22 Feb 2023 18:39:36 GMT
ENV XWIKI_URL_PREFIX=https://maven.xwiki.org/releases/org/xwiki/platform/xwiki-platform-distribution-war/14.10.5
# Wed, 22 Feb 2023 18:39:36 GMT
ENV XWIKI_DOWNLOAD_SHA256=f58465d0869e4c5605ae8375a09c79399d1149c7131fed3cf9959918267eb6a8
# Wed, 22 Feb 2023 18:40:15 GMT
RUN rm -rf /usr/local/tomcat/webapps/* &&   mkdir -p /usr/local/tomcat/temp &&   mkdir -p /usr/local/xwiki/data &&   curl -fSL "${XWIKI_URL_PREFIX}/xwiki-platform-distribution-war-${XWIKI_VERSION}.war" -o xwiki.war &&   echo "$XWIKI_DOWNLOAD_SHA256 xwiki.war" | sha256sum -c - &&   unzip -d /usr/local/tomcat/webapps/ROOT xwiki.war &&   rm -f xwiki.war
# Wed, 22 Feb 2023 18:41:14 GMT
ENV MARIADB_JDBC_VERSION=3.1.2
# Wed, 22 Feb 2023 18:41:14 GMT
ENV MARIADB_JDBC_SHA256=aaec1ad348d030a65b25c93c65cdaf472bf8b4b6b314b965e5ba13aec81bc622
# Wed, 22 Feb 2023 18:41:14 GMT
ENV MARIADB_JDBC_PREFIX=https://repo1.maven.org/maven2/org/mariadb/jdbc/mariadb-java-client/3.1.2
# Wed, 22 Feb 2023 18:41:14 GMT
ENV MARIADB_JDBC_ARTIFACT=mariadb-java-client-3.1.2.jar
# Wed, 22 Feb 2023 18:41:14 GMT
ENV MARIADB_JDBC_TARGET=/usr/local/tomcat/webapps/ROOT/WEB-INF/lib/mariadb-java-client-3.1.2.jar
# Wed, 22 Feb 2023 18:41:15 GMT
RUN curl -fSL "${MARIADB_JDBC_PREFIX}/${MARIADB_JDBC_ARTIFACT}" -o $MARIADB_JDBC_TARGET &&   echo "$MARIADB_JDBC_SHA256 $MARIADB_JDBC_TARGET" | sha256sum -c -
# Wed, 22 Feb 2023 18:41:15 GMT
COPY file:0a1be11e2eb610a1dbcd415404e3a592641110b93090030cb831e3a19a163017 in /usr/local/tomcat/bin/ 
# Wed, 22 Feb 2023 18:41:15 GMT
COPY file:0e237c3876eeb3b5f3473a064d3e507da2df6c228ca714687930b34e3b687601 in /usr/local/tomcat/webapps/ROOT/WEB-INF/hibernate.cfg.xml 
# Wed, 22 Feb 2023 18:41:15 GMT
RUN sed -i 's/<id>org.xwiki.platform:xwiki-platform-distribution-war/<id>org.xwiki.platform:xwiki-platform-distribution-docker/'   /usr/local/tomcat/webapps/ROOT/META-INF/extension.xed
# Wed, 22 Feb 2023 18:41:16 GMT
COPY file:a47c4dcd87c9dad97aff38c49188357e6193bcad50757e516cfb08a60d4de611 in /usr/local/bin/docker-entrypoint.sh 
# Wed, 22 Feb 2023 18:41:16 GMT
VOLUME [/usr/local/xwiki]
# Wed, 22 Feb 2023 18:41:16 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 22 Feb 2023 18:41:16 GMT
CMD ["xwiki"]
```

-	Layers:
	-	`sha256:e96e057aae67380a4ddb16c337c5c3669d97fdff69ec537f02aa2cc30d814281`  
		Last Modified: Wed, 02 Nov 2022 03:03:36 GMT  
		Size: 30.4 MB (30425607 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4ced2591451da3a02e2b6bb44752b9e3f00d77789921be4df5082fb9f9880ad0`  
		Last Modified: Wed, 02 Nov 2022 18:48:43 GMT  
		Size: 12.4 MB (12439006 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:df8f874ae8c08a9e69e5fbe6c5a64200a45386132a3203d1a9a7f1146d94cfbc`  
		Last Modified: Fri, 04 Nov 2022 23:29:33 GMT  
		Size: 46.6 MB (46629936 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:111b6c7486426c4b6989102c2ee5be856e8a58e20ab0a350b24a905d536e8e7f`  
		Last Modified: Fri, 04 Nov 2022 23:29:26 GMT  
		Size: 161.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e6f84dce457c6d4f7b7291fce05f8e77998a3a7722a54125a1f1d52ca83043b4`  
		Last Modified: Sat, 05 Nov 2022 01:50:51 GMT  
		Size: 173.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a6c26749ee782392e38845ee2ba79b0da586ef6a45d8e7f29c7af14612278547`  
		Last Modified: Tue, 15 Nov 2022 03:19:57 GMT  
		Size: 12.2 MB (12200249 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4dddc6d9fa6024025b3fcfe729cab2dc544fb25476eca6e80b1af8e8d93bb0ee`  
		Last Modified: Tue, 15 Nov 2022 03:19:56 GMT  
		Size: 452.7 KB (452680 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:06637eebe5e72c8ad9019ad4eb4cdde1f11f7d4c24c7ed7374cf8966343aa2fb`  
		Last Modified: Tue, 15 Nov 2022 03:19:56 GMT  
		Size: 131.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b276fb8390410a8208724033e325715ea26000d5a1a762d4c3699b927884fbfe`  
		Last Modified: Wed, 11 Jan 2023 02:52:45 GMT  
		Size: 178.8 MB (178805608 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:89de9d9e2c09cd5b84430562516cbcd5695a0a3b2347b451e157bde75c2b5619`  
		Last Modified: Wed, 22 Feb 2023 18:42:21 GMT  
		Size: 307.1 MB (307141303 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c34f6e86e4b4ce021fdc5c26a390f8682b638ef5b002596f5d85721a5b4f8b78`  
		Last Modified: Wed, 22 Feb 2023 18:43:25 GMT  
		Size: 589.9 KB (589888 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7c59af828719a4990baaba43861a4b7dfcf7c9301bc8c1c17b1977363ae47d8f`  
		Last Modified: Wed, 22 Feb 2023 18:43:25 GMT  
		Size: 1.3 KB (1345 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a1ce8abe653003fb1cf66551dd2e3daf88c2ec88e42e874179577314bcb129d7`  
		Last Modified: Wed, 22 Feb 2023 18:43:25 GMT  
		Size: 2.3 KB (2312 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:68e8b10875b16f8254c97d2580791e4ed6c27787f670ac843c0508addb3b38b3`  
		Last Modified: Wed, 22 Feb 2023 18:43:25 GMT  
		Size: 6.0 KB (6013 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ed46c896037147ae7b8029b5b7e890b7930132f0eec078e1211ccb92ff45c89e`  
		Last Modified: Wed, 22 Feb 2023 18:43:25 GMT  
		Size: 2.5 KB (2504 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `xwiki:14.10-mariadb-tomcat` - linux; arm64 variant v8

```console
$ docker pull xwiki@sha256:7325fc8b1c018497044befd011b0c006d687105f4227efb007aa304e9a7aae36
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **579.9 MB (579910180 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e16df67b6f15552144570116827b8b364c740abb52e9ca29c35e0c5ed526fe1b`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["xwiki"]`

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
# Wed, 02 Nov 2022 19:44:32 GMT
RUN apt-get update     && DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends tzdata curl wget ca-certificates fontconfig locales     && echo "en_US.UTF-8 UTF-8" >> /etc/locale.gen     && locale-gen en_US.UTF-8     && rm -rf /var/lib/apt/lists/*
# Fri, 04 Nov 2022 22:40:54 GMT
ENV JAVA_VERSION=jdk-11.0.17+8
# Fri, 04 Nov 2022 22:41:33 GMT
RUN set -eux;     ARCH="$(dpkg --print-architecture)";     case "${ARCH}" in        aarch64|arm64)          ESUM='bd6efe3290c8b5a42f695a55a26f3e3c9c284288574879d4b7089f31f5114177';          BINARY_URL='https://github.com/adoptium/temurin11-binaries/releases/download/jdk-11.0.17%2B8/OpenJDK11U-jre_aarch64_linux_hotspot_11.0.17_8.tar.gz';          ;;        armhf|arm)          ESUM='8cf113d3d7fa808895c8d2e41bb890af21c47e38c2460e0588147a4bb8fc658d';          BINARY_URL='https://github.com/adoptium/temurin11-binaries/releases/download/jdk-11.0.17%2B8/OpenJDK11U-jre_arm_linux_hotspot_11.0.17_8.tar.gz';          ;;        ppc64el|powerpc:common64)          ESUM='0ca3d806131ab5834c501f9c625bb0248cd528af361c704503348e9c9605bedf';          BINARY_URL='https://github.com/adoptium/temurin11-binaries/releases/download/jdk-11.0.17%2B8/OpenJDK11U-jre_ppc64le_linux_hotspot_11.0.17_8.tar.gz';          ;;        s390x|s390:64-bit)          ESUM='dd3b159a374086e65cb07c4ccb226c90f9c02ef929cba6f0b642171d7ed97fa4';          BINARY_URL='https://github.com/adoptium/temurin11-binaries/releases/download/jdk-11.0.17%2B8/OpenJDK11U-jre_s390x_linux_hotspot_11.0.17_8.tar.gz';          ;;        amd64|i386:x86-64)          ESUM='752616097e09d7f60a3ad8bd312f90eaf50ac72577e55df229fe6e8091148f79';          BINARY_URL='https://github.com/adoptium/temurin11-binaries/releases/download/jdk-11.0.17%2B8/OpenJDK11U-jre_x64_linux_hotspot_11.0.17_8.tar.gz';          ;;        *)          echo "Unsupported arch: ${ARCH}";          exit 1;          ;;     esac; 	  wget -O /tmp/openjdk.tar.gz ${BINARY_URL}; 	  echo "${ESUM} */tmp/openjdk.tar.gz" | sha256sum -c -; 	  mkdir -p "$JAVA_HOME"; 	  tar --extract 	      --file /tmp/openjdk.tar.gz 	      --directory "$JAVA_HOME" 	      --strip-components 1 	      --no-same-owner 	  ;     rm /tmp/openjdk.tar.gz;     find "$JAVA_HOME/lib" -name '*.so' -exec dirname '{}' ';' | sort -u > /etc/ld.so.conf.d/docker-openjdk.conf;     ldconfig;     java -Xshare:dump;
# Fri, 04 Nov 2022 22:41:34 GMT
RUN echo Verifying install ...     && fileEncoding="$(echo 'System.out.println(System.getProperty("file.encoding"))' | jshell -s -)"; [ "$fileEncoding" = 'UTF-8' ]; rm -rf ~/.java     && echo java --version && java --version     && echo Complete.
# Fri, 04 Nov 2022 23:48:38 GMT
ENV CATALINA_HOME=/usr/local/tomcat
# Fri, 04 Nov 2022 23:48:38 GMT
ENV PATH=/usr/local/tomcat/bin:/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Fri, 04 Nov 2022 23:48:38 GMT
RUN mkdir -p "$CATALINA_HOME"
# Fri, 04 Nov 2022 23:48:39 GMT
WORKDIR /usr/local/tomcat
# Fri, 04 Nov 2022 23:48:39 GMT
ENV TOMCAT_NATIVE_LIBDIR=/usr/local/tomcat/native-jni-lib
# Fri, 04 Nov 2022 23:48:39 GMT
ENV LD_LIBRARY_PATH=/usr/local/tomcat/native-jni-lib
# Fri, 04 Nov 2022 23:53:12 GMT
ENV GPG_KEYS=48F8E69F6390C9F25CFEDCD268248959359E722B A9C5DF4D22E99998D9875A5110C01C5A2F6059E7 DCFD35E0BF8CA7344752DE8B6FB21E8933C60243
# Fri, 04 Nov 2022 23:53:12 GMT
ENV TOMCAT_MAJOR=9
# Tue, 15 Nov 2022 04:57:22 GMT
ENV TOMCAT_VERSION=9.0.69
# Tue, 15 Nov 2022 04:57:22 GMT
ENV TOMCAT_SHA512=8c883c54ce9ce43eba37756a6404cdf3477879883a3e6d146dc8a7aa5e0425f487466afe6b6da4a895927cb7cb59177b9379cec18000f2de12785be57408c779
# Tue, 15 Nov 2022 04:57:22 GMT
COPY dir:096b403a5f78b17e6b4bff63128a9c93941b97f22470991610dd641633d977f1 in /usr/local/tomcat 
# Tue, 15 Nov 2022 04:57:25 GMT
RUN set -eux; 	apt-get update; 	xargs -rt apt-get install -y --no-install-recommends < "$TOMCAT_NATIVE_LIBDIR/.dependencies.txt"; 	rm -rf /var/lib/apt/lists/*
# Tue, 15 Nov 2022 04:57:26 GMT
RUN set -eux; 	nativeLines="$(catalina.sh configtest 2>&1)"; 	nativeLines="$(echo "$nativeLines" | grep 'Apache Tomcat Native')"; 	nativeLines="$(echo "$nativeLines" | sort -u)"; 	if ! echo "$nativeLines" | grep -E 'INFO: Loaded( APR based)? Apache Tomcat Native library' >&2; then 		echo >&2 "$nativeLines"; 		exit 1; 	fi
# Tue, 15 Nov 2022 04:57:26 GMT
EXPOSE 8080
# Tue, 15 Nov 2022 04:57:27 GMT
CMD ["catalina.sh" "run"]
# Wed, 11 Jan 2023 03:05:10 GMT
LABEL org.opencontainers.image.authors=XWiki Development Team <committers@xwiki.org>
# Wed, 11 Jan 2023 03:05:10 GMT
LABEL org.opencontainers.image.url=https://hub.docker.com/_/xwiki
# Wed, 11 Jan 2023 03:05:10 GMT
LABEL org.opencontainers.image.documentation=https://hub.docker.com/_/xwiki
# Wed, 11 Jan 2023 03:05:10 GMT
LABEL org.opencontainers.image.source=https://github.com/xwiki/xwiki-docker.git
# Wed, 11 Jan 2023 03:05:11 GMT
LABEL org.opencontainers.image.vendor=xwiki.org
# Wed, 11 Jan 2023 03:05:11 GMT
LABEL org.opencontainers.image.licenses=LGPL-2.1
# Wed, 11 Jan 2023 03:07:37 GMT
RUN apt-get update &&   apt-get --no-install-recommends -y install     curl     libreoffice     unzip     procps &&   rm -rf /var/lib/apt/lists/*
# Wed, 01 Feb 2023 22:26:19 GMT
ENV XWIKI_VERSION=14.10.4
# Wed, 01 Feb 2023 22:26:19 GMT
ENV XWIKI_URL_PREFIX=https://maven.xwiki.org/releases/org/xwiki/platform/xwiki-platform-distribution-war/14.10.4
# Wed, 01 Feb 2023 22:26:19 GMT
ENV XWIKI_DOWNLOAD_SHA256=2fcfb622319172c2e424b9c11848ebfabe27cf8ef69cba39ceb5d124b7ebe713
# Wed, 01 Feb 2023 22:27:00 GMT
RUN rm -rf /usr/local/tomcat/webapps/* &&   mkdir -p /usr/local/tomcat/temp &&   mkdir -p /usr/local/xwiki/data &&   curl -fSL "${XWIKI_URL_PREFIX}/xwiki-platform-distribution-war-${XWIKI_VERSION}.war" -o xwiki.war &&   echo "$XWIKI_DOWNLOAD_SHA256 xwiki.war" | sha256sum -c - &&   unzip -d /usr/local/tomcat/webapps/ROOT xwiki.war &&   rm -f xwiki.war
# Wed, 01 Feb 2023 22:27:55 GMT
ENV MARIADB_JDBC_VERSION=3.1.1
# Wed, 01 Feb 2023 22:27:55 GMT
ENV MARIADB_JDBC_SHA256=a554541fd88047905fb0c4c10e1d85295f5e38c7bb5fb408b425392a79fc26e3
# Wed, 01 Feb 2023 22:27:55 GMT
ENV MARIADB_JDBC_PREFIX=https://repo1.maven.org/maven2/org/mariadb/jdbc/mariadb-java-client/3.1.1
# Wed, 01 Feb 2023 22:27:55 GMT
ENV MARIADB_JDBC_ARTIFACT=mariadb-java-client-3.1.1.jar
# Wed, 01 Feb 2023 22:27:55 GMT
ENV MARIADB_JDBC_TARGET=/usr/local/tomcat/webapps/ROOT/WEB-INF/lib/mariadb-java-client-3.1.1.jar
# Wed, 01 Feb 2023 22:27:56 GMT
RUN curl -fSL "${MARIADB_JDBC_PREFIX}/${MARIADB_JDBC_ARTIFACT}" -o $MARIADB_JDBC_TARGET &&   echo "$MARIADB_JDBC_SHA256 $MARIADB_JDBC_TARGET" | sha256sum -c -
# Wed, 01 Feb 2023 22:27:56 GMT
COPY file:0a1be11e2eb610a1dbcd415404e3a592641110b93090030cb831e3a19a163017 in /usr/local/tomcat/bin/ 
# Wed, 01 Feb 2023 22:27:56 GMT
COPY file:0e237c3876eeb3b5f3473a064d3e507da2df6c228ca714687930b34e3b687601 in /usr/local/tomcat/webapps/ROOT/WEB-INF/hibernate.cfg.xml 
# Wed, 01 Feb 2023 22:27:57 GMT
RUN sed -i 's/<id>org.xwiki.platform:xwiki-platform-distribution-war/<id>org.xwiki.platform:xwiki-platform-distribution-docker/'   /usr/local/tomcat/webapps/ROOT/META-INF/extension.xed
# Wed, 01 Feb 2023 22:27:57 GMT
COPY file:a47c4dcd87c9dad97aff38c49188357e6193bcad50757e516cfb08a60d4de611 in /usr/local/bin/docker-entrypoint.sh 
# Wed, 01 Feb 2023 22:27:57 GMT
VOLUME [/usr/local/xwiki]
# Wed, 01 Feb 2023 22:27:57 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 01 Feb 2023 22:27:57 GMT
CMD ["xwiki"]
```

-	Layers:
	-	`sha256:0509fae36eb0656f8bdb23f8ae64100d893bcea2563e97468d337e04d2d0410b`  
		Last Modified: Wed, 02 Nov 2022 18:50:21 GMT  
		Size: 28.4 MB (28382154 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e502a1af2bcd98f5f0d2f5e4da1a0e7bbe07a2c548e2662f7d37dce5ae1df46c`  
		Last Modified: Wed, 02 Nov 2022 19:48:28 GMT  
		Size: 12.4 MB (12396330 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bc4598c07dd818f03a0378b0341a4a8e80f0152fbb3e7d5246ca4f466f42e611`  
		Last Modified: Fri, 04 Nov 2022 22:46:46 GMT  
		Size: 45.0 MB (44958470 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:715a937a1066f998b331fcd62256ad01a5571bdf46804e97825afc64f9ebb427`  
		Last Modified: Fri, 04 Nov 2022 22:46:41 GMT  
		Size: 160.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5fb623f082f74b2fa9fc2c4e3f3a4802875cb9753cfa26ed940201ce72bb56cb`  
		Last Modified: Sat, 05 Nov 2022 00:03:40 GMT  
		Size: 172.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:33260b83200262bbd546be371ad3c1f50f5ae7228afb87982d6fa9d6b11bf26f`  
		Last Modified: Tue, 15 Nov 2022 05:10:19 GMT  
		Size: 12.2 MB (12207235 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0955fb697ea9b30a1b4f95385464f646aa1525cb6efba648e22df84ebef6b2ee`  
		Last Modified: Tue, 15 Nov 2022 05:10:18 GMT  
		Size: 452.0 KB (452021 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6eddcf66f2083b1487296a0308e0b058917c97f614f12428d82d89662038dc2e`  
		Last Modified: Tue, 15 Nov 2022 05:10:18 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ae5f60bb64f3fa11da3d15a9639f886186b4c2c021455c3f9db22e0cfe1b1311`  
		Last Modified: Wed, 11 Jan 2023 03:11:14 GMT  
		Size: 173.8 MB (173806827 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:13334e257ce7313ca9d6028534e3ec6c7858c374c4afedea7f96c51da716806e`  
		Last Modified: Wed, 01 Feb 2023 22:29:16 GMT  
		Size: 307.1 MB (307104849 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a825dc0bda4f4de7842c41ce3db12885844733a8717fc3072c599678278e4b9b`  
		Last Modified: Wed, 01 Feb 2023 22:30:19 GMT  
		Size: 589.7 KB (589668 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0d3b831d82d4e981ad4dd1f4ef4cb7a5b16e7e27fff8121997366b1c93b836b7`  
		Last Modified: Wed, 01 Feb 2023 22:30:19 GMT  
		Size: 1.3 KB (1343 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b4b1db4f27135bc027a5f8478949b1118838f79760f5c779a18756553b080ac0`  
		Last Modified: Wed, 01 Feb 2023 22:30:19 GMT  
		Size: 2.3 KB (2309 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7f634a749b61f1dc714bb14b2b20c7fedd422c285161bdce24613edffc1feaca`  
		Last Modified: Wed, 01 Feb 2023 22:30:19 GMT  
		Size: 6.0 KB (6007 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f68b784196e13fd8e6790aa86b2f5a906f53094387165b175a9b981413e22fe1`  
		Last Modified: Wed, 01 Feb 2023 22:30:20 GMT  
		Size: 2.5 KB (2506 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `xwiki:14.10-mysql-tomcat`

```console
$ docker pull xwiki@sha256:32e51c9775fda50082b0f02856f2af444a67284446679c9a3a13a78c02ec0c4b
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `xwiki:14.10-mysql-tomcat` - linux; amd64

```console
$ docker pull xwiki@sha256:a2e996a399fc68cbccfe11eaeb0115a15314bd69f06c483fef3cba244fa07cbf
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **590.4 MB (590449604 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:6b73fd725d5c1dd8044289fdb0e76f973e7e1d4a64e1efc44428235a718b550a`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["xwiki"]`

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
# Wed, 02 Nov 2022 18:44:10 GMT
RUN apt-get update     && DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends tzdata curl wget ca-certificates fontconfig locales     && echo "en_US.UTF-8 UTF-8" >> /etc/locale.gen     && locale-gen en_US.UTF-8     && rm -rf /var/lib/apt/lists/*
# Fri, 04 Nov 2022 23:21:41 GMT
ENV JAVA_VERSION=jdk-11.0.17+8
# Fri, 04 Nov 2022 23:22:31 GMT
RUN set -eux;     ARCH="$(dpkg --print-architecture)";     case "${ARCH}" in        aarch64|arm64)          ESUM='bd6efe3290c8b5a42f695a55a26f3e3c9c284288574879d4b7089f31f5114177';          BINARY_URL='https://github.com/adoptium/temurin11-binaries/releases/download/jdk-11.0.17%2B8/OpenJDK11U-jre_aarch64_linux_hotspot_11.0.17_8.tar.gz';          ;;        armhf|arm)          ESUM='8cf113d3d7fa808895c8d2e41bb890af21c47e38c2460e0588147a4bb8fc658d';          BINARY_URL='https://github.com/adoptium/temurin11-binaries/releases/download/jdk-11.0.17%2B8/OpenJDK11U-jre_arm_linux_hotspot_11.0.17_8.tar.gz';          ;;        ppc64el|powerpc:common64)          ESUM='0ca3d806131ab5834c501f9c625bb0248cd528af361c704503348e9c9605bedf';          BINARY_URL='https://github.com/adoptium/temurin11-binaries/releases/download/jdk-11.0.17%2B8/OpenJDK11U-jre_ppc64le_linux_hotspot_11.0.17_8.tar.gz';          ;;        s390x|s390:64-bit)          ESUM='dd3b159a374086e65cb07c4ccb226c90f9c02ef929cba6f0b642171d7ed97fa4';          BINARY_URL='https://github.com/adoptium/temurin11-binaries/releases/download/jdk-11.0.17%2B8/OpenJDK11U-jre_s390x_linux_hotspot_11.0.17_8.tar.gz';          ;;        amd64|i386:x86-64)          ESUM='752616097e09d7f60a3ad8bd312f90eaf50ac72577e55df229fe6e8091148f79';          BINARY_URL='https://github.com/adoptium/temurin11-binaries/releases/download/jdk-11.0.17%2B8/OpenJDK11U-jre_x64_linux_hotspot_11.0.17_8.tar.gz';          ;;        *)          echo "Unsupported arch: ${ARCH}";          exit 1;          ;;     esac; 	  wget -O /tmp/openjdk.tar.gz ${BINARY_URL}; 	  echo "${ESUM} */tmp/openjdk.tar.gz" | sha256sum -c -; 	  mkdir -p "$JAVA_HOME"; 	  tar --extract 	      --file /tmp/openjdk.tar.gz 	      --directory "$JAVA_HOME" 	      --strip-components 1 	      --no-same-owner 	  ;     rm /tmp/openjdk.tar.gz;     find "$JAVA_HOME/lib" -name '*.so' -exec dirname '{}' ';' | sort -u > /etc/ld.so.conf.d/docker-openjdk.conf;     ldconfig;     java -Xshare:dump;
# Fri, 04 Nov 2022 23:22:32 GMT
RUN echo Verifying install ...     && fileEncoding="$(echo 'System.out.println(System.getProperty("file.encoding"))' | jshell -s -)"; [ "$fileEncoding" = 'UTF-8' ]; rm -rf ~/.java     && echo java --version && java --version     && echo Complete.
# Sat, 05 Nov 2022 01:35:16 GMT
ENV CATALINA_HOME=/usr/local/tomcat
# Sat, 05 Nov 2022 01:35:16 GMT
ENV PATH=/usr/local/tomcat/bin:/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Sat, 05 Nov 2022 01:35:17 GMT
RUN mkdir -p "$CATALINA_HOME"
# Sat, 05 Nov 2022 01:35:17 GMT
WORKDIR /usr/local/tomcat
# Sat, 05 Nov 2022 01:35:17 GMT
ENV TOMCAT_NATIVE_LIBDIR=/usr/local/tomcat/native-jni-lib
# Sat, 05 Nov 2022 01:35:17 GMT
ENV LD_LIBRARY_PATH=/usr/local/tomcat/native-jni-lib
# Sat, 05 Nov 2022 01:39:54 GMT
ENV GPG_KEYS=48F8E69F6390C9F25CFEDCD268248959359E722B A9C5DF4D22E99998D9875A5110C01C5A2F6059E7 DCFD35E0BF8CA7344752DE8B6FB21E8933C60243
# Sat, 05 Nov 2022 01:39:54 GMT
ENV TOMCAT_MAJOR=9
# Tue, 15 Nov 2022 03:06:43 GMT
ENV TOMCAT_VERSION=9.0.69
# Tue, 15 Nov 2022 03:06:43 GMT
ENV TOMCAT_SHA512=8c883c54ce9ce43eba37756a6404cdf3477879883a3e6d146dc8a7aa5e0425f487466afe6b6da4a895927cb7cb59177b9379cec18000f2de12785be57408c779
# Tue, 15 Nov 2022 03:06:44 GMT
COPY dir:b1a33aa3993dbbfbebb33bd9aa546b60c2f2191abf1227f453d4e830f6deb35f in /usr/local/tomcat 
# Tue, 15 Nov 2022 03:06:48 GMT
RUN set -eux; 	apt-get update; 	xargs -rt apt-get install -y --no-install-recommends < "$TOMCAT_NATIVE_LIBDIR/.dependencies.txt"; 	rm -rf /var/lib/apt/lists/*
# Tue, 15 Nov 2022 03:06:49 GMT
RUN set -eux; 	nativeLines="$(catalina.sh configtest 2>&1)"; 	nativeLines="$(echo "$nativeLines" | grep 'Apache Tomcat Native')"; 	nativeLines="$(echo "$nativeLines" | sort -u)"; 	if ! echo "$nativeLines" | grep -E 'INFO: Loaded( APR based)? Apache Tomcat Native library' >&2; then 		echo >&2 "$nativeLines"; 		exit 1; 	fi
# Tue, 15 Nov 2022 03:06:49 GMT
EXPOSE 8080
# Tue, 15 Nov 2022 03:06:49 GMT
CMD ["catalina.sh" "run"]
# Wed, 11 Jan 2023 02:47:03 GMT
LABEL org.opencontainers.image.authors=XWiki Development Team <committers@xwiki.org>
# Wed, 11 Jan 2023 02:47:03 GMT
LABEL org.opencontainers.image.url=https://hub.docker.com/_/xwiki
# Wed, 11 Jan 2023 02:47:03 GMT
LABEL org.opencontainers.image.documentation=https://hub.docker.com/_/xwiki
# Wed, 11 Jan 2023 02:47:03 GMT
LABEL org.opencontainers.image.source=https://github.com/xwiki/xwiki-docker.git
# Wed, 11 Jan 2023 02:47:04 GMT
LABEL org.opencontainers.image.vendor=xwiki.org
# Wed, 11 Jan 2023 02:47:04 GMT
LABEL org.opencontainers.image.licenses=LGPL-2.1
# Wed, 11 Jan 2023 02:49:03 GMT
RUN apt-get update &&   apt-get --no-install-recommends -y install     curl     libreoffice     unzip     procps &&   rm -rf /var/lib/apt/lists/*
# Wed, 22 Feb 2023 18:39:36 GMT
ENV XWIKI_VERSION=14.10.5
# Wed, 22 Feb 2023 18:39:36 GMT
ENV XWIKI_URL_PREFIX=https://maven.xwiki.org/releases/org/xwiki/platform/xwiki-platform-distribution-war/14.10.5
# Wed, 22 Feb 2023 18:39:36 GMT
ENV XWIKI_DOWNLOAD_SHA256=f58465d0869e4c5605ae8375a09c79399d1149c7131fed3cf9959918267eb6a8
# Wed, 22 Feb 2023 18:40:15 GMT
RUN rm -rf /usr/local/tomcat/webapps/* &&   mkdir -p /usr/local/tomcat/temp &&   mkdir -p /usr/local/xwiki/data &&   curl -fSL "${XWIKI_URL_PREFIX}/xwiki-platform-distribution-war-${XWIKI_VERSION}.war" -o xwiki.war &&   echo "$XWIKI_DOWNLOAD_SHA256 xwiki.war" | sha256sum -c - &&   unzip -d /usr/local/tomcat/webapps/ROOT xwiki.war &&   rm -f xwiki.war
# Wed, 22 Feb 2023 18:40:17 GMT
ENV MYSQL_JDBC_VERSION=8.0.32
# Wed, 22 Feb 2023 18:40:17 GMT
ENV MYSQL_JDBC_SHA256=522329fe925980f02e5eb89b59d227245d345415ff0c08932a68c9765c13acc5
# Wed, 22 Feb 2023 18:40:17 GMT
ENV MYSQL_JDBC_PREFIX=https://repo1.maven.org/maven2/com/mysql/mysql-connector-j/8.0.32
# Wed, 22 Feb 2023 18:40:17 GMT
ENV MYSQL_JDBC_ARTIFACT=mysql-connector-j-8.0.32.jar
# Wed, 22 Feb 2023 18:40:17 GMT
ENV MYSQL_JDBC_TARGET=/usr/local/tomcat/webapps/ROOT/WEB-INF/lib/mysql-connector-j-8.0.32.jar
# Wed, 22 Feb 2023 18:40:18 GMT
RUN curl -fSL "${MYSQL_JDBC_PREFIX}/${MYSQL_JDBC_ARTIFACT}" -o $MYSQL_JDBC_TARGET &&   echo "$MYSQL_JDBC_SHA256 $MYSQL_JDBC_TARGET" | sha256sum -c -
# Wed, 22 Feb 2023 18:40:18 GMT
COPY file:0a1be11e2eb610a1dbcd415404e3a592641110b93090030cb831e3a19a163017 in /usr/local/tomcat/bin/ 
# Wed, 22 Feb 2023 18:40:18 GMT
COPY file:1b8409986f3e4eb79a7a0b18472cb2692a61d504fb5ef34292bc997b79fd760d in /usr/local/tomcat/webapps/ROOT/WEB-INF/hibernate.cfg.xml 
# Wed, 22 Feb 2023 18:40:19 GMT
RUN sed -i 's/<id>org.xwiki.platform:xwiki-platform-distribution-war/<id>org.xwiki.platform:xwiki-platform-distribution-docker/'   /usr/local/tomcat/webapps/ROOT/META-INF/extension.xed
# Wed, 22 Feb 2023 18:40:19 GMT
COPY file:a47c4dcd87c9dad97aff38c49188357e6193bcad50757e516cfb08a60d4de611 in /usr/local/bin/docker-entrypoint.sh 
# Wed, 22 Feb 2023 18:40:19 GMT
VOLUME [/usr/local/xwiki]
# Wed, 22 Feb 2023 18:40:19 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 22 Feb 2023 18:40:19 GMT
CMD ["xwiki"]
```

-	Layers:
	-	`sha256:e96e057aae67380a4ddb16c337c5c3669d97fdff69ec537f02aa2cc30d814281`  
		Last Modified: Wed, 02 Nov 2022 03:03:36 GMT  
		Size: 30.4 MB (30425607 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4ced2591451da3a02e2b6bb44752b9e3f00d77789921be4df5082fb9f9880ad0`  
		Last Modified: Wed, 02 Nov 2022 18:48:43 GMT  
		Size: 12.4 MB (12439006 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:df8f874ae8c08a9e69e5fbe6c5a64200a45386132a3203d1a9a7f1146d94cfbc`  
		Last Modified: Fri, 04 Nov 2022 23:29:33 GMT  
		Size: 46.6 MB (46629936 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:111b6c7486426c4b6989102c2ee5be856e8a58e20ab0a350b24a905d536e8e7f`  
		Last Modified: Fri, 04 Nov 2022 23:29:26 GMT  
		Size: 161.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e6f84dce457c6d4f7b7291fce05f8e77998a3a7722a54125a1f1d52ca83043b4`  
		Last Modified: Sat, 05 Nov 2022 01:50:51 GMT  
		Size: 173.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a6c26749ee782392e38845ee2ba79b0da586ef6a45d8e7f29c7af14612278547`  
		Last Modified: Tue, 15 Nov 2022 03:19:57 GMT  
		Size: 12.2 MB (12200249 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4dddc6d9fa6024025b3fcfe729cab2dc544fb25476eca6e80b1af8e8d93bb0ee`  
		Last Modified: Tue, 15 Nov 2022 03:19:56 GMT  
		Size: 452.7 KB (452680 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:06637eebe5e72c8ad9019ad4eb4cdde1f11f7d4c24c7ed7374cf8966343aa2fb`  
		Last Modified: Tue, 15 Nov 2022 03:19:56 GMT  
		Size: 131.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b276fb8390410a8208724033e325715ea26000d5a1a762d4c3699b927884fbfe`  
		Last Modified: Wed, 11 Jan 2023 02:52:45 GMT  
		Size: 178.8 MB (178805608 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:89de9d9e2c09cd5b84430562516cbcd5695a0a3b2347b451e157bde75c2b5619`  
		Last Modified: Wed, 22 Feb 2023 18:42:21 GMT  
		Size: 307.1 MB (307141303 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4a2089179b7c1db514d0502e476e09b8f9313d08d4c4e4f3981be456288fe507`  
		Last Modified: Wed, 22 Feb 2023 18:42:04 GMT  
		Size: 2.3 MB (2342572 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e7c4ef360ff3673244adb3dfc4769b5710fa68fcc1fbe1c08b2f5fa32dbd4976`  
		Last Modified: Wed, 22 Feb 2023 18:42:04 GMT  
		Size: 1.3 KB (1348 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:08441c368d4b01e361491d7fbf1ac579fcc303b8484123c309a8d5a3b6657c46`  
		Last Modified: Wed, 22 Feb 2023 18:42:04 GMT  
		Size: 2.3 KB (2311 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:542b4bb846d438395e458c08de292f72d14d289fae6ffe7eba6fec1cd8518475`  
		Last Modified: Wed, 22 Feb 2023 18:42:04 GMT  
		Size: 6.0 KB (6013 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:039c0305df9e64c69bb546e64f0658dba6e728eee13022cfd682aa1ee76b8b7f`  
		Last Modified: Wed, 22 Feb 2023 18:42:04 GMT  
		Size: 2.5 KB (2506 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `xwiki:14.10-mysql-tomcat` - linux; arm64 variant v8

```console
$ docker pull xwiki@sha256:33e36167828fe9bae944e7d4cbbe3b69dd2415595d40610ac2ebcd73f2c2fa7f
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **581.7 MB (581697690 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:44013daf43fd09deb7221eef006c4d30d484a03c433118e5b59da0a44b573f06`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["xwiki"]`

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
# Wed, 02 Nov 2022 19:44:32 GMT
RUN apt-get update     && DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends tzdata curl wget ca-certificates fontconfig locales     && echo "en_US.UTF-8 UTF-8" >> /etc/locale.gen     && locale-gen en_US.UTF-8     && rm -rf /var/lib/apt/lists/*
# Fri, 04 Nov 2022 22:40:54 GMT
ENV JAVA_VERSION=jdk-11.0.17+8
# Fri, 04 Nov 2022 22:41:33 GMT
RUN set -eux;     ARCH="$(dpkg --print-architecture)";     case "${ARCH}" in        aarch64|arm64)          ESUM='bd6efe3290c8b5a42f695a55a26f3e3c9c284288574879d4b7089f31f5114177';          BINARY_URL='https://github.com/adoptium/temurin11-binaries/releases/download/jdk-11.0.17%2B8/OpenJDK11U-jre_aarch64_linux_hotspot_11.0.17_8.tar.gz';          ;;        armhf|arm)          ESUM='8cf113d3d7fa808895c8d2e41bb890af21c47e38c2460e0588147a4bb8fc658d';          BINARY_URL='https://github.com/adoptium/temurin11-binaries/releases/download/jdk-11.0.17%2B8/OpenJDK11U-jre_arm_linux_hotspot_11.0.17_8.tar.gz';          ;;        ppc64el|powerpc:common64)          ESUM='0ca3d806131ab5834c501f9c625bb0248cd528af361c704503348e9c9605bedf';          BINARY_URL='https://github.com/adoptium/temurin11-binaries/releases/download/jdk-11.0.17%2B8/OpenJDK11U-jre_ppc64le_linux_hotspot_11.0.17_8.tar.gz';          ;;        s390x|s390:64-bit)          ESUM='dd3b159a374086e65cb07c4ccb226c90f9c02ef929cba6f0b642171d7ed97fa4';          BINARY_URL='https://github.com/adoptium/temurin11-binaries/releases/download/jdk-11.0.17%2B8/OpenJDK11U-jre_s390x_linux_hotspot_11.0.17_8.tar.gz';          ;;        amd64|i386:x86-64)          ESUM='752616097e09d7f60a3ad8bd312f90eaf50ac72577e55df229fe6e8091148f79';          BINARY_URL='https://github.com/adoptium/temurin11-binaries/releases/download/jdk-11.0.17%2B8/OpenJDK11U-jre_x64_linux_hotspot_11.0.17_8.tar.gz';          ;;        *)          echo "Unsupported arch: ${ARCH}";          exit 1;          ;;     esac; 	  wget -O /tmp/openjdk.tar.gz ${BINARY_URL}; 	  echo "${ESUM} */tmp/openjdk.tar.gz" | sha256sum -c -; 	  mkdir -p "$JAVA_HOME"; 	  tar --extract 	      --file /tmp/openjdk.tar.gz 	      --directory "$JAVA_HOME" 	      --strip-components 1 	      --no-same-owner 	  ;     rm /tmp/openjdk.tar.gz;     find "$JAVA_HOME/lib" -name '*.so' -exec dirname '{}' ';' | sort -u > /etc/ld.so.conf.d/docker-openjdk.conf;     ldconfig;     java -Xshare:dump;
# Fri, 04 Nov 2022 22:41:34 GMT
RUN echo Verifying install ...     && fileEncoding="$(echo 'System.out.println(System.getProperty("file.encoding"))' | jshell -s -)"; [ "$fileEncoding" = 'UTF-8' ]; rm -rf ~/.java     && echo java --version && java --version     && echo Complete.
# Fri, 04 Nov 2022 23:48:38 GMT
ENV CATALINA_HOME=/usr/local/tomcat
# Fri, 04 Nov 2022 23:48:38 GMT
ENV PATH=/usr/local/tomcat/bin:/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Fri, 04 Nov 2022 23:48:38 GMT
RUN mkdir -p "$CATALINA_HOME"
# Fri, 04 Nov 2022 23:48:39 GMT
WORKDIR /usr/local/tomcat
# Fri, 04 Nov 2022 23:48:39 GMT
ENV TOMCAT_NATIVE_LIBDIR=/usr/local/tomcat/native-jni-lib
# Fri, 04 Nov 2022 23:48:39 GMT
ENV LD_LIBRARY_PATH=/usr/local/tomcat/native-jni-lib
# Fri, 04 Nov 2022 23:53:12 GMT
ENV GPG_KEYS=48F8E69F6390C9F25CFEDCD268248959359E722B A9C5DF4D22E99998D9875A5110C01C5A2F6059E7 DCFD35E0BF8CA7344752DE8B6FB21E8933C60243
# Fri, 04 Nov 2022 23:53:12 GMT
ENV TOMCAT_MAJOR=9
# Tue, 15 Nov 2022 04:57:22 GMT
ENV TOMCAT_VERSION=9.0.69
# Tue, 15 Nov 2022 04:57:22 GMT
ENV TOMCAT_SHA512=8c883c54ce9ce43eba37756a6404cdf3477879883a3e6d146dc8a7aa5e0425f487466afe6b6da4a895927cb7cb59177b9379cec18000f2de12785be57408c779
# Tue, 15 Nov 2022 04:57:22 GMT
COPY dir:096b403a5f78b17e6b4bff63128a9c93941b97f22470991610dd641633d977f1 in /usr/local/tomcat 
# Tue, 15 Nov 2022 04:57:25 GMT
RUN set -eux; 	apt-get update; 	xargs -rt apt-get install -y --no-install-recommends < "$TOMCAT_NATIVE_LIBDIR/.dependencies.txt"; 	rm -rf /var/lib/apt/lists/*
# Tue, 15 Nov 2022 04:57:26 GMT
RUN set -eux; 	nativeLines="$(catalina.sh configtest 2>&1)"; 	nativeLines="$(echo "$nativeLines" | grep 'Apache Tomcat Native')"; 	nativeLines="$(echo "$nativeLines" | sort -u)"; 	if ! echo "$nativeLines" | grep -E 'INFO: Loaded( APR based)? Apache Tomcat Native library' >&2; then 		echo >&2 "$nativeLines"; 		exit 1; 	fi
# Tue, 15 Nov 2022 04:57:26 GMT
EXPOSE 8080
# Tue, 15 Nov 2022 04:57:27 GMT
CMD ["catalina.sh" "run"]
# Wed, 11 Jan 2023 03:05:10 GMT
LABEL org.opencontainers.image.authors=XWiki Development Team <committers@xwiki.org>
# Wed, 11 Jan 2023 03:05:10 GMT
LABEL org.opencontainers.image.url=https://hub.docker.com/_/xwiki
# Wed, 11 Jan 2023 03:05:10 GMT
LABEL org.opencontainers.image.documentation=https://hub.docker.com/_/xwiki
# Wed, 11 Jan 2023 03:05:10 GMT
LABEL org.opencontainers.image.source=https://github.com/xwiki/xwiki-docker.git
# Wed, 11 Jan 2023 03:05:11 GMT
LABEL org.opencontainers.image.vendor=xwiki.org
# Wed, 11 Jan 2023 03:05:11 GMT
LABEL org.opencontainers.image.licenses=LGPL-2.1
# Wed, 11 Jan 2023 03:07:37 GMT
RUN apt-get update &&   apt-get --no-install-recommends -y install     curl     libreoffice     unzip     procps &&   rm -rf /var/lib/apt/lists/*
# Wed, 01 Feb 2023 22:26:19 GMT
ENV XWIKI_VERSION=14.10.4
# Wed, 01 Feb 2023 22:26:19 GMT
ENV XWIKI_URL_PREFIX=https://maven.xwiki.org/releases/org/xwiki/platform/xwiki-platform-distribution-war/14.10.4
# Wed, 01 Feb 2023 22:26:19 GMT
ENV XWIKI_DOWNLOAD_SHA256=2fcfb622319172c2e424b9c11848ebfabe27cf8ef69cba39ceb5d124b7ebe713
# Wed, 01 Feb 2023 22:27:00 GMT
RUN rm -rf /usr/local/tomcat/webapps/* &&   mkdir -p /usr/local/tomcat/temp &&   mkdir -p /usr/local/xwiki/data &&   curl -fSL "${XWIKI_URL_PREFIX}/xwiki-platform-distribution-war-${XWIKI_VERSION}.war" -o xwiki.war &&   echo "$XWIKI_DOWNLOAD_SHA256 xwiki.war" | sha256sum -c - &&   unzip -d /usr/local/tomcat/webapps/ROOT xwiki.war &&   rm -f xwiki.war
# Wed, 01 Feb 2023 22:27:03 GMT
ENV MYSQL_JDBC_VERSION=8.0.31
# Wed, 01 Feb 2023 22:27:03 GMT
ENV MYSQL_JDBC_SHA256=5249e3dc6d6531b37790e3f61845b96db5e41e891d3d8edb0e2e3a1b53ca2f4f
# Wed, 01 Feb 2023 22:27:03 GMT
ENV MYSQL_JDBC_PREFIX=https://repo1.maven.org/maven2/com/mysql/mysql-connector-j/8.0.31
# Wed, 01 Feb 2023 22:27:03 GMT
ENV MYSQL_JDBC_ARTIFACT=mysql-connector-j-8.0.31.jar
# Wed, 01 Feb 2023 22:27:03 GMT
ENV MYSQL_JDBC_TARGET=/usr/local/tomcat/webapps/ROOT/WEB-INF/lib/mysql-connector-j-8.0.31.jar
# Wed, 01 Feb 2023 22:27:04 GMT
RUN curl -fSL "${MYSQL_JDBC_PREFIX}/${MYSQL_JDBC_ARTIFACT}" -o $MYSQL_JDBC_TARGET &&   echo "$MYSQL_JDBC_SHA256 $MYSQL_JDBC_TARGET" | sha256sum -c -
# Wed, 01 Feb 2023 22:27:04 GMT
COPY file:0a1be11e2eb610a1dbcd415404e3a592641110b93090030cb831e3a19a163017 in /usr/local/tomcat/bin/ 
# Wed, 01 Feb 2023 22:27:04 GMT
COPY file:1b8409986f3e4eb79a7a0b18472cb2692a61d504fb5ef34292bc997b79fd760d in /usr/local/tomcat/webapps/ROOT/WEB-INF/hibernate.cfg.xml 
# Wed, 01 Feb 2023 22:27:05 GMT
RUN sed -i 's/<id>org.xwiki.platform:xwiki-platform-distribution-war/<id>org.xwiki.platform:xwiki-platform-distribution-docker/'   /usr/local/tomcat/webapps/ROOT/META-INF/extension.xed
# Wed, 01 Feb 2023 22:27:05 GMT
COPY file:a47c4dcd87c9dad97aff38c49188357e6193bcad50757e516cfb08a60d4de611 in /usr/local/bin/docker-entrypoint.sh 
# Wed, 01 Feb 2023 22:27:05 GMT
VOLUME [/usr/local/xwiki]
# Wed, 01 Feb 2023 22:27:05 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 01 Feb 2023 22:27:05 GMT
CMD ["xwiki"]
```

-	Layers:
	-	`sha256:0509fae36eb0656f8bdb23f8ae64100d893bcea2563e97468d337e04d2d0410b`  
		Last Modified: Wed, 02 Nov 2022 18:50:21 GMT  
		Size: 28.4 MB (28382154 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e502a1af2bcd98f5f0d2f5e4da1a0e7bbe07a2c548e2662f7d37dce5ae1df46c`  
		Last Modified: Wed, 02 Nov 2022 19:48:28 GMT  
		Size: 12.4 MB (12396330 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bc4598c07dd818f03a0378b0341a4a8e80f0152fbb3e7d5246ca4f466f42e611`  
		Last Modified: Fri, 04 Nov 2022 22:46:46 GMT  
		Size: 45.0 MB (44958470 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:715a937a1066f998b331fcd62256ad01a5571bdf46804e97825afc64f9ebb427`  
		Last Modified: Fri, 04 Nov 2022 22:46:41 GMT  
		Size: 160.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5fb623f082f74b2fa9fc2c4e3f3a4802875cb9753cfa26ed940201ce72bb56cb`  
		Last Modified: Sat, 05 Nov 2022 00:03:40 GMT  
		Size: 172.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:33260b83200262bbd546be371ad3c1f50f5ae7228afb87982d6fa9d6b11bf26f`  
		Last Modified: Tue, 15 Nov 2022 05:10:19 GMT  
		Size: 12.2 MB (12207235 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0955fb697ea9b30a1b4f95385464f646aa1525cb6efba648e22df84ebef6b2ee`  
		Last Modified: Tue, 15 Nov 2022 05:10:18 GMT  
		Size: 452.0 KB (452021 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6eddcf66f2083b1487296a0308e0b058917c97f614f12428d82d89662038dc2e`  
		Last Modified: Tue, 15 Nov 2022 05:10:18 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ae5f60bb64f3fa11da3d15a9639f886186b4c2c021455c3f9db22e0cfe1b1311`  
		Last Modified: Wed, 11 Jan 2023 03:11:14 GMT  
		Size: 173.8 MB (173806827 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:13334e257ce7313ca9d6028534e3ec6c7858c374c4afedea7f96c51da716806e`  
		Last Modified: Wed, 01 Feb 2023 22:29:16 GMT  
		Size: 307.1 MB (307104849 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ccb59878c7670194b75b6af22dd3908f9ae1a12dc1074f0b5ed156a5e3afdf0a`  
		Last Modified: Wed, 01 Feb 2023 22:29:02 GMT  
		Size: 2.4 MB (2377177 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d3946fb25102529cda96bcad4925905c9b997e442b447675d89066505cbe1026`  
		Last Modified: Wed, 01 Feb 2023 22:29:02 GMT  
		Size: 1.3 KB (1344 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1ba832da71f2ed07bae5269bb37e7ea79724a069ad63032f2af14996893baa37`  
		Last Modified: Wed, 01 Feb 2023 22:29:02 GMT  
		Size: 2.3 KB (2307 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6616193191331001a42a5d452ea69a215bbc414eca5cb00914c359665be5817f`  
		Last Modified: Wed, 01 Feb 2023 22:29:02 GMT  
		Size: 6.0 KB (6009 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6de4b8ce214cd9b76eda5b4955e5abb249a0b0292e8a38d39683e3002d6534bf`  
		Last Modified: Wed, 01 Feb 2023 22:29:03 GMT  
		Size: 2.5 KB (2506 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `xwiki:14.10-postgres-tomcat`

```console
$ docker pull xwiki@sha256:48a8c82a2dcfa36f6d55a5f3e75d3e2b3aca3f80de56276b35838dc7bcb6a4a6
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `xwiki:14.10-postgres-tomcat` - linux; amd64

```console
$ docker pull xwiki@sha256:5cd23e4200b4eed664a61d05e3d436d0e372a3e4e985e29cb866dd9dbb573713
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **590.0 MB (589983532 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ab0dc70572c5101e5837a6281e7cb29a2b4dbf26ad0b9c91860a748aeb3360e1`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["xwiki"]`

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
# Wed, 02 Nov 2022 18:44:10 GMT
RUN apt-get update     && DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends tzdata curl wget ca-certificates fontconfig locales     && echo "en_US.UTF-8 UTF-8" >> /etc/locale.gen     && locale-gen en_US.UTF-8     && rm -rf /var/lib/apt/lists/*
# Fri, 04 Nov 2022 23:21:41 GMT
ENV JAVA_VERSION=jdk-11.0.17+8
# Fri, 04 Nov 2022 23:22:31 GMT
RUN set -eux;     ARCH="$(dpkg --print-architecture)";     case "${ARCH}" in        aarch64|arm64)          ESUM='bd6efe3290c8b5a42f695a55a26f3e3c9c284288574879d4b7089f31f5114177';          BINARY_URL='https://github.com/adoptium/temurin11-binaries/releases/download/jdk-11.0.17%2B8/OpenJDK11U-jre_aarch64_linux_hotspot_11.0.17_8.tar.gz';          ;;        armhf|arm)          ESUM='8cf113d3d7fa808895c8d2e41bb890af21c47e38c2460e0588147a4bb8fc658d';          BINARY_URL='https://github.com/adoptium/temurin11-binaries/releases/download/jdk-11.0.17%2B8/OpenJDK11U-jre_arm_linux_hotspot_11.0.17_8.tar.gz';          ;;        ppc64el|powerpc:common64)          ESUM='0ca3d806131ab5834c501f9c625bb0248cd528af361c704503348e9c9605bedf';          BINARY_URL='https://github.com/adoptium/temurin11-binaries/releases/download/jdk-11.0.17%2B8/OpenJDK11U-jre_ppc64le_linux_hotspot_11.0.17_8.tar.gz';          ;;        s390x|s390:64-bit)          ESUM='dd3b159a374086e65cb07c4ccb226c90f9c02ef929cba6f0b642171d7ed97fa4';          BINARY_URL='https://github.com/adoptium/temurin11-binaries/releases/download/jdk-11.0.17%2B8/OpenJDK11U-jre_s390x_linux_hotspot_11.0.17_8.tar.gz';          ;;        amd64|i386:x86-64)          ESUM='752616097e09d7f60a3ad8bd312f90eaf50ac72577e55df229fe6e8091148f79';          BINARY_URL='https://github.com/adoptium/temurin11-binaries/releases/download/jdk-11.0.17%2B8/OpenJDK11U-jre_x64_linux_hotspot_11.0.17_8.tar.gz';          ;;        *)          echo "Unsupported arch: ${ARCH}";          exit 1;          ;;     esac; 	  wget -O /tmp/openjdk.tar.gz ${BINARY_URL}; 	  echo "${ESUM} */tmp/openjdk.tar.gz" | sha256sum -c -; 	  mkdir -p "$JAVA_HOME"; 	  tar --extract 	      --file /tmp/openjdk.tar.gz 	      --directory "$JAVA_HOME" 	      --strip-components 1 	      --no-same-owner 	  ;     rm /tmp/openjdk.tar.gz;     find "$JAVA_HOME/lib" -name '*.so' -exec dirname '{}' ';' | sort -u > /etc/ld.so.conf.d/docker-openjdk.conf;     ldconfig;     java -Xshare:dump;
# Fri, 04 Nov 2022 23:22:32 GMT
RUN echo Verifying install ...     && fileEncoding="$(echo 'System.out.println(System.getProperty("file.encoding"))' | jshell -s -)"; [ "$fileEncoding" = 'UTF-8' ]; rm -rf ~/.java     && echo java --version && java --version     && echo Complete.
# Sat, 05 Nov 2022 01:35:16 GMT
ENV CATALINA_HOME=/usr/local/tomcat
# Sat, 05 Nov 2022 01:35:16 GMT
ENV PATH=/usr/local/tomcat/bin:/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Sat, 05 Nov 2022 01:35:17 GMT
RUN mkdir -p "$CATALINA_HOME"
# Sat, 05 Nov 2022 01:35:17 GMT
WORKDIR /usr/local/tomcat
# Sat, 05 Nov 2022 01:35:17 GMT
ENV TOMCAT_NATIVE_LIBDIR=/usr/local/tomcat/native-jni-lib
# Sat, 05 Nov 2022 01:35:17 GMT
ENV LD_LIBRARY_PATH=/usr/local/tomcat/native-jni-lib
# Sat, 05 Nov 2022 01:39:54 GMT
ENV GPG_KEYS=48F8E69F6390C9F25CFEDCD268248959359E722B A9C5DF4D22E99998D9875A5110C01C5A2F6059E7 DCFD35E0BF8CA7344752DE8B6FB21E8933C60243
# Sat, 05 Nov 2022 01:39:54 GMT
ENV TOMCAT_MAJOR=9
# Tue, 15 Nov 2022 03:06:43 GMT
ENV TOMCAT_VERSION=9.0.69
# Tue, 15 Nov 2022 03:06:43 GMT
ENV TOMCAT_SHA512=8c883c54ce9ce43eba37756a6404cdf3477879883a3e6d146dc8a7aa5e0425f487466afe6b6da4a895927cb7cb59177b9379cec18000f2de12785be57408c779
# Tue, 15 Nov 2022 03:06:44 GMT
COPY dir:b1a33aa3993dbbfbebb33bd9aa546b60c2f2191abf1227f453d4e830f6deb35f in /usr/local/tomcat 
# Tue, 15 Nov 2022 03:06:48 GMT
RUN set -eux; 	apt-get update; 	xargs -rt apt-get install -y --no-install-recommends < "$TOMCAT_NATIVE_LIBDIR/.dependencies.txt"; 	rm -rf /var/lib/apt/lists/*
# Tue, 15 Nov 2022 03:06:49 GMT
RUN set -eux; 	nativeLines="$(catalina.sh configtest 2>&1)"; 	nativeLines="$(echo "$nativeLines" | grep 'Apache Tomcat Native')"; 	nativeLines="$(echo "$nativeLines" | sort -u)"; 	if ! echo "$nativeLines" | grep -E 'INFO: Loaded( APR based)? Apache Tomcat Native library' >&2; then 		echo >&2 "$nativeLines"; 		exit 1; 	fi
# Tue, 15 Nov 2022 03:06:49 GMT
EXPOSE 8080
# Tue, 15 Nov 2022 03:06:49 GMT
CMD ["catalina.sh" "run"]
# Wed, 11 Jan 2023 02:47:03 GMT
LABEL org.opencontainers.image.authors=XWiki Development Team <committers@xwiki.org>
# Wed, 11 Jan 2023 02:47:03 GMT
LABEL org.opencontainers.image.url=https://hub.docker.com/_/xwiki
# Wed, 11 Jan 2023 02:47:03 GMT
LABEL org.opencontainers.image.documentation=https://hub.docker.com/_/xwiki
# Wed, 11 Jan 2023 02:47:03 GMT
LABEL org.opencontainers.image.source=https://github.com/xwiki/xwiki-docker.git
# Wed, 11 Jan 2023 02:47:04 GMT
LABEL org.opencontainers.image.vendor=xwiki.org
# Wed, 11 Jan 2023 02:47:04 GMT
LABEL org.opencontainers.image.licenses=LGPL-2.1
# Wed, 11 Jan 2023 02:50:25 GMT
RUN apt-get update &&   apt-get --no-install-recommends -y install     curl     libreoffice     unzip     procps     libpostgresql-jdbc-java &&   rm -rf /var/lib/apt/lists/*
# Wed, 22 Feb 2023 18:40:25 GMT
ENV XWIKI_VERSION=14.10.5
# Wed, 22 Feb 2023 18:40:25 GMT
ENV XWIKI_URL_PREFIX=https://maven.xwiki.org/releases/org/xwiki/platform/xwiki-platform-distribution-war/14.10.5
# Wed, 22 Feb 2023 18:40:25 GMT
ENV XWIKI_DOWNLOAD_SHA256=f58465d0869e4c5605ae8375a09c79399d1149c7131fed3cf9959918267eb6a8
# Wed, 22 Feb 2023 18:41:04 GMT
RUN rm -rf /usr/local/tomcat/webapps/* &&   mkdir -p /usr/local/tomcat/temp &&   mkdir -p /usr/local/xwiki/data &&   curl -fSL "${XWIKI_URL_PREFIX}/xwiki-platform-distribution-war-${XWIKI_VERSION}.war" -o xwiki.war &&   echo "$XWIKI_DOWNLOAD_SHA256 xwiki.war" | sha256sum -c - &&   unzip -d /usr/local/tomcat/webapps/ROOT xwiki.war &&   rm -f xwiki.war
# Wed, 22 Feb 2023 18:41:05 GMT
RUN cp /usr/share/java/postgresql-jdbc4.jar /usr/local/tomcat/webapps/ROOT/WEB-INF/lib/
# Wed, 22 Feb 2023 18:41:05 GMT
COPY file:0a1be11e2eb610a1dbcd415404e3a592641110b93090030cb831e3a19a163017 in /usr/local/tomcat/bin/ 
# Wed, 22 Feb 2023 18:41:05 GMT
COPY file:4a923f484bb29a26630c19e1d617d3bf6aa6ae7c6c4a5561e97b037bcde0847c in /usr/local/tomcat/webapps/ROOT/WEB-INF/hibernate.cfg.xml 
# Wed, 22 Feb 2023 18:41:06 GMT
RUN sed -i 's/<id>org.xwiki.platform:xwiki-platform-distribution-war/<id>org.xwiki.platform:xwiki-platform-distribution-docker/'   /usr/local/tomcat/webapps/ROOT/META-INF/extension.xed
# Wed, 22 Feb 2023 18:41:06 GMT
COPY file:a47c4dcd87c9dad97aff38c49188357e6193bcad50757e516cfb08a60d4de611 in /usr/local/bin/docker-entrypoint.sh 
# Wed, 22 Feb 2023 18:41:06 GMT
VOLUME [/usr/local/xwiki]
# Wed, 22 Feb 2023 18:41:06 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 22 Feb 2023 18:41:06 GMT
CMD ["xwiki"]
```

-	Layers:
	-	`sha256:e96e057aae67380a4ddb16c337c5c3669d97fdff69ec537f02aa2cc30d814281`  
		Last Modified: Wed, 02 Nov 2022 03:03:36 GMT  
		Size: 30.4 MB (30425607 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4ced2591451da3a02e2b6bb44752b9e3f00d77789921be4df5082fb9f9880ad0`  
		Last Modified: Wed, 02 Nov 2022 18:48:43 GMT  
		Size: 12.4 MB (12439006 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:df8f874ae8c08a9e69e5fbe6c5a64200a45386132a3203d1a9a7f1146d94cfbc`  
		Last Modified: Fri, 04 Nov 2022 23:29:33 GMT  
		Size: 46.6 MB (46629936 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:111b6c7486426c4b6989102c2ee5be856e8a58e20ab0a350b24a905d536e8e7f`  
		Last Modified: Fri, 04 Nov 2022 23:29:26 GMT  
		Size: 161.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e6f84dce457c6d4f7b7291fce05f8e77998a3a7722a54125a1f1d52ca83043b4`  
		Last Modified: Sat, 05 Nov 2022 01:50:51 GMT  
		Size: 173.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a6c26749ee782392e38845ee2ba79b0da586ef6a45d8e7f29c7af14612278547`  
		Last Modified: Tue, 15 Nov 2022 03:19:57 GMT  
		Size: 12.2 MB (12200249 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4dddc6d9fa6024025b3fcfe729cab2dc544fb25476eca6e80b1af8e8d93bb0ee`  
		Last Modified: Tue, 15 Nov 2022 03:19:56 GMT  
		Size: 452.7 KB (452680 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:06637eebe5e72c8ad9019ad4eb4cdde1f11f7d4c24c7ed7374cf8966343aa2fb`  
		Last Modified: Tue, 15 Nov 2022 03:19:56 GMT  
		Size: 131.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b57f6f8bcfb0d93b8e21d3068d1f65d3f08dba05c5fab7d4c36e2359317b18c7`  
		Last Modified: Wed, 11 Jan 2023 02:53:53 GMT  
		Size: 179.7 MB (179745182 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b26b00a2f6717a934b9a1b08bac612aaaf57a4cfb4d82db521e7d36755621933`  
		Last Modified: Wed, 22 Feb 2023 18:43:06 GMT  
		Size: 307.1 MB (307141251 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:11801aa48fd913e3278b4d0a512df366a8ef26c1cc3e95a8439a1be90aadfd5a`  
		Last Modified: Wed, 22 Feb 2023 18:42:50 GMT  
		Size: 936.9 KB (936850 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fb4e8755162307a316ff405759f2417dc77e746651f89c83a0477ab19dc7da5d`  
		Last Modified: Wed, 22 Feb 2023 18:42:50 GMT  
		Size: 1.3 KB (1342 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2ba124a3d49367a8e2f46fc2043189f91e2dd282d40a301d9c1f79a705d35e66`  
		Last Modified: Wed, 22 Feb 2023 18:42:50 GMT  
		Size: 2.5 KB (2450 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8f421201132c3966dbb37a473df5922718780304fa03993ef75bb78522d5cafd`  
		Last Modified: Wed, 22 Feb 2023 18:42:50 GMT  
		Size: 6.0 KB (6012 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1b5dc6b32b3d1d9a80058f5ffc684363a0cfadf60ade5875fa37854ec7b46fff`  
		Last Modified: Wed, 22 Feb 2023 18:42:50 GMT  
		Size: 2.5 KB (2502 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `xwiki:14.10-postgres-tomcat` - linux; arm64 variant v8

```console
$ docker pull xwiki@sha256:e04b6d052b479b648834e5d960deff2f28274834a9dc812b628ccb9a624c53ef
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **581.2 MB (581199952 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:4693188024e4d84ad63e783e3377e2d600a040c344f7f36ab1bff14f5630ffe7`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["xwiki"]`

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
# Wed, 02 Nov 2022 19:44:32 GMT
RUN apt-get update     && DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends tzdata curl wget ca-certificates fontconfig locales     && echo "en_US.UTF-8 UTF-8" >> /etc/locale.gen     && locale-gen en_US.UTF-8     && rm -rf /var/lib/apt/lists/*
# Fri, 04 Nov 2022 22:40:54 GMT
ENV JAVA_VERSION=jdk-11.0.17+8
# Fri, 04 Nov 2022 22:41:33 GMT
RUN set -eux;     ARCH="$(dpkg --print-architecture)";     case "${ARCH}" in        aarch64|arm64)          ESUM='bd6efe3290c8b5a42f695a55a26f3e3c9c284288574879d4b7089f31f5114177';          BINARY_URL='https://github.com/adoptium/temurin11-binaries/releases/download/jdk-11.0.17%2B8/OpenJDK11U-jre_aarch64_linux_hotspot_11.0.17_8.tar.gz';          ;;        armhf|arm)          ESUM='8cf113d3d7fa808895c8d2e41bb890af21c47e38c2460e0588147a4bb8fc658d';          BINARY_URL='https://github.com/adoptium/temurin11-binaries/releases/download/jdk-11.0.17%2B8/OpenJDK11U-jre_arm_linux_hotspot_11.0.17_8.tar.gz';          ;;        ppc64el|powerpc:common64)          ESUM='0ca3d806131ab5834c501f9c625bb0248cd528af361c704503348e9c9605bedf';          BINARY_URL='https://github.com/adoptium/temurin11-binaries/releases/download/jdk-11.0.17%2B8/OpenJDK11U-jre_ppc64le_linux_hotspot_11.0.17_8.tar.gz';          ;;        s390x|s390:64-bit)          ESUM='dd3b159a374086e65cb07c4ccb226c90f9c02ef929cba6f0b642171d7ed97fa4';          BINARY_URL='https://github.com/adoptium/temurin11-binaries/releases/download/jdk-11.0.17%2B8/OpenJDK11U-jre_s390x_linux_hotspot_11.0.17_8.tar.gz';          ;;        amd64|i386:x86-64)          ESUM='752616097e09d7f60a3ad8bd312f90eaf50ac72577e55df229fe6e8091148f79';          BINARY_URL='https://github.com/adoptium/temurin11-binaries/releases/download/jdk-11.0.17%2B8/OpenJDK11U-jre_x64_linux_hotspot_11.0.17_8.tar.gz';          ;;        *)          echo "Unsupported arch: ${ARCH}";          exit 1;          ;;     esac; 	  wget -O /tmp/openjdk.tar.gz ${BINARY_URL}; 	  echo "${ESUM} */tmp/openjdk.tar.gz" | sha256sum -c -; 	  mkdir -p "$JAVA_HOME"; 	  tar --extract 	      --file /tmp/openjdk.tar.gz 	      --directory "$JAVA_HOME" 	      --strip-components 1 	      --no-same-owner 	  ;     rm /tmp/openjdk.tar.gz;     find "$JAVA_HOME/lib" -name '*.so' -exec dirname '{}' ';' | sort -u > /etc/ld.so.conf.d/docker-openjdk.conf;     ldconfig;     java -Xshare:dump;
# Fri, 04 Nov 2022 22:41:34 GMT
RUN echo Verifying install ...     && fileEncoding="$(echo 'System.out.println(System.getProperty("file.encoding"))' | jshell -s -)"; [ "$fileEncoding" = 'UTF-8' ]; rm -rf ~/.java     && echo java --version && java --version     && echo Complete.
# Fri, 04 Nov 2022 23:48:38 GMT
ENV CATALINA_HOME=/usr/local/tomcat
# Fri, 04 Nov 2022 23:48:38 GMT
ENV PATH=/usr/local/tomcat/bin:/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Fri, 04 Nov 2022 23:48:38 GMT
RUN mkdir -p "$CATALINA_HOME"
# Fri, 04 Nov 2022 23:48:39 GMT
WORKDIR /usr/local/tomcat
# Fri, 04 Nov 2022 23:48:39 GMT
ENV TOMCAT_NATIVE_LIBDIR=/usr/local/tomcat/native-jni-lib
# Fri, 04 Nov 2022 23:48:39 GMT
ENV LD_LIBRARY_PATH=/usr/local/tomcat/native-jni-lib
# Fri, 04 Nov 2022 23:53:12 GMT
ENV GPG_KEYS=48F8E69F6390C9F25CFEDCD268248959359E722B A9C5DF4D22E99998D9875A5110C01C5A2F6059E7 DCFD35E0BF8CA7344752DE8B6FB21E8933C60243
# Fri, 04 Nov 2022 23:53:12 GMT
ENV TOMCAT_MAJOR=9
# Tue, 15 Nov 2022 04:57:22 GMT
ENV TOMCAT_VERSION=9.0.69
# Tue, 15 Nov 2022 04:57:22 GMT
ENV TOMCAT_SHA512=8c883c54ce9ce43eba37756a6404cdf3477879883a3e6d146dc8a7aa5e0425f487466afe6b6da4a895927cb7cb59177b9379cec18000f2de12785be57408c779
# Tue, 15 Nov 2022 04:57:22 GMT
COPY dir:096b403a5f78b17e6b4bff63128a9c93941b97f22470991610dd641633d977f1 in /usr/local/tomcat 
# Tue, 15 Nov 2022 04:57:25 GMT
RUN set -eux; 	apt-get update; 	xargs -rt apt-get install -y --no-install-recommends < "$TOMCAT_NATIVE_LIBDIR/.dependencies.txt"; 	rm -rf /var/lib/apt/lists/*
# Tue, 15 Nov 2022 04:57:26 GMT
RUN set -eux; 	nativeLines="$(catalina.sh configtest 2>&1)"; 	nativeLines="$(echo "$nativeLines" | grep 'Apache Tomcat Native')"; 	nativeLines="$(echo "$nativeLines" | sort -u)"; 	if ! echo "$nativeLines" | grep -E 'INFO: Loaded( APR based)? Apache Tomcat Native library' >&2; then 		echo >&2 "$nativeLines"; 		exit 1; 	fi
# Tue, 15 Nov 2022 04:57:26 GMT
EXPOSE 8080
# Tue, 15 Nov 2022 04:57:27 GMT
CMD ["catalina.sh" "run"]
# Wed, 11 Jan 2023 03:05:10 GMT
LABEL org.opencontainers.image.authors=XWiki Development Team <committers@xwiki.org>
# Wed, 11 Jan 2023 03:05:10 GMT
LABEL org.opencontainers.image.url=https://hub.docker.com/_/xwiki
# Wed, 11 Jan 2023 03:05:10 GMT
LABEL org.opencontainers.image.documentation=https://hub.docker.com/_/xwiki
# Wed, 11 Jan 2023 03:05:10 GMT
LABEL org.opencontainers.image.source=https://github.com/xwiki/xwiki-docker.git
# Wed, 11 Jan 2023 03:05:11 GMT
LABEL org.opencontainers.image.vendor=xwiki.org
# Wed, 11 Jan 2023 03:05:11 GMT
LABEL org.opencontainers.image.licenses=LGPL-2.1
# Wed, 11 Jan 2023 03:08:55 GMT
RUN apt-get update &&   apt-get --no-install-recommends -y install     curl     libreoffice     unzip     procps     libpostgresql-jdbc-java &&   rm -rf /var/lib/apt/lists/*
# Wed, 01 Feb 2023 22:27:07 GMT
ENV XWIKI_VERSION=14.10.4
# Wed, 01 Feb 2023 22:27:07 GMT
ENV XWIKI_URL_PREFIX=https://maven.xwiki.org/releases/org/xwiki/platform/xwiki-platform-distribution-war/14.10.4
# Wed, 01 Feb 2023 22:27:07 GMT
ENV XWIKI_DOWNLOAD_SHA256=2fcfb622319172c2e424b9c11848ebfabe27cf8ef69cba39ceb5d124b7ebe713
# Wed, 01 Feb 2023 22:27:47 GMT
RUN rm -rf /usr/local/tomcat/webapps/* &&   mkdir -p /usr/local/tomcat/temp &&   mkdir -p /usr/local/xwiki/data &&   curl -fSL "${XWIKI_URL_PREFIX}/xwiki-platform-distribution-war-${XWIKI_VERSION}.war" -o xwiki.war &&   echo "$XWIKI_DOWNLOAD_SHA256 xwiki.war" | sha256sum -c - &&   unzip -d /usr/local/tomcat/webapps/ROOT xwiki.war &&   rm -f xwiki.war
# Wed, 01 Feb 2023 22:27:50 GMT
RUN cp /usr/share/java/postgresql-jdbc4.jar /usr/local/tomcat/webapps/ROOT/WEB-INF/lib/
# Wed, 01 Feb 2023 22:27:50 GMT
COPY file:0a1be11e2eb610a1dbcd415404e3a592641110b93090030cb831e3a19a163017 in /usr/local/tomcat/bin/ 
# Wed, 01 Feb 2023 22:27:50 GMT
COPY file:4a923f484bb29a26630c19e1d617d3bf6aa6ae7c6c4a5561e97b037bcde0847c in /usr/local/tomcat/webapps/ROOT/WEB-INF/hibernate.cfg.xml 
# Wed, 01 Feb 2023 22:27:50 GMT
RUN sed -i 's/<id>org.xwiki.platform:xwiki-platform-distribution-war/<id>org.xwiki.platform:xwiki-platform-distribution-docker/'   /usr/local/tomcat/webapps/ROOT/META-INF/extension.xed
# Wed, 01 Feb 2023 22:27:50 GMT
COPY file:a47c4dcd87c9dad97aff38c49188357e6193bcad50757e516cfb08a60d4de611 in /usr/local/bin/docker-entrypoint.sh 
# Wed, 01 Feb 2023 22:27:50 GMT
VOLUME [/usr/local/xwiki]
# Wed, 01 Feb 2023 22:27:51 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 01 Feb 2023 22:27:51 GMT
CMD ["xwiki"]
```

-	Layers:
	-	`sha256:0509fae36eb0656f8bdb23f8ae64100d893bcea2563e97468d337e04d2d0410b`  
		Last Modified: Wed, 02 Nov 2022 18:50:21 GMT  
		Size: 28.4 MB (28382154 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e502a1af2bcd98f5f0d2f5e4da1a0e7bbe07a2c548e2662f7d37dce5ae1df46c`  
		Last Modified: Wed, 02 Nov 2022 19:48:28 GMT  
		Size: 12.4 MB (12396330 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bc4598c07dd818f03a0378b0341a4a8e80f0152fbb3e7d5246ca4f466f42e611`  
		Last Modified: Fri, 04 Nov 2022 22:46:46 GMT  
		Size: 45.0 MB (44958470 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:715a937a1066f998b331fcd62256ad01a5571bdf46804e97825afc64f9ebb427`  
		Last Modified: Fri, 04 Nov 2022 22:46:41 GMT  
		Size: 160.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5fb623f082f74b2fa9fc2c4e3f3a4802875cb9753cfa26ed940201ce72bb56cb`  
		Last Modified: Sat, 05 Nov 2022 00:03:40 GMT  
		Size: 172.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:33260b83200262bbd546be371ad3c1f50f5ae7228afb87982d6fa9d6b11bf26f`  
		Last Modified: Tue, 15 Nov 2022 05:10:19 GMT  
		Size: 12.2 MB (12207235 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0955fb697ea9b30a1b4f95385464f646aa1525cb6efba648e22df84ebef6b2ee`  
		Last Modified: Tue, 15 Nov 2022 05:10:18 GMT  
		Size: 452.0 KB (452021 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6eddcf66f2083b1487296a0308e0b058917c97f614f12428d82d89662038dc2e`  
		Last Modified: Tue, 15 Nov 2022 05:10:18 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1ae6a8fce0f2cd131007393c1a4eba9ce9d0501da8406af5c5ce9deb5dc187b8`  
		Last Modified: Wed, 11 Jan 2023 03:12:13 GMT  
		Size: 174.7 MB (174749274 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:64fdf9e1ef0289a65afb558897bc408557b353c604c9e3bd5dfe845ddc54ab93`  
		Last Modified: Wed, 01 Feb 2023 22:30:00 GMT  
		Size: 307.1 MB (307104835 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0eee07814c2c9ef72478213f8e0091378d617e777e157e5f5550dbf992e4a8bb`  
		Last Modified: Wed, 01 Feb 2023 22:29:45 GMT  
		Size: 936.9 KB (936853 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:889aa9ab03d69382e94096e25991f58b06afde5b4238b94ac1136db5337d1028`  
		Last Modified: Wed, 01 Feb 2023 22:29:45 GMT  
		Size: 1.3 KB (1347 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d0d21fec462339352953dc0188b312a1e80154e3e38402e546f0e4200627f5dc`  
		Last Modified: Wed, 01 Feb 2023 22:29:45 GMT  
		Size: 2.5 KB (2455 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9c6493af5a9b0ca2b189b7be35d0f796b0243ab70d7f92a34a7eae40d269c8f3`  
		Last Modified: Wed, 01 Feb 2023 22:29:45 GMT  
		Size: 6.0 KB (6011 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3a5f6da30b6a4dcd443e582890b4a323952b0320b4c3474d31c01236b8f4cf5e`  
		Last Modified: Wed, 01 Feb 2023 22:29:45 GMT  
		Size: 2.5 KB (2506 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `xwiki:14.10.5`

```console
$ docker pull xwiki@sha256:301390c7e6252467e1773acbf7ca050b66a47a1277f29e6e40bf5bd98202eb00
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `xwiki:14.10.5` - linux; amd64

```console
$ docker pull xwiki@sha256:a2e996a399fc68cbccfe11eaeb0115a15314bd69f06c483fef3cba244fa07cbf
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **590.4 MB (590449604 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:6b73fd725d5c1dd8044289fdb0e76f973e7e1d4a64e1efc44428235a718b550a`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["xwiki"]`

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
# Wed, 02 Nov 2022 18:44:10 GMT
RUN apt-get update     && DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends tzdata curl wget ca-certificates fontconfig locales     && echo "en_US.UTF-8 UTF-8" >> /etc/locale.gen     && locale-gen en_US.UTF-8     && rm -rf /var/lib/apt/lists/*
# Fri, 04 Nov 2022 23:21:41 GMT
ENV JAVA_VERSION=jdk-11.0.17+8
# Fri, 04 Nov 2022 23:22:31 GMT
RUN set -eux;     ARCH="$(dpkg --print-architecture)";     case "${ARCH}" in        aarch64|arm64)          ESUM='bd6efe3290c8b5a42f695a55a26f3e3c9c284288574879d4b7089f31f5114177';          BINARY_URL='https://github.com/adoptium/temurin11-binaries/releases/download/jdk-11.0.17%2B8/OpenJDK11U-jre_aarch64_linux_hotspot_11.0.17_8.tar.gz';          ;;        armhf|arm)          ESUM='8cf113d3d7fa808895c8d2e41bb890af21c47e38c2460e0588147a4bb8fc658d';          BINARY_URL='https://github.com/adoptium/temurin11-binaries/releases/download/jdk-11.0.17%2B8/OpenJDK11U-jre_arm_linux_hotspot_11.0.17_8.tar.gz';          ;;        ppc64el|powerpc:common64)          ESUM='0ca3d806131ab5834c501f9c625bb0248cd528af361c704503348e9c9605bedf';          BINARY_URL='https://github.com/adoptium/temurin11-binaries/releases/download/jdk-11.0.17%2B8/OpenJDK11U-jre_ppc64le_linux_hotspot_11.0.17_8.tar.gz';          ;;        s390x|s390:64-bit)          ESUM='dd3b159a374086e65cb07c4ccb226c90f9c02ef929cba6f0b642171d7ed97fa4';          BINARY_URL='https://github.com/adoptium/temurin11-binaries/releases/download/jdk-11.0.17%2B8/OpenJDK11U-jre_s390x_linux_hotspot_11.0.17_8.tar.gz';          ;;        amd64|i386:x86-64)          ESUM='752616097e09d7f60a3ad8bd312f90eaf50ac72577e55df229fe6e8091148f79';          BINARY_URL='https://github.com/adoptium/temurin11-binaries/releases/download/jdk-11.0.17%2B8/OpenJDK11U-jre_x64_linux_hotspot_11.0.17_8.tar.gz';          ;;        *)          echo "Unsupported arch: ${ARCH}";          exit 1;          ;;     esac; 	  wget -O /tmp/openjdk.tar.gz ${BINARY_URL}; 	  echo "${ESUM} */tmp/openjdk.tar.gz" | sha256sum -c -; 	  mkdir -p "$JAVA_HOME"; 	  tar --extract 	      --file /tmp/openjdk.tar.gz 	      --directory "$JAVA_HOME" 	      --strip-components 1 	      --no-same-owner 	  ;     rm /tmp/openjdk.tar.gz;     find "$JAVA_HOME/lib" -name '*.so' -exec dirname '{}' ';' | sort -u > /etc/ld.so.conf.d/docker-openjdk.conf;     ldconfig;     java -Xshare:dump;
# Fri, 04 Nov 2022 23:22:32 GMT
RUN echo Verifying install ...     && fileEncoding="$(echo 'System.out.println(System.getProperty("file.encoding"))' | jshell -s -)"; [ "$fileEncoding" = 'UTF-8' ]; rm -rf ~/.java     && echo java --version && java --version     && echo Complete.
# Sat, 05 Nov 2022 01:35:16 GMT
ENV CATALINA_HOME=/usr/local/tomcat
# Sat, 05 Nov 2022 01:35:16 GMT
ENV PATH=/usr/local/tomcat/bin:/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Sat, 05 Nov 2022 01:35:17 GMT
RUN mkdir -p "$CATALINA_HOME"
# Sat, 05 Nov 2022 01:35:17 GMT
WORKDIR /usr/local/tomcat
# Sat, 05 Nov 2022 01:35:17 GMT
ENV TOMCAT_NATIVE_LIBDIR=/usr/local/tomcat/native-jni-lib
# Sat, 05 Nov 2022 01:35:17 GMT
ENV LD_LIBRARY_PATH=/usr/local/tomcat/native-jni-lib
# Sat, 05 Nov 2022 01:39:54 GMT
ENV GPG_KEYS=48F8E69F6390C9F25CFEDCD268248959359E722B A9C5DF4D22E99998D9875A5110C01C5A2F6059E7 DCFD35E0BF8CA7344752DE8B6FB21E8933C60243
# Sat, 05 Nov 2022 01:39:54 GMT
ENV TOMCAT_MAJOR=9
# Tue, 15 Nov 2022 03:06:43 GMT
ENV TOMCAT_VERSION=9.0.69
# Tue, 15 Nov 2022 03:06:43 GMT
ENV TOMCAT_SHA512=8c883c54ce9ce43eba37756a6404cdf3477879883a3e6d146dc8a7aa5e0425f487466afe6b6da4a895927cb7cb59177b9379cec18000f2de12785be57408c779
# Tue, 15 Nov 2022 03:06:44 GMT
COPY dir:b1a33aa3993dbbfbebb33bd9aa546b60c2f2191abf1227f453d4e830f6deb35f in /usr/local/tomcat 
# Tue, 15 Nov 2022 03:06:48 GMT
RUN set -eux; 	apt-get update; 	xargs -rt apt-get install -y --no-install-recommends < "$TOMCAT_NATIVE_LIBDIR/.dependencies.txt"; 	rm -rf /var/lib/apt/lists/*
# Tue, 15 Nov 2022 03:06:49 GMT
RUN set -eux; 	nativeLines="$(catalina.sh configtest 2>&1)"; 	nativeLines="$(echo "$nativeLines" | grep 'Apache Tomcat Native')"; 	nativeLines="$(echo "$nativeLines" | sort -u)"; 	if ! echo "$nativeLines" | grep -E 'INFO: Loaded( APR based)? Apache Tomcat Native library' >&2; then 		echo >&2 "$nativeLines"; 		exit 1; 	fi
# Tue, 15 Nov 2022 03:06:49 GMT
EXPOSE 8080
# Tue, 15 Nov 2022 03:06:49 GMT
CMD ["catalina.sh" "run"]
# Wed, 11 Jan 2023 02:47:03 GMT
LABEL org.opencontainers.image.authors=XWiki Development Team <committers@xwiki.org>
# Wed, 11 Jan 2023 02:47:03 GMT
LABEL org.opencontainers.image.url=https://hub.docker.com/_/xwiki
# Wed, 11 Jan 2023 02:47:03 GMT
LABEL org.opencontainers.image.documentation=https://hub.docker.com/_/xwiki
# Wed, 11 Jan 2023 02:47:03 GMT
LABEL org.opencontainers.image.source=https://github.com/xwiki/xwiki-docker.git
# Wed, 11 Jan 2023 02:47:04 GMT
LABEL org.opencontainers.image.vendor=xwiki.org
# Wed, 11 Jan 2023 02:47:04 GMT
LABEL org.opencontainers.image.licenses=LGPL-2.1
# Wed, 11 Jan 2023 02:49:03 GMT
RUN apt-get update &&   apt-get --no-install-recommends -y install     curl     libreoffice     unzip     procps &&   rm -rf /var/lib/apt/lists/*
# Wed, 22 Feb 2023 18:39:36 GMT
ENV XWIKI_VERSION=14.10.5
# Wed, 22 Feb 2023 18:39:36 GMT
ENV XWIKI_URL_PREFIX=https://maven.xwiki.org/releases/org/xwiki/platform/xwiki-platform-distribution-war/14.10.5
# Wed, 22 Feb 2023 18:39:36 GMT
ENV XWIKI_DOWNLOAD_SHA256=f58465d0869e4c5605ae8375a09c79399d1149c7131fed3cf9959918267eb6a8
# Wed, 22 Feb 2023 18:40:15 GMT
RUN rm -rf /usr/local/tomcat/webapps/* &&   mkdir -p /usr/local/tomcat/temp &&   mkdir -p /usr/local/xwiki/data &&   curl -fSL "${XWIKI_URL_PREFIX}/xwiki-platform-distribution-war-${XWIKI_VERSION}.war" -o xwiki.war &&   echo "$XWIKI_DOWNLOAD_SHA256 xwiki.war" | sha256sum -c - &&   unzip -d /usr/local/tomcat/webapps/ROOT xwiki.war &&   rm -f xwiki.war
# Wed, 22 Feb 2023 18:40:17 GMT
ENV MYSQL_JDBC_VERSION=8.0.32
# Wed, 22 Feb 2023 18:40:17 GMT
ENV MYSQL_JDBC_SHA256=522329fe925980f02e5eb89b59d227245d345415ff0c08932a68c9765c13acc5
# Wed, 22 Feb 2023 18:40:17 GMT
ENV MYSQL_JDBC_PREFIX=https://repo1.maven.org/maven2/com/mysql/mysql-connector-j/8.0.32
# Wed, 22 Feb 2023 18:40:17 GMT
ENV MYSQL_JDBC_ARTIFACT=mysql-connector-j-8.0.32.jar
# Wed, 22 Feb 2023 18:40:17 GMT
ENV MYSQL_JDBC_TARGET=/usr/local/tomcat/webapps/ROOT/WEB-INF/lib/mysql-connector-j-8.0.32.jar
# Wed, 22 Feb 2023 18:40:18 GMT
RUN curl -fSL "${MYSQL_JDBC_PREFIX}/${MYSQL_JDBC_ARTIFACT}" -o $MYSQL_JDBC_TARGET &&   echo "$MYSQL_JDBC_SHA256 $MYSQL_JDBC_TARGET" | sha256sum -c -
# Wed, 22 Feb 2023 18:40:18 GMT
COPY file:0a1be11e2eb610a1dbcd415404e3a592641110b93090030cb831e3a19a163017 in /usr/local/tomcat/bin/ 
# Wed, 22 Feb 2023 18:40:18 GMT
COPY file:1b8409986f3e4eb79a7a0b18472cb2692a61d504fb5ef34292bc997b79fd760d in /usr/local/tomcat/webapps/ROOT/WEB-INF/hibernate.cfg.xml 
# Wed, 22 Feb 2023 18:40:19 GMT
RUN sed -i 's/<id>org.xwiki.platform:xwiki-platform-distribution-war/<id>org.xwiki.platform:xwiki-platform-distribution-docker/'   /usr/local/tomcat/webapps/ROOT/META-INF/extension.xed
# Wed, 22 Feb 2023 18:40:19 GMT
COPY file:a47c4dcd87c9dad97aff38c49188357e6193bcad50757e516cfb08a60d4de611 in /usr/local/bin/docker-entrypoint.sh 
# Wed, 22 Feb 2023 18:40:19 GMT
VOLUME [/usr/local/xwiki]
# Wed, 22 Feb 2023 18:40:19 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 22 Feb 2023 18:40:19 GMT
CMD ["xwiki"]
```

-	Layers:
	-	`sha256:e96e057aae67380a4ddb16c337c5c3669d97fdff69ec537f02aa2cc30d814281`  
		Last Modified: Wed, 02 Nov 2022 03:03:36 GMT  
		Size: 30.4 MB (30425607 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4ced2591451da3a02e2b6bb44752b9e3f00d77789921be4df5082fb9f9880ad0`  
		Last Modified: Wed, 02 Nov 2022 18:48:43 GMT  
		Size: 12.4 MB (12439006 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:df8f874ae8c08a9e69e5fbe6c5a64200a45386132a3203d1a9a7f1146d94cfbc`  
		Last Modified: Fri, 04 Nov 2022 23:29:33 GMT  
		Size: 46.6 MB (46629936 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:111b6c7486426c4b6989102c2ee5be856e8a58e20ab0a350b24a905d536e8e7f`  
		Last Modified: Fri, 04 Nov 2022 23:29:26 GMT  
		Size: 161.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e6f84dce457c6d4f7b7291fce05f8e77998a3a7722a54125a1f1d52ca83043b4`  
		Last Modified: Sat, 05 Nov 2022 01:50:51 GMT  
		Size: 173.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a6c26749ee782392e38845ee2ba79b0da586ef6a45d8e7f29c7af14612278547`  
		Last Modified: Tue, 15 Nov 2022 03:19:57 GMT  
		Size: 12.2 MB (12200249 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4dddc6d9fa6024025b3fcfe729cab2dc544fb25476eca6e80b1af8e8d93bb0ee`  
		Last Modified: Tue, 15 Nov 2022 03:19:56 GMT  
		Size: 452.7 KB (452680 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:06637eebe5e72c8ad9019ad4eb4cdde1f11f7d4c24c7ed7374cf8966343aa2fb`  
		Last Modified: Tue, 15 Nov 2022 03:19:56 GMT  
		Size: 131.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b276fb8390410a8208724033e325715ea26000d5a1a762d4c3699b927884fbfe`  
		Last Modified: Wed, 11 Jan 2023 02:52:45 GMT  
		Size: 178.8 MB (178805608 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:89de9d9e2c09cd5b84430562516cbcd5695a0a3b2347b451e157bde75c2b5619`  
		Last Modified: Wed, 22 Feb 2023 18:42:21 GMT  
		Size: 307.1 MB (307141303 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4a2089179b7c1db514d0502e476e09b8f9313d08d4c4e4f3981be456288fe507`  
		Last Modified: Wed, 22 Feb 2023 18:42:04 GMT  
		Size: 2.3 MB (2342572 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e7c4ef360ff3673244adb3dfc4769b5710fa68fcc1fbe1c08b2f5fa32dbd4976`  
		Last Modified: Wed, 22 Feb 2023 18:42:04 GMT  
		Size: 1.3 KB (1348 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:08441c368d4b01e361491d7fbf1ac579fcc303b8484123c309a8d5a3b6657c46`  
		Last Modified: Wed, 22 Feb 2023 18:42:04 GMT  
		Size: 2.3 KB (2311 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:542b4bb846d438395e458c08de292f72d14d289fae6ffe7eba6fec1cd8518475`  
		Last Modified: Wed, 22 Feb 2023 18:42:04 GMT  
		Size: 6.0 KB (6013 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:039c0305df9e64c69bb546e64f0658dba6e728eee13022cfd682aa1ee76b8b7f`  
		Last Modified: Wed, 22 Feb 2023 18:42:04 GMT  
		Size: 2.5 KB (2506 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `xwiki:14.10.5-mariadb-tomcat`

```console
$ docker pull xwiki@sha256:1f3f5c24a758b34d8c61e835089fb931b0edaeb4c747715746c6913362c87408
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `xwiki:14.10.5-mariadb-tomcat` - linux; amd64

```console
$ docker pull xwiki@sha256:4aec14b2a2ae95584b839238412bbe33a7314bf32edc3e05f34f532d07fdedce
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **588.7 MB (588696916 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f5fbe86c66c7ac80e07663234a80353ce71d1847f409e2e2a603e0eb2a3342bc`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["xwiki"]`

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
# Wed, 02 Nov 2022 18:44:10 GMT
RUN apt-get update     && DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends tzdata curl wget ca-certificates fontconfig locales     && echo "en_US.UTF-8 UTF-8" >> /etc/locale.gen     && locale-gen en_US.UTF-8     && rm -rf /var/lib/apt/lists/*
# Fri, 04 Nov 2022 23:21:41 GMT
ENV JAVA_VERSION=jdk-11.0.17+8
# Fri, 04 Nov 2022 23:22:31 GMT
RUN set -eux;     ARCH="$(dpkg --print-architecture)";     case "${ARCH}" in        aarch64|arm64)          ESUM='bd6efe3290c8b5a42f695a55a26f3e3c9c284288574879d4b7089f31f5114177';          BINARY_URL='https://github.com/adoptium/temurin11-binaries/releases/download/jdk-11.0.17%2B8/OpenJDK11U-jre_aarch64_linux_hotspot_11.0.17_8.tar.gz';          ;;        armhf|arm)          ESUM='8cf113d3d7fa808895c8d2e41bb890af21c47e38c2460e0588147a4bb8fc658d';          BINARY_URL='https://github.com/adoptium/temurin11-binaries/releases/download/jdk-11.0.17%2B8/OpenJDK11U-jre_arm_linux_hotspot_11.0.17_8.tar.gz';          ;;        ppc64el|powerpc:common64)          ESUM='0ca3d806131ab5834c501f9c625bb0248cd528af361c704503348e9c9605bedf';          BINARY_URL='https://github.com/adoptium/temurin11-binaries/releases/download/jdk-11.0.17%2B8/OpenJDK11U-jre_ppc64le_linux_hotspot_11.0.17_8.tar.gz';          ;;        s390x|s390:64-bit)          ESUM='dd3b159a374086e65cb07c4ccb226c90f9c02ef929cba6f0b642171d7ed97fa4';          BINARY_URL='https://github.com/adoptium/temurin11-binaries/releases/download/jdk-11.0.17%2B8/OpenJDK11U-jre_s390x_linux_hotspot_11.0.17_8.tar.gz';          ;;        amd64|i386:x86-64)          ESUM='752616097e09d7f60a3ad8bd312f90eaf50ac72577e55df229fe6e8091148f79';          BINARY_URL='https://github.com/adoptium/temurin11-binaries/releases/download/jdk-11.0.17%2B8/OpenJDK11U-jre_x64_linux_hotspot_11.0.17_8.tar.gz';          ;;        *)          echo "Unsupported arch: ${ARCH}";          exit 1;          ;;     esac; 	  wget -O /tmp/openjdk.tar.gz ${BINARY_URL}; 	  echo "${ESUM} */tmp/openjdk.tar.gz" | sha256sum -c -; 	  mkdir -p "$JAVA_HOME"; 	  tar --extract 	      --file /tmp/openjdk.tar.gz 	      --directory "$JAVA_HOME" 	      --strip-components 1 	      --no-same-owner 	  ;     rm /tmp/openjdk.tar.gz;     find "$JAVA_HOME/lib" -name '*.so' -exec dirname '{}' ';' | sort -u > /etc/ld.so.conf.d/docker-openjdk.conf;     ldconfig;     java -Xshare:dump;
# Fri, 04 Nov 2022 23:22:32 GMT
RUN echo Verifying install ...     && fileEncoding="$(echo 'System.out.println(System.getProperty("file.encoding"))' | jshell -s -)"; [ "$fileEncoding" = 'UTF-8' ]; rm -rf ~/.java     && echo java --version && java --version     && echo Complete.
# Sat, 05 Nov 2022 01:35:16 GMT
ENV CATALINA_HOME=/usr/local/tomcat
# Sat, 05 Nov 2022 01:35:16 GMT
ENV PATH=/usr/local/tomcat/bin:/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Sat, 05 Nov 2022 01:35:17 GMT
RUN mkdir -p "$CATALINA_HOME"
# Sat, 05 Nov 2022 01:35:17 GMT
WORKDIR /usr/local/tomcat
# Sat, 05 Nov 2022 01:35:17 GMT
ENV TOMCAT_NATIVE_LIBDIR=/usr/local/tomcat/native-jni-lib
# Sat, 05 Nov 2022 01:35:17 GMT
ENV LD_LIBRARY_PATH=/usr/local/tomcat/native-jni-lib
# Sat, 05 Nov 2022 01:39:54 GMT
ENV GPG_KEYS=48F8E69F6390C9F25CFEDCD268248959359E722B A9C5DF4D22E99998D9875A5110C01C5A2F6059E7 DCFD35E0BF8CA7344752DE8B6FB21E8933C60243
# Sat, 05 Nov 2022 01:39:54 GMT
ENV TOMCAT_MAJOR=9
# Tue, 15 Nov 2022 03:06:43 GMT
ENV TOMCAT_VERSION=9.0.69
# Tue, 15 Nov 2022 03:06:43 GMT
ENV TOMCAT_SHA512=8c883c54ce9ce43eba37756a6404cdf3477879883a3e6d146dc8a7aa5e0425f487466afe6b6da4a895927cb7cb59177b9379cec18000f2de12785be57408c779
# Tue, 15 Nov 2022 03:06:44 GMT
COPY dir:b1a33aa3993dbbfbebb33bd9aa546b60c2f2191abf1227f453d4e830f6deb35f in /usr/local/tomcat 
# Tue, 15 Nov 2022 03:06:48 GMT
RUN set -eux; 	apt-get update; 	xargs -rt apt-get install -y --no-install-recommends < "$TOMCAT_NATIVE_LIBDIR/.dependencies.txt"; 	rm -rf /var/lib/apt/lists/*
# Tue, 15 Nov 2022 03:06:49 GMT
RUN set -eux; 	nativeLines="$(catalina.sh configtest 2>&1)"; 	nativeLines="$(echo "$nativeLines" | grep 'Apache Tomcat Native')"; 	nativeLines="$(echo "$nativeLines" | sort -u)"; 	if ! echo "$nativeLines" | grep -E 'INFO: Loaded( APR based)? Apache Tomcat Native library' >&2; then 		echo >&2 "$nativeLines"; 		exit 1; 	fi
# Tue, 15 Nov 2022 03:06:49 GMT
EXPOSE 8080
# Tue, 15 Nov 2022 03:06:49 GMT
CMD ["catalina.sh" "run"]
# Wed, 11 Jan 2023 02:47:03 GMT
LABEL org.opencontainers.image.authors=XWiki Development Team <committers@xwiki.org>
# Wed, 11 Jan 2023 02:47:03 GMT
LABEL org.opencontainers.image.url=https://hub.docker.com/_/xwiki
# Wed, 11 Jan 2023 02:47:03 GMT
LABEL org.opencontainers.image.documentation=https://hub.docker.com/_/xwiki
# Wed, 11 Jan 2023 02:47:03 GMT
LABEL org.opencontainers.image.source=https://github.com/xwiki/xwiki-docker.git
# Wed, 11 Jan 2023 02:47:04 GMT
LABEL org.opencontainers.image.vendor=xwiki.org
# Wed, 11 Jan 2023 02:47:04 GMT
LABEL org.opencontainers.image.licenses=LGPL-2.1
# Wed, 11 Jan 2023 02:49:03 GMT
RUN apt-get update &&   apt-get --no-install-recommends -y install     curl     libreoffice     unzip     procps &&   rm -rf /var/lib/apt/lists/*
# Wed, 22 Feb 2023 18:39:36 GMT
ENV XWIKI_VERSION=14.10.5
# Wed, 22 Feb 2023 18:39:36 GMT
ENV XWIKI_URL_PREFIX=https://maven.xwiki.org/releases/org/xwiki/platform/xwiki-platform-distribution-war/14.10.5
# Wed, 22 Feb 2023 18:39:36 GMT
ENV XWIKI_DOWNLOAD_SHA256=f58465d0869e4c5605ae8375a09c79399d1149c7131fed3cf9959918267eb6a8
# Wed, 22 Feb 2023 18:40:15 GMT
RUN rm -rf /usr/local/tomcat/webapps/* &&   mkdir -p /usr/local/tomcat/temp &&   mkdir -p /usr/local/xwiki/data &&   curl -fSL "${XWIKI_URL_PREFIX}/xwiki-platform-distribution-war-${XWIKI_VERSION}.war" -o xwiki.war &&   echo "$XWIKI_DOWNLOAD_SHA256 xwiki.war" | sha256sum -c - &&   unzip -d /usr/local/tomcat/webapps/ROOT xwiki.war &&   rm -f xwiki.war
# Wed, 22 Feb 2023 18:41:14 GMT
ENV MARIADB_JDBC_VERSION=3.1.2
# Wed, 22 Feb 2023 18:41:14 GMT
ENV MARIADB_JDBC_SHA256=aaec1ad348d030a65b25c93c65cdaf472bf8b4b6b314b965e5ba13aec81bc622
# Wed, 22 Feb 2023 18:41:14 GMT
ENV MARIADB_JDBC_PREFIX=https://repo1.maven.org/maven2/org/mariadb/jdbc/mariadb-java-client/3.1.2
# Wed, 22 Feb 2023 18:41:14 GMT
ENV MARIADB_JDBC_ARTIFACT=mariadb-java-client-3.1.2.jar
# Wed, 22 Feb 2023 18:41:14 GMT
ENV MARIADB_JDBC_TARGET=/usr/local/tomcat/webapps/ROOT/WEB-INF/lib/mariadb-java-client-3.1.2.jar
# Wed, 22 Feb 2023 18:41:15 GMT
RUN curl -fSL "${MARIADB_JDBC_PREFIX}/${MARIADB_JDBC_ARTIFACT}" -o $MARIADB_JDBC_TARGET &&   echo "$MARIADB_JDBC_SHA256 $MARIADB_JDBC_TARGET" | sha256sum -c -
# Wed, 22 Feb 2023 18:41:15 GMT
COPY file:0a1be11e2eb610a1dbcd415404e3a592641110b93090030cb831e3a19a163017 in /usr/local/tomcat/bin/ 
# Wed, 22 Feb 2023 18:41:15 GMT
COPY file:0e237c3876eeb3b5f3473a064d3e507da2df6c228ca714687930b34e3b687601 in /usr/local/tomcat/webapps/ROOT/WEB-INF/hibernate.cfg.xml 
# Wed, 22 Feb 2023 18:41:15 GMT
RUN sed -i 's/<id>org.xwiki.platform:xwiki-platform-distribution-war/<id>org.xwiki.platform:xwiki-platform-distribution-docker/'   /usr/local/tomcat/webapps/ROOT/META-INF/extension.xed
# Wed, 22 Feb 2023 18:41:16 GMT
COPY file:a47c4dcd87c9dad97aff38c49188357e6193bcad50757e516cfb08a60d4de611 in /usr/local/bin/docker-entrypoint.sh 
# Wed, 22 Feb 2023 18:41:16 GMT
VOLUME [/usr/local/xwiki]
# Wed, 22 Feb 2023 18:41:16 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 22 Feb 2023 18:41:16 GMT
CMD ["xwiki"]
```

-	Layers:
	-	`sha256:e96e057aae67380a4ddb16c337c5c3669d97fdff69ec537f02aa2cc30d814281`  
		Last Modified: Wed, 02 Nov 2022 03:03:36 GMT  
		Size: 30.4 MB (30425607 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4ced2591451da3a02e2b6bb44752b9e3f00d77789921be4df5082fb9f9880ad0`  
		Last Modified: Wed, 02 Nov 2022 18:48:43 GMT  
		Size: 12.4 MB (12439006 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:df8f874ae8c08a9e69e5fbe6c5a64200a45386132a3203d1a9a7f1146d94cfbc`  
		Last Modified: Fri, 04 Nov 2022 23:29:33 GMT  
		Size: 46.6 MB (46629936 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:111b6c7486426c4b6989102c2ee5be856e8a58e20ab0a350b24a905d536e8e7f`  
		Last Modified: Fri, 04 Nov 2022 23:29:26 GMT  
		Size: 161.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e6f84dce457c6d4f7b7291fce05f8e77998a3a7722a54125a1f1d52ca83043b4`  
		Last Modified: Sat, 05 Nov 2022 01:50:51 GMT  
		Size: 173.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a6c26749ee782392e38845ee2ba79b0da586ef6a45d8e7f29c7af14612278547`  
		Last Modified: Tue, 15 Nov 2022 03:19:57 GMT  
		Size: 12.2 MB (12200249 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4dddc6d9fa6024025b3fcfe729cab2dc544fb25476eca6e80b1af8e8d93bb0ee`  
		Last Modified: Tue, 15 Nov 2022 03:19:56 GMT  
		Size: 452.7 KB (452680 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:06637eebe5e72c8ad9019ad4eb4cdde1f11f7d4c24c7ed7374cf8966343aa2fb`  
		Last Modified: Tue, 15 Nov 2022 03:19:56 GMT  
		Size: 131.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b276fb8390410a8208724033e325715ea26000d5a1a762d4c3699b927884fbfe`  
		Last Modified: Wed, 11 Jan 2023 02:52:45 GMT  
		Size: 178.8 MB (178805608 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:89de9d9e2c09cd5b84430562516cbcd5695a0a3b2347b451e157bde75c2b5619`  
		Last Modified: Wed, 22 Feb 2023 18:42:21 GMT  
		Size: 307.1 MB (307141303 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c34f6e86e4b4ce021fdc5c26a390f8682b638ef5b002596f5d85721a5b4f8b78`  
		Last Modified: Wed, 22 Feb 2023 18:43:25 GMT  
		Size: 589.9 KB (589888 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7c59af828719a4990baaba43861a4b7dfcf7c9301bc8c1c17b1977363ae47d8f`  
		Last Modified: Wed, 22 Feb 2023 18:43:25 GMT  
		Size: 1.3 KB (1345 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a1ce8abe653003fb1cf66551dd2e3daf88c2ec88e42e874179577314bcb129d7`  
		Last Modified: Wed, 22 Feb 2023 18:43:25 GMT  
		Size: 2.3 KB (2312 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:68e8b10875b16f8254c97d2580791e4ed6c27787f670ac843c0508addb3b38b3`  
		Last Modified: Wed, 22 Feb 2023 18:43:25 GMT  
		Size: 6.0 KB (6013 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ed46c896037147ae7b8029b5b7e890b7930132f0eec078e1211ccb92ff45c89e`  
		Last Modified: Wed, 22 Feb 2023 18:43:25 GMT  
		Size: 2.5 KB (2504 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `xwiki:14.10.5-mysql-tomcat`

```console
$ docker pull xwiki@sha256:301390c7e6252467e1773acbf7ca050b66a47a1277f29e6e40bf5bd98202eb00
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `xwiki:14.10.5-mysql-tomcat` - linux; amd64

```console
$ docker pull xwiki@sha256:a2e996a399fc68cbccfe11eaeb0115a15314bd69f06c483fef3cba244fa07cbf
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **590.4 MB (590449604 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:6b73fd725d5c1dd8044289fdb0e76f973e7e1d4a64e1efc44428235a718b550a`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["xwiki"]`

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
# Wed, 02 Nov 2022 18:44:10 GMT
RUN apt-get update     && DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends tzdata curl wget ca-certificates fontconfig locales     && echo "en_US.UTF-8 UTF-8" >> /etc/locale.gen     && locale-gen en_US.UTF-8     && rm -rf /var/lib/apt/lists/*
# Fri, 04 Nov 2022 23:21:41 GMT
ENV JAVA_VERSION=jdk-11.0.17+8
# Fri, 04 Nov 2022 23:22:31 GMT
RUN set -eux;     ARCH="$(dpkg --print-architecture)";     case "${ARCH}" in        aarch64|arm64)          ESUM='bd6efe3290c8b5a42f695a55a26f3e3c9c284288574879d4b7089f31f5114177';          BINARY_URL='https://github.com/adoptium/temurin11-binaries/releases/download/jdk-11.0.17%2B8/OpenJDK11U-jre_aarch64_linux_hotspot_11.0.17_8.tar.gz';          ;;        armhf|arm)          ESUM='8cf113d3d7fa808895c8d2e41bb890af21c47e38c2460e0588147a4bb8fc658d';          BINARY_URL='https://github.com/adoptium/temurin11-binaries/releases/download/jdk-11.0.17%2B8/OpenJDK11U-jre_arm_linux_hotspot_11.0.17_8.tar.gz';          ;;        ppc64el|powerpc:common64)          ESUM='0ca3d806131ab5834c501f9c625bb0248cd528af361c704503348e9c9605bedf';          BINARY_URL='https://github.com/adoptium/temurin11-binaries/releases/download/jdk-11.0.17%2B8/OpenJDK11U-jre_ppc64le_linux_hotspot_11.0.17_8.tar.gz';          ;;        s390x|s390:64-bit)          ESUM='dd3b159a374086e65cb07c4ccb226c90f9c02ef929cba6f0b642171d7ed97fa4';          BINARY_URL='https://github.com/adoptium/temurin11-binaries/releases/download/jdk-11.0.17%2B8/OpenJDK11U-jre_s390x_linux_hotspot_11.0.17_8.tar.gz';          ;;        amd64|i386:x86-64)          ESUM='752616097e09d7f60a3ad8bd312f90eaf50ac72577e55df229fe6e8091148f79';          BINARY_URL='https://github.com/adoptium/temurin11-binaries/releases/download/jdk-11.0.17%2B8/OpenJDK11U-jre_x64_linux_hotspot_11.0.17_8.tar.gz';          ;;        *)          echo "Unsupported arch: ${ARCH}";          exit 1;          ;;     esac; 	  wget -O /tmp/openjdk.tar.gz ${BINARY_URL}; 	  echo "${ESUM} */tmp/openjdk.tar.gz" | sha256sum -c -; 	  mkdir -p "$JAVA_HOME"; 	  tar --extract 	      --file /tmp/openjdk.tar.gz 	      --directory "$JAVA_HOME" 	      --strip-components 1 	      --no-same-owner 	  ;     rm /tmp/openjdk.tar.gz;     find "$JAVA_HOME/lib" -name '*.so' -exec dirname '{}' ';' | sort -u > /etc/ld.so.conf.d/docker-openjdk.conf;     ldconfig;     java -Xshare:dump;
# Fri, 04 Nov 2022 23:22:32 GMT
RUN echo Verifying install ...     && fileEncoding="$(echo 'System.out.println(System.getProperty("file.encoding"))' | jshell -s -)"; [ "$fileEncoding" = 'UTF-8' ]; rm -rf ~/.java     && echo java --version && java --version     && echo Complete.
# Sat, 05 Nov 2022 01:35:16 GMT
ENV CATALINA_HOME=/usr/local/tomcat
# Sat, 05 Nov 2022 01:35:16 GMT
ENV PATH=/usr/local/tomcat/bin:/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Sat, 05 Nov 2022 01:35:17 GMT
RUN mkdir -p "$CATALINA_HOME"
# Sat, 05 Nov 2022 01:35:17 GMT
WORKDIR /usr/local/tomcat
# Sat, 05 Nov 2022 01:35:17 GMT
ENV TOMCAT_NATIVE_LIBDIR=/usr/local/tomcat/native-jni-lib
# Sat, 05 Nov 2022 01:35:17 GMT
ENV LD_LIBRARY_PATH=/usr/local/tomcat/native-jni-lib
# Sat, 05 Nov 2022 01:39:54 GMT
ENV GPG_KEYS=48F8E69F6390C9F25CFEDCD268248959359E722B A9C5DF4D22E99998D9875A5110C01C5A2F6059E7 DCFD35E0BF8CA7344752DE8B6FB21E8933C60243
# Sat, 05 Nov 2022 01:39:54 GMT
ENV TOMCAT_MAJOR=9
# Tue, 15 Nov 2022 03:06:43 GMT
ENV TOMCAT_VERSION=9.0.69
# Tue, 15 Nov 2022 03:06:43 GMT
ENV TOMCAT_SHA512=8c883c54ce9ce43eba37756a6404cdf3477879883a3e6d146dc8a7aa5e0425f487466afe6b6da4a895927cb7cb59177b9379cec18000f2de12785be57408c779
# Tue, 15 Nov 2022 03:06:44 GMT
COPY dir:b1a33aa3993dbbfbebb33bd9aa546b60c2f2191abf1227f453d4e830f6deb35f in /usr/local/tomcat 
# Tue, 15 Nov 2022 03:06:48 GMT
RUN set -eux; 	apt-get update; 	xargs -rt apt-get install -y --no-install-recommends < "$TOMCAT_NATIVE_LIBDIR/.dependencies.txt"; 	rm -rf /var/lib/apt/lists/*
# Tue, 15 Nov 2022 03:06:49 GMT
RUN set -eux; 	nativeLines="$(catalina.sh configtest 2>&1)"; 	nativeLines="$(echo "$nativeLines" | grep 'Apache Tomcat Native')"; 	nativeLines="$(echo "$nativeLines" | sort -u)"; 	if ! echo "$nativeLines" | grep -E 'INFO: Loaded( APR based)? Apache Tomcat Native library' >&2; then 		echo >&2 "$nativeLines"; 		exit 1; 	fi
# Tue, 15 Nov 2022 03:06:49 GMT
EXPOSE 8080
# Tue, 15 Nov 2022 03:06:49 GMT
CMD ["catalina.sh" "run"]
# Wed, 11 Jan 2023 02:47:03 GMT
LABEL org.opencontainers.image.authors=XWiki Development Team <committers@xwiki.org>
# Wed, 11 Jan 2023 02:47:03 GMT
LABEL org.opencontainers.image.url=https://hub.docker.com/_/xwiki
# Wed, 11 Jan 2023 02:47:03 GMT
LABEL org.opencontainers.image.documentation=https://hub.docker.com/_/xwiki
# Wed, 11 Jan 2023 02:47:03 GMT
LABEL org.opencontainers.image.source=https://github.com/xwiki/xwiki-docker.git
# Wed, 11 Jan 2023 02:47:04 GMT
LABEL org.opencontainers.image.vendor=xwiki.org
# Wed, 11 Jan 2023 02:47:04 GMT
LABEL org.opencontainers.image.licenses=LGPL-2.1
# Wed, 11 Jan 2023 02:49:03 GMT
RUN apt-get update &&   apt-get --no-install-recommends -y install     curl     libreoffice     unzip     procps &&   rm -rf /var/lib/apt/lists/*
# Wed, 22 Feb 2023 18:39:36 GMT
ENV XWIKI_VERSION=14.10.5
# Wed, 22 Feb 2023 18:39:36 GMT
ENV XWIKI_URL_PREFIX=https://maven.xwiki.org/releases/org/xwiki/platform/xwiki-platform-distribution-war/14.10.5
# Wed, 22 Feb 2023 18:39:36 GMT
ENV XWIKI_DOWNLOAD_SHA256=f58465d0869e4c5605ae8375a09c79399d1149c7131fed3cf9959918267eb6a8
# Wed, 22 Feb 2023 18:40:15 GMT
RUN rm -rf /usr/local/tomcat/webapps/* &&   mkdir -p /usr/local/tomcat/temp &&   mkdir -p /usr/local/xwiki/data &&   curl -fSL "${XWIKI_URL_PREFIX}/xwiki-platform-distribution-war-${XWIKI_VERSION}.war" -o xwiki.war &&   echo "$XWIKI_DOWNLOAD_SHA256 xwiki.war" | sha256sum -c - &&   unzip -d /usr/local/tomcat/webapps/ROOT xwiki.war &&   rm -f xwiki.war
# Wed, 22 Feb 2023 18:40:17 GMT
ENV MYSQL_JDBC_VERSION=8.0.32
# Wed, 22 Feb 2023 18:40:17 GMT
ENV MYSQL_JDBC_SHA256=522329fe925980f02e5eb89b59d227245d345415ff0c08932a68c9765c13acc5
# Wed, 22 Feb 2023 18:40:17 GMT
ENV MYSQL_JDBC_PREFIX=https://repo1.maven.org/maven2/com/mysql/mysql-connector-j/8.0.32
# Wed, 22 Feb 2023 18:40:17 GMT
ENV MYSQL_JDBC_ARTIFACT=mysql-connector-j-8.0.32.jar
# Wed, 22 Feb 2023 18:40:17 GMT
ENV MYSQL_JDBC_TARGET=/usr/local/tomcat/webapps/ROOT/WEB-INF/lib/mysql-connector-j-8.0.32.jar
# Wed, 22 Feb 2023 18:40:18 GMT
RUN curl -fSL "${MYSQL_JDBC_PREFIX}/${MYSQL_JDBC_ARTIFACT}" -o $MYSQL_JDBC_TARGET &&   echo "$MYSQL_JDBC_SHA256 $MYSQL_JDBC_TARGET" | sha256sum -c -
# Wed, 22 Feb 2023 18:40:18 GMT
COPY file:0a1be11e2eb610a1dbcd415404e3a592641110b93090030cb831e3a19a163017 in /usr/local/tomcat/bin/ 
# Wed, 22 Feb 2023 18:40:18 GMT
COPY file:1b8409986f3e4eb79a7a0b18472cb2692a61d504fb5ef34292bc997b79fd760d in /usr/local/tomcat/webapps/ROOT/WEB-INF/hibernate.cfg.xml 
# Wed, 22 Feb 2023 18:40:19 GMT
RUN sed -i 's/<id>org.xwiki.platform:xwiki-platform-distribution-war/<id>org.xwiki.platform:xwiki-platform-distribution-docker/'   /usr/local/tomcat/webapps/ROOT/META-INF/extension.xed
# Wed, 22 Feb 2023 18:40:19 GMT
COPY file:a47c4dcd87c9dad97aff38c49188357e6193bcad50757e516cfb08a60d4de611 in /usr/local/bin/docker-entrypoint.sh 
# Wed, 22 Feb 2023 18:40:19 GMT
VOLUME [/usr/local/xwiki]
# Wed, 22 Feb 2023 18:40:19 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 22 Feb 2023 18:40:19 GMT
CMD ["xwiki"]
```

-	Layers:
	-	`sha256:e96e057aae67380a4ddb16c337c5c3669d97fdff69ec537f02aa2cc30d814281`  
		Last Modified: Wed, 02 Nov 2022 03:03:36 GMT  
		Size: 30.4 MB (30425607 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4ced2591451da3a02e2b6bb44752b9e3f00d77789921be4df5082fb9f9880ad0`  
		Last Modified: Wed, 02 Nov 2022 18:48:43 GMT  
		Size: 12.4 MB (12439006 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:df8f874ae8c08a9e69e5fbe6c5a64200a45386132a3203d1a9a7f1146d94cfbc`  
		Last Modified: Fri, 04 Nov 2022 23:29:33 GMT  
		Size: 46.6 MB (46629936 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:111b6c7486426c4b6989102c2ee5be856e8a58e20ab0a350b24a905d536e8e7f`  
		Last Modified: Fri, 04 Nov 2022 23:29:26 GMT  
		Size: 161.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e6f84dce457c6d4f7b7291fce05f8e77998a3a7722a54125a1f1d52ca83043b4`  
		Last Modified: Sat, 05 Nov 2022 01:50:51 GMT  
		Size: 173.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a6c26749ee782392e38845ee2ba79b0da586ef6a45d8e7f29c7af14612278547`  
		Last Modified: Tue, 15 Nov 2022 03:19:57 GMT  
		Size: 12.2 MB (12200249 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4dddc6d9fa6024025b3fcfe729cab2dc544fb25476eca6e80b1af8e8d93bb0ee`  
		Last Modified: Tue, 15 Nov 2022 03:19:56 GMT  
		Size: 452.7 KB (452680 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:06637eebe5e72c8ad9019ad4eb4cdde1f11f7d4c24c7ed7374cf8966343aa2fb`  
		Last Modified: Tue, 15 Nov 2022 03:19:56 GMT  
		Size: 131.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b276fb8390410a8208724033e325715ea26000d5a1a762d4c3699b927884fbfe`  
		Last Modified: Wed, 11 Jan 2023 02:52:45 GMT  
		Size: 178.8 MB (178805608 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:89de9d9e2c09cd5b84430562516cbcd5695a0a3b2347b451e157bde75c2b5619`  
		Last Modified: Wed, 22 Feb 2023 18:42:21 GMT  
		Size: 307.1 MB (307141303 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4a2089179b7c1db514d0502e476e09b8f9313d08d4c4e4f3981be456288fe507`  
		Last Modified: Wed, 22 Feb 2023 18:42:04 GMT  
		Size: 2.3 MB (2342572 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e7c4ef360ff3673244adb3dfc4769b5710fa68fcc1fbe1c08b2f5fa32dbd4976`  
		Last Modified: Wed, 22 Feb 2023 18:42:04 GMT  
		Size: 1.3 KB (1348 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:08441c368d4b01e361491d7fbf1ac579fcc303b8484123c309a8d5a3b6657c46`  
		Last Modified: Wed, 22 Feb 2023 18:42:04 GMT  
		Size: 2.3 KB (2311 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:542b4bb846d438395e458c08de292f72d14d289fae6ffe7eba6fec1cd8518475`  
		Last Modified: Wed, 22 Feb 2023 18:42:04 GMT  
		Size: 6.0 KB (6013 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:039c0305df9e64c69bb546e64f0658dba6e728eee13022cfd682aa1ee76b8b7f`  
		Last Modified: Wed, 22 Feb 2023 18:42:04 GMT  
		Size: 2.5 KB (2506 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `xwiki:14.10.5-postgres-tomcat`

```console
$ docker pull xwiki@sha256:2421e9bd66d2821f6e160a204790ede74e7ac216ecb85ab8899292fd67dfe624
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `xwiki:14.10.5-postgres-tomcat` - linux; amd64

```console
$ docker pull xwiki@sha256:5cd23e4200b4eed664a61d05e3d436d0e372a3e4e985e29cb866dd9dbb573713
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **590.0 MB (589983532 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ab0dc70572c5101e5837a6281e7cb29a2b4dbf26ad0b9c91860a748aeb3360e1`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["xwiki"]`

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
# Wed, 02 Nov 2022 18:44:10 GMT
RUN apt-get update     && DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends tzdata curl wget ca-certificates fontconfig locales     && echo "en_US.UTF-8 UTF-8" >> /etc/locale.gen     && locale-gen en_US.UTF-8     && rm -rf /var/lib/apt/lists/*
# Fri, 04 Nov 2022 23:21:41 GMT
ENV JAVA_VERSION=jdk-11.0.17+8
# Fri, 04 Nov 2022 23:22:31 GMT
RUN set -eux;     ARCH="$(dpkg --print-architecture)";     case "${ARCH}" in        aarch64|arm64)          ESUM='bd6efe3290c8b5a42f695a55a26f3e3c9c284288574879d4b7089f31f5114177';          BINARY_URL='https://github.com/adoptium/temurin11-binaries/releases/download/jdk-11.0.17%2B8/OpenJDK11U-jre_aarch64_linux_hotspot_11.0.17_8.tar.gz';          ;;        armhf|arm)          ESUM='8cf113d3d7fa808895c8d2e41bb890af21c47e38c2460e0588147a4bb8fc658d';          BINARY_URL='https://github.com/adoptium/temurin11-binaries/releases/download/jdk-11.0.17%2B8/OpenJDK11U-jre_arm_linux_hotspot_11.0.17_8.tar.gz';          ;;        ppc64el|powerpc:common64)          ESUM='0ca3d806131ab5834c501f9c625bb0248cd528af361c704503348e9c9605bedf';          BINARY_URL='https://github.com/adoptium/temurin11-binaries/releases/download/jdk-11.0.17%2B8/OpenJDK11U-jre_ppc64le_linux_hotspot_11.0.17_8.tar.gz';          ;;        s390x|s390:64-bit)          ESUM='dd3b159a374086e65cb07c4ccb226c90f9c02ef929cba6f0b642171d7ed97fa4';          BINARY_URL='https://github.com/adoptium/temurin11-binaries/releases/download/jdk-11.0.17%2B8/OpenJDK11U-jre_s390x_linux_hotspot_11.0.17_8.tar.gz';          ;;        amd64|i386:x86-64)          ESUM='752616097e09d7f60a3ad8bd312f90eaf50ac72577e55df229fe6e8091148f79';          BINARY_URL='https://github.com/adoptium/temurin11-binaries/releases/download/jdk-11.0.17%2B8/OpenJDK11U-jre_x64_linux_hotspot_11.0.17_8.tar.gz';          ;;        *)          echo "Unsupported arch: ${ARCH}";          exit 1;          ;;     esac; 	  wget -O /tmp/openjdk.tar.gz ${BINARY_URL}; 	  echo "${ESUM} */tmp/openjdk.tar.gz" | sha256sum -c -; 	  mkdir -p "$JAVA_HOME"; 	  tar --extract 	      --file /tmp/openjdk.tar.gz 	      --directory "$JAVA_HOME" 	      --strip-components 1 	      --no-same-owner 	  ;     rm /tmp/openjdk.tar.gz;     find "$JAVA_HOME/lib" -name '*.so' -exec dirname '{}' ';' | sort -u > /etc/ld.so.conf.d/docker-openjdk.conf;     ldconfig;     java -Xshare:dump;
# Fri, 04 Nov 2022 23:22:32 GMT
RUN echo Verifying install ...     && fileEncoding="$(echo 'System.out.println(System.getProperty("file.encoding"))' | jshell -s -)"; [ "$fileEncoding" = 'UTF-8' ]; rm -rf ~/.java     && echo java --version && java --version     && echo Complete.
# Sat, 05 Nov 2022 01:35:16 GMT
ENV CATALINA_HOME=/usr/local/tomcat
# Sat, 05 Nov 2022 01:35:16 GMT
ENV PATH=/usr/local/tomcat/bin:/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Sat, 05 Nov 2022 01:35:17 GMT
RUN mkdir -p "$CATALINA_HOME"
# Sat, 05 Nov 2022 01:35:17 GMT
WORKDIR /usr/local/tomcat
# Sat, 05 Nov 2022 01:35:17 GMT
ENV TOMCAT_NATIVE_LIBDIR=/usr/local/tomcat/native-jni-lib
# Sat, 05 Nov 2022 01:35:17 GMT
ENV LD_LIBRARY_PATH=/usr/local/tomcat/native-jni-lib
# Sat, 05 Nov 2022 01:39:54 GMT
ENV GPG_KEYS=48F8E69F6390C9F25CFEDCD268248959359E722B A9C5DF4D22E99998D9875A5110C01C5A2F6059E7 DCFD35E0BF8CA7344752DE8B6FB21E8933C60243
# Sat, 05 Nov 2022 01:39:54 GMT
ENV TOMCAT_MAJOR=9
# Tue, 15 Nov 2022 03:06:43 GMT
ENV TOMCAT_VERSION=9.0.69
# Tue, 15 Nov 2022 03:06:43 GMT
ENV TOMCAT_SHA512=8c883c54ce9ce43eba37756a6404cdf3477879883a3e6d146dc8a7aa5e0425f487466afe6b6da4a895927cb7cb59177b9379cec18000f2de12785be57408c779
# Tue, 15 Nov 2022 03:06:44 GMT
COPY dir:b1a33aa3993dbbfbebb33bd9aa546b60c2f2191abf1227f453d4e830f6deb35f in /usr/local/tomcat 
# Tue, 15 Nov 2022 03:06:48 GMT
RUN set -eux; 	apt-get update; 	xargs -rt apt-get install -y --no-install-recommends < "$TOMCAT_NATIVE_LIBDIR/.dependencies.txt"; 	rm -rf /var/lib/apt/lists/*
# Tue, 15 Nov 2022 03:06:49 GMT
RUN set -eux; 	nativeLines="$(catalina.sh configtest 2>&1)"; 	nativeLines="$(echo "$nativeLines" | grep 'Apache Tomcat Native')"; 	nativeLines="$(echo "$nativeLines" | sort -u)"; 	if ! echo "$nativeLines" | grep -E 'INFO: Loaded( APR based)? Apache Tomcat Native library' >&2; then 		echo >&2 "$nativeLines"; 		exit 1; 	fi
# Tue, 15 Nov 2022 03:06:49 GMT
EXPOSE 8080
# Tue, 15 Nov 2022 03:06:49 GMT
CMD ["catalina.sh" "run"]
# Wed, 11 Jan 2023 02:47:03 GMT
LABEL org.opencontainers.image.authors=XWiki Development Team <committers@xwiki.org>
# Wed, 11 Jan 2023 02:47:03 GMT
LABEL org.opencontainers.image.url=https://hub.docker.com/_/xwiki
# Wed, 11 Jan 2023 02:47:03 GMT
LABEL org.opencontainers.image.documentation=https://hub.docker.com/_/xwiki
# Wed, 11 Jan 2023 02:47:03 GMT
LABEL org.opencontainers.image.source=https://github.com/xwiki/xwiki-docker.git
# Wed, 11 Jan 2023 02:47:04 GMT
LABEL org.opencontainers.image.vendor=xwiki.org
# Wed, 11 Jan 2023 02:47:04 GMT
LABEL org.opencontainers.image.licenses=LGPL-2.1
# Wed, 11 Jan 2023 02:50:25 GMT
RUN apt-get update &&   apt-get --no-install-recommends -y install     curl     libreoffice     unzip     procps     libpostgresql-jdbc-java &&   rm -rf /var/lib/apt/lists/*
# Wed, 22 Feb 2023 18:40:25 GMT
ENV XWIKI_VERSION=14.10.5
# Wed, 22 Feb 2023 18:40:25 GMT
ENV XWIKI_URL_PREFIX=https://maven.xwiki.org/releases/org/xwiki/platform/xwiki-platform-distribution-war/14.10.5
# Wed, 22 Feb 2023 18:40:25 GMT
ENV XWIKI_DOWNLOAD_SHA256=f58465d0869e4c5605ae8375a09c79399d1149c7131fed3cf9959918267eb6a8
# Wed, 22 Feb 2023 18:41:04 GMT
RUN rm -rf /usr/local/tomcat/webapps/* &&   mkdir -p /usr/local/tomcat/temp &&   mkdir -p /usr/local/xwiki/data &&   curl -fSL "${XWIKI_URL_PREFIX}/xwiki-platform-distribution-war-${XWIKI_VERSION}.war" -o xwiki.war &&   echo "$XWIKI_DOWNLOAD_SHA256 xwiki.war" | sha256sum -c - &&   unzip -d /usr/local/tomcat/webapps/ROOT xwiki.war &&   rm -f xwiki.war
# Wed, 22 Feb 2023 18:41:05 GMT
RUN cp /usr/share/java/postgresql-jdbc4.jar /usr/local/tomcat/webapps/ROOT/WEB-INF/lib/
# Wed, 22 Feb 2023 18:41:05 GMT
COPY file:0a1be11e2eb610a1dbcd415404e3a592641110b93090030cb831e3a19a163017 in /usr/local/tomcat/bin/ 
# Wed, 22 Feb 2023 18:41:05 GMT
COPY file:4a923f484bb29a26630c19e1d617d3bf6aa6ae7c6c4a5561e97b037bcde0847c in /usr/local/tomcat/webapps/ROOT/WEB-INF/hibernate.cfg.xml 
# Wed, 22 Feb 2023 18:41:06 GMT
RUN sed -i 's/<id>org.xwiki.platform:xwiki-platform-distribution-war/<id>org.xwiki.platform:xwiki-platform-distribution-docker/'   /usr/local/tomcat/webapps/ROOT/META-INF/extension.xed
# Wed, 22 Feb 2023 18:41:06 GMT
COPY file:a47c4dcd87c9dad97aff38c49188357e6193bcad50757e516cfb08a60d4de611 in /usr/local/bin/docker-entrypoint.sh 
# Wed, 22 Feb 2023 18:41:06 GMT
VOLUME [/usr/local/xwiki]
# Wed, 22 Feb 2023 18:41:06 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 22 Feb 2023 18:41:06 GMT
CMD ["xwiki"]
```

-	Layers:
	-	`sha256:e96e057aae67380a4ddb16c337c5c3669d97fdff69ec537f02aa2cc30d814281`  
		Last Modified: Wed, 02 Nov 2022 03:03:36 GMT  
		Size: 30.4 MB (30425607 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4ced2591451da3a02e2b6bb44752b9e3f00d77789921be4df5082fb9f9880ad0`  
		Last Modified: Wed, 02 Nov 2022 18:48:43 GMT  
		Size: 12.4 MB (12439006 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:df8f874ae8c08a9e69e5fbe6c5a64200a45386132a3203d1a9a7f1146d94cfbc`  
		Last Modified: Fri, 04 Nov 2022 23:29:33 GMT  
		Size: 46.6 MB (46629936 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:111b6c7486426c4b6989102c2ee5be856e8a58e20ab0a350b24a905d536e8e7f`  
		Last Modified: Fri, 04 Nov 2022 23:29:26 GMT  
		Size: 161.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e6f84dce457c6d4f7b7291fce05f8e77998a3a7722a54125a1f1d52ca83043b4`  
		Last Modified: Sat, 05 Nov 2022 01:50:51 GMT  
		Size: 173.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a6c26749ee782392e38845ee2ba79b0da586ef6a45d8e7f29c7af14612278547`  
		Last Modified: Tue, 15 Nov 2022 03:19:57 GMT  
		Size: 12.2 MB (12200249 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4dddc6d9fa6024025b3fcfe729cab2dc544fb25476eca6e80b1af8e8d93bb0ee`  
		Last Modified: Tue, 15 Nov 2022 03:19:56 GMT  
		Size: 452.7 KB (452680 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:06637eebe5e72c8ad9019ad4eb4cdde1f11f7d4c24c7ed7374cf8966343aa2fb`  
		Last Modified: Tue, 15 Nov 2022 03:19:56 GMT  
		Size: 131.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b57f6f8bcfb0d93b8e21d3068d1f65d3f08dba05c5fab7d4c36e2359317b18c7`  
		Last Modified: Wed, 11 Jan 2023 02:53:53 GMT  
		Size: 179.7 MB (179745182 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b26b00a2f6717a934b9a1b08bac612aaaf57a4cfb4d82db521e7d36755621933`  
		Last Modified: Wed, 22 Feb 2023 18:43:06 GMT  
		Size: 307.1 MB (307141251 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:11801aa48fd913e3278b4d0a512df366a8ef26c1cc3e95a8439a1be90aadfd5a`  
		Last Modified: Wed, 22 Feb 2023 18:42:50 GMT  
		Size: 936.9 KB (936850 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fb4e8755162307a316ff405759f2417dc77e746651f89c83a0477ab19dc7da5d`  
		Last Modified: Wed, 22 Feb 2023 18:42:50 GMT  
		Size: 1.3 KB (1342 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2ba124a3d49367a8e2f46fc2043189f91e2dd282d40a301d9c1f79a705d35e66`  
		Last Modified: Wed, 22 Feb 2023 18:42:50 GMT  
		Size: 2.5 KB (2450 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8f421201132c3966dbb37a473df5922718780304fa03993ef75bb78522d5cafd`  
		Last Modified: Wed, 22 Feb 2023 18:42:50 GMT  
		Size: 6.0 KB (6012 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1b5dc6b32b3d1d9a80058f5ffc684363a0cfadf60ade5875fa37854ec7b46fff`  
		Last Modified: Wed, 22 Feb 2023 18:42:50 GMT  
		Size: 2.5 KB (2502 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `xwiki:15`

```console
$ docker pull xwiki@sha256:33e789838f82ce73efec6664859feb1ced7a5b7605fbfaddb81916716bce524f
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `xwiki:15` - linux; amd64

```console
$ docker pull xwiki@sha256:481fdb46e8c043a6709d11310e2083ce71d6ba63ee6517f84da3ba06f320598e
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **590.5 MB (590459982 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:bd630aa0aa5c679e23ea7d52cbbdd6b817eab27a820c25d3c50b54eca83b9744`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["xwiki"]`

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
# Wed, 02 Nov 2022 18:44:10 GMT
RUN apt-get update     && DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends tzdata curl wget ca-certificates fontconfig locales     && echo "en_US.UTF-8 UTF-8" >> /etc/locale.gen     && locale-gen en_US.UTF-8     && rm -rf /var/lib/apt/lists/*
# Fri, 04 Nov 2022 23:21:41 GMT
ENV JAVA_VERSION=jdk-11.0.17+8
# Fri, 04 Nov 2022 23:22:31 GMT
RUN set -eux;     ARCH="$(dpkg --print-architecture)";     case "${ARCH}" in        aarch64|arm64)          ESUM='bd6efe3290c8b5a42f695a55a26f3e3c9c284288574879d4b7089f31f5114177';          BINARY_URL='https://github.com/adoptium/temurin11-binaries/releases/download/jdk-11.0.17%2B8/OpenJDK11U-jre_aarch64_linux_hotspot_11.0.17_8.tar.gz';          ;;        armhf|arm)          ESUM='8cf113d3d7fa808895c8d2e41bb890af21c47e38c2460e0588147a4bb8fc658d';          BINARY_URL='https://github.com/adoptium/temurin11-binaries/releases/download/jdk-11.0.17%2B8/OpenJDK11U-jre_arm_linux_hotspot_11.0.17_8.tar.gz';          ;;        ppc64el|powerpc:common64)          ESUM='0ca3d806131ab5834c501f9c625bb0248cd528af361c704503348e9c9605bedf';          BINARY_URL='https://github.com/adoptium/temurin11-binaries/releases/download/jdk-11.0.17%2B8/OpenJDK11U-jre_ppc64le_linux_hotspot_11.0.17_8.tar.gz';          ;;        s390x|s390:64-bit)          ESUM='dd3b159a374086e65cb07c4ccb226c90f9c02ef929cba6f0b642171d7ed97fa4';          BINARY_URL='https://github.com/adoptium/temurin11-binaries/releases/download/jdk-11.0.17%2B8/OpenJDK11U-jre_s390x_linux_hotspot_11.0.17_8.tar.gz';          ;;        amd64|i386:x86-64)          ESUM='752616097e09d7f60a3ad8bd312f90eaf50ac72577e55df229fe6e8091148f79';          BINARY_URL='https://github.com/adoptium/temurin11-binaries/releases/download/jdk-11.0.17%2B8/OpenJDK11U-jre_x64_linux_hotspot_11.0.17_8.tar.gz';          ;;        *)          echo "Unsupported arch: ${ARCH}";          exit 1;          ;;     esac; 	  wget -O /tmp/openjdk.tar.gz ${BINARY_URL}; 	  echo "${ESUM} */tmp/openjdk.tar.gz" | sha256sum -c -; 	  mkdir -p "$JAVA_HOME"; 	  tar --extract 	      --file /tmp/openjdk.tar.gz 	      --directory "$JAVA_HOME" 	      --strip-components 1 	      --no-same-owner 	  ;     rm /tmp/openjdk.tar.gz;     find "$JAVA_HOME/lib" -name '*.so' -exec dirname '{}' ';' | sort -u > /etc/ld.so.conf.d/docker-openjdk.conf;     ldconfig;     java -Xshare:dump;
# Fri, 04 Nov 2022 23:22:32 GMT
RUN echo Verifying install ...     && fileEncoding="$(echo 'System.out.println(System.getProperty("file.encoding"))' | jshell -s -)"; [ "$fileEncoding" = 'UTF-8' ]; rm -rf ~/.java     && echo java --version && java --version     && echo Complete.
# Sat, 05 Nov 2022 01:35:16 GMT
ENV CATALINA_HOME=/usr/local/tomcat
# Sat, 05 Nov 2022 01:35:16 GMT
ENV PATH=/usr/local/tomcat/bin:/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Sat, 05 Nov 2022 01:35:17 GMT
RUN mkdir -p "$CATALINA_HOME"
# Sat, 05 Nov 2022 01:35:17 GMT
WORKDIR /usr/local/tomcat
# Sat, 05 Nov 2022 01:35:17 GMT
ENV TOMCAT_NATIVE_LIBDIR=/usr/local/tomcat/native-jni-lib
# Sat, 05 Nov 2022 01:35:17 GMT
ENV LD_LIBRARY_PATH=/usr/local/tomcat/native-jni-lib
# Sat, 05 Nov 2022 01:39:54 GMT
ENV GPG_KEYS=48F8E69F6390C9F25CFEDCD268248959359E722B A9C5DF4D22E99998D9875A5110C01C5A2F6059E7 DCFD35E0BF8CA7344752DE8B6FB21E8933C60243
# Sat, 05 Nov 2022 01:39:54 GMT
ENV TOMCAT_MAJOR=9
# Tue, 15 Nov 2022 03:06:43 GMT
ENV TOMCAT_VERSION=9.0.69
# Tue, 15 Nov 2022 03:06:43 GMT
ENV TOMCAT_SHA512=8c883c54ce9ce43eba37756a6404cdf3477879883a3e6d146dc8a7aa5e0425f487466afe6b6da4a895927cb7cb59177b9379cec18000f2de12785be57408c779
# Tue, 15 Nov 2022 03:06:44 GMT
COPY dir:b1a33aa3993dbbfbebb33bd9aa546b60c2f2191abf1227f453d4e830f6deb35f in /usr/local/tomcat 
# Tue, 15 Nov 2022 03:06:48 GMT
RUN set -eux; 	apt-get update; 	xargs -rt apt-get install -y --no-install-recommends < "$TOMCAT_NATIVE_LIBDIR/.dependencies.txt"; 	rm -rf /var/lib/apt/lists/*
# Tue, 15 Nov 2022 03:06:49 GMT
RUN set -eux; 	nativeLines="$(catalina.sh configtest 2>&1)"; 	nativeLines="$(echo "$nativeLines" | grep 'Apache Tomcat Native')"; 	nativeLines="$(echo "$nativeLines" | sort -u)"; 	if ! echo "$nativeLines" | grep -E 'INFO: Loaded( APR based)? Apache Tomcat Native library' >&2; then 		echo >&2 "$nativeLines"; 		exit 1; 	fi
# Tue, 15 Nov 2022 03:06:49 GMT
EXPOSE 8080
# Tue, 15 Nov 2022 03:06:49 GMT
CMD ["catalina.sh" "run"]
# Wed, 11 Jan 2023 02:47:03 GMT
LABEL org.opencontainers.image.authors=XWiki Development Team <committers@xwiki.org>
# Wed, 11 Jan 2023 02:47:03 GMT
LABEL org.opencontainers.image.url=https://hub.docker.com/_/xwiki
# Wed, 11 Jan 2023 02:47:03 GMT
LABEL org.opencontainers.image.documentation=https://hub.docker.com/_/xwiki
# Wed, 11 Jan 2023 02:47:03 GMT
LABEL org.opencontainers.image.source=https://github.com/xwiki/xwiki-docker.git
# Wed, 11 Jan 2023 02:47:04 GMT
LABEL org.opencontainers.image.vendor=xwiki.org
# Wed, 11 Jan 2023 02:47:04 GMT
LABEL org.opencontainers.image.licenses=LGPL-2.1
# Wed, 11 Jan 2023 02:49:03 GMT
RUN apt-get update &&   apt-get --no-install-recommends -y install     curl     libreoffice     unzip     procps &&   rm -rf /var/lib/apt/lists/*
# Tue, 31 Jan 2023 00:20:17 GMT
ENV XWIKI_VERSION=15.0
# Tue, 31 Jan 2023 00:20:17 GMT
ENV XWIKI_URL_PREFIX=https://maven.xwiki.org/releases/org/xwiki/platform/xwiki-platform-distribution-war/15.0
# Tue, 31 Jan 2023 00:20:17 GMT
ENV XWIKI_DOWNLOAD_SHA256=79ba0f479bbc49521c113821adc9d91141075a9470d7f9bbb6994ca59c30d121
# Tue, 31 Jan 2023 00:21:18 GMT
RUN rm -rf /usr/local/tomcat/webapps/* &&   mkdir -p /usr/local/tomcat/temp &&   mkdir -p /usr/local/xwiki/data &&   curl -fSL "${XWIKI_URL_PREFIX}/xwiki-platform-distribution-war-${XWIKI_VERSION}.war" -o xwiki.war &&   echo "$XWIKI_DOWNLOAD_SHA256 xwiki.war" | sha256sum -c - &&   unzip -d /usr/local/tomcat/webapps/ROOT xwiki.war &&   rm -f xwiki.war
# Tue, 31 Jan 2023 00:21:19 GMT
ENV MYSQL_JDBC_VERSION=8.0.31
# Tue, 31 Jan 2023 00:21:19 GMT
ENV MYSQL_JDBC_SHA256=5249e3dc6d6531b37790e3f61845b96db5e41e891d3d8edb0e2e3a1b53ca2f4f
# Tue, 31 Jan 2023 00:21:19 GMT
ENV MYSQL_JDBC_PREFIX=https://repo1.maven.org/maven2/com/mysql/mysql-connector-j/8.0.31
# Tue, 31 Jan 2023 00:21:19 GMT
ENV MYSQL_JDBC_ARTIFACT=mysql-connector-j-8.0.31.jar
# Tue, 31 Jan 2023 00:21:19 GMT
ENV MYSQL_JDBC_TARGET=/usr/local/tomcat/webapps/ROOT/WEB-INF/lib/mysql-connector-j-8.0.31.jar
# Tue, 31 Jan 2023 00:21:20 GMT
RUN curl -fSL "${MYSQL_JDBC_PREFIX}/${MYSQL_JDBC_ARTIFACT}" -o $MYSQL_JDBC_TARGET &&   echo "$MYSQL_JDBC_SHA256 $MYSQL_JDBC_TARGET" | sha256sum -c -
# Tue, 31 Jan 2023 00:21:21 GMT
COPY file:0a1be11e2eb610a1dbcd415404e3a592641110b93090030cb831e3a19a163017 in /usr/local/tomcat/bin/ 
# Tue, 31 Jan 2023 00:21:21 GMT
COPY file:1b8409986f3e4eb79a7a0b18472cb2692a61d504fb5ef34292bc997b79fd760d in /usr/local/tomcat/webapps/ROOT/WEB-INF/hibernate.cfg.xml 
# Tue, 31 Jan 2023 00:21:21 GMT
RUN sed -i 's/<id>org.xwiki.platform:xwiki-platform-distribution-war/<id>org.xwiki.platform:xwiki-platform-distribution-docker/'   /usr/local/tomcat/webapps/ROOT/META-INF/extension.xed
# Tue, 31 Jan 2023 00:21:21 GMT
COPY file:a47c4dcd87c9dad97aff38c49188357e6193bcad50757e516cfb08a60d4de611 in /usr/local/bin/docker-entrypoint.sh 
# Tue, 31 Jan 2023 00:21:22 GMT
VOLUME [/usr/local/xwiki]
# Tue, 31 Jan 2023 00:21:22 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 31 Jan 2023 00:21:22 GMT
CMD ["xwiki"]
```

-	Layers:
	-	`sha256:e96e057aae67380a4ddb16c337c5c3669d97fdff69ec537f02aa2cc30d814281`  
		Last Modified: Wed, 02 Nov 2022 03:03:36 GMT  
		Size: 30.4 MB (30425607 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4ced2591451da3a02e2b6bb44752b9e3f00d77789921be4df5082fb9f9880ad0`  
		Last Modified: Wed, 02 Nov 2022 18:48:43 GMT  
		Size: 12.4 MB (12439006 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:df8f874ae8c08a9e69e5fbe6c5a64200a45386132a3203d1a9a7f1146d94cfbc`  
		Last Modified: Fri, 04 Nov 2022 23:29:33 GMT  
		Size: 46.6 MB (46629936 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:111b6c7486426c4b6989102c2ee5be856e8a58e20ab0a350b24a905d536e8e7f`  
		Last Modified: Fri, 04 Nov 2022 23:29:26 GMT  
		Size: 161.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e6f84dce457c6d4f7b7291fce05f8e77998a3a7722a54125a1f1d52ca83043b4`  
		Last Modified: Sat, 05 Nov 2022 01:50:51 GMT  
		Size: 173.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a6c26749ee782392e38845ee2ba79b0da586ef6a45d8e7f29c7af14612278547`  
		Last Modified: Tue, 15 Nov 2022 03:19:57 GMT  
		Size: 12.2 MB (12200249 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4dddc6d9fa6024025b3fcfe729cab2dc544fb25476eca6e80b1af8e8d93bb0ee`  
		Last Modified: Tue, 15 Nov 2022 03:19:56 GMT  
		Size: 452.7 KB (452680 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:06637eebe5e72c8ad9019ad4eb4cdde1f11f7d4c24c7ed7374cf8966343aa2fb`  
		Last Modified: Tue, 15 Nov 2022 03:19:56 GMT  
		Size: 131.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b276fb8390410a8208724033e325715ea26000d5a1a762d4c3699b927884fbfe`  
		Last Modified: Wed, 11 Jan 2023 02:52:45 GMT  
		Size: 178.8 MB (178805608 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:156ca91198173149698aa0396648a9608b6ab1f2bc2666800843ce33c9f85b6e`  
		Last Modified: Tue, 31 Jan 2023 00:24:09 GMT  
		Size: 307.1 MB (307117069 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4c8b70d250c6d507901857473b0dcb67132d7b2a30ce9a69b07b1036853df738`  
		Last Modified: Tue, 31 Jan 2023 00:23:52 GMT  
		Size: 2.4 MB (2377191 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a9681fd36be674d25231c69d6a39f9e8fa65034eeaef5d1bd885fdbeac7f0f6b`  
		Last Modified: Tue, 31 Jan 2023 00:23:51 GMT  
		Size: 1.3 KB (1346 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a9d0d5da840f4d7da9943942b38cd092fae11f41dc6c19afd58d655cd6192d66`  
		Last Modified: Tue, 31 Jan 2023 00:23:51 GMT  
		Size: 2.3 KB (2312 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d65610da4f1da86fea8fbec0189b066afd4b86e4e8f7d049e3c4bc6ade9ba90a`  
		Last Modified: Tue, 31 Jan 2023 00:23:51 GMT  
		Size: 6.0 KB (6009 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3d41686284d7675eaa0f92c9cc27ebe73b4c30768c8eef9f23ee3b1ad06da00a`  
		Last Modified: Tue, 31 Jan 2023 00:23:51 GMT  
		Size: 2.5 KB (2504 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `xwiki:15` - linux; arm64 variant v8

```console
$ docker pull xwiki@sha256:6bf63d9025b07b69d744200c05efd4ffb8a52f3c38380f5d59a0b48514203cd2
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **581.7 MB (581709921 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:6600f2bb05836c703d53944bbcb5399d509a9813a27a35e99ff717becc308330`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["xwiki"]`

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
# Wed, 02 Nov 2022 19:44:32 GMT
RUN apt-get update     && DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends tzdata curl wget ca-certificates fontconfig locales     && echo "en_US.UTF-8 UTF-8" >> /etc/locale.gen     && locale-gen en_US.UTF-8     && rm -rf /var/lib/apt/lists/*
# Fri, 04 Nov 2022 22:40:54 GMT
ENV JAVA_VERSION=jdk-11.0.17+8
# Fri, 04 Nov 2022 22:41:33 GMT
RUN set -eux;     ARCH="$(dpkg --print-architecture)";     case "${ARCH}" in        aarch64|arm64)          ESUM='bd6efe3290c8b5a42f695a55a26f3e3c9c284288574879d4b7089f31f5114177';          BINARY_URL='https://github.com/adoptium/temurin11-binaries/releases/download/jdk-11.0.17%2B8/OpenJDK11U-jre_aarch64_linux_hotspot_11.0.17_8.tar.gz';          ;;        armhf|arm)          ESUM='8cf113d3d7fa808895c8d2e41bb890af21c47e38c2460e0588147a4bb8fc658d';          BINARY_URL='https://github.com/adoptium/temurin11-binaries/releases/download/jdk-11.0.17%2B8/OpenJDK11U-jre_arm_linux_hotspot_11.0.17_8.tar.gz';          ;;        ppc64el|powerpc:common64)          ESUM='0ca3d806131ab5834c501f9c625bb0248cd528af361c704503348e9c9605bedf';          BINARY_URL='https://github.com/adoptium/temurin11-binaries/releases/download/jdk-11.0.17%2B8/OpenJDK11U-jre_ppc64le_linux_hotspot_11.0.17_8.tar.gz';          ;;        s390x|s390:64-bit)          ESUM='dd3b159a374086e65cb07c4ccb226c90f9c02ef929cba6f0b642171d7ed97fa4';          BINARY_URL='https://github.com/adoptium/temurin11-binaries/releases/download/jdk-11.0.17%2B8/OpenJDK11U-jre_s390x_linux_hotspot_11.0.17_8.tar.gz';          ;;        amd64|i386:x86-64)          ESUM='752616097e09d7f60a3ad8bd312f90eaf50ac72577e55df229fe6e8091148f79';          BINARY_URL='https://github.com/adoptium/temurin11-binaries/releases/download/jdk-11.0.17%2B8/OpenJDK11U-jre_x64_linux_hotspot_11.0.17_8.tar.gz';          ;;        *)          echo "Unsupported arch: ${ARCH}";          exit 1;          ;;     esac; 	  wget -O /tmp/openjdk.tar.gz ${BINARY_URL}; 	  echo "${ESUM} */tmp/openjdk.tar.gz" | sha256sum -c -; 	  mkdir -p "$JAVA_HOME"; 	  tar --extract 	      --file /tmp/openjdk.tar.gz 	      --directory "$JAVA_HOME" 	      --strip-components 1 	      --no-same-owner 	  ;     rm /tmp/openjdk.tar.gz;     find "$JAVA_HOME/lib" -name '*.so' -exec dirname '{}' ';' | sort -u > /etc/ld.so.conf.d/docker-openjdk.conf;     ldconfig;     java -Xshare:dump;
# Fri, 04 Nov 2022 22:41:34 GMT
RUN echo Verifying install ...     && fileEncoding="$(echo 'System.out.println(System.getProperty("file.encoding"))' | jshell -s -)"; [ "$fileEncoding" = 'UTF-8' ]; rm -rf ~/.java     && echo java --version && java --version     && echo Complete.
# Fri, 04 Nov 2022 23:48:38 GMT
ENV CATALINA_HOME=/usr/local/tomcat
# Fri, 04 Nov 2022 23:48:38 GMT
ENV PATH=/usr/local/tomcat/bin:/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Fri, 04 Nov 2022 23:48:38 GMT
RUN mkdir -p "$CATALINA_HOME"
# Fri, 04 Nov 2022 23:48:39 GMT
WORKDIR /usr/local/tomcat
# Fri, 04 Nov 2022 23:48:39 GMT
ENV TOMCAT_NATIVE_LIBDIR=/usr/local/tomcat/native-jni-lib
# Fri, 04 Nov 2022 23:48:39 GMT
ENV LD_LIBRARY_PATH=/usr/local/tomcat/native-jni-lib
# Fri, 04 Nov 2022 23:53:12 GMT
ENV GPG_KEYS=48F8E69F6390C9F25CFEDCD268248959359E722B A9C5DF4D22E99998D9875A5110C01C5A2F6059E7 DCFD35E0BF8CA7344752DE8B6FB21E8933C60243
# Fri, 04 Nov 2022 23:53:12 GMT
ENV TOMCAT_MAJOR=9
# Tue, 15 Nov 2022 04:57:22 GMT
ENV TOMCAT_VERSION=9.0.69
# Tue, 15 Nov 2022 04:57:22 GMT
ENV TOMCAT_SHA512=8c883c54ce9ce43eba37756a6404cdf3477879883a3e6d146dc8a7aa5e0425f487466afe6b6da4a895927cb7cb59177b9379cec18000f2de12785be57408c779
# Tue, 15 Nov 2022 04:57:22 GMT
COPY dir:096b403a5f78b17e6b4bff63128a9c93941b97f22470991610dd641633d977f1 in /usr/local/tomcat 
# Tue, 15 Nov 2022 04:57:25 GMT
RUN set -eux; 	apt-get update; 	xargs -rt apt-get install -y --no-install-recommends < "$TOMCAT_NATIVE_LIBDIR/.dependencies.txt"; 	rm -rf /var/lib/apt/lists/*
# Tue, 15 Nov 2022 04:57:26 GMT
RUN set -eux; 	nativeLines="$(catalina.sh configtest 2>&1)"; 	nativeLines="$(echo "$nativeLines" | grep 'Apache Tomcat Native')"; 	nativeLines="$(echo "$nativeLines" | sort -u)"; 	if ! echo "$nativeLines" | grep -E 'INFO: Loaded( APR based)? Apache Tomcat Native library' >&2; then 		echo >&2 "$nativeLines"; 		exit 1; 	fi
# Tue, 15 Nov 2022 04:57:26 GMT
EXPOSE 8080
# Tue, 15 Nov 2022 04:57:27 GMT
CMD ["catalina.sh" "run"]
# Wed, 11 Jan 2023 03:05:10 GMT
LABEL org.opencontainers.image.authors=XWiki Development Team <committers@xwiki.org>
# Wed, 11 Jan 2023 03:05:10 GMT
LABEL org.opencontainers.image.url=https://hub.docker.com/_/xwiki
# Wed, 11 Jan 2023 03:05:10 GMT
LABEL org.opencontainers.image.documentation=https://hub.docker.com/_/xwiki
# Wed, 11 Jan 2023 03:05:10 GMT
LABEL org.opencontainers.image.source=https://github.com/xwiki/xwiki-docker.git
# Wed, 11 Jan 2023 03:05:11 GMT
LABEL org.opencontainers.image.vendor=xwiki.org
# Wed, 11 Jan 2023 03:05:11 GMT
LABEL org.opencontainers.image.licenses=LGPL-2.1
# Wed, 11 Jan 2023 03:07:37 GMT
RUN apt-get update &&   apt-get --no-install-recommends -y install     curl     libreoffice     unzip     procps &&   rm -rf /var/lib/apt/lists/*
# Tue, 31 Jan 2023 00:47:12 GMT
ENV XWIKI_VERSION=15.0
# Tue, 31 Jan 2023 00:47:12 GMT
ENV XWIKI_URL_PREFIX=https://maven.xwiki.org/releases/org/xwiki/platform/xwiki-platform-distribution-war/15.0
# Tue, 31 Jan 2023 00:47:12 GMT
ENV XWIKI_DOWNLOAD_SHA256=79ba0f479bbc49521c113821adc9d91141075a9470d7f9bbb6994ca59c30d121
# Tue, 31 Jan 2023 00:47:58 GMT
RUN rm -rf /usr/local/tomcat/webapps/* &&   mkdir -p /usr/local/tomcat/temp &&   mkdir -p /usr/local/xwiki/data &&   curl -fSL "${XWIKI_URL_PREFIX}/xwiki-platform-distribution-war-${XWIKI_VERSION}.war" -o xwiki.war &&   echo "$XWIKI_DOWNLOAD_SHA256 xwiki.war" | sha256sum -c - &&   unzip -d /usr/local/tomcat/webapps/ROOT xwiki.war &&   rm -f xwiki.war
# Tue, 31 Jan 2023 00:48:01 GMT
ENV MYSQL_JDBC_VERSION=8.0.31
# Tue, 31 Jan 2023 00:48:01 GMT
ENV MYSQL_JDBC_SHA256=5249e3dc6d6531b37790e3f61845b96db5e41e891d3d8edb0e2e3a1b53ca2f4f
# Tue, 31 Jan 2023 00:48:01 GMT
ENV MYSQL_JDBC_PREFIX=https://repo1.maven.org/maven2/com/mysql/mysql-connector-j/8.0.31
# Tue, 31 Jan 2023 00:48:01 GMT
ENV MYSQL_JDBC_ARTIFACT=mysql-connector-j-8.0.31.jar
# Tue, 31 Jan 2023 00:48:01 GMT
ENV MYSQL_JDBC_TARGET=/usr/local/tomcat/webapps/ROOT/WEB-INF/lib/mysql-connector-j-8.0.31.jar
# Tue, 31 Jan 2023 00:48:02 GMT
RUN curl -fSL "${MYSQL_JDBC_PREFIX}/${MYSQL_JDBC_ARTIFACT}" -o $MYSQL_JDBC_TARGET &&   echo "$MYSQL_JDBC_SHA256 $MYSQL_JDBC_TARGET" | sha256sum -c -
# Tue, 31 Jan 2023 00:48:02 GMT
COPY file:0a1be11e2eb610a1dbcd415404e3a592641110b93090030cb831e3a19a163017 in /usr/local/tomcat/bin/ 
# Tue, 31 Jan 2023 00:48:02 GMT
COPY file:1b8409986f3e4eb79a7a0b18472cb2692a61d504fb5ef34292bc997b79fd760d in /usr/local/tomcat/webapps/ROOT/WEB-INF/hibernate.cfg.xml 
# Tue, 31 Jan 2023 00:48:03 GMT
RUN sed -i 's/<id>org.xwiki.platform:xwiki-platform-distribution-war/<id>org.xwiki.platform:xwiki-platform-distribution-docker/'   /usr/local/tomcat/webapps/ROOT/META-INF/extension.xed
# Tue, 31 Jan 2023 00:48:03 GMT
COPY file:a47c4dcd87c9dad97aff38c49188357e6193bcad50757e516cfb08a60d4de611 in /usr/local/bin/docker-entrypoint.sh 
# Tue, 31 Jan 2023 00:48:03 GMT
VOLUME [/usr/local/xwiki]
# Tue, 31 Jan 2023 00:48:03 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 31 Jan 2023 00:48:03 GMT
CMD ["xwiki"]
```

-	Layers:
	-	`sha256:0509fae36eb0656f8bdb23f8ae64100d893bcea2563e97468d337e04d2d0410b`  
		Last Modified: Wed, 02 Nov 2022 18:50:21 GMT  
		Size: 28.4 MB (28382154 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e502a1af2bcd98f5f0d2f5e4da1a0e7bbe07a2c548e2662f7d37dce5ae1df46c`  
		Last Modified: Wed, 02 Nov 2022 19:48:28 GMT  
		Size: 12.4 MB (12396330 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bc4598c07dd818f03a0378b0341a4a8e80f0152fbb3e7d5246ca4f466f42e611`  
		Last Modified: Fri, 04 Nov 2022 22:46:46 GMT  
		Size: 45.0 MB (44958470 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:715a937a1066f998b331fcd62256ad01a5571bdf46804e97825afc64f9ebb427`  
		Last Modified: Fri, 04 Nov 2022 22:46:41 GMT  
		Size: 160.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5fb623f082f74b2fa9fc2c4e3f3a4802875cb9753cfa26ed940201ce72bb56cb`  
		Last Modified: Sat, 05 Nov 2022 00:03:40 GMT  
		Size: 172.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:33260b83200262bbd546be371ad3c1f50f5ae7228afb87982d6fa9d6b11bf26f`  
		Last Modified: Tue, 15 Nov 2022 05:10:19 GMT  
		Size: 12.2 MB (12207235 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0955fb697ea9b30a1b4f95385464f646aa1525cb6efba648e22df84ebef6b2ee`  
		Last Modified: Tue, 15 Nov 2022 05:10:18 GMT  
		Size: 452.0 KB (452021 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6eddcf66f2083b1487296a0308e0b058917c97f614f12428d82d89662038dc2e`  
		Last Modified: Tue, 15 Nov 2022 05:10:18 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ae5f60bb64f3fa11da3d15a9639f886186b4c2c021455c3f9db22e0cfe1b1311`  
		Last Modified: Wed, 11 Jan 2023 03:11:14 GMT  
		Size: 173.8 MB (173806827 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1814d85fce571b42f2cfa7c8a904e1a184ee6f49642242a44bbe0037088994a0`  
		Last Modified: Tue, 31 Jan 2023 00:56:04 GMT  
		Size: 307.1 MB (307117070 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8aec0e24b4fa870989f014944c3c7d535355a2371fc8c948b2b11f9b377efe6e`  
		Last Modified: Tue, 31 Jan 2023 00:55:50 GMT  
		Size: 2.4 MB (2377182 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0b65081619aa0114a7f367836ef421eb8d951e559e0f089c7728af7813b1ea62`  
		Last Modified: Tue, 31 Jan 2023 00:55:49 GMT  
		Size: 1.3 KB (1348 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:46ebad072e608146426d8dc30828937049eea36c2e636d7790b4960d6d586977`  
		Last Modified: Tue, 31 Jan 2023 00:55:49 GMT  
		Size: 2.3 KB (2308 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:708fefcedd4ee6c106da247a68c5790f5ab00225d1cdfff8465575265c3a54e6`  
		Last Modified: Tue, 31 Jan 2023 00:55:49 GMT  
		Size: 6.0 KB (6008 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:81e3bf8e20bc921031e7549a41dec1b2d7795cc6da40a0e7096bf654b25c5c3e`  
		Last Modified: Tue, 31 Jan 2023 00:55:49 GMT  
		Size: 2.5 KB (2507 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `xwiki:15-mariadb-tomcat`

```console
$ docker pull xwiki@sha256:725347355967f33745268f1167cc3c1b12fc85e327ccfa96da0848d05e3836c4
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `xwiki:15-mariadb-tomcat` - linux; amd64

```console
$ docker pull xwiki@sha256:cca1fb53bc2f0240f7f4843b846210e341a6002d7b18a0b90202520ce2f4ead0
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **588.7 MB (588672467 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:0088d72e62c01c9996a75e1b7e2296ba530b2dbd4054be70a006b33295aa4ff9`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["xwiki"]`

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
# Wed, 02 Nov 2022 18:44:10 GMT
RUN apt-get update     && DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends tzdata curl wget ca-certificates fontconfig locales     && echo "en_US.UTF-8 UTF-8" >> /etc/locale.gen     && locale-gen en_US.UTF-8     && rm -rf /var/lib/apt/lists/*
# Fri, 04 Nov 2022 23:21:41 GMT
ENV JAVA_VERSION=jdk-11.0.17+8
# Fri, 04 Nov 2022 23:22:31 GMT
RUN set -eux;     ARCH="$(dpkg --print-architecture)";     case "${ARCH}" in        aarch64|arm64)          ESUM='bd6efe3290c8b5a42f695a55a26f3e3c9c284288574879d4b7089f31f5114177';          BINARY_URL='https://github.com/adoptium/temurin11-binaries/releases/download/jdk-11.0.17%2B8/OpenJDK11U-jre_aarch64_linux_hotspot_11.0.17_8.tar.gz';          ;;        armhf|arm)          ESUM='8cf113d3d7fa808895c8d2e41bb890af21c47e38c2460e0588147a4bb8fc658d';          BINARY_URL='https://github.com/adoptium/temurin11-binaries/releases/download/jdk-11.0.17%2B8/OpenJDK11U-jre_arm_linux_hotspot_11.0.17_8.tar.gz';          ;;        ppc64el|powerpc:common64)          ESUM='0ca3d806131ab5834c501f9c625bb0248cd528af361c704503348e9c9605bedf';          BINARY_URL='https://github.com/adoptium/temurin11-binaries/releases/download/jdk-11.0.17%2B8/OpenJDK11U-jre_ppc64le_linux_hotspot_11.0.17_8.tar.gz';          ;;        s390x|s390:64-bit)          ESUM='dd3b159a374086e65cb07c4ccb226c90f9c02ef929cba6f0b642171d7ed97fa4';          BINARY_URL='https://github.com/adoptium/temurin11-binaries/releases/download/jdk-11.0.17%2B8/OpenJDK11U-jre_s390x_linux_hotspot_11.0.17_8.tar.gz';          ;;        amd64|i386:x86-64)          ESUM='752616097e09d7f60a3ad8bd312f90eaf50ac72577e55df229fe6e8091148f79';          BINARY_URL='https://github.com/adoptium/temurin11-binaries/releases/download/jdk-11.0.17%2B8/OpenJDK11U-jre_x64_linux_hotspot_11.0.17_8.tar.gz';          ;;        *)          echo "Unsupported arch: ${ARCH}";          exit 1;          ;;     esac; 	  wget -O /tmp/openjdk.tar.gz ${BINARY_URL}; 	  echo "${ESUM} */tmp/openjdk.tar.gz" | sha256sum -c -; 	  mkdir -p "$JAVA_HOME"; 	  tar --extract 	      --file /tmp/openjdk.tar.gz 	      --directory "$JAVA_HOME" 	      --strip-components 1 	      --no-same-owner 	  ;     rm /tmp/openjdk.tar.gz;     find "$JAVA_HOME/lib" -name '*.so' -exec dirname '{}' ';' | sort -u > /etc/ld.so.conf.d/docker-openjdk.conf;     ldconfig;     java -Xshare:dump;
# Fri, 04 Nov 2022 23:22:32 GMT
RUN echo Verifying install ...     && fileEncoding="$(echo 'System.out.println(System.getProperty("file.encoding"))' | jshell -s -)"; [ "$fileEncoding" = 'UTF-8' ]; rm -rf ~/.java     && echo java --version && java --version     && echo Complete.
# Sat, 05 Nov 2022 01:35:16 GMT
ENV CATALINA_HOME=/usr/local/tomcat
# Sat, 05 Nov 2022 01:35:16 GMT
ENV PATH=/usr/local/tomcat/bin:/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Sat, 05 Nov 2022 01:35:17 GMT
RUN mkdir -p "$CATALINA_HOME"
# Sat, 05 Nov 2022 01:35:17 GMT
WORKDIR /usr/local/tomcat
# Sat, 05 Nov 2022 01:35:17 GMT
ENV TOMCAT_NATIVE_LIBDIR=/usr/local/tomcat/native-jni-lib
# Sat, 05 Nov 2022 01:35:17 GMT
ENV LD_LIBRARY_PATH=/usr/local/tomcat/native-jni-lib
# Sat, 05 Nov 2022 01:39:54 GMT
ENV GPG_KEYS=48F8E69F6390C9F25CFEDCD268248959359E722B A9C5DF4D22E99998D9875A5110C01C5A2F6059E7 DCFD35E0BF8CA7344752DE8B6FB21E8933C60243
# Sat, 05 Nov 2022 01:39:54 GMT
ENV TOMCAT_MAJOR=9
# Tue, 15 Nov 2022 03:06:43 GMT
ENV TOMCAT_VERSION=9.0.69
# Tue, 15 Nov 2022 03:06:43 GMT
ENV TOMCAT_SHA512=8c883c54ce9ce43eba37756a6404cdf3477879883a3e6d146dc8a7aa5e0425f487466afe6b6da4a895927cb7cb59177b9379cec18000f2de12785be57408c779
# Tue, 15 Nov 2022 03:06:44 GMT
COPY dir:b1a33aa3993dbbfbebb33bd9aa546b60c2f2191abf1227f453d4e830f6deb35f in /usr/local/tomcat 
# Tue, 15 Nov 2022 03:06:48 GMT
RUN set -eux; 	apt-get update; 	xargs -rt apt-get install -y --no-install-recommends < "$TOMCAT_NATIVE_LIBDIR/.dependencies.txt"; 	rm -rf /var/lib/apt/lists/*
# Tue, 15 Nov 2022 03:06:49 GMT
RUN set -eux; 	nativeLines="$(catalina.sh configtest 2>&1)"; 	nativeLines="$(echo "$nativeLines" | grep 'Apache Tomcat Native')"; 	nativeLines="$(echo "$nativeLines" | sort -u)"; 	if ! echo "$nativeLines" | grep -E 'INFO: Loaded( APR based)? Apache Tomcat Native library' >&2; then 		echo >&2 "$nativeLines"; 		exit 1; 	fi
# Tue, 15 Nov 2022 03:06:49 GMT
EXPOSE 8080
# Tue, 15 Nov 2022 03:06:49 GMT
CMD ["catalina.sh" "run"]
# Wed, 11 Jan 2023 02:47:03 GMT
LABEL org.opencontainers.image.authors=XWiki Development Team <committers@xwiki.org>
# Wed, 11 Jan 2023 02:47:03 GMT
LABEL org.opencontainers.image.url=https://hub.docker.com/_/xwiki
# Wed, 11 Jan 2023 02:47:03 GMT
LABEL org.opencontainers.image.documentation=https://hub.docker.com/_/xwiki
# Wed, 11 Jan 2023 02:47:03 GMT
LABEL org.opencontainers.image.source=https://github.com/xwiki/xwiki-docker.git
# Wed, 11 Jan 2023 02:47:04 GMT
LABEL org.opencontainers.image.vendor=xwiki.org
# Wed, 11 Jan 2023 02:47:04 GMT
LABEL org.opencontainers.image.licenses=LGPL-2.1
# Wed, 11 Jan 2023 02:49:03 GMT
RUN apt-get update &&   apt-get --no-install-recommends -y install     curl     libreoffice     unzip     procps &&   rm -rf /var/lib/apt/lists/*
# Tue, 31 Jan 2023 00:20:17 GMT
ENV XWIKI_VERSION=15.0
# Tue, 31 Jan 2023 00:20:17 GMT
ENV XWIKI_URL_PREFIX=https://maven.xwiki.org/releases/org/xwiki/platform/xwiki-platform-distribution-war/15.0
# Tue, 31 Jan 2023 00:20:17 GMT
ENV XWIKI_DOWNLOAD_SHA256=79ba0f479bbc49521c113821adc9d91141075a9470d7f9bbb6994ca59c30d121
# Tue, 31 Jan 2023 00:21:18 GMT
RUN rm -rf /usr/local/tomcat/webapps/* &&   mkdir -p /usr/local/tomcat/temp &&   mkdir -p /usr/local/xwiki/data &&   curl -fSL "${XWIKI_URL_PREFIX}/xwiki-platform-distribution-war-${XWIKI_VERSION}.war" -o xwiki.war &&   echo "$XWIKI_DOWNLOAD_SHA256 xwiki.war" | sha256sum -c - &&   unzip -d /usr/local/tomcat/webapps/ROOT xwiki.war &&   rm -f xwiki.war
# Tue, 31 Jan 2023 00:22:50 GMT
ENV MARIADB_JDBC_VERSION=3.1.1
# Tue, 31 Jan 2023 00:22:50 GMT
ENV MARIADB_JDBC_SHA256=a554541fd88047905fb0c4c10e1d85295f5e38c7bb5fb408b425392a79fc26e3
# Tue, 31 Jan 2023 00:22:50 GMT
ENV MARIADB_JDBC_PREFIX=https://repo1.maven.org/maven2/org/mariadb/jdbc/mariadb-java-client/3.1.1
# Tue, 31 Jan 2023 00:22:50 GMT
ENV MARIADB_JDBC_ARTIFACT=mariadb-java-client-3.1.1.jar
# Tue, 31 Jan 2023 00:22:50 GMT
ENV MARIADB_JDBC_TARGET=/usr/local/tomcat/webapps/ROOT/WEB-INF/lib/mariadb-java-client-3.1.1.jar
# Tue, 31 Jan 2023 00:22:51 GMT
RUN curl -fSL "${MARIADB_JDBC_PREFIX}/${MARIADB_JDBC_ARTIFACT}" -o $MARIADB_JDBC_TARGET &&   echo "$MARIADB_JDBC_SHA256 $MARIADB_JDBC_TARGET" | sha256sum -c -
# Tue, 31 Jan 2023 00:22:51 GMT
COPY file:0a1be11e2eb610a1dbcd415404e3a592641110b93090030cb831e3a19a163017 in /usr/local/tomcat/bin/ 
# Tue, 31 Jan 2023 00:22:51 GMT
COPY file:0e237c3876eeb3b5f3473a064d3e507da2df6c228ca714687930b34e3b687601 in /usr/local/tomcat/webapps/ROOT/WEB-INF/hibernate.cfg.xml 
# Tue, 31 Jan 2023 00:22:52 GMT
RUN sed -i 's/<id>org.xwiki.platform:xwiki-platform-distribution-war/<id>org.xwiki.platform:xwiki-platform-distribution-docker/'   /usr/local/tomcat/webapps/ROOT/META-INF/extension.xed
# Tue, 31 Jan 2023 00:22:52 GMT
COPY file:a47c4dcd87c9dad97aff38c49188357e6193bcad50757e516cfb08a60d4de611 in /usr/local/bin/docker-entrypoint.sh 
# Tue, 31 Jan 2023 00:22:52 GMT
VOLUME [/usr/local/xwiki]
# Tue, 31 Jan 2023 00:22:52 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 31 Jan 2023 00:22:52 GMT
CMD ["xwiki"]
```

-	Layers:
	-	`sha256:e96e057aae67380a4ddb16c337c5c3669d97fdff69ec537f02aa2cc30d814281`  
		Last Modified: Wed, 02 Nov 2022 03:03:36 GMT  
		Size: 30.4 MB (30425607 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4ced2591451da3a02e2b6bb44752b9e3f00d77789921be4df5082fb9f9880ad0`  
		Last Modified: Wed, 02 Nov 2022 18:48:43 GMT  
		Size: 12.4 MB (12439006 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:df8f874ae8c08a9e69e5fbe6c5a64200a45386132a3203d1a9a7f1146d94cfbc`  
		Last Modified: Fri, 04 Nov 2022 23:29:33 GMT  
		Size: 46.6 MB (46629936 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:111b6c7486426c4b6989102c2ee5be856e8a58e20ab0a350b24a905d536e8e7f`  
		Last Modified: Fri, 04 Nov 2022 23:29:26 GMT  
		Size: 161.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e6f84dce457c6d4f7b7291fce05f8e77998a3a7722a54125a1f1d52ca83043b4`  
		Last Modified: Sat, 05 Nov 2022 01:50:51 GMT  
		Size: 173.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a6c26749ee782392e38845ee2ba79b0da586ef6a45d8e7f29c7af14612278547`  
		Last Modified: Tue, 15 Nov 2022 03:19:57 GMT  
		Size: 12.2 MB (12200249 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4dddc6d9fa6024025b3fcfe729cab2dc544fb25476eca6e80b1af8e8d93bb0ee`  
		Last Modified: Tue, 15 Nov 2022 03:19:56 GMT  
		Size: 452.7 KB (452680 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:06637eebe5e72c8ad9019ad4eb4cdde1f11f7d4c24c7ed7374cf8966343aa2fb`  
		Last Modified: Tue, 15 Nov 2022 03:19:56 GMT  
		Size: 131.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b276fb8390410a8208724033e325715ea26000d5a1a762d4c3699b927884fbfe`  
		Last Modified: Wed, 11 Jan 2023 02:52:45 GMT  
		Size: 178.8 MB (178805608 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:156ca91198173149698aa0396648a9608b6ab1f2bc2666800843ce33c9f85b6e`  
		Last Modified: Tue, 31 Jan 2023 00:24:09 GMT  
		Size: 307.1 MB (307117069 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:457b62e39784bb863cc6a7514f591232a9b9442f2f105a85bdbd5e4abb166ad6`  
		Last Modified: Tue, 31 Jan 2023 00:25:23 GMT  
		Size: 589.7 KB (589675 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:30adbbecb36197c3e48c90be60a50c089cb9738a771c968b36240b05b8164a30`  
		Last Modified: Tue, 31 Jan 2023 00:25:22 GMT  
		Size: 1.3 KB (1345 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3bfcc8a896e6e21d5c28da101d5d57167a5cfc49c542a407feabe27f6c355b6f`  
		Last Modified: Tue, 31 Jan 2023 00:25:22 GMT  
		Size: 2.3 KB (2312 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5cbacf6c3ece365f64b683c8ab4fe61301319c8f1bd26d38ea40abbbd15bc7d4`  
		Last Modified: Tue, 31 Jan 2023 00:25:23 GMT  
		Size: 6.0 KB (6008 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6687ecee0e041196fd810c316565d70808b445cdce0b089b2177e6636bffd9fe`  
		Last Modified: Tue, 31 Jan 2023 00:25:23 GMT  
		Size: 2.5 KB (2507 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `xwiki:15-mariadb-tomcat` - linux; arm64 variant v8

```console
$ docker pull xwiki@sha256:14b1c6df2a5c5c9b549f372fce50719f39fc809b8b02c945d92eb29c29f7bc75
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **579.9 MB (579922416 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d9a728666283f6f4b71f567ce6c5ef1e2dc544facfd01d52fdf1577be95c6b07`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["xwiki"]`

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
# Wed, 02 Nov 2022 19:44:32 GMT
RUN apt-get update     && DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends tzdata curl wget ca-certificates fontconfig locales     && echo "en_US.UTF-8 UTF-8" >> /etc/locale.gen     && locale-gen en_US.UTF-8     && rm -rf /var/lib/apt/lists/*
# Fri, 04 Nov 2022 22:40:54 GMT
ENV JAVA_VERSION=jdk-11.0.17+8
# Fri, 04 Nov 2022 22:41:33 GMT
RUN set -eux;     ARCH="$(dpkg --print-architecture)";     case "${ARCH}" in        aarch64|arm64)          ESUM='bd6efe3290c8b5a42f695a55a26f3e3c9c284288574879d4b7089f31f5114177';          BINARY_URL='https://github.com/adoptium/temurin11-binaries/releases/download/jdk-11.0.17%2B8/OpenJDK11U-jre_aarch64_linux_hotspot_11.0.17_8.tar.gz';          ;;        armhf|arm)          ESUM='8cf113d3d7fa808895c8d2e41bb890af21c47e38c2460e0588147a4bb8fc658d';          BINARY_URL='https://github.com/adoptium/temurin11-binaries/releases/download/jdk-11.0.17%2B8/OpenJDK11U-jre_arm_linux_hotspot_11.0.17_8.tar.gz';          ;;        ppc64el|powerpc:common64)          ESUM='0ca3d806131ab5834c501f9c625bb0248cd528af361c704503348e9c9605bedf';          BINARY_URL='https://github.com/adoptium/temurin11-binaries/releases/download/jdk-11.0.17%2B8/OpenJDK11U-jre_ppc64le_linux_hotspot_11.0.17_8.tar.gz';          ;;        s390x|s390:64-bit)          ESUM='dd3b159a374086e65cb07c4ccb226c90f9c02ef929cba6f0b642171d7ed97fa4';          BINARY_URL='https://github.com/adoptium/temurin11-binaries/releases/download/jdk-11.0.17%2B8/OpenJDK11U-jre_s390x_linux_hotspot_11.0.17_8.tar.gz';          ;;        amd64|i386:x86-64)          ESUM='752616097e09d7f60a3ad8bd312f90eaf50ac72577e55df229fe6e8091148f79';          BINARY_URL='https://github.com/adoptium/temurin11-binaries/releases/download/jdk-11.0.17%2B8/OpenJDK11U-jre_x64_linux_hotspot_11.0.17_8.tar.gz';          ;;        *)          echo "Unsupported arch: ${ARCH}";          exit 1;          ;;     esac; 	  wget -O /tmp/openjdk.tar.gz ${BINARY_URL}; 	  echo "${ESUM} */tmp/openjdk.tar.gz" | sha256sum -c -; 	  mkdir -p "$JAVA_HOME"; 	  tar --extract 	      --file /tmp/openjdk.tar.gz 	      --directory "$JAVA_HOME" 	      --strip-components 1 	      --no-same-owner 	  ;     rm /tmp/openjdk.tar.gz;     find "$JAVA_HOME/lib" -name '*.so' -exec dirname '{}' ';' | sort -u > /etc/ld.so.conf.d/docker-openjdk.conf;     ldconfig;     java -Xshare:dump;
# Fri, 04 Nov 2022 22:41:34 GMT
RUN echo Verifying install ...     && fileEncoding="$(echo 'System.out.println(System.getProperty("file.encoding"))' | jshell -s -)"; [ "$fileEncoding" = 'UTF-8' ]; rm -rf ~/.java     && echo java --version && java --version     && echo Complete.
# Fri, 04 Nov 2022 23:48:38 GMT
ENV CATALINA_HOME=/usr/local/tomcat
# Fri, 04 Nov 2022 23:48:38 GMT
ENV PATH=/usr/local/tomcat/bin:/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Fri, 04 Nov 2022 23:48:38 GMT
RUN mkdir -p "$CATALINA_HOME"
# Fri, 04 Nov 2022 23:48:39 GMT
WORKDIR /usr/local/tomcat
# Fri, 04 Nov 2022 23:48:39 GMT
ENV TOMCAT_NATIVE_LIBDIR=/usr/local/tomcat/native-jni-lib
# Fri, 04 Nov 2022 23:48:39 GMT
ENV LD_LIBRARY_PATH=/usr/local/tomcat/native-jni-lib
# Fri, 04 Nov 2022 23:53:12 GMT
ENV GPG_KEYS=48F8E69F6390C9F25CFEDCD268248959359E722B A9C5DF4D22E99998D9875A5110C01C5A2F6059E7 DCFD35E0BF8CA7344752DE8B6FB21E8933C60243
# Fri, 04 Nov 2022 23:53:12 GMT
ENV TOMCAT_MAJOR=9
# Tue, 15 Nov 2022 04:57:22 GMT
ENV TOMCAT_VERSION=9.0.69
# Tue, 15 Nov 2022 04:57:22 GMT
ENV TOMCAT_SHA512=8c883c54ce9ce43eba37756a6404cdf3477879883a3e6d146dc8a7aa5e0425f487466afe6b6da4a895927cb7cb59177b9379cec18000f2de12785be57408c779
# Tue, 15 Nov 2022 04:57:22 GMT
COPY dir:096b403a5f78b17e6b4bff63128a9c93941b97f22470991610dd641633d977f1 in /usr/local/tomcat 
# Tue, 15 Nov 2022 04:57:25 GMT
RUN set -eux; 	apt-get update; 	xargs -rt apt-get install -y --no-install-recommends < "$TOMCAT_NATIVE_LIBDIR/.dependencies.txt"; 	rm -rf /var/lib/apt/lists/*
# Tue, 15 Nov 2022 04:57:26 GMT
RUN set -eux; 	nativeLines="$(catalina.sh configtest 2>&1)"; 	nativeLines="$(echo "$nativeLines" | grep 'Apache Tomcat Native')"; 	nativeLines="$(echo "$nativeLines" | sort -u)"; 	if ! echo "$nativeLines" | grep -E 'INFO: Loaded( APR based)? Apache Tomcat Native library' >&2; then 		echo >&2 "$nativeLines"; 		exit 1; 	fi
# Tue, 15 Nov 2022 04:57:26 GMT
EXPOSE 8080
# Tue, 15 Nov 2022 04:57:27 GMT
CMD ["catalina.sh" "run"]
# Wed, 11 Jan 2023 03:05:10 GMT
LABEL org.opencontainers.image.authors=XWiki Development Team <committers@xwiki.org>
# Wed, 11 Jan 2023 03:05:10 GMT
LABEL org.opencontainers.image.url=https://hub.docker.com/_/xwiki
# Wed, 11 Jan 2023 03:05:10 GMT
LABEL org.opencontainers.image.documentation=https://hub.docker.com/_/xwiki
# Wed, 11 Jan 2023 03:05:10 GMT
LABEL org.opencontainers.image.source=https://github.com/xwiki/xwiki-docker.git
# Wed, 11 Jan 2023 03:05:11 GMT
LABEL org.opencontainers.image.vendor=xwiki.org
# Wed, 11 Jan 2023 03:05:11 GMT
LABEL org.opencontainers.image.licenses=LGPL-2.1
# Wed, 11 Jan 2023 03:07:37 GMT
RUN apt-get update &&   apt-get --no-install-recommends -y install     curl     libreoffice     unzip     procps &&   rm -rf /var/lib/apt/lists/*
# Tue, 31 Jan 2023 00:47:12 GMT
ENV XWIKI_VERSION=15.0
# Tue, 31 Jan 2023 00:47:12 GMT
ENV XWIKI_URL_PREFIX=https://maven.xwiki.org/releases/org/xwiki/platform/xwiki-platform-distribution-war/15.0
# Tue, 31 Jan 2023 00:47:12 GMT
ENV XWIKI_DOWNLOAD_SHA256=79ba0f479bbc49521c113821adc9d91141075a9470d7f9bbb6994ca59c30d121
# Tue, 31 Jan 2023 00:47:58 GMT
RUN rm -rf /usr/local/tomcat/webapps/* &&   mkdir -p /usr/local/tomcat/temp &&   mkdir -p /usr/local/xwiki/data &&   curl -fSL "${XWIKI_URL_PREFIX}/xwiki-platform-distribution-war-${XWIKI_VERSION}.war" -o xwiki.war &&   echo "$XWIKI_DOWNLOAD_SHA256 xwiki.war" | sha256sum -c - &&   unzip -d /usr/local/tomcat/webapps/ROOT xwiki.war &&   rm -f xwiki.war
# Tue, 31 Jan 2023 00:54:48 GMT
ENV MARIADB_JDBC_VERSION=3.1.1
# Tue, 31 Jan 2023 00:54:48 GMT
ENV MARIADB_JDBC_SHA256=a554541fd88047905fb0c4c10e1d85295f5e38c7bb5fb408b425392a79fc26e3
# Tue, 31 Jan 2023 00:54:48 GMT
ENV MARIADB_JDBC_PREFIX=https://repo1.maven.org/maven2/org/mariadb/jdbc/mariadb-java-client/3.1.1
# Tue, 31 Jan 2023 00:54:48 GMT
ENV MARIADB_JDBC_ARTIFACT=mariadb-java-client-3.1.1.jar
# Tue, 31 Jan 2023 00:54:48 GMT
ENV MARIADB_JDBC_TARGET=/usr/local/tomcat/webapps/ROOT/WEB-INF/lib/mariadb-java-client-3.1.1.jar
# Tue, 31 Jan 2023 00:54:49 GMT
RUN curl -fSL "${MARIADB_JDBC_PREFIX}/${MARIADB_JDBC_ARTIFACT}" -o $MARIADB_JDBC_TARGET &&   echo "$MARIADB_JDBC_SHA256 $MARIADB_JDBC_TARGET" | sha256sum -c -
# Tue, 31 Jan 2023 00:54:49 GMT
COPY file:0a1be11e2eb610a1dbcd415404e3a592641110b93090030cb831e3a19a163017 in /usr/local/tomcat/bin/ 
# Tue, 31 Jan 2023 00:54:49 GMT
COPY file:0e237c3876eeb3b5f3473a064d3e507da2df6c228ca714687930b34e3b687601 in /usr/local/tomcat/webapps/ROOT/WEB-INF/hibernate.cfg.xml 
# Tue, 31 Jan 2023 00:54:49 GMT
RUN sed -i 's/<id>org.xwiki.platform:xwiki-platform-distribution-war/<id>org.xwiki.platform:xwiki-platform-distribution-docker/'   /usr/local/tomcat/webapps/ROOT/META-INF/extension.xed
# Tue, 31 Jan 2023 00:54:49 GMT
COPY file:a47c4dcd87c9dad97aff38c49188357e6193bcad50757e516cfb08a60d4de611 in /usr/local/bin/docker-entrypoint.sh 
# Tue, 31 Jan 2023 00:54:49 GMT
VOLUME [/usr/local/xwiki]
# Tue, 31 Jan 2023 00:54:50 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 31 Jan 2023 00:54:50 GMT
CMD ["xwiki"]
```

-	Layers:
	-	`sha256:0509fae36eb0656f8bdb23f8ae64100d893bcea2563e97468d337e04d2d0410b`  
		Last Modified: Wed, 02 Nov 2022 18:50:21 GMT  
		Size: 28.4 MB (28382154 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e502a1af2bcd98f5f0d2f5e4da1a0e7bbe07a2c548e2662f7d37dce5ae1df46c`  
		Last Modified: Wed, 02 Nov 2022 19:48:28 GMT  
		Size: 12.4 MB (12396330 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bc4598c07dd818f03a0378b0341a4a8e80f0152fbb3e7d5246ca4f466f42e611`  
		Last Modified: Fri, 04 Nov 2022 22:46:46 GMT  
		Size: 45.0 MB (44958470 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:715a937a1066f998b331fcd62256ad01a5571bdf46804e97825afc64f9ebb427`  
		Last Modified: Fri, 04 Nov 2022 22:46:41 GMT  
		Size: 160.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5fb623f082f74b2fa9fc2c4e3f3a4802875cb9753cfa26ed940201ce72bb56cb`  
		Last Modified: Sat, 05 Nov 2022 00:03:40 GMT  
		Size: 172.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:33260b83200262bbd546be371ad3c1f50f5ae7228afb87982d6fa9d6b11bf26f`  
		Last Modified: Tue, 15 Nov 2022 05:10:19 GMT  
		Size: 12.2 MB (12207235 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0955fb697ea9b30a1b4f95385464f646aa1525cb6efba648e22df84ebef6b2ee`  
		Last Modified: Tue, 15 Nov 2022 05:10:18 GMT  
		Size: 452.0 KB (452021 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6eddcf66f2083b1487296a0308e0b058917c97f614f12428d82d89662038dc2e`  
		Last Modified: Tue, 15 Nov 2022 05:10:18 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ae5f60bb64f3fa11da3d15a9639f886186b4c2c021455c3f9db22e0cfe1b1311`  
		Last Modified: Wed, 11 Jan 2023 03:11:14 GMT  
		Size: 173.8 MB (173806827 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1814d85fce571b42f2cfa7c8a904e1a184ee6f49642242a44bbe0037088994a0`  
		Last Modified: Tue, 31 Jan 2023 00:56:04 GMT  
		Size: 307.1 MB (307117070 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e8637677b7ba0da683afa4e56ff0561e4ba77c8782d5a98da785f4ef58d1caf9`  
		Last Modified: Tue, 31 Jan 2023 00:57:14 GMT  
		Size: 589.7 KB (589677 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:61a67398bc888bcce1656edec9bb40409ce0ffc2fe83d0437c28dd64a8f697ce`  
		Last Modified: Tue, 31 Jan 2023 00:57:14 GMT  
		Size: 1.3 KB (1345 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7ebda7e506ea819ce9717c3d0334df81608bc4c7149cd47ebc9a32790141a637`  
		Last Modified: Tue, 31 Jan 2023 00:57:14 GMT  
		Size: 2.3 KB (2313 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2ceebbf08640e235a928c9df650ca3ab8d0c6b506faa158ecde5fdde34bf8813`  
		Last Modified: Tue, 31 Jan 2023 00:57:14 GMT  
		Size: 6.0 KB (6007 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:12b1d23eae23b1a09ecd4185941d43f13d4ad633d4c6257ab8107a8eebd5fb12`  
		Last Modified: Tue, 31 Jan 2023 00:57:14 GMT  
		Size: 2.5 KB (2506 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `xwiki:15-mysql-tomcat`

```console
$ docker pull xwiki@sha256:33e789838f82ce73efec6664859feb1ced7a5b7605fbfaddb81916716bce524f
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `xwiki:15-mysql-tomcat` - linux; amd64

```console
$ docker pull xwiki@sha256:481fdb46e8c043a6709d11310e2083ce71d6ba63ee6517f84da3ba06f320598e
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **590.5 MB (590459982 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:bd630aa0aa5c679e23ea7d52cbbdd6b817eab27a820c25d3c50b54eca83b9744`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["xwiki"]`

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
# Wed, 02 Nov 2022 18:44:10 GMT
RUN apt-get update     && DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends tzdata curl wget ca-certificates fontconfig locales     && echo "en_US.UTF-8 UTF-8" >> /etc/locale.gen     && locale-gen en_US.UTF-8     && rm -rf /var/lib/apt/lists/*
# Fri, 04 Nov 2022 23:21:41 GMT
ENV JAVA_VERSION=jdk-11.0.17+8
# Fri, 04 Nov 2022 23:22:31 GMT
RUN set -eux;     ARCH="$(dpkg --print-architecture)";     case "${ARCH}" in        aarch64|arm64)          ESUM='bd6efe3290c8b5a42f695a55a26f3e3c9c284288574879d4b7089f31f5114177';          BINARY_URL='https://github.com/adoptium/temurin11-binaries/releases/download/jdk-11.0.17%2B8/OpenJDK11U-jre_aarch64_linux_hotspot_11.0.17_8.tar.gz';          ;;        armhf|arm)          ESUM='8cf113d3d7fa808895c8d2e41bb890af21c47e38c2460e0588147a4bb8fc658d';          BINARY_URL='https://github.com/adoptium/temurin11-binaries/releases/download/jdk-11.0.17%2B8/OpenJDK11U-jre_arm_linux_hotspot_11.0.17_8.tar.gz';          ;;        ppc64el|powerpc:common64)          ESUM='0ca3d806131ab5834c501f9c625bb0248cd528af361c704503348e9c9605bedf';          BINARY_URL='https://github.com/adoptium/temurin11-binaries/releases/download/jdk-11.0.17%2B8/OpenJDK11U-jre_ppc64le_linux_hotspot_11.0.17_8.tar.gz';          ;;        s390x|s390:64-bit)          ESUM='dd3b159a374086e65cb07c4ccb226c90f9c02ef929cba6f0b642171d7ed97fa4';          BINARY_URL='https://github.com/adoptium/temurin11-binaries/releases/download/jdk-11.0.17%2B8/OpenJDK11U-jre_s390x_linux_hotspot_11.0.17_8.tar.gz';          ;;        amd64|i386:x86-64)          ESUM='752616097e09d7f60a3ad8bd312f90eaf50ac72577e55df229fe6e8091148f79';          BINARY_URL='https://github.com/adoptium/temurin11-binaries/releases/download/jdk-11.0.17%2B8/OpenJDK11U-jre_x64_linux_hotspot_11.0.17_8.tar.gz';          ;;        *)          echo "Unsupported arch: ${ARCH}";          exit 1;          ;;     esac; 	  wget -O /tmp/openjdk.tar.gz ${BINARY_URL}; 	  echo "${ESUM} */tmp/openjdk.tar.gz" | sha256sum -c -; 	  mkdir -p "$JAVA_HOME"; 	  tar --extract 	      --file /tmp/openjdk.tar.gz 	      --directory "$JAVA_HOME" 	      --strip-components 1 	      --no-same-owner 	  ;     rm /tmp/openjdk.tar.gz;     find "$JAVA_HOME/lib" -name '*.so' -exec dirname '{}' ';' | sort -u > /etc/ld.so.conf.d/docker-openjdk.conf;     ldconfig;     java -Xshare:dump;
# Fri, 04 Nov 2022 23:22:32 GMT
RUN echo Verifying install ...     && fileEncoding="$(echo 'System.out.println(System.getProperty("file.encoding"))' | jshell -s -)"; [ "$fileEncoding" = 'UTF-8' ]; rm -rf ~/.java     && echo java --version && java --version     && echo Complete.
# Sat, 05 Nov 2022 01:35:16 GMT
ENV CATALINA_HOME=/usr/local/tomcat
# Sat, 05 Nov 2022 01:35:16 GMT
ENV PATH=/usr/local/tomcat/bin:/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Sat, 05 Nov 2022 01:35:17 GMT
RUN mkdir -p "$CATALINA_HOME"
# Sat, 05 Nov 2022 01:35:17 GMT
WORKDIR /usr/local/tomcat
# Sat, 05 Nov 2022 01:35:17 GMT
ENV TOMCAT_NATIVE_LIBDIR=/usr/local/tomcat/native-jni-lib
# Sat, 05 Nov 2022 01:35:17 GMT
ENV LD_LIBRARY_PATH=/usr/local/tomcat/native-jni-lib
# Sat, 05 Nov 2022 01:39:54 GMT
ENV GPG_KEYS=48F8E69F6390C9F25CFEDCD268248959359E722B A9C5DF4D22E99998D9875A5110C01C5A2F6059E7 DCFD35E0BF8CA7344752DE8B6FB21E8933C60243
# Sat, 05 Nov 2022 01:39:54 GMT
ENV TOMCAT_MAJOR=9
# Tue, 15 Nov 2022 03:06:43 GMT
ENV TOMCAT_VERSION=9.0.69
# Tue, 15 Nov 2022 03:06:43 GMT
ENV TOMCAT_SHA512=8c883c54ce9ce43eba37756a6404cdf3477879883a3e6d146dc8a7aa5e0425f487466afe6b6da4a895927cb7cb59177b9379cec18000f2de12785be57408c779
# Tue, 15 Nov 2022 03:06:44 GMT
COPY dir:b1a33aa3993dbbfbebb33bd9aa546b60c2f2191abf1227f453d4e830f6deb35f in /usr/local/tomcat 
# Tue, 15 Nov 2022 03:06:48 GMT
RUN set -eux; 	apt-get update; 	xargs -rt apt-get install -y --no-install-recommends < "$TOMCAT_NATIVE_LIBDIR/.dependencies.txt"; 	rm -rf /var/lib/apt/lists/*
# Tue, 15 Nov 2022 03:06:49 GMT
RUN set -eux; 	nativeLines="$(catalina.sh configtest 2>&1)"; 	nativeLines="$(echo "$nativeLines" | grep 'Apache Tomcat Native')"; 	nativeLines="$(echo "$nativeLines" | sort -u)"; 	if ! echo "$nativeLines" | grep -E 'INFO: Loaded( APR based)? Apache Tomcat Native library' >&2; then 		echo >&2 "$nativeLines"; 		exit 1; 	fi
# Tue, 15 Nov 2022 03:06:49 GMT
EXPOSE 8080
# Tue, 15 Nov 2022 03:06:49 GMT
CMD ["catalina.sh" "run"]
# Wed, 11 Jan 2023 02:47:03 GMT
LABEL org.opencontainers.image.authors=XWiki Development Team <committers@xwiki.org>
# Wed, 11 Jan 2023 02:47:03 GMT
LABEL org.opencontainers.image.url=https://hub.docker.com/_/xwiki
# Wed, 11 Jan 2023 02:47:03 GMT
LABEL org.opencontainers.image.documentation=https://hub.docker.com/_/xwiki
# Wed, 11 Jan 2023 02:47:03 GMT
LABEL org.opencontainers.image.source=https://github.com/xwiki/xwiki-docker.git
# Wed, 11 Jan 2023 02:47:04 GMT
LABEL org.opencontainers.image.vendor=xwiki.org
# Wed, 11 Jan 2023 02:47:04 GMT
LABEL org.opencontainers.image.licenses=LGPL-2.1
# Wed, 11 Jan 2023 02:49:03 GMT
RUN apt-get update &&   apt-get --no-install-recommends -y install     curl     libreoffice     unzip     procps &&   rm -rf /var/lib/apt/lists/*
# Tue, 31 Jan 2023 00:20:17 GMT
ENV XWIKI_VERSION=15.0
# Tue, 31 Jan 2023 00:20:17 GMT
ENV XWIKI_URL_PREFIX=https://maven.xwiki.org/releases/org/xwiki/platform/xwiki-platform-distribution-war/15.0
# Tue, 31 Jan 2023 00:20:17 GMT
ENV XWIKI_DOWNLOAD_SHA256=79ba0f479bbc49521c113821adc9d91141075a9470d7f9bbb6994ca59c30d121
# Tue, 31 Jan 2023 00:21:18 GMT
RUN rm -rf /usr/local/tomcat/webapps/* &&   mkdir -p /usr/local/tomcat/temp &&   mkdir -p /usr/local/xwiki/data &&   curl -fSL "${XWIKI_URL_PREFIX}/xwiki-platform-distribution-war-${XWIKI_VERSION}.war" -o xwiki.war &&   echo "$XWIKI_DOWNLOAD_SHA256 xwiki.war" | sha256sum -c - &&   unzip -d /usr/local/tomcat/webapps/ROOT xwiki.war &&   rm -f xwiki.war
# Tue, 31 Jan 2023 00:21:19 GMT
ENV MYSQL_JDBC_VERSION=8.0.31
# Tue, 31 Jan 2023 00:21:19 GMT
ENV MYSQL_JDBC_SHA256=5249e3dc6d6531b37790e3f61845b96db5e41e891d3d8edb0e2e3a1b53ca2f4f
# Tue, 31 Jan 2023 00:21:19 GMT
ENV MYSQL_JDBC_PREFIX=https://repo1.maven.org/maven2/com/mysql/mysql-connector-j/8.0.31
# Tue, 31 Jan 2023 00:21:19 GMT
ENV MYSQL_JDBC_ARTIFACT=mysql-connector-j-8.0.31.jar
# Tue, 31 Jan 2023 00:21:19 GMT
ENV MYSQL_JDBC_TARGET=/usr/local/tomcat/webapps/ROOT/WEB-INF/lib/mysql-connector-j-8.0.31.jar
# Tue, 31 Jan 2023 00:21:20 GMT
RUN curl -fSL "${MYSQL_JDBC_PREFIX}/${MYSQL_JDBC_ARTIFACT}" -o $MYSQL_JDBC_TARGET &&   echo "$MYSQL_JDBC_SHA256 $MYSQL_JDBC_TARGET" | sha256sum -c -
# Tue, 31 Jan 2023 00:21:21 GMT
COPY file:0a1be11e2eb610a1dbcd415404e3a592641110b93090030cb831e3a19a163017 in /usr/local/tomcat/bin/ 
# Tue, 31 Jan 2023 00:21:21 GMT
COPY file:1b8409986f3e4eb79a7a0b18472cb2692a61d504fb5ef34292bc997b79fd760d in /usr/local/tomcat/webapps/ROOT/WEB-INF/hibernate.cfg.xml 
# Tue, 31 Jan 2023 00:21:21 GMT
RUN sed -i 's/<id>org.xwiki.platform:xwiki-platform-distribution-war/<id>org.xwiki.platform:xwiki-platform-distribution-docker/'   /usr/local/tomcat/webapps/ROOT/META-INF/extension.xed
# Tue, 31 Jan 2023 00:21:21 GMT
COPY file:a47c4dcd87c9dad97aff38c49188357e6193bcad50757e516cfb08a60d4de611 in /usr/local/bin/docker-entrypoint.sh 
# Tue, 31 Jan 2023 00:21:22 GMT
VOLUME [/usr/local/xwiki]
# Tue, 31 Jan 2023 00:21:22 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 31 Jan 2023 00:21:22 GMT
CMD ["xwiki"]
```

-	Layers:
	-	`sha256:e96e057aae67380a4ddb16c337c5c3669d97fdff69ec537f02aa2cc30d814281`  
		Last Modified: Wed, 02 Nov 2022 03:03:36 GMT  
		Size: 30.4 MB (30425607 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4ced2591451da3a02e2b6bb44752b9e3f00d77789921be4df5082fb9f9880ad0`  
		Last Modified: Wed, 02 Nov 2022 18:48:43 GMT  
		Size: 12.4 MB (12439006 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:df8f874ae8c08a9e69e5fbe6c5a64200a45386132a3203d1a9a7f1146d94cfbc`  
		Last Modified: Fri, 04 Nov 2022 23:29:33 GMT  
		Size: 46.6 MB (46629936 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:111b6c7486426c4b6989102c2ee5be856e8a58e20ab0a350b24a905d536e8e7f`  
		Last Modified: Fri, 04 Nov 2022 23:29:26 GMT  
		Size: 161.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e6f84dce457c6d4f7b7291fce05f8e77998a3a7722a54125a1f1d52ca83043b4`  
		Last Modified: Sat, 05 Nov 2022 01:50:51 GMT  
		Size: 173.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a6c26749ee782392e38845ee2ba79b0da586ef6a45d8e7f29c7af14612278547`  
		Last Modified: Tue, 15 Nov 2022 03:19:57 GMT  
		Size: 12.2 MB (12200249 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4dddc6d9fa6024025b3fcfe729cab2dc544fb25476eca6e80b1af8e8d93bb0ee`  
		Last Modified: Tue, 15 Nov 2022 03:19:56 GMT  
		Size: 452.7 KB (452680 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:06637eebe5e72c8ad9019ad4eb4cdde1f11f7d4c24c7ed7374cf8966343aa2fb`  
		Last Modified: Tue, 15 Nov 2022 03:19:56 GMT  
		Size: 131.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b276fb8390410a8208724033e325715ea26000d5a1a762d4c3699b927884fbfe`  
		Last Modified: Wed, 11 Jan 2023 02:52:45 GMT  
		Size: 178.8 MB (178805608 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:156ca91198173149698aa0396648a9608b6ab1f2bc2666800843ce33c9f85b6e`  
		Last Modified: Tue, 31 Jan 2023 00:24:09 GMT  
		Size: 307.1 MB (307117069 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4c8b70d250c6d507901857473b0dcb67132d7b2a30ce9a69b07b1036853df738`  
		Last Modified: Tue, 31 Jan 2023 00:23:52 GMT  
		Size: 2.4 MB (2377191 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a9681fd36be674d25231c69d6a39f9e8fa65034eeaef5d1bd885fdbeac7f0f6b`  
		Last Modified: Tue, 31 Jan 2023 00:23:51 GMT  
		Size: 1.3 KB (1346 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a9d0d5da840f4d7da9943942b38cd092fae11f41dc6c19afd58d655cd6192d66`  
		Last Modified: Tue, 31 Jan 2023 00:23:51 GMT  
		Size: 2.3 KB (2312 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d65610da4f1da86fea8fbec0189b066afd4b86e4e8f7d049e3c4bc6ade9ba90a`  
		Last Modified: Tue, 31 Jan 2023 00:23:51 GMT  
		Size: 6.0 KB (6009 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3d41686284d7675eaa0f92c9cc27ebe73b4c30768c8eef9f23ee3b1ad06da00a`  
		Last Modified: Tue, 31 Jan 2023 00:23:51 GMT  
		Size: 2.5 KB (2504 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `xwiki:15-mysql-tomcat` - linux; arm64 variant v8

```console
$ docker pull xwiki@sha256:6bf63d9025b07b69d744200c05efd4ffb8a52f3c38380f5d59a0b48514203cd2
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **581.7 MB (581709921 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:6600f2bb05836c703d53944bbcb5399d509a9813a27a35e99ff717becc308330`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["xwiki"]`

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
# Wed, 02 Nov 2022 19:44:32 GMT
RUN apt-get update     && DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends tzdata curl wget ca-certificates fontconfig locales     && echo "en_US.UTF-8 UTF-8" >> /etc/locale.gen     && locale-gen en_US.UTF-8     && rm -rf /var/lib/apt/lists/*
# Fri, 04 Nov 2022 22:40:54 GMT
ENV JAVA_VERSION=jdk-11.0.17+8
# Fri, 04 Nov 2022 22:41:33 GMT
RUN set -eux;     ARCH="$(dpkg --print-architecture)";     case "${ARCH}" in        aarch64|arm64)          ESUM='bd6efe3290c8b5a42f695a55a26f3e3c9c284288574879d4b7089f31f5114177';          BINARY_URL='https://github.com/adoptium/temurin11-binaries/releases/download/jdk-11.0.17%2B8/OpenJDK11U-jre_aarch64_linux_hotspot_11.0.17_8.tar.gz';          ;;        armhf|arm)          ESUM='8cf113d3d7fa808895c8d2e41bb890af21c47e38c2460e0588147a4bb8fc658d';          BINARY_URL='https://github.com/adoptium/temurin11-binaries/releases/download/jdk-11.0.17%2B8/OpenJDK11U-jre_arm_linux_hotspot_11.0.17_8.tar.gz';          ;;        ppc64el|powerpc:common64)          ESUM='0ca3d806131ab5834c501f9c625bb0248cd528af361c704503348e9c9605bedf';          BINARY_URL='https://github.com/adoptium/temurin11-binaries/releases/download/jdk-11.0.17%2B8/OpenJDK11U-jre_ppc64le_linux_hotspot_11.0.17_8.tar.gz';          ;;        s390x|s390:64-bit)          ESUM='dd3b159a374086e65cb07c4ccb226c90f9c02ef929cba6f0b642171d7ed97fa4';          BINARY_URL='https://github.com/adoptium/temurin11-binaries/releases/download/jdk-11.0.17%2B8/OpenJDK11U-jre_s390x_linux_hotspot_11.0.17_8.tar.gz';          ;;        amd64|i386:x86-64)          ESUM='752616097e09d7f60a3ad8bd312f90eaf50ac72577e55df229fe6e8091148f79';          BINARY_URL='https://github.com/adoptium/temurin11-binaries/releases/download/jdk-11.0.17%2B8/OpenJDK11U-jre_x64_linux_hotspot_11.0.17_8.tar.gz';          ;;        *)          echo "Unsupported arch: ${ARCH}";          exit 1;          ;;     esac; 	  wget -O /tmp/openjdk.tar.gz ${BINARY_URL}; 	  echo "${ESUM} */tmp/openjdk.tar.gz" | sha256sum -c -; 	  mkdir -p "$JAVA_HOME"; 	  tar --extract 	      --file /tmp/openjdk.tar.gz 	      --directory "$JAVA_HOME" 	      --strip-components 1 	      --no-same-owner 	  ;     rm /tmp/openjdk.tar.gz;     find "$JAVA_HOME/lib" -name '*.so' -exec dirname '{}' ';' | sort -u > /etc/ld.so.conf.d/docker-openjdk.conf;     ldconfig;     java -Xshare:dump;
# Fri, 04 Nov 2022 22:41:34 GMT
RUN echo Verifying install ...     && fileEncoding="$(echo 'System.out.println(System.getProperty("file.encoding"))' | jshell -s -)"; [ "$fileEncoding" = 'UTF-8' ]; rm -rf ~/.java     && echo java --version && java --version     && echo Complete.
# Fri, 04 Nov 2022 23:48:38 GMT
ENV CATALINA_HOME=/usr/local/tomcat
# Fri, 04 Nov 2022 23:48:38 GMT
ENV PATH=/usr/local/tomcat/bin:/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Fri, 04 Nov 2022 23:48:38 GMT
RUN mkdir -p "$CATALINA_HOME"
# Fri, 04 Nov 2022 23:48:39 GMT
WORKDIR /usr/local/tomcat
# Fri, 04 Nov 2022 23:48:39 GMT
ENV TOMCAT_NATIVE_LIBDIR=/usr/local/tomcat/native-jni-lib
# Fri, 04 Nov 2022 23:48:39 GMT
ENV LD_LIBRARY_PATH=/usr/local/tomcat/native-jni-lib
# Fri, 04 Nov 2022 23:53:12 GMT
ENV GPG_KEYS=48F8E69F6390C9F25CFEDCD268248959359E722B A9C5DF4D22E99998D9875A5110C01C5A2F6059E7 DCFD35E0BF8CA7344752DE8B6FB21E8933C60243
# Fri, 04 Nov 2022 23:53:12 GMT
ENV TOMCAT_MAJOR=9
# Tue, 15 Nov 2022 04:57:22 GMT
ENV TOMCAT_VERSION=9.0.69
# Tue, 15 Nov 2022 04:57:22 GMT
ENV TOMCAT_SHA512=8c883c54ce9ce43eba37756a6404cdf3477879883a3e6d146dc8a7aa5e0425f487466afe6b6da4a895927cb7cb59177b9379cec18000f2de12785be57408c779
# Tue, 15 Nov 2022 04:57:22 GMT
COPY dir:096b403a5f78b17e6b4bff63128a9c93941b97f22470991610dd641633d977f1 in /usr/local/tomcat 
# Tue, 15 Nov 2022 04:57:25 GMT
RUN set -eux; 	apt-get update; 	xargs -rt apt-get install -y --no-install-recommends < "$TOMCAT_NATIVE_LIBDIR/.dependencies.txt"; 	rm -rf /var/lib/apt/lists/*
# Tue, 15 Nov 2022 04:57:26 GMT
RUN set -eux; 	nativeLines="$(catalina.sh configtest 2>&1)"; 	nativeLines="$(echo "$nativeLines" | grep 'Apache Tomcat Native')"; 	nativeLines="$(echo "$nativeLines" | sort -u)"; 	if ! echo "$nativeLines" | grep -E 'INFO: Loaded( APR based)? Apache Tomcat Native library' >&2; then 		echo >&2 "$nativeLines"; 		exit 1; 	fi
# Tue, 15 Nov 2022 04:57:26 GMT
EXPOSE 8080
# Tue, 15 Nov 2022 04:57:27 GMT
CMD ["catalina.sh" "run"]
# Wed, 11 Jan 2023 03:05:10 GMT
LABEL org.opencontainers.image.authors=XWiki Development Team <committers@xwiki.org>
# Wed, 11 Jan 2023 03:05:10 GMT
LABEL org.opencontainers.image.url=https://hub.docker.com/_/xwiki
# Wed, 11 Jan 2023 03:05:10 GMT
LABEL org.opencontainers.image.documentation=https://hub.docker.com/_/xwiki
# Wed, 11 Jan 2023 03:05:10 GMT
LABEL org.opencontainers.image.source=https://github.com/xwiki/xwiki-docker.git
# Wed, 11 Jan 2023 03:05:11 GMT
LABEL org.opencontainers.image.vendor=xwiki.org
# Wed, 11 Jan 2023 03:05:11 GMT
LABEL org.opencontainers.image.licenses=LGPL-2.1
# Wed, 11 Jan 2023 03:07:37 GMT
RUN apt-get update &&   apt-get --no-install-recommends -y install     curl     libreoffice     unzip     procps &&   rm -rf /var/lib/apt/lists/*
# Tue, 31 Jan 2023 00:47:12 GMT
ENV XWIKI_VERSION=15.0
# Tue, 31 Jan 2023 00:47:12 GMT
ENV XWIKI_URL_PREFIX=https://maven.xwiki.org/releases/org/xwiki/platform/xwiki-platform-distribution-war/15.0
# Tue, 31 Jan 2023 00:47:12 GMT
ENV XWIKI_DOWNLOAD_SHA256=79ba0f479bbc49521c113821adc9d91141075a9470d7f9bbb6994ca59c30d121
# Tue, 31 Jan 2023 00:47:58 GMT
RUN rm -rf /usr/local/tomcat/webapps/* &&   mkdir -p /usr/local/tomcat/temp &&   mkdir -p /usr/local/xwiki/data &&   curl -fSL "${XWIKI_URL_PREFIX}/xwiki-platform-distribution-war-${XWIKI_VERSION}.war" -o xwiki.war &&   echo "$XWIKI_DOWNLOAD_SHA256 xwiki.war" | sha256sum -c - &&   unzip -d /usr/local/tomcat/webapps/ROOT xwiki.war &&   rm -f xwiki.war
# Tue, 31 Jan 2023 00:48:01 GMT
ENV MYSQL_JDBC_VERSION=8.0.31
# Tue, 31 Jan 2023 00:48:01 GMT
ENV MYSQL_JDBC_SHA256=5249e3dc6d6531b37790e3f61845b96db5e41e891d3d8edb0e2e3a1b53ca2f4f
# Tue, 31 Jan 2023 00:48:01 GMT
ENV MYSQL_JDBC_PREFIX=https://repo1.maven.org/maven2/com/mysql/mysql-connector-j/8.0.31
# Tue, 31 Jan 2023 00:48:01 GMT
ENV MYSQL_JDBC_ARTIFACT=mysql-connector-j-8.0.31.jar
# Tue, 31 Jan 2023 00:48:01 GMT
ENV MYSQL_JDBC_TARGET=/usr/local/tomcat/webapps/ROOT/WEB-INF/lib/mysql-connector-j-8.0.31.jar
# Tue, 31 Jan 2023 00:48:02 GMT
RUN curl -fSL "${MYSQL_JDBC_PREFIX}/${MYSQL_JDBC_ARTIFACT}" -o $MYSQL_JDBC_TARGET &&   echo "$MYSQL_JDBC_SHA256 $MYSQL_JDBC_TARGET" | sha256sum -c -
# Tue, 31 Jan 2023 00:48:02 GMT
COPY file:0a1be11e2eb610a1dbcd415404e3a592641110b93090030cb831e3a19a163017 in /usr/local/tomcat/bin/ 
# Tue, 31 Jan 2023 00:48:02 GMT
COPY file:1b8409986f3e4eb79a7a0b18472cb2692a61d504fb5ef34292bc997b79fd760d in /usr/local/tomcat/webapps/ROOT/WEB-INF/hibernate.cfg.xml 
# Tue, 31 Jan 2023 00:48:03 GMT
RUN sed -i 's/<id>org.xwiki.platform:xwiki-platform-distribution-war/<id>org.xwiki.platform:xwiki-platform-distribution-docker/'   /usr/local/tomcat/webapps/ROOT/META-INF/extension.xed
# Tue, 31 Jan 2023 00:48:03 GMT
COPY file:a47c4dcd87c9dad97aff38c49188357e6193bcad50757e516cfb08a60d4de611 in /usr/local/bin/docker-entrypoint.sh 
# Tue, 31 Jan 2023 00:48:03 GMT
VOLUME [/usr/local/xwiki]
# Tue, 31 Jan 2023 00:48:03 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 31 Jan 2023 00:48:03 GMT
CMD ["xwiki"]
```

-	Layers:
	-	`sha256:0509fae36eb0656f8bdb23f8ae64100d893bcea2563e97468d337e04d2d0410b`  
		Last Modified: Wed, 02 Nov 2022 18:50:21 GMT  
		Size: 28.4 MB (28382154 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e502a1af2bcd98f5f0d2f5e4da1a0e7bbe07a2c548e2662f7d37dce5ae1df46c`  
		Last Modified: Wed, 02 Nov 2022 19:48:28 GMT  
		Size: 12.4 MB (12396330 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bc4598c07dd818f03a0378b0341a4a8e80f0152fbb3e7d5246ca4f466f42e611`  
		Last Modified: Fri, 04 Nov 2022 22:46:46 GMT  
		Size: 45.0 MB (44958470 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:715a937a1066f998b331fcd62256ad01a5571bdf46804e97825afc64f9ebb427`  
		Last Modified: Fri, 04 Nov 2022 22:46:41 GMT  
		Size: 160.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5fb623f082f74b2fa9fc2c4e3f3a4802875cb9753cfa26ed940201ce72bb56cb`  
		Last Modified: Sat, 05 Nov 2022 00:03:40 GMT  
		Size: 172.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:33260b83200262bbd546be371ad3c1f50f5ae7228afb87982d6fa9d6b11bf26f`  
		Last Modified: Tue, 15 Nov 2022 05:10:19 GMT  
		Size: 12.2 MB (12207235 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0955fb697ea9b30a1b4f95385464f646aa1525cb6efba648e22df84ebef6b2ee`  
		Last Modified: Tue, 15 Nov 2022 05:10:18 GMT  
		Size: 452.0 KB (452021 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6eddcf66f2083b1487296a0308e0b058917c97f614f12428d82d89662038dc2e`  
		Last Modified: Tue, 15 Nov 2022 05:10:18 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ae5f60bb64f3fa11da3d15a9639f886186b4c2c021455c3f9db22e0cfe1b1311`  
		Last Modified: Wed, 11 Jan 2023 03:11:14 GMT  
		Size: 173.8 MB (173806827 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1814d85fce571b42f2cfa7c8a904e1a184ee6f49642242a44bbe0037088994a0`  
		Last Modified: Tue, 31 Jan 2023 00:56:04 GMT  
		Size: 307.1 MB (307117070 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8aec0e24b4fa870989f014944c3c7d535355a2371fc8c948b2b11f9b377efe6e`  
		Last Modified: Tue, 31 Jan 2023 00:55:50 GMT  
		Size: 2.4 MB (2377182 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0b65081619aa0114a7f367836ef421eb8d951e559e0f089c7728af7813b1ea62`  
		Last Modified: Tue, 31 Jan 2023 00:55:49 GMT  
		Size: 1.3 KB (1348 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:46ebad072e608146426d8dc30828937049eea36c2e636d7790b4960d6d586977`  
		Last Modified: Tue, 31 Jan 2023 00:55:49 GMT  
		Size: 2.3 KB (2308 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:708fefcedd4ee6c106da247a68c5790f5ab00225d1cdfff8465575265c3a54e6`  
		Last Modified: Tue, 31 Jan 2023 00:55:49 GMT  
		Size: 6.0 KB (6008 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:81e3bf8e20bc921031e7549a41dec1b2d7795cc6da40a0e7096bf654b25c5c3e`  
		Last Modified: Tue, 31 Jan 2023 00:55:49 GMT  
		Size: 2.5 KB (2507 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `xwiki:15-postgres-tomcat`

```console
$ docker pull xwiki@sha256:f6739c1133cbbece87973ddea5fbc57222abb9d7d3f8064eee9d2c2c0d46ecfa
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `xwiki:15-postgres-tomcat` - linux; amd64

```console
$ docker pull xwiki@sha256:72928baeace929e42f17f01362700392a90c6750b2ec1f84f24bbba1c4ff0236
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **590.0 MB (589959353 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b71f03d7d3a1760e73e6f4370f49317d16a7e0cb22532f49c11c0ee73b2c6262`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["xwiki"]`

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
# Wed, 02 Nov 2022 18:44:10 GMT
RUN apt-get update     && DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends tzdata curl wget ca-certificates fontconfig locales     && echo "en_US.UTF-8 UTF-8" >> /etc/locale.gen     && locale-gen en_US.UTF-8     && rm -rf /var/lib/apt/lists/*
# Fri, 04 Nov 2022 23:21:41 GMT
ENV JAVA_VERSION=jdk-11.0.17+8
# Fri, 04 Nov 2022 23:22:31 GMT
RUN set -eux;     ARCH="$(dpkg --print-architecture)";     case "${ARCH}" in        aarch64|arm64)          ESUM='bd6efe3290c8b5a42f695a55a26f3e3c9c284288574879d4b7089f31f5114177';          BINARY_URL='https://github.com/adoptium/temurin11-binaries/releases/download/jdk-11.0.17%2B8/OpenJDK11U-jre_aarch64_linux_hotspot_11.0.17_8.tar.gz';          ;;        armhf|arm)          ESUM='8cf113d3d7fa808895c8d2e41bb890af21c47e38c2460e0588147a4bb8fc658d';          BINARY_URL='https://github.com/adoptium/temurin11-binaries/releases/download/jdk-11.0.17%2B8/OpenJDK11U-jre_arm_linux_hotspot_11.0.17_8.tar.gz';          ;;        ppc64el|powerpc:common64)          ESUM='0ca3d806131ab5834c501f9c625bb0248cd528af361c704503348e9c9605bedf';          BINARY_URL='https://github.com/adoptium/temurin11-binaries/releases/download/jdk-11.0.17%2B8/OpenJDK11U-jre_ppc64le_linux_hotspot_11.0.17_8.tar.gz';          ;;        s390x|s390:64-bit)          ESUM='dd3b159a374086e65cb07c4ccb226c90f9c02ef929cba6f0b642171d7ed97fa4';          BINARY_URL='https://github.com/adoptium/temurin11-binaries/releases/download/jdk-11.0.17%2B8/OpenJDK11U-jre_s390x_linux_hotspot_11.0.17_8.tar.gz';          ;;        amd64|i386:x86-64)          ESUM='752616097e09d7f60a3ad8bd312f90eaf50ac72577e55df229fe6e8091148f79';          BINARY_URL='https://github.com/adoptium/temurin11-binaries/releases/download/jdk-11.0.17%2B8/OpenJDK11U-jre_x64_linux_hotspot_11.0.17_8.tar.gz';          ;;        *)          echo "Unsupported arch: ${ARCH}";          exit 1;          ;;     esac; 	  wget -O /tmp/openjdk.tar.gz ${BINARY_URL}; 	  echo "${ESUM} */tmp/openjdk.tar.gz" | sha256sum -c -; 	  mkdir -p "$JAVA_HOME"; 	  tar --extract 	      --file /tmp/openjdk.tar.gz 	      --directory "$JAVA_HOME" 	      --strip-components 1 	      --no-same-owner 	  ;     rm /tmp/openjdk.tar.gz;     find "$JAVA_HOME/lib" -name '*.so' -exec dirname '{}' ';' | sort -u > /etc/ld.so.conf.d/docker-openjdk.conf;     ldconfig;     java -Xshare:dump;
# Fri, 04 Nov 2022 23:22:32 GMT
RUN echo Verifying install ...     && fileEncoding="$(echo 'System.out.println(System.getProperty("file.encoding"))' | jshell -s -)"; [ "$fileEncoding" = 'UTF-8' ]; rm -rf ~/.java     && echo java --version && java --version     && echo Complete.
# Sat, 05 Nov 2022 01:35:16 GMT
ENV CATALINA_HOME=/usr/local/tomcat
# Sat, 05 Nov 2022 01:35:16 GMT
ENV PATH=/usr/local/tomcat/bin:/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Sat, 05 Nov 2022 01:35:17 GMT
RUN mkdir -p "$CATALINA_HOME"
# Sat, 05 Nov 2022 01:35:17 GMT
WORKDIR /usr/local/tomcat
# Sat, 05 Nov 2022 01:35:17 GMT
ENV TOMCAT_NATIVE_LIBDIR=/usr/local/tomcat/native-jni-lib
# Sat, 05 Nov 2022 01:35:17 GMT
ENV LD_LIBRARY_PATH=/usr/local/tomcat/native-jni-lib
# Sat, 05 Nov 2022 01:39:54 GMT
ENV GPG_KEYS=48F8E69F6390C9F25CFEDCD268248959359E722B A9C5DF4D22E99998D9875A5110C01C5A2F6059E7 DCFD35E0BF8CA7344752DE8B6FB21E8933C60243
# Sat, 05 Nov 2022 01:39:54 GMT
ENV TOMCAT_MAJOR=9
# Tue, 15 Nov 2022 03:06:43 GMT
ENV TOMCAT_VERSION=9.0.69
# Tue, 15 Nov 2022 03:06:43 GMT
ENV TOMCAT_SHA512=8c883c54ce9ce43eba37756a6404cdf3477879883a3e6d146dc8a7aa5e0425f487466afe6b6da4a895927cb7cb59177b9379cec18000f2de12785be57408c779
# Tue, 15 Nov 2022 03:06:44 GMT
COPY dir:b1a33aa3993dbbfbebb33bd9aa546b60c2f2191abf1227f453d4e830f6deb35f in /usr/local/tomcat 
# Tue, 15 Nov 2022 03:06:48 GMT
RUN set -eux; 	apt-get update; 	xargs -rt apt-get install -y --no-install-recommends < "$TOMCAT_NATIVE_LIBDIR/.dependencies.txt"; 	rm -rf /var/lib/apt/lists/*
# Tue, 15 Nov 2022 03:06:49 GMT
RUN set -eux; 	nativeLines="$(catalina.sh configtest 2>&1)"; 	nativeLines="$(echo "$nativeLines" | grep 'Apache Tomcat Native')"; 	nativeLines="$(echo "$nativeLines" | sort -u)"; 	if ! echo "$nativeLines" | grep -E 'INFO: Loaded( APR based)? Apache Tomcat Native library' >&2; then 		echo >&2 "$nativeLines"; 		exit 1; 	fi
# Tue, 15 Nov 2022 03:06:49 GMT
EXPOSE 8080
# Tue, 15 Nov 2022 03:06:49 GMT
CMD ["catalina.sh" "run"]
# Wed, 11 Jan 2023 02:47:03 GMT
LABEL org.opencontainers.image.authors=XWiki Development Team <committers@xwiki.org>
# Wed, 11 Jan 2023 02:47:03 GMT
LABEL org.opencontainers.image.url=https://hub.docker.com/_/xwiki
# Wed, 11 Jan 2023 02:47:03 GMT
LABEL org.opencontainers.image.documentation=https://hub.docker.com/_/xwiki
# Wed, 11 Jan 2023 02:47:03 GMT
LABEL org.opencontainers.image.source=https://github.com/xwiki/xwiki-docker.git
# Wed, 11 Jan 2023 02:47:04 GMT
LABEL org.opencontainers.image.vendor=xwiki.org
# Wed, 11 Jan 2023 02:47:04 GMT
LABEL org.opencontainers.image.licenses=LGPL-2.1
# Wed, 11 Jan 2023 02:50:25 GMT
RUN apt-get update &&   apt-get --no-install-recommends -y install     curl     libreoffice     unzip     procps     libpostgresql-jdbc-java &&   rm -rf /var/lib/apt/lists/*
# Tue, 31 Jan 2023 00:21:26 GMT
ENV XWIKI_VERSION=15.0
# Tue, 31 Jan 2023 00:21:27 GMT
ENV XWIKI_URL_PREFIX=https://maven.xwiki.org/releases/org/xwiki/platform/xwiki-platform-distribution-war/15.0
# Tue, 31 Jan 2023 00:21:27 GMT
ENV XWIKI_DOWNLOAD_SHA256=79ba0f479bbc49521c113821adc9d91141075a9470d7f9bbb6994ca59c30d121
# Tue, 31 Jan 2023 00:22:39 GMT
RUN rm -rf /usr/local/tomcat/webapps/* &&   mkdir -p /usr/local/tomcat/temp &&   mkdir -p /usr/local/xwiki/data &&   curl -fSL "${XWIKI_URL_PREFIX}/xwiki-platform-distribution-war-${XWIKI_VERSION}.war" -o xwiki.war &&   echo "$XWIKI_DOWNLOAD_SHA256 xwiki.war" | sha256sum -c - &&   unzip -d /usr/local/tomcat/webapps/ROOT xwiki.war &&   rm -f xwiki.war
# Tue, 31 Jan 2023 00:22:40 GMT
RUN cp /usr/share/java/postgresql-jdbc4.jar /usr/local/tomcat/webapps/ROOT/WEB-INF/lib/
# Tue, 31 Jan 2023 00:22:41 GMT
COPY file:0a1be11e2eb610a1dbcd415404e3a592641110b93090030cb831e3a19a163017 in /usr/local/tomcat/bin/ 
# Tue, 31 Jan 2023 00:22:41 GMT
COPY file:4a923f484bb29a26630c19e1d617d3bf6aa6ae7c6c4a5561e97b037bcde0847c in /usr/local/tomcat/webapps/ROOT/WEB-INF/hibernate.cfg.xml 
# Tue, 31 Jan 2023 00:22:41 GMT
RUN sed -i 's/<id>org.xwiki.platform:xwiki-platform-distribution-war/<id>org.xwiki.platform:xwiki-platform-distribution-docker/'   /usr/local/tomcat/webapps/ROOT/META-INF/extension.xed
# Tue, 31 Jan 2023 00:22:41 GMT
COPY file:a47c4dcd87c9dad97aff38c49188357e6193bcad50757e516cfb08a60d4de611 in /usr/local/bin/docker-entrypoint.sh 
# Tue, 31 Jan 2023 00:22:41 GMT
VOLUME [/usr/local/xwiki]
# Tue, 31 Jan 2023 00:22:42 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 31 Jan 2023 00:22:42 GMT
CMD ["xwiki"]
```

-	Layers:
	-	`sha256:e96e057aae67380a4ddb16c337c5c3669d97fdff69ec537f02aa2cc30d814281`  
		Last Modified: Wed, 02 Nov 2022 03:03:36 GMT  
		Size: 30.4 MB (30425607 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4ced2591451da3a02e2b6bb44752b9e3f00d77789921be4df5082fb9f9880ad0`  
		Last Modified: Wed, 02 Nov 2022 18:48:43 GMT  
		Size: 12.4 MB (12439006 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:df8f874ae8c08a9e69e5fbe6c5a64200a45386132a3203d1a9a7f1146d94cfbc`  
		Last Modified: Fri, 04 Nov 2022 23:29:33 GMT  
		Size: 46.6 MB (46629936 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:111b6c7486426c4b6989102c2ee5be856e8a58e20ab0a350b24a905d536e8e7f`  
		Last Modified: Fri, 04 Nov 2022 23:29:26 GMT  
		Size: 161.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e6f84dce457c6d4f7b7291fce05f8e77998a3a7722a54125a1f1d52ca83043b4`  
		Last Modified: Sat, 05 Nov 2022 01:50:51 GMT  
		Size: 173.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a6c26749ee782392e38845ee2ba79b0da586ef6a45d8e7f29c7af14612278547`  
		Last Modified: Tue, 15 Nov 2022 03:19:57 GMT  
		Size: 12.2 MB (12200249 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4dddc6d9fa6024025b3fcfe729cab2dc544fb25476eca6e80b1af8e8d93bb0ee`  
		Last Modified: Tue, 15 Nov 2022 03:19:56 GMT  
		Size: 452.7 KB (452680 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:06637eebe5e72c8ad9019ad4eb4cdde1f11f7d4c24c7ed7374cf8966343aa2fb`  
		Last Modified: Tue, 15 Nov 2022 03:19:56 GMT  
		Size: 131.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b57f6f8bcfb0d93b8e21d3068d1f65d3f08dba05c5fab7d4c36e2359317b18c7`  
		Last Modified: Wed, 11 Jan 2023 02:53:53 GMT  
		Size: 179.7 MB (179745182 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:71a0aee972ff5a36a4c5d67f5bf6416b1b78d06c906ce727c5e8e11098d0dfd1`  
		Last Modified: Tue, 31 Jan 2023 00:25:01 GMT  
		Size: 307.1 MB (307117070 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ccc745f1273896cef68a5af6cd5713c4a2d8704628920a53e318a008f8096426`  
		Last Modified: Tue, 31 Jan 2023 00:24:44 GMT  
		Size: 936.8 KB (936848 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1593979548bc568ed36dc9f5adb8f00d8b7d3eb1fa850fc06426c2c9345b8472`  
		Last Modified: Tue, 31 Jan 2023 00:24:43 GMT  
		Size: 1.3 KB (1345 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e1e58b32c2c2a52907f7e4ad05462d3b2afd11404a9678bc656fb96029b12d8d`  
		Last Modified: Tue, 31 Jan 2023 00:24:43 GMT  
		Size: 2.5 KB (2454 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c43ce01c7b867ce6cda62f86175ba6a53f44000797d61fe604aded86980c4d41`  
		Last Modified: Tue, 31 Jan 2023 00:24:43 GMT  
		Size: 6.0 KB (6006 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6fe6f306aa61d9839a01e62f4c308a9a7d3bd4cd5ce9a58407b6585f6950f054`  
		Last Modified: Tue, 31 Jan 2023 00:24:43 GMT  
		Size: 2.5 KB (2505 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `xwiki:15-postgres-tomcat` - linux; arm64 variant v8

```console
$ docker pull xwiki@sha256:ae51c629c7a76aa7c15ebb33fcfdae3e529ef6456ada6d0dbcf9ed8fc5ecf00d
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **581.2 MB (581212250 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:70277ae3ffdca68401bb57e24e6302cc64a403bf36869f0959e54d03216b0005`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["xwiki"]`

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
# Wed, 02 Nov 2022 19:44:32 GMT
RUN apt-get update     && DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends tzdata curl wget ca-certificates fontconfig locales     && echo "en_US.UTF-8 UTF-8" >> /etc/locale.gen     && locale-gen en_US.UTF-8     && rm -rf /var/lib/apt/lists/*
# Fri, 04 Nov 2022 22:40:54 GMT
ENV JAVA_VERSION=jdk-11.0.17+8
# Fri, 04 Nov 2022 22:41:33 GMT
RUN set -eux;     ARCH="$(dpkg --print-architecture)";     case "${ARCH}" in        aarch64|arm64)          ESUM='bd6efe3290c8b5a42f695a55a26f3e3c9c284288574879d4b7089f31f5114177';          BINARY_URL='https://github.com/adoptium/temurin11-binaries/releases/download/jdk-11.0.17%2B8/OpenJDK11U-jre_aarch64_linux_hotspot_11.0.17_8.tar.gz';          ;;        armhf|arm)          ESUM='8cf113d3d7fa808895c8d2e41bb890af21c47e38c2460e0588147a4bb8fc658d';          BINARY_URL='https://github.com/adoptium/temurin11-binaries/releases/download/jdk-11.0.17%2B8/OpenJDK11U-jre_arm_linux_hotspot_11.0.17_8.tar.gz';          ;;        ppc64el|powerpc:common64)          ESUM='0ca3d806131ab5834c501f9c625bb0248cd528af361c704503348e9c9605bedf';          BINARY_URL='https://github.com/adoptium/temurin11-binaries/releases/download/jdk-11.0.17%2B8/OpenJDK11U-jre_ppc64le_linux_hotspot_11.0.17_8.tar.gz';          ;;        s390x|s390:64-bit)          ESUM='dd3b159a374086e65cb07c4ccb226c90f9c02ef929cba6f0b642171d7ed97fa4';          BINARY_URL='https://github.com/adoptium/temurin11-binaries/releases/download/jdk-11.0.17%2B8/OpenJDK11U-jre_s390x_linux_hotspot_11.0.17_8.tar.gz';          ;;        amd64|i386:x86-64)          ESUM='752616097e09d7f60a3ad8bd312f90eaf50ac72577e55df229fe6e8091148f79';          BINARY_URL='https://github.com/adoptium/temurin11-binaries/releases/download/jdk-11.0.17%2B8/OpenJDK11U-jre_x64_linux_hotspot_11.0.17_8.tar.gz';          ;;        *)          echo "Unsupported arch: ${ARCH}";          exit 1;          ;;     esac; 	  wget -O /tmp/openjdk.tar.gz ${BINARY_URL}; 	  echo "${ESUM} */tmp/openjdk.tar.gz" | sha256sum -c -; 	  mkdir -p "$JAVA_HOME"; 	  tar --extract 	      --file /tmp/openjdk.tar.gz 	      --directory "$JAVA_HOME" 	      --strip-components 1 	      --no-same-owner 	  ;     rm /tmp/openjdk.tar.gz;     find "$JAVA_HOME/lib" -name '*.so' -exec dirname '{}' ';' | sort -u > /etc/ld.so.conf.d/docker-openjdk.conf;     ldconfig;     java -Xshare:dump;
# Fri, 04 Nov 2022 22:41:34 GMT
RUN echo Verifying install ...     && fileEncoding="$(echo 'System.out.println(System.getProperty("file.encoding"))' | jshell -s -)"; [ "$fileEncoding" = 'UTF-8' ]; rm -rf ~/.java     && echo java --version && java --version     && echo Complete.
# Fri, 04 Nov 2022 23:48:38 GMT
ENV CATALINA_HOME=/usr/local/tomcat
# Fri, 04 Nov 2022 23:48:38 GMT
ENV PATH=/usr/local/tomcat/bin:/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Fri, 04 Nov 2022 23:48:38 GMT
RUN mkdir -p "$CATALINA_HOME"
# Fri, 04 Nov 2022 23:48:39 GMT
WORKDIR /usr/local/tomcat
# Fri, 04 Nov 2022 23:48:39 GMT
ENV TOMCAT_NATIVE_LIBDIR=/usr/local/tomcat/native-jni-lib
# Fri, 04 Nov 2022 23:48:39 GMT
ENV LD_LIBRARY_PATH=/usr/local/tomcat/native-jni-lib
# Fri, 04 Nov 2022 23:53:12 GMT
ENV GPG_KEYS=48F8E69F6390C9F25CFEDCD268248959359E722B A9C5DF4D22E99998D9875A5110C01C5A2F6059E7 DCFD35E0BF8CA7344752DE8B6FB21E8933C60243
# Fri, 04 Nov 2022 23:53:12 GMT
ENV TOMCAT_MAJOR=9
# Tue, 15 Nov 2022 04:57:22 GMT
ENV TOMCAT_VERSION=9.0.69
# Tue, 15 Nov 2022 04:57:22 GMT
ENV TOMCAT_SHA512=8c883c54ce9ce43eba37756a6404cdf3477879883a3e6d146dc8a7aa5e0425f487466afe6b6da4a895927cb7cb59177b9379cec18000f2de12785be57408c779
# Tue, 15 Nov 2022 04:57:22 GMT
COPY dir:096b403a5f78b17e6b4bff63128a9c93941b97f22470991610dd641633d977f1 in /usr/local/tomcat 
# Tue, 15 Nov 2022 04:57:25 GMT
RUN set -eux; 	apt-get update; 	xargs -rt apt-get install -y --no-install-recommends < "$TOMCAT_NATIVE_LIBDIR/.dependencies.txt"; 	rm -rf /var/lib/apt/lists/*
# Tue, 15 Nov 2022 04:57:26 GMT
RUN set -eux; 	nativeLines="$(catalina.sh configtest 2>&1)"; 	nativeLines="$(echo "$nativeLines" | grep 'Apache Tomcat Native')"; 	nativeLines="$(echo "$nativeLines" | sort -u)"; 	if ! echo "$nativeLines" | grep -E 'INFO: Loaded( APR based)? Apache Tomcat Native library' >&2; then 		echo >&2 "$nativeLines"; 		exit 1; 	fi
# Tue, 15 Nov 2022 04:57:26 GMT
EXPOSE 8080
# Tue, 15 Nov 2022 04:57:27 GMT
CMD ["catalina.sh" "run"]
# Wed, 11 Jan 2023 03:05:10 GMT
LABEL org.opencontainers.image.authors=XWiki Development Team <committers@xwiki.org>
# Wed, 11 Jan 2023 03:05:10 GMT
LABEL org.opencontainers.image.url=https://hub.docker.com/_/xwiki
# Wed, 11 Jan 2023 03:05:10 GMT
LABEL org.opencontainers.image.documentation=https://hub.docker.com/_/xwiki
# Wed, 11 Jan 2023 03:05:10 GMT
LABEL org.opencontainers.image.source=https://github.com/xwiki/xwiki-docker.git
# Wed, 11 Jan 2023 03:05:11 GMT
LABEL org.opencontainers.image.vendor=xwiki.org
# Wed, 11 Jan 2023 03:05:11 GMT
LABEL org.opencontainers.image.licenses=LGPL-2.1
# Wed, 11 Jan 2023 03:08:55 GMT
RUN apt-get update &&   apt-get --no-install-recommends -y install     curl     libreoffice     unzip     procps     libpostgresql-jdbc-java &&   rm -rf /var/lib/apt/lists/*
# Tue, 31 Jan 2023 00:48:10 GMT
ENV XWIKI_VERSION=15.0
# Tue, 31 Jan 2023 00:48:10 GMT
ENV XWIKI_URL_PREFIX=https://maven.xwiki.org/releases/org/xwiki/platform/xwiki-platform-distribution-war/15.0
# Tue, 31 Jan 2023 00:48:10 GMT
ENV XWIKI_DOWNLOAD_SHA256=79ba0f479bbc49521c113821adc9d91141075a9470d7f9bbb6994ca59c30d121
# Tue, 31 Jan 2023 00:54:38 GMT
RUN rm -rf /usr/local/tomcat/webapps/* &&   mkdir -p /usr/local/tomcat/temp &&   mkdir -p /usr/local/xwiki/data &&   curl -fSL "${XWIKI_URL_PREFIX}/xwiki-platform-distribution-war-${XWIKI_VERSION}.war" -o xwiki.war &&   echo "$XWIKI_DOWNLOAD_SHA256 xwiki.war" | sha256sum -c - &&   unzip -d /usr/local/tomcat/webapps/ROOT xwiki.war &&   rm -f xwiki.war
# Tue, 31 Jan 2023 00:54:41 GMT
RUN cp /usr/share/java/postgresql-jdbc4.jar /usr/local/tomcat/webapps/ROOT/WEB-INF/lib/
# Tue, 31 Jan 2023 00:54:41 GMT
COPY file:0a1be11e2eb610a1dbcd415404e3a592641110b93090030cb831e3a19a163017 in /usr/local/tomcat/bin/ 
# Tue, 31 Jan 2023 00:54:41 GMT
COPY file:4a923f484bb29a26630c19e1d617d3bf6aa6ae7c6c4a5561e97b037bcde0847c in /usr/local/tomcat/webapps/ROOT/WEB-INF/hibernate.cfg.xml 
# Tue, 31 Jan 2023 00:54:42 GMT
RUN sed -i 's/<id>org.xwiki.platform:xwiki-platform-distribution-war/<id>org.xwiki.platform:xwiki-platform-distribution-docker/'   /usr/local/tomcat/webapps/ROOT/META-INF/extension.xed
# Tue, 31 Jan 2023 00:54:42 GMT
COPY file:a47c4dcd87c9dad97aff38c49188357e6193bcad50757e516cfb08a60d4de611 in /usr/local/bin/docker-entrypoint.sh 
# Tue, 31 Jan 2023 00:54:42 GMT
VOLUME [/usr/local/xwiki]
# Tue, 31 Jan 2023 00:54:42 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 31 Jan 2023 00:54:42 GMT
CMD ["xwiki"]
```

-	Layers:
	-	`sha256:0509fae36eb0656f8bdb23f8ae64100d893bcea2563e97468d337e04d2d0410b`  
		Last Modified: Wed, 02 Nov 2022 18:50:21 GMT  
		Size: 28.4 MB (28382154 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e502a1af2bcd98f5f0d2f5e4da1a0e7bbe07a2c548e2662f7d37dce5ae1df46c`  
		Last Modified: Wed, 02 Nov 2022 19:48:28 GMT  
		Size: 12.4 MB (12396330 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bc4598c07dd818f03a0378b0341a4a8e80f0152fbb3e7d5246ca4f466f42e611`  
		Last Modified: Fri, 04 Nov 2022 22:46:46 GMT  
		Size: 45.0 MB (44958470 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:715a937a1066f998b331fcd62256ad01a5571bdf46804e97825afc64f9ebb427`  
		Last Modified: Fri, 04 Nov 2022 22:46:41 GMT  
		Size: 160.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5fb623f082f74b2fa9fc2c4e3f3a4802875cb9753cfa26ed940201ce72bb56cb`  
		Last Modified: Sat, 05 Nov 2022 00:03:40 GMT  
		Size: 172.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:33260b83200262bbd546be371ad3c1f50f5ae7228afb87982d6fa9d6b11bf26f`  
		Last Modified: Tue, 15 Nov 2022 05:10:19 GMT  
		Size: 12.2 MB (12207235 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0955fb697ea9b30a1b4f95385464f646aa1525cb6efba648e22df84ebef6b2ee`  
		Last Modified: Tue, 15 Nov 2022 05:10:18 GMT  
		Size: 452.0 KB (452021 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6eddcf66f2083b1487296a0308e0b058917c97f614f12428d82d89662038dc2e`  
		Last Modified: Tue, 15 Nov 2022 05:10:18 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1ae6a8fce0f2cd131007393c1a4eba9ce9d0501da8406af5c5ce9deb5dc187b8`  
		Last Modified: Wed, 11 Jan 2023 03:12:13 GMT  
		Size: 174.7 MB (174749274 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5351c17af011e98fdd3db4781945e719f390748d66dc50d28bef46bb2d6b6418`  
		Last Modified: Tue, 31 Jan 2023 00:56:53 GMT  
		Size: 307.1 MB (307117134 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6b632a2f6afda42ce5dc291920d8f03e04b69034e314687eb551be8eafedd92d`  
		Last Modified: Tue, 31 Jan 2023 00:56:38 GMT  
		Size: 936.9 KB (936854 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cbd6cbb6ae05692db55d5e4f46142d2e20e051631dc2fc44e5b20d3316143305`  
		Last Modified: Tue, 31 Jan 2023 00:56:38 GMT  
		Size: 1.3 KB (1348 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ceb1d88f8fd44412961c0db372cd86a999c6b2619ce80a916a4fe8ca0e63acc9`  
		Last Modified: Tue, 31 Jan 2023 00:56:38 GMT  
		Size: 2.5 KB (2458 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8d0ee5cad12d41a6d530031aabd4a92619995eb0ee20dcd24d2bb9aec6a694db`  
		Last Modified: Tue, 31 Jan 2023 00:56:38 GMT  
		Size: 6.0 KB (6006 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3c980b95519f007aea60be042d36cd33de21e6265aed0e443c5ecf9bb1f40980`  
		Last Modified: Tue, 31 Jan 2023 00:56:38 GMT  
		Size: 2.5 KB (2505 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `xwiki:15.0`

```console
$ docker pull xwiki@sha256:33e789838f82ce73efec6664859feb1ced7a5b7605fbfaddb81916716bce524f
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `xwiki:15.0` - linux; amd64

```console
$ docker pull xwiki@sha256:481fdb46e8c043a6709d11310e2083ce71d6ba63ee6517f84da3ba06f320598e
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **590.5 MB (590459982 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:bd630aa0aa5c679e23ea7d52cbbdd6b817eab27a820c25d3c50b54eca83b9744`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["xwiki"]`

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
# Wed, 02 Nov 2022 18:44:10 GMT
RUN apt-get update     && DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends tzdata curl wget ca-certificates fontconfig locales     && echo "en_US.UTF-8 UTF-8" >> /etc/locale.gen     && locale-gen en_US.UTF-8     && rm -rf /var/lib/apt/lists/*
# Fri, 04 Nov 2022 23:21:41 GMT
ENV JAVA_VERSION=jdk-11.0.17+8
# Fri, 04 Nov 2022 23:22:31 GMT
RUN set -eux;     ARCH="$(dpkg --print-architecture)";     case "${ARCH}" in        aarch64|arm64)          ESUM='bd6efe3290c8b5a42f695a55a26f3e3c9c284288574879d4b7089f31f5114177';          BINARY_URL='https://github.com/adoptium/temurin11-binaries/releases/download/jdk-11.0.17%2B8/OpenJDK11U-jre_aarch64_linux_hotspot_11.0.17_8.tar.gz';          ;;        armhf|arm)          ESUM='8cf113d3d7fa808895c8d2e41bb890af21c47e38c2460e0588147a4bb8fc658d';          BINARY_URL='https://github.com/adoptium/temurin11-binaries/releases/download/jdk-11.0.17%2B8/OpenJDK11U-jre_arm_linux_hotspot_11.0.17_8.tar.gz';          ;;        ppc64el|powerpc:common64)          ESUM='0ca3d806131ab5834c501f9c625bb0248cd528af361c704503348e9c9605bedf';          BINARY_URL='https://github.com/adoptium/temurin11-binaries/releases/download/jdk-11.0.17%2B8/OpenJDK11U-jre_ppc64le_linux_hotspot_11.0.17_8.tar.gz';          ;;        s390x|s390:64-bit)          ESUM='dd3b159a374086e65cb07c4ccb226c90f9c02ef929cba6f0b642171d7ed97fa4';          BINARY_URL='https://github.com/adoptium/temurin11-binaries/releases/download/jdk-11.0.17%2B8/OpenJDK11U-jre_s390x_linux_hotspot_11.0.17_8.tar.gz';          ;;        amd64|i386:x86-64)          ESUM='752616097e09d7f60a3ad8bd312f90eaf50ac72577e55df229fe6e8091148f79';          BINARY_URL='https://github.com/adoptium/temurin11-binaries/releases/download/jdk-11.0.17%2B8/OpenJDK11U-jre_x64_linux_hotspot_11.0.17_8.tar.gz';          ;;        *)          echo "Unsupported arch: ${ARCH}";          exit 1;          ;;     esac; 	  wget -O /tmp/openjdk.tar.gz ${BINARY_URL}; 	  echo "${ESUM} */tmp/openjdk.tar.gz" | sha256sum -c -; 	  mkdir -p "$JAVA_HOME"; 	  tar --extract 	      --file /tmp/openjdk.tar.gz 	      --directory "$JAVA_HOME" 	      --strip-components 1 	      --no-same-owner 	  ;     rm /tmp/openjdk.tar.gz;     find "$JAVA_HOME/lib" -name '*.so' -exec dirname '{}' ';' | sort -u > /etc/ld.so.conf.d/docker-openjdk.conf;     ldconfig;     java -Xshare:dump;
# Fri, 04 Nov 2022 23:22:32 GMT
RUN echo Verifying install ...     && fileEncoding="$(echo 'System.out.println(System.getProperty("file.encoding"))' | jshell -s -)"; [ "$fileEncoding" = 'UTF-8' ]; rm -rf ~/.java     && echo java --version && java --version     && echo Complete.
# Sat, 05 Nov 2022 01:35:16 GMT
ENV CATALINA_HOME=/usr/local/tomcat
# Sat, 05 Nov 2022 01:35:16 GMT
ENV PATH=/usr/local/tomcat/bin:/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Sat, 05 Nov 2022 01:35:17 GMT
RUN mkdir -p "$CATALINA_HOME"
# Sat, 05 Nov 2022 01:35:17 GMT
WORKDIR /usr/local/tomcat
# Sat, 05 Nov 2022 01:35:17 GMT
ENV TOMCAT_NATIVE_LIBDIR=/usr/local/tomcat/native-jni-lib
# Sat, 05 Nov 2022 01:35:17 GMT
ENV LD_LIBRARY_PATH=/usr/local/tomcat/native-jni-lib
# Sat, 05 Nov 2022 01:39:54 GMT
ENV GPG_KEYS=48F8E69F6390C9F25CFEDCD268248959359E722B A9C5DF4D22E99998D9875A5110C01C5A2F6059E7 DCFD35E0BF8CA7344752DE8B6FB21E8933C60243
# Sat, 05 Nov 2022 01:39:54 GMT
ENV TOMCAT_MAJOR=9
# Tue, 15 Nov 2022 03:06:43 GMT
ENV TOMCAT_VERSION=9.0.69
# Tue, 15 Nov 2022 03:06:43 GMT
ENV TOMCAT_SHA512=8c883c54ce9ce43eba37756a6404cdf3477879883a3e6d146dc8a7aa5e0425f487466afe6b6da4a895927cb7cb59177b9379cec18000f2de12785be57408c779
# Tue, 15 Nov 2022 03:06:44 GMT
COPY dir:b1a33aa3993dbbfbebb33bd9aa546b60c2f2191abf1227f453d4e830f6deb35f in /usr/local/tomcat 
# Tue, 15 Nov 2022 03:06:48 GMT
RUN set -eux; 	apt-get update; 	xargs -rt apt-get install -y --no-install-recommends < "$TOMCAT_NATIVE_LIBDIR/.dependencies.txt"; 	rm -rf /var/lib/apt/lists/*
# Tue, 15 Nov 2022 03:06:49 GMT
RUN set -eux; 	nativeLines="$(catalina.sh configtest 2>&1)"; 	nativeLines="$(echo "$nativeLines" | grep 'Apache Tomcat Native')"; 	nativeLines="$(echo "$nativeLines" | sort -u)"; 	if ! echo "$nativeLines" | grep -E 'INFO: Loaded( APR based)? Apache Tomcat Native library' >&2; then 		echo >&2 "$nativeLines"; 		exit 1; 	fi
# Tue, 15 Nov 2022 03:06:49 GMT
EXPOSE 8080
# Tue, 15 Nov 2022 03:06:49 GMT
CMD ["catalina.sh" "run"]
# Wed, 11 Jan 2023 02:47:03 GMT
LABEL org.opencontainers.image.authors=XWiki Development Team <committers@xwiki.org>
# Wed, 11 Jan 2023 02:47:03 GMT
LABEL org.opencontainers.image.url=https://hub.docker.com/_/xwiki
# Wed, 11 Jan 2023 02:47:03 GMT
LABEL org.opencontainers.image.documentation=https://hub.docker.com/_/xwiki
# Wed, 11 Jan 2023 02:47:03 GMT
LABEL org.opencontainers.image.source=https://github.com/xwiki/xwiki-docker.git
# Wed, 11 Jan 2023 02:47:04 GMT
LABEL org.opencontainers.image.vendor=xwiki.org
# Wed, 11 Jan 2023 02:47:04 GMT
LABEL org.opencontainers.image.licenses=LGPL-2.1
# Wed, 11 Jan 2023 02:49:03 GMT
RUN apt-get update &&   apt-get --no-install-recommends -y install     curl     libreoffice     unzip     procps &&   rm -rf /var/lib/apt/lists/*
# Tue, 31 Jan 2023 00:20:17 GMT
ENV XWIKI_VERSION=15.0
# Tue, 31 Jan 2023 00:20:17 GMT
ENV XWIKI_URL_PREFIX=https://maven.xwiki.org/releases/org/xwiki/platform/xwiki-platform-distribution-war/15.0
# Tue, 31 Jan 2023 00:20:17 GMT
ENV XWIKI_DOWNLOAD_SHA256=79ba0f479bbc49521c113821adc9d91141075a9470d7f9bbb6994ca59c30d121
# Tue, 31 Jan 2023 00:21:18 GMT
RUN rm -rf /usr/local/tomcat/webapps/* &&   mkdir -p /usr/local/tomcat/temp &&   mkdir -p /usr/local/xwiki/data &&   curl -fSL "${XWIKI_URL_PREFIX}/xwiki-platform-distribution-war-${XWIKI_VERSION}.war" -o xwiki.war &&   echo "$XWIKI_DOWNLOAD_SHA256 xwiki.war" | sha256sum -c - &&   unzip -d /usr/local/tomcat/webapps/ROOT xwiki.war &&   rm -f xwiki.war
# Tue, 31 Jan 2023 00:21:19 GMT
ENV MYSQL_JDBC_VERSION=8.0.31
# Tue, 31 Jan 2023 00:21:19 GMT
ENV MYSQL_JDBC_SHA256=5249e3dc6d6531b37790e3f61845b96db5e41e891d3d8edb0e2e3a1b53ca2f4f
# Tue, 31 Jan 2023 00:21:19 GMT
ENV MYSQL_JDBC_PREFIX=https://repo1.maven.org/maven2/com/mysql/mysql-connector-j/8.0.31
# Tue, 31 Jan 2023 00:21:19 GMT
ENV MYSQL_JDBC_ARTIFACT=mysql-connector-j-8.0.31.jar
# Tue, 31 Jan 2023 00:21:19 GMT
ENV MYSQL_JDBC_TARGET=/usr/local/tomcat/webapps/ROOT/WEB-INF/lib/mysql-connector-j-8.0.31.jar
# Tue, 31 Jan 2023 00:21:20 GMT
RUN curl -fSL "${MYSQL_JDBC_PREFIX}/${MYSQL_JDBC_ARTIFACT}" -o $MYSQL_JDBC_TARGET &&   echo "$MYSQL_JDBC_SHA256 $MYSQL_JDBC_TARGET" | sha256sum -c -
# Tue, 31 Jan 2023 00:21:21 GMT
COPY file:0a1be11e2eb610a1dbcd415404e3a592641110b93090030cb831e3a19a163017 in /usr/local/tomcat/bin/ 
# Tue, 31 Jan 2023 00:21:21 GMT
COPY file:1b8409986f3e4eb79a7a0b18472cb2692a61d504fb5ef34292bc997b79fd760d in /usr/local/tomcat/webapps/ROOT/WEB-INF/hibernate.cfg.xml 
# Tue, 31 Jan 2023 00:21:21 GMT
RUN sed -i 's/<id>org.xwiki.platform:xwiki-platform-distribution-war/<id>org.xwiki.platform:xwiki-platform-distribution-docker/'   /usr/local/tomcat/webapps/ROOT/META-INF/extension.xed
# Tue, 31 Jan 2023 00:21:21 GMT
COPY file:a47c4dcd87c9dad97aff38c49188357e6193bcad50757e516cfb08a60d4de611 in /usr/local/bin/docker-entrypoint.sh 
# Tue, 31 Jan 2023 00:21:22 GMT
VOLUME [/usr/local/xwiki]
# Tue, 31 Jan 2023 00:21:22 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 31 Jan 2023 00:21:22 GMT
CMD ["xwiki"]
```

-	Layers:
	-	`sha256:e96e057aae67380a4ddb16c337c5c3669d97fdff69ec537f02aa2cc30d814281`  
		Last Modified: Wed, 02 Nov 2022 03:03:36 GMT  
		Size: 30.4 MB (30425607 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4ced2591451da3a02e2b6bb44752b9e3f00d77789921be4df5082fb9f9880ad0`  
		Last Modified: Wed, 02 Nov 2022 18:48:43 GMT  
		Size: 12.4 MB (12439006 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:df8f874ae8c08a9e69e5fbe6c5a64200a45386132a3203d1a9a7f1146d94cfbc`  
		Last Modified: Fri, 04 Nov 2022 23:29:33 GMT  
		Size: 46.6 MB (46629936 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:111b6c7486426c4b6989102c2ee5be856e8a58e20ab0a350b24a905d536e8e7f`  
		Last Modified: Fri, 04 Nov 2022 23:29:26 GMT  
		Size: 161.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e6f84dce457c6d4f7b7291fce05f8e77998a3a7722a54125a1f1d52ca83043b4`  
		Last Modified: Sat, 05 Nov 2022 01:50:51 GMT  
		Size: 173.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a6c26749ee782392e38845ee2ba79b0da586ef6a45d8e7f29c7af14612278547`  
		Last Modified: Tue, 15 Nov 2022 03:19:57 GMT  
		Size: 12.2 MB (12200249 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4dddc6d9fa6024025b3fcfe729cab2dc544fb25476eca6e80b1af8e8d93bb0ee`  
		Last Modified: Tue, 15 Nov 2022 03:19:56 GMT  
		Size: 452.7 KB (452680 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:06637eebe5e72c8ad9019ad4eb4cdde1f11f7d4c24c7ed7374cf8966343aa2fb`  
		Last Modified: Tue, 15 Nov 2022 03:19:56 GMT  
		Size: 131.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b276fb8390410a8208724033e325715ea26000d5a1a762d4c3699b927884fbfe`  
		Last Modified: Wed, 11 Jan 2023 02:52:45 GMT  
		Size: 178.8 MB (178805608 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:156ca91198173149698aa0396648a9608b6ab1f2bc2666800843ce33c9f85b6e`  
		Last Modified: Tue, 31 Jan 2023 00:24:09 GMT  
		Size: 307.1 MB (307117069 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4c8b70d250c6d507901857473b0dcb67132d7b2a30ce9a69b07b1036853df738`  
		Last Modified: Tue, 31 Jan 2023 00:23:52 GMT  
		Size: 2.4 MB (2377191 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a9681fd36be674d25231c69d6a39f9e8fa65034eeaef5d1bd885fdbeac7f0f6b`  
		Last Modified: Tue, 31 Jan 2023 00:23:51 GMT  
		Size: 1.3 KB (1346 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a9d0d5da840f4d7da9943942b38cd092fae11f41dc6c19afd58d655cd6192d66`  
		Last Modified: Tue, 31 Jan 2023 00:23:51 GMT  
		Size: 2.3 KB (2312 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d65610da4f1da86fea8fbec0189b066afd4b86e4e8f7d049e3c4bc6ade9ba90a`  
		Last Modified: Tue, 31 Jan 2023 00:23:51 GMT  
		Size: 6.0 KB (6009 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3d41686284d7675eaa0f92c9cc27ebe73b4c30768c8eef9f23ee3b1ad06da00a`  
		Last Modified: Tue, 31 Jan 2023 00:23:51 GMT  
		Size: 2.5 KB (2504 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `xwiki:15.0` - linux; arm64 variant v8

```console
$ docker pull xwiki@sha256:6bf63d9025b07b69d744200c05efd4ffb8a52f3c38380f5d59a0b48514203cd2
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **581.7 MB (581709921 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:6600f2bb05836c703d53944bbcb5399d509a9813a27a35e99ff717becc308330`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["xwiki"]`

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
# Wed, 02 Nov 2022 19:44:32 GMT
RUN apt-get update     && DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends tzdata curl wget ca-certificates fontconfig locales     && echo "en_US.UTF-8 UTF-8" >> /etc/locale.gen     && locale-gen en_US.UTF-8     && rm -rf /var/lib/apt/lists/*
# Fri, 04 Nov 2022 22:40:54 GMT
ENV JAVA_VERSION=jdk-11.0.17+8
# Fri, 04 Nov 2022 22:41:33 GMT
RUN set -eux;     ARCH="$(dpkg --print-architecture)";     case "${ARCH}" in        aarch64|arm64)          ESUM='bd6efe3290c8b5a42f695a55a26f3e3c9c284288574879d4b7089f31f5114177';          BINARY_URL='https://github.com/adoptium/temurin11-binaries/releases/download/jdk-11.0.17%2B8/OpenJDK11U-jre_aarch64_linux_hotspot_11.0.17_8.tar.gz';          ;;        armhf|arm)          ESUM='8cf113d3d7fa808895c8d2e41bb890af21c47e38c2460e0588147a4bb8fc658d';          BINARY_URL='https://github.com/adoptium/temurin11-binaries/releases/download/jdk-11.0.17%2B8/OpenJDK11U-jre_arm_linux_hotspot_11.0.17_8.tar.gz';          ;;        ppc64el|powerpc:common64)          ESUM='0ca3d806131ab5834c501f9c625bb0248cd528af361c704503348e9c9605bedf';          BINARY_URL='https://github.com/adoptium/temurin11-binaries/releases/download/jdk-11.0.17%2B8/OpenJDK11U-jre_ppc64le_linux_hotspot_11.0.17_8.tar.gz';          ;;        s390x|s390:64-bit)          ESUM='dd3b159a374086e65cb07c4ccb226c90f9c02ef929cba6f0b642171d7ed97fa4';          BINARY_URL='https://github.com/adoptium/temurin11-binaries/releases/download/jdk-11.0.17%2B8/OpenJDK11U-jre_s390x_linux_hotspot_11.0.17_8.tar.gz';          ;;        amd64|i386:x86-64)          ESUM='752616097e09d7f60a3ad8bd312f90eaf50ac72577e55df229fe6e8091148f79';          BINARY_URL='https://github.com/adoptium/temurin11-binaries/releases/download/jdk-11.0.17%2B8/OpenJDK11U-jre_x64_linux_hotspot_11.0.17_8.tar.gz';          ;;        *)          echo "Unsupported arch: ${ARCH}";          exit 1;          ;;     esac; 	  wget -O /tmp/openjdk.tar.gz ${BINARY_URL}; 	  echo "${ESUM} */tmp/openjdk.tar.gz" | sha256sum -c -; 	  mkdir -p "$JAVA_HOME"; 	  tar --extract 	      --file /tmp/openjdk.tar.gz 	      --directory "$JAVA_HOME" 	      --strip-components 1 	      --no-same-owner 	  ;     rm /tmp/openjdk.tar.gz;     find "$JAVA_HOME/lib" -name '*.so' -exec dirname '{}' ';' | sort -u > /etc/ld.so.conf.d/docker-openjdk.conf;     ldconfig;     java -Xshare:dump;
# Fri, 04 Nov 2022 22:41:34 GMT
RUN echo Verifying install ...     && fileEncoding="$(echo 'System.out.println(System.getProperty("file.encoding"))' | jshell -s -)"; [ "$fileEncoding" = 'UTF-8' ]; rm -rf ~/.java     && echo java --version && java --version     && echo Complete.
# Fri, 04 Nov 2022 23:48:38 GMT
ENV CATALINA_HOME=/usr/local/tomcat
# Fri, 04 Nov 2022 23:48:38 GMT
ENV PATH=/usr/local/tomcat/bin:/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Fri, 04 Nov 2022 23:48:38 GMT
RUN mkdir -p "$CATALINA_HOME"
# Fri, 04 Nov 2022 23:48:39 GMT
WORKDIR /usr/local/tomcat
# Fri, 04 Nov 2022 23:48:39 GMT
ENV TOMCAT_NATIVE_LIBDIR=/usr/local/tomcat/native-jni-lib
# Fri, 04 Nov 2022 23:48:39 GMT
ENV LD_LIBRARY_PATH=/usr/local/tomcat/native-jni-lib
# Fri, 04 Nov 2022 23:53:12 GMT
ENV GPG_KEYS=48F8E69F6390C9F25CFEDCD268248959359E722B A9C5DF4D22E99998D9875A5110C01C5A2F6059E7 DCFD35E0BF8CA7344752DE8B6FB21E8933C60243
# Fri, 04 Nov 2022 23:53:12 GMT
ENV TOMCAT_MAJOR=9
# Tue, 15 Nov 2022 04:57:22 GMT
ENV TOMCAT_VERSION=9.0.69
# Tue, 15 Nov 2022 04:57:22 GMT
ENV TOMCAT_SHA512=8c883c54ce9ce43eba37756a6404cdf3477879883a3e6d146dc8a7aa5e0425f487466afe6b6da4a895927cb7cb59177b9379cec18000f2de12785be57408c779
# Tue, 15 Nov 2022 04:57:22 GMT
COPY dir:096b403a5f78b17e6b4bff63128a9c93941b97f22470991610dd641633d977f1 in /usr/local/tomcat 
# Tue, 15 Nov 2022 04:57:25 GMT
RUN set -eux; 	apt-get update; 	xargs -rt apt-get install -y --no-install-recommends < "$TOMCAT_NATIVE_LIBDIR/.dependencies.txt"; 	rm -rf /var/lib/apt/lists/*
# Tue, 15 Nov 2022 04:57:26 GMT
RUN set -eux; 	nativeLines="$(catalina.sh configtest 2>&1)"; 	nativeLines="$(echo "$nativeLines" | grep 'Apache Tomcat Native')"; 	nativeLines="$(echo "$nativeLines" | sort -u)"; 	if ! echo "$nativeLines" | grep -E 'INFO: Loaded( APR based)? Apache Tomcat Native library' >&2; then 		echo >&2 "$nativeLines"; 		exit 1; 	fi
# Tue, 15 Nov 2022 04:57:26 GMT
EXPOSE 8080
# Tue, 15 Nov 2022 04:57:27 GMT
CMD ["catalina.sh" "run"]
# Wed, 11 Jan 2023 03:05:10 GMT
LABEL org.opencontainers.image.authors=XWiki Development Team <committers@xwiki.org>
# Wed, 11 Jan 2023 03:05:10 GMT
LABEL org.opencontainers.image.url=https://hub.docker.com/_/xwiki
# Wed, 11 Jan 2023 03:05:10 GMT
LABEL org.opencontainers.image.documentation=https://hub.docker.com/_/xwiki
# Wed, 11 Jan 2023 03:05:10 GMT
LABEL org.opencontainers.image.source=https://github.com/xwiki/xwiki-docker.git
# Wed, 11 Jan 2023 03:05:11 GMT
LABEL org.opencontainers.image.vendor=xwiki.org
# Wed, 11 Jan 2023 03:05:11 GMT
LABEL org.opencontainers.image.licenses=LGPL-2.1
# Wed, 11 Jan 2023 03:07:37 GMT
RUN apt-get update &&   apt-get --no-install-recommends -y install     curl     libreoffice     unzip     procps &&   rm -rf /var/lib/apt/lists/*
# Tue, 31 Jan 2023 00:47:12 GMT
ENV XWIKI_VERSION=15.0
# Tue, 31 Jan 2023 00:47:12 GMT
ENV XWIKI_URL_PREFIX=https://maven.xwiki.org/releases/org/xwiki/platform/xwiki-platform-distribution-war/15.0
# Tue, 31 Jan 2023 00:47:12 GMT
ENV XWIKI_DOWNLOAD_SHA256=79ba0f479bbc49521c113821adc9d91141075a9470d7f9bbb6994ca59c30d121
# Tue, 31 Jan 2023 00:47:58 GMT
RUN rm -rf /usr/local/tomcat/webapps/* &&   mkdir -p /usr/local/tomcat/temp &&   mkdir -p /usr/local/xwiki/data &&   curl -fSL "${XWIKI_URL_PREFIX}/xwiki-platform-distribution-war-${XWIKI_VERSION}.war" -o xwiki.war &&   echo "$XWIKI_DOWNLOAD_SHA256 xwiki.war" | sha256sum -c - &&   unzip -d /usr/local/tomcat/webapps/ROOT xwiki.war &&   rm -f xwiki.war
# Tue, 31 Jan 2023 00:48:01 GMT
ENV MYSQL_JDBC_VERSION=8.0.31
# Tue, 31 Jan 2023 00:48:01 GMT
ENV MYSQL_JDBC_SHA256=5249e3dc6d6531b37790e3f61845b96db5e41e891d3d8edb0e2e3a1b53ca2f4f
# Tue, 31 Jan 2023 00:48:01 GMT
ENV MYSQL_JDBC_PREFIX=https://repo1.maven.org/maven2/com/mysql/mysql-connector-j/8.0.31
# Tue, 31 Jan 2023 00:48:01 GMT
ENV MYSQL_JDBC_ARTIFACT=mysql-connector-j-8.0.31.jar
# Tue, 31 Jan 2023 00:48:01 GMT
ENV MYSQL_JDBC_TARGET=/usr/local/tomcat/webapps/ROOT/WEB-INF/lib/mysql-connector-j-8.0.31.jar
# Tue, 31 Jan 2023 00:48:02 GMT
RUN curl -fSL "${MYSQL_JDBC_PREFIX}/${MYSQL_JDBC_ARTIFACT}" -o $MYSQL_JDBC_TARGET &&   echo "$MYSQL_JDBC_SHA256 $MYSQL_JDBC_TARGET" | sha256sum -c -
# Tue, 31 Jan 2023 00:48:02 GMT
COPY file:0a1be11e2eb610a1dbcd415404e3a592641110b93090030cb831e3a19a163017 in /usr/local/tomcat/bin/ 
# Tue, 31 Jan 2023 00:48:02 GMT
COPY file:1b8409986f3e4eb79a7a0b18472cb2692a61d504fb5ef34292bc997b79fd760d in /usr/local/tomcat/webapps/ROOT/WEB-INF/hibernate.cfg.xml 
# Tue, 31 Jan 2023 00:48:03 GMT
RUN sed -i 's/<id>org.xwiki.platform:xwiki-platform-distribution-war/<id>org.xwiki.platform:xwiki-platform-distribution-docker/'   /usr/local/tomcat/webapps/ROOT/META-INF/extension.xed
# Tue, 31 Jan 2023 00:48:03 GMT
COPY file:a47c4dcd87c9dad97aff38c49188357e6193bcad50757e516cfb08a60d4de611 in /usr/local/bin/docker-entrypoint.sh 
# Tue, 31 Jan 2023 00:48:03 GMT
VOLUME [/usr/local/xwiki]
# Tue, 31 Jan 2023 00:48:03 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 31 Jan 2023 00:48:03 GMT
CMD ["xwiki"]
```

-	Layers:
	-	`sha256:0509fae36eb0656f8bdb23f8ae64100d893bcea2563e97468d337e04d2d0410b`  
		Last Modified: Wed, 02 Nov 2022 18:50:21 GMT  
		Size: 28.4 MB (28382154 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e502a1af2bcd98f5f0d2f5e4da1a0e7bbe07a2c548e2662f7d37dce5ae1df46c`  
		Last Modified: Wed, 02 Nov 2022 19:48:28 GMT  
		Size: 12.4 MB (12396330 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bc4598c07dd818f03a0378b0341a4a8e80f0152fbb3e7d5246ca4f466f42e611`  
		Last Modified: Fri, 04 Nov 2022 22:46:46 GMT  
		Size: 45.0 MB (44958470 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:715a937a1066f998b331fcd62256ad01a5571bdf46804e97825afc64f9ebb427`  
		Last Modified: Fri, 04 Nov 2022 22:46:41 GMT  
		Size: 160.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5fb623f082f74b2fa9fc2c4e3f3a4802875cb9753cfa26ed940201ce72bb56cb`  
		Last Modified: Sat, 05 Nov 2022 00:03:40 GMT  
		Size: 172.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:33260b83200262bbd546be371ad3c1f50f5ae7228afb87982d6fa9d6b11bf26f`  
		Last Modified: Tue, 15 Nov 2022 05:10:19 GMT  
		Size: 12.2 MB (12207235 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0955fb697ea9b30a1b4f95385464f646aa1525cb6efba648e22df84ebef6b2ee`  
		Last Modified: Tue, 15 Nov 2022 05:10:18 GMT  
		Size: 452.0 KB (452021 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6eddcf66f2083b1487296a0308e0b058917c97f614f12428d82d89662038dc2e`  
		Last Modified: Tue, 15 Nov 2022 05:10:18 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ae5f60bb64f3fa11da3d15a9639f886186b4c2c021455c3f9db22e0cfe1b1311`  
		Last Modified: Wed, 11 Jan 2023 03:11:14 GMT  
		Size: 173.8 MB (173806827 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1814d85fce571b42f2cfa7c8a904e1a184ee6f49642242a44bbe0037088994a0`  
		Last Modified: Tue, 31 Jan 2023 00:56:04 GMT  
		Size: 307.1 MB (307117070 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8aec0e24b4fa870989f014944c3c7d535355a2371fc8c948b2b11f9b377efe6e`  
		Last Modified: Tue, 31 Jan 2023 00:55:50 GMT  
		Size: 2.4 MB (2377182 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0b65081619aa0114a7f367836ef421eb8d951e559e0f089c7728af7813b1ea62`  
		Last Modified: Tue, 31 Jan 2023 00:55:49 GMT  
		Size: 1.3 KB (1348 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:46ebad072e608146426d8dc30828937049eea36c2e636d7790b4960d6d586977`  
		Last Modified: Tue, 31 Jan 2023 00:55:49 GMT  
		Size: 2.3 KB (2308 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:708fefcedd4ee6c106da247a68c5790f5ab00225d1cdfff8465575265c3a54e6`  
		Last Modified: Tue, 31 Jan 2023 00:55:49 GMT  
		Size: 6.0 KB (6008 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:81e3bf8e20bc921031e7549a41dec1b2d7795cc6da40a0e7096bf654b25c5c3e`  
		Last Modified: Tue, 31 Jan 2023 00:55:49 GMT  
		Size: 2.5 KB (2507 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `xwiki:15.0-mariadb-tomcat`

```console
$ docker pull xwiki@sha256:725347355967f33745268f1167cc3c1b12fc85e327ccfa96da0848d05e3836c4
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `xwiki:15.0-mariadb-tomcat` - linux; amd64

```console
$ docker pull xwiki@sha256:cca1fb53bc2f0240f7f4843b846210e341a6002d7b18a0b90202520ce2f4ead0
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **588.7 MB (588672467 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:0088d72e62c01c9996a75e1b7e2296ba530b2dbd4054be70a006b33295aa4ff9`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["xwiki"]`

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
# Wed, 02 Nov 2022 18:44:10 GMT
RUN apt-get update     && DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends tzdata curl wget ca-certificates fontconfig locales     && echo "en_US.UTF-8 UTF-8" >> /etc/locale.gen     && locale-gen en_US.UTF-8     && rm -rf /var/lib/apt/lists/*
# Fri, 04 Nov 2022 23:21:41 GMT
ENV JAVA_VERSION=jdk-11.0.17+8
# Fri, 04 Nov 2022 23:22:31 GMT
RUN set -eux;     ARCH="$(dpkg --print-architecture)";     case "${ARCH}" in        aarch64|arm64)          ESUM='bd6efe3290c8b5a42f695a55a26f3e3c9c284288574879d4b7089f31f5114177';          BINARY_URL='https://github.com/adoptium/temurin11-binaries/releases/download/jdk-11.0.17%2B8/OpenJDK11U-jre_aarch64_linux_hotspot_11.0.17_8.tar.gz';          ;;        armhf|arm)          ESUM='8cf113d3d7fa808895c8d2e41bb890af21c47e38c2460e0588147a4bb8fc658d';          BINARY_URL='https://github.com/adoptium/temurin11-binaries/releases/download/jdk-11.0.17%2B8/OpenJDK11U-jre_arm_linux_hotspot_11.0.17_8.tar.gz';          ;;        ppc64el|powerpc:common64)          ESUM='0ca3d806131ab5834c501f9c625bb0248cd528af361c704503348e9c9605bedf';          BINARY_URL='https://github.com/adoptium/temurin11-binaries/releases/download/jdk-11.0.17%2B8/OpenJDK11U-jre_ppc64le_linux_hotspot_11.0.17_8.tar.gz';          ;;        s390x|s390:64-bit)          ESUM='dd3b159a374086e65cb07c4ccb226c90f9c02ef929cba6f0b642171d7ed97fa4';          BINARY_URL='https://github.com/adoptium/temurin11-binaries/releases/download/jdk-11.0.17%2B8/OpenJDK11U-jre_s390x_linux_hotspot_11.0.17_8.tar.gz';          ;;        amd64|i386:x86-64)          ESUM='752616097e09d7f60a3ad8bd312f90eaf50ac72577e55df229fe6e8091148f79';          BINARY_URL='https://github.com/adoptium/temurin11-binaries/releases/download/jdk-11.0.17%2B8/OpenJDK11U-jre_x64_linux_hotspot_11.0.17_8.tar.gz';          ;;        *)          echo "Unsupported arch: ${ARCH}";          exit 1;          ;;     esac; 	  wget -O /tmp/openjdk.tar.gz ${BINARY_URL}; 	  echo "${ESUM} */tmp/openjdk.tar.gz" | sha256sum -c -; 	  mkdir -p "$JAVA_HOME"; 	  tar --extract 	      --file /tmp/openjdk.tar.gz 	      --directory "$JAVA_HOME" 	      --strip-components 1 	      --no-same-owner 	  ;     rm /tmp/openjdk.tar.gz;     find "$JAVA_HOME/lib" -name '*.so' -exec dirname '{}' ';' | sort -u > /etc/ld.so.conf.d/docker-openjdk.conf;     ldconfig;     java -Xshare:dump;
# Fri, 04 Nov 2022 23:22:32 GMT
RUN echo Verifying install ...     && fileEncoding="$(echo 'System.out.println(System.getProperty("file.encoding"))' | jshell -s -)"; [ "$fileEncoding" = 'UTF-8' ]; rm -rf ~/.java     && echo java --version && java --version     && echo Complete.
# Sat, 05 Nov 2022 01:35:16 GMT
ENV CATALINA_HOME=/usr/local/tomcat
# Sat, 05 Nov 2022 01:35:16 GMT
ENV PATH=/usr/local/tomcat/bin:/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Sat, 05 Nov 2022 01:35:17 GMT
RUN mkdir -p "$CATALINA_HOME"
# Sat, 05 Nov 2022 01:35:17 GMT
WORKDIR /usr/local/tomcat
# Sat, 05 Nov 2022 01:35:17 GMT
ENV TOMCAT_NATIVE_LIBDIR=/usr/local/tomcat/native-jni-lib
# Sat, 05 Nov 2022 01:35:17 GMT
ENV LD_LIBRARY_PATH=/usr/local/tomcat/native-jni-lib
# Sat, 05 Nov 2022 01:39:54 GMT
ENV GPG_KEYS=48F8E69F6390C9F25CFEDCD268248959359E722B A9C5DF4D22E99998D9875A5110C01C5A2F6059E7 DCFD35E0BF8CA7344752DE8B6FB21E8933C60243
# Sat, 05 Nov 2022 01:39:54 GMT
ENV TOMCAT_MAJOR=9
# Tue, 15 Nov 2022 03:06:43 GMT
ENV TOMCAT_VERSION=9.0.69
# Tue, 15 Nov 2022 03:06:43 GMT
ENV TOMCAT_SHA512=8c883c54ce9ce43eba37756a6404cdf3477879883a3e6d146dc8a7aa5e0425f487466afe6b6da4a895927cb7cb59177b9379cec18000f2de12785be57408c779
# Tue, 15 Nov 2022 03:06:44 GMT
COPY dir:b1a33aa3993dbbfbebb33bd9aa546b60c2f2191abf1227f453d4e830f6deb35f in /usr/local/tomcat 
# Tue, 15 Nov 2022 03:06:48 GMT
RUN set -eux; 	apt-get update; 	xargs -rt apt-get install -y --no-install-recommends < "$TOMCAT_NATIVE_LIBDIR/.dependencies.txt"; 	rm -rf /var/lib/apt/lists/*
# Tue, 15 Nov 2022 03:06:49 GMT
RUN set -eux; 	nativeLines="$(catalina.sh configtest 2>&1)"; 	nativeLines="$(echo "$nativeLines" | grep 'Apache Tomcat Native')"; 	nativeLines="$(echo "$nativeLines" | sort -u)"; 	if ! echo "$nativeLines" | grep -E 'INFO: Loaded( APR based)? Apache Tomcat Native library' >&2; then 		echo >&2 "$nativeLines"; 		exit 1; 	fi
# Tue, 15 Nov 2022 03:06:49 GMT
EXPOSE 8080
# Tue, 15 Nov 2022 03:06:49 GMT
CMD ["catalina.sh" "run"]
# Wed, 11 Jan 2023 02:47:03 GMT
LABEL org.opencontainers.image.authors=XWiki Development Team <committers@xwiki.org>
# Wed, 11 Jan 2023 02:47:03 GMT
LABEL org.opencontainers.image.url=https://hub.docker.com/_/xwiki
# Wed, 11 Jan 2023 02:47:03 GMT
LABEL org.opencontainers.image.documentation=https://hub.docker.com/_/xwiki
# Wed, 11 Jan 2023 02:47:03 GMT
LABEL org.opencontainers.image.source=https://github.com/xwiki/xwiki-docker.git
# Wed, 11 Jan 2023 02:47:04 GMT
LABEL org.opencontainers.image.vendor=xwiki.org
# Wed, 11 Jan 2023 02:47:04 GMT
LABEL org.opencontainers.image.licenses=LGPL-2.1
# Wed, 11 Jan 2023 02:49:03 GMT
RUN apt-get update &&   apt-get --no-install-recommends -y install     curl     libreoffice     unzip     procps &&   rm -rf /var/lib/apt/lists/*
# Tue, 31 Jan 2023 00:20:17 GMT
ENV XWIKI_VERSION=15.0
# Tue, 31 Jan 2023 00:20:17 GMT
ENV XWIKI_URL_PREFIX=https://maven.xwiki.org/releases/org/xwiki/platform/xwiki-platform-distribution-war/15.0
# Tue, 31 Jan 2023 00:20:17 GMT
ENV XWIKI_DOWNLOAD_SHA256=79ba0f479bbc49521c113821adc9d91141075a9470d7f9bbb6994ca59c30d121
# Tue, 31 Jan 2023 00:21:18 GMT
RUN rm -rf /usr/local/tomcat/webapps/* &&   mkdir -p /usr/local/tomcat/temp &&   mkdir -p /usr/local/xwiki/data &&   curl -fSL "${XWIKI_URL_PREFIX}/xwiki-platform-distribution-war-${XWIKI_VERSION}.war" -o xwiki.war &&   echo "$XWIKI_DOWNLOAD_SHA256 xwiki.war" | sha256sum -c - &&   unzip -d /usr/local/tomcat/webapps/ROOT xwiki.war &&   rm -f xwiki.war
# Tue, 31 Jan 2023 00:22:50 GMT
ENV MARIADB_JDBC_VERSION=3.1.1
# Tue, 31 Jan 2023 00:22:50 GMT
ENV MARIADB_JDBC_SHA256=a554541fd88047905fb0c4c10e1d85295f5e38c7bb5fb408b425392a79fc26e3
# Tue, 31 Jan 2023 00:22:50 GMT
ENV MARIADB_JDBC_PREFIX=https://repo1.maven.org/maven2/org/mariadb/jdbc/mariadb-java-client/3.1.1
# Tue, 31 Jan 2023 00:22:50 GMT
ENV MARIADB_JDBC_ARTIFACT=mariadb-java-client-3.1.1.jar
# Tue, 31 Jan 2023 00:22:50 GMT
ENV MARIADB_JDBC_TARGET=/usr/local/tomcat/webapps/ROOT/WEB-INF/lib/mariadb-java-client-3.1.1.jar
# Tue, 31 Jan 2023 00:22:51 GMT
RUN curl -fSL "${MARIADB_JDBC_PREFIX}/${MARIADB_JDBC_ARTIFACT}" -o $MARIADB_JDBC_TARGET &&   echo "$MARIADB_JDBC_SHA256 $MARIADB_JDBC_TARGET" | sha256sum -c -
# Tue, 31 Jan 2023 00:22:51 GMT
COPY file:0a1be11e2eb610a1dbcd415404e3a592641110b93090030cb831e3a19a163017 in /usr/local/tomcat/bin/ 
# Tue, 31 Jan 2023 00:22:51 GMT
COPY file:0e237c3876eeb3b5f3473a064d3e507da2df6c228ca714687930b34e3b687601 in /usr/local/tomcat/webapps/ROOT/WEB-INF/hibernate.cfg.xml 
# Tue, 31 Jan 2023 00:22:52 GMT
RUN sed -i 's/<id>org.xwiki.platform:xwiki-platform-distribution-war/<id>org.xwiki.platform:xwiki-platform-distribution-docker/'   /usr/local/tomcat/webapps/ROOT/META-INF/extension.xed
# Tue, 31 Jan 2023 00:22:52 GMT
COPY file:a47c4dcd87c9dad97aff38c49188357e6193bcad50757e516cfb08a60d4de611 in /usr/local/bin/docker-entrypoint.sh 
# Tue, 31 Jan 2023 00:22:52 GMT
VOLUME [/usr/local/xwiki]
# Tue, 31 Jan 2023 00:22:52 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 31 Jan 2023 00:22:52 GMT
CMD ["xwiki"]
```

-	Layers:
	-	`sha256:e96e057aae67380a4ddb16c337c5c3669d97fdff69ec537f02aa2cc30d814281`  
		Last Modified: Wed, 02 Nov 2022 03:03:36 GMT  
		Size: 30.4 MB (30425607 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4ced2591451da3a02e2b6bb44752b9e3f00d77789921be4df5082fb9f9880ad0`  
		Last Modified: Wed, 02 Nov 2022 18:48:43 GMT  
		Size: 12.4 MB (12439006 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:df8f874ae8c08a9e69e5fbe6c5a64200a45386132a3203d1a9a7f1146d94cfbc`  
		Last Modified: Fri, 04 Nov 2022 23:29:33 GMT  
		Size: 46.6 MB (46629936 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:111b6c7486426c4b6989102c2ee5be856e8a58e20ab0a350b24a905d536e8e7f`  
		Last Modified: Fri, 04 Nov 2022 23:29:26 GMT  
		Size: 161.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e6f84dce457c6d4f7b7291fce05f8e77998a3a7722a54125a1f1d52ca83043b4`  
		Last Modified: Sat, 05 Nov 2022 01:50:51 GMT  
		Size: 173.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a6c26749ee782392e38845ee2ba79b0da586ef6a45d8e7f29c7af14612278547`  
		Last Modified: Tue, 15 Nov 2022 03:19:57 GMT  
		Size: 12.2 MB (12200249 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4dddc6d9fa6024025b3fcfe729cab2dc544fb25476eca6e80b1af8e8d93bb0ee`  
		Last Modified: Tue, 15 Nov 2022 03:19:56 GMT  
		Size: 452.7 KB (452680 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:06637eebe5e72c8ad9019ad4eb4cdde1f11f7d4c24c7ed7374cf8966343aa2fb`  
		Last Modified: Tue, 15 Nov 2022 03:19:56 GMT  
		Size: 131.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b276fb8390410a8208724033e325715ea26000d5a1a762d4c3699b927884fbfe`  
		Last Modified: Wed, 11 Jan 2023 02:52:45 GMT  
		Size: 178.8 MB (178805608 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:156ca91198173149698aa0396648a9608b6ab1f2bc2666800843ce33c9f85b6e`  
		Last Modified: Tue, 31 Jan 2023 00:24:09 GMT  
		Size: 307.1 MB (307117069 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:457b62e39784bb863cc6a7514f591232a9b9442f2f105a85bdbd5e4abb166ad6`  
		Last Modified: Tue, 31 Jan 2023 00:25:23 GMT  
		Size: 589.7 KB (589675 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:30adbbecb36197c3e48c90be60a50c089cb9738a771c968b36240b05b8164a30`  
		Last Modified: Tue, 31 Jan 2023 00:25:22 GMT  
		Size: 1.3 KB (1345 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3bfcc8a896e6e21d5c28da101d5d57167a5cfc49c542a407feabe27f6c355b6f`  
		Last Modified: Tue, 31 Jan 2023 00:25:22 GMT  
		Size: 2.3 KB (2312 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5cbacf6c3ece365f64b683c8ab4fe61301319c8f1bd26d38ea40abbbd15bc7d4`  
		Last Modified: Tue, 31 Jan 2023 00:25:23 GMT  
		Size: 6.0 KB (6008 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6687ecee0e041196fd810c316565d70808b445cdce0b089b2177e6636bffd9fe`  
		Last Modified: Tue, 31 Jan 2023 00:25:23 GMT  
		Size: 2.5 KB (2507 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `xwiki:15.0-mariadb-tomcat` - linux; arm64 variant v8

```console
$ docker pull xwiki@sha256:14b1c6df2a5c5c9b549f372fce50719f39fc809b8b02c945d92eb29c29f7bc75
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **579.9 MB (579922416 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d9a728666283f6f4b71f567ce6c5ef1e2dc544facfd01d52fdf1577be95c6b07`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["xwiki"]`

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
# Wed, 02 Nov 2022 19:44:32 GMT
RUN apt-get update     && DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends tzdata curl wget ca-certificates fontconfig locales     && echo "en_US.UTF-8 UTF-8" >> /etc/locale.gen     && locale-gen en_US.UTF-8     && rm -rf /var/lib/apt/lists/*
# Fri, 04 Nov 2022 22:40:54 GMT
ENV JAVA_VERSION=jdk-11.0.17+8
# Fri, 04 Nov 2022 22:41:33 GMT
RUN set -eux;     ARCH="$(dpkg --print-architecture)";     case "${ARCH}" in        aarch64|arm64)          ESUM='bd6efe3290c8b5a42f695a55a26f3e3c9c284288574879d4b7089f31f5114177';          BINARY_URL='https://github.com/adoptium/temurin11-binaries/releases/download/jdk-11.0.17%2B8/OpenJDK11U-jre_aarch64_linux_hotspot_11.0.17_8.tar.gz';          ;;        armhf|arm)          ESUM='8cf113d3d7fa808895c8d2e41bb890af21c47e38c2460e0588147a4bb8fc658d';          BINARY_URL='https://github.com/adoptium/temurin11-binaries/releases/download/jdk-11.0.17%2B8/OpenJDK11U-jre_arm_linux_hotspot_11.0.17_8.tar.gz';          ;;        ppc64el|powerpc:common64)          ESUM='0ca3d806131ab5834c501f9c625bb0248cd528af361c704503348e9c9605bedf';          BINARY_URL='https://github.com/adoptium/temurin11-binaries/releases/download/jdk-11.0.17%2B8/OpenJDK11U-jre_ppc64le_linux_hotspot_11.0.17_8.tar.gz';          ;;        s390x|s390:64-bit)          ESUM='dd3b159a374086e65cb07c4ccb226c90f9c02ef929cba6f0b642171d7ed97fa4';          BINARY_URL='https://github.com/adoptium/temurin11-binaries/releases/download/jdk-11.0.17%2B8/OpenJDK11U-jre_s390x_linux_hotspot_11.0.17_8.tar.gz';          ;;        amd64|i386:x86-64)          ESUM='752616097e09d7f60a3ad8bd312f90eaf50ac72577e55df229fe6e8091148f79';          BINARY_URL='https://github.com/adoptium/temurin11-binaries/releases/download/jdk-11.0.17%2B8/OpenJDK11U-jre_x64_linux_hotspot_11.0.17_8.tar.gz';          ;;        *)          echo "Unsupported arch: ${ARCH}";          exit 1;          ;;     esac; 	  wget -O /tmp/openjdk.tar.gz ${BINARY_URL}; 	  echo "${ESUM} */tmp/openjdk.tar.gz" | sha256sum -c -; 	  mkdir -p "$JAVA_HOME"; 	  tar --extract 	      --file /tmp/openjdk.tar.gz 	      --directory "$JAVA_HOME" 	      --strip-components 1 	      --no-same-owner 	  ;     rm /tmp/openjdk.tar.gz;     find "$JAVA_HOME/lib" -name '*.so' -exec dirname '{}' ';' | sort -u > /etc/ld.so.conf.d/docker-openjdk.conf;     ldconfig;     java -Xshare:dump;
# Fri, 04 Nov 2022 22:41:34 GMT
RUN echo Verifying install ...     && fileEncoding="$(echo 'System.out.println(System.getProperty("file.encoding"))' | jshell -s -)"; [ "$fileEncoding" = 'UTF-8' ]; rm -rf ~/.java     && echo java --version && java --version     && echo Complete.
# Fri, 04 Nov 2022 23:48:38 GMT
ENV CATALINA_HOME=/usr/local/tomcat
# Fri, 04 Nov 2022 23:48:38 GMT
ENV PATH=/usr/local/tomcat/bin:/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Fri, 04 Nov 2022 23:48:38 GMT
RUN mkdir -p "$CATALINA_HOME"
# Fri, 04 Nov 2022 23:48:39 GMT
WORKDIR /usr/local/tomcat
# Fri, 04 Nov 2022 23:48:39 GMT
ENV TOMCAT_NATIVE_LIBDIR=/usr/local/tomcat/native-jni-lib
# Fri, 04 Nov 2022 23:48:39 GMT
ENV LD_LIBRARY_PATH=/usr/local/tomcat/native-jni-lib
# Fri, 04 Nov 2022 23:53:12 GMT
ENV GPG_KEYS=48F8E69F6390C9F25CFEDCD268248959359E722B A9C5DF4D22E99998D9875A5110C01C5A2F6059E7 DCFD35E0BF8CA7344752DE8B6FB21E8933C60243
# Fri, 04 Nov 2022 23:53:12 GMT
ENV TOMCAT_MAJOR=9
# Tue, 15 Nov 2022 04:57:22 GMT
ENV TOMCAT_VERSION=9.0.69
# Tue, 15 Nov 2022 04:57:22 GMT
ENV TOMCAT_SHA512=8c883c54ce9ce43eba37756a6404cdf3477879883a3e6d146dc8a7aa5e0425f487466afe6b6da4a895927cb7cb59177b9379cec18000f2de12785be57408c779
# Tue, 15 Nov 2022 04:57:22 GMT
COPY dir:096b403a5f78b17e6b4bff63128a9c93941b97f22470991610dd641633d977f1 in /usr/local/tomcat 
# Tue, 15 Nov 2022 04:57:25 GMT
RUN set -eux; 	apt-get update; 	xargs -rt apt-get install -y --no-install-recommends < "$TOMCAT_NATIVE_LIBDIR/.dependencies.txt"; 	rm -rf /var/lib/apt/lists/*
# Tue, 15 Nov 2022 04:57:26 GMT
RUN set -eux; 	nativeLines="$(catalina.sh configtest 2>&1)"; 	nativeLines="$(echo "$nativeLines" | grep 'Apache Tomcat Native')"; 	nativeLines="$(echo "$nativeLines" | sort -u)"; 	if ! echo "$nativeLines" | grep -E 'INFO: Loaded( APR based)? Apache Tomcat Native library' >&2; then 		echo >&2 "$nativeLines"; 		exit 1; 	fi
# Tue, 15 Nov 2022 04:57:26 GMT
EXPOSE 8080
# Tue, 15 Nov 2022 04:57:27 GMT
CMD ["catalina.sh" "run"]
# Wed, 11 Jan 2023 03:05:10 GMT
LABEL org.opencontainers.image.authors=XWiki Development Team <committers@xwiki.org>
# Wed, 11 Jan 2023 03:05:10 GMT
LABEL org.opencontainers.image.url=https://hub.docker.com/_/xwiki
# Wed, 11 Jan 2023 03:05:10 GMT
LABEL org.opencontainers.image.documentation=https://hub.docker.com/_/xwiki
# Wed, 11 Jan 2023 03:05:10 GMT
LABEL org.opencontainers.image.source=https://github.com/xwiki/xwiki-docker.git
# Wed, 11 Jan 2023 03:05:11 GMT
LABEL org.opencontainers.image.vendor=xwiki.org
# Wed, 11 Jan 2023 03:05:11 GMT
LABEL org.opencontainers.image.licenses=LGPL-2.1
# Wed, 11 Jan 2023 03:07:37 GMT
RUN apt-get update &&   apt-get --no-install-recommends -y install     curl     libreoffice     unzip     procps &&   rm -rf /var/lib/apt/lists/*
# Tue, 31 Jan 2023 00:47:12 GMT
ENV XWIKI_VERSION=15.0
# Tue, 31 Jan 2023 00:47:12 GMT
ENV XWIKI_URL_PREFIX=https://maven.xwiki.org/releases/org/xwiki/platform/xwiki-platform-distribution-war/15.0
# Tue, 31 Jan 2023 00:47:12 GMT
ENV XWIKI_DOWNLOAD_SHA256=79ba0f479bbc49521c113821adc9d91141075a9470d7f9bbb6994ca59c30d121
# Tue, 31 Jan 2023 00:47:58 GMT
RUN rm -rf /usr/local/tomcat/webapps/* &&   mkdir -p /usr/local/tomcat/temp &&   mkdir -p /usr/local/xwiki/data &&   curl -fSL "${XWIKI_URL_PREFIX}/xwiki-platform-distribution-war-${XWIKI_VERSION}.war" -o xwiki.war &&   echo "$XWIKI_DOWNLOAD_SHA256 xwiki.war" | sha256sum -c - &&   unzip -d /usr/local/tomcat/webapps/ROOT xwiki.war &&   rm -f xwiki.war
# Tue, 31 Jan 2023 00:54:48 GMT
ENV MARIADB_JDBC_VERSION=3.1.1
# Tue, 31 Jan 2023 00:54:48 GMT
ENV MARIADB_JDBC_SHA256=a554541fd88047905fb0c4c10e1d85295f5e38c7bb5fb408b425392a79fc26e3
# Tue, 31 Jan 2023 00:54:48 GMT
ENV MARIADB_JDBC_PREFIX=https://repo1.maven.org/maven2/org/mariadb/jdbc/mariadb-java-client/3.1.1
# Tue, 31 Jan 2023 00:54:48 GMT
ENV MARIADB_JDBC_ARTIFACT=mariadb-java-client-3.1.1.jar
# Tue, 31 Jan 2023 00:54:48 GMT
ENV MARIADB_JDBC_TARGET=/usr/local/tomcat/webapps/ROOT/WEB-INF/lib/mariadb-java-client-3.1.1.jar
# Tue, 31 Jan 2023 00:54:49 GMT
RUN curl -fSL "${MARIADB_JDBC_PREFIX}/${MARIADB_JDBC_ARTIFACT}" -o $MARIADB_JDBC_TARGET &&   echo "$MARIADB_JDBC_SHA256 $MARIADB_JDBC_TARGET" | sha256sum -c -
# Tue, 31 Jan 2023 00:54:49 GMT
COPY file:0a1be11e2eb610a1dbcd415404e3a592641110b93090030cb831e3a19a163017 in /usr/local/tomcat/bin/ 
# Tue, 31 Jan 2023 00:54:49 GMT
COPY file:0e237c3876eeb3b5f3473a064d3e507da2df6c228ca714687930b34e3b687601 in /usr/local/tomcat/webapps/ROOT/WEB-INF/hibernate.cfg.xml 
# Tue, 31 Jan 2023 00:54:49 GMT
RUN sed -i 's/<id>org.xwiki.platform:xwiki-platform-distribution-war/<id>org.xwiki.platform:xwiki-platform-distribution-docker/'   /usr/local/tomcat/webapps/ROOT/META-INF/extension.xed
# Tue, 31 Jan 2023 00:54:49 GMT
COPY file:a47c4dcd87c9dad97aff38c49188357e6193bcad50757e516cfb08a60d4de611 in /usr/local/bin/docker-entrypoint.sh 
# Tue, 31 Jan 2023 00:54:49 GMT
VOLUME [/usr/local/xwiki]
# Tue, 31 Jan 2023 00:54:50 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 31 Jan 2023 00:54:50 GMT
CMD ["xwiki"]
```

-	Layers:
	-	`sha256:0509fae36eb0656f8bdb23f8ae64100d893bcea2563e97468d337e04d2d0410b`  
		Last Modified: Wed, 02 Nov 2022 18:50:21 GMT  
		Size: 28.4 MB (28382154 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e502a1af2bcd98f5f0d2f5e4da1a0e7bbe07a2c548e2662f7d37dce5ae1df46c`  
		Last Modified: Wed, 02 Nov 2022 19:48:28 GMT  
		Size: 12.4 MB (12396330 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bc4598c07dd818f03a0378b0341a4a8e80f0152fbb3e7d5246ca4f466f42e611`  
		Last Modified: Fri, 04 Nov 2022 22:46:46 GMT  
		Size: 45.0 MB (44958470 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:715a937a1066f998b331fcd62256ad01a5571bdf46804e97825afc64f9ebb427`  
		Last Modified: Fri, 04 Nov 2022 22:46:41 GMT  
		Size: 160.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5fb623f082f74b2fa9fc2c4e3f3a4802875cb9753cfa26ed940201ce72bb56cb`  
		Last Modified: Sat, 05 Nov 2022 00:03:40 GMT  
		Size: 172.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:33260b83200262bbd546be371ad3c1f50f5ae7228afb87982d6fa9d6b11bf26f`  
		Last Modified: Tue, 15 Nov 2022 05:10:19 GMT  
		Size: 12.2 MB (12207235 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0955fb697ea9b30a1b4f95385464f646aa1525cb6efba648e22df84ebef6b2ee`  
		Last Modified: Tue, 15 Nov 2022 05:10:18 GMT  
		Size: 452.0 KB (452021 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6eddcf66f2083b1487296a0308e0b058917c97f614f12428d82d89662038dc2e`  
		Last Modified: Tue, 15 Nov 2022 05:10:18 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ae5f60bb64f3fa11da3d15a9639f886186b4c2c021455c3f9db22e0cfe1b1311`  
		Last Modified: Wed, 11 Jan 2023 03:11:14 GMT  
		Size: 173.8 MB (173806827 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1814d85fce571b42f2cfa7c8a904e1a184ee6f49642242a44bbe0037088994a0`  
		Last Modified: Tue, 31 Jan 2023 00:56:04 GMT  
		Size: 307.1 MB (307117070 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e8637677b7ba0da683afa4e56ff0561e4ba77c8782d5a98da785f4ef58d1caf9`  
		Last Modified: Tue, 31 Jan 2023 00:57:14 GMT  
		Size: 589.7 KB (589677 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:61a67398bc888bcce1656edec9bb40409ce0ffc2fe83d0437c28dd64a8f697ce`  
		Last Modified: Tue, 31 Jan 2023 00:57:14 GMT  
		Size: 1.3 KB (1345 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7ebda7e506ea819ce9717c3d0334df81608bc4c7149cd47ebc9a32790141a637`  
		Last Modified: Tue, 31 Jan 2023 00:57:14 GMT  
		Size: 2.3 KB (2313 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2ceebbf08640e235a928c9df650ca3ab8d0c6b506faa158ecde5fdde34bf8813`  
		Last Modified: Tue, 31 Jan 2023 00:57:14 GMT  
		Size: 6.0 KB (6007 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:12b1d23eae23b1a09ecd4185941d43f13d4ad633d4c6257ab8107a8eebd5fb12`  
		Last Modified: Tue, 31 Jan 2023 00:57:14 GMT  
		Size: 2.5 KB (2506 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `xwiki:15.0-mysql-tomcat`

```console
$ docker pull xwiki@sha256:33e789838f82ce73efec6664859feb1ced7a5b7605fbfaddb81916716bce524f
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `xwiki:15.0-mysql-tomcat` - linux; amd64

```console
$ docker pull xwiki@sha256:481fdb46e8c043a6709d11310e2083ce71d6ba63ee6517f84da3ba06f320598e
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **590.5 MB (590459982 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:bd630aa0aa5c679e23ea7d52cbbdd6b817eab27a820c25d3c50b54eca83b9744`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["xwiki"]`

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
# Wed, 02 Nov 2022 18:44:10 GMT
RUN apt-get update     && DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends tzdata curl wget ca-certificates fontconfig locales     && echo "en_US.UTF-8 UTF-8" >> /etc/locale.gen     && locale-gen en_US.UTF-8     && rm -rf /var/lib/apt/lists/*
# Fri, 04 Nov 2022 23:21:41 GMT
ENV JAVA_VERSION=jdk-11.0.17+8
# Fri, 04 Nov 2022 23:22:31 GMT
RUN set -eux;     ARCH="$(dpkg --print-architecture)";     case "${ARCH}" in        aarch64|arm64)          ESUM='bd6efe3290c8b5a42f695a55a26f3e3c9c284288574879d4b7089f31f5114177';          BINARY_URL='https://github.com/adoptium/temurin11-binaries/releases/download/jdk-11.0.17%2B8/OpenJDK11U-jre_aarch64_linux_hotspot_11.0.17_8.tar.gz';          ;;        armhf|arm)          ESUM='8cf113d3d7fa808895c8d2e41bb890af21c47e38c2460e0588147a4bb8fc658d';          BINARY_URL='https://github.com/adoptium/temurin11-binaries/releases/download/jdk-11.0.17%2B8/OpenJDK11U-jre_arm_linux_hotspot_11.0.17_8.tar.gz';          ;;        ppc64el|powerpc:common64)          ESUM='0ca3d806131ab5834c501f9c625bb0248cd528af361c704503348e9c9605bedf';          BINARY_URL='https://github.com/adoptium/temurin11-binaries/releases/download/jdk-11.0.17%2B8/OpenJDK11U-jre_ppc64le_linux_hotspot_11.0.17_8.tar.gz';          ;;        s390x|s390:64-bit)          ESUM='dd3b159a374086e65cb07c4ccb226c90f9c02ef929cba6f0b642171d7ed97fa4';          BINARY_URL='https://github.com/adoptium/temurin11-binaries/releases/download/jdk-11.0.17%2B8/OpenJDK11U-jre_s390x_linux_hotspot_11.0.17_8.tar.gz';          ;;        amd64|i386:x86-64)          ESUM='752616097e09d7f60a3ad8bd312f90eaf50ac72577e55df229fe6e8091148f79';          BINARY_URL='https://github.com/adoptium/temurin11-binaries/releases/download/jdk-11.0.17%2B8/OpenJDK11U-jre_x64_linux_hotspot_11.0.17_8.tar.gz';          ;;        *)          echo "Unsupported arch: ${ARCH}";          exit 1;          ;;     esac; 	  wget -O /tmp/openjdk.tar.gz ${BINARY_URL}; 	  echo "${ESUM} */tmp/openjdk.tar.gz" | sha256sum -c -; 	  mkdir -p "$JAVA_HOME"; 	  tar --extract 	      --file /tmp/openjdk.tar.gz 	      --directory "$JAVA_HOME" 	      --strip-components 1 	      --no-same-owner 	  ;     rm /tmp/openjdk.tar.gz;     find "$JAVA_HOME/lib" -name '*.so' -exec dirname '{}' ';' | sort -u > /etc/ld.so.conf.d/docker-openjdk.conf;     ldconfig;     java -Xshare:dump;
# Fri, 04 Nov 2022 23:22:32 GMT
RUN echo Verifying install ...     && fileEncoding="$(echo 'System.out.println(System.getProperty("file.encoding"))' | jshell -s -)"; [ "$fileEncoding" = 'UTF-8' ]; rm -rf ~/.java     && echo java --version && java --version     && echo Complete.
# Sat, 05 Nov 2022 01:35:16 GMT
ENV CATALINA_HOME=/usr/local/tomcat
# Sat, 05 Nov 2022 01:35:16 GMT
ENV PATH=/usr/local/tomcat/bin:/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Sat, 05 Nov 2022 01:35:17 GMT
RUN mkdir -p "$CATALINA_HOME"
# Sat, 05 Nov 2022 01:35:17 GMT
WORKDIR /usr/local/tomcat
# Sat, 05 Nov 2022 01:35:17 GMT
ENV TOMCAT_NATIVE_LIBDIR=/usr/local/tomcat/native-jni-lib
# Sat, 05 Nov 2022 01:35:17 GMT
ENV LD_LIBRARY_PATH=/usr/local/tomcat/native-jni-lib
# Sat, 05 Nov 2022 01:39:54 GMT
ENV GPG_KEYS=48F8E69F6390C9F25CFEDCD268248959359E722B A9C5DF4D22E99998D9875A5110C01C5A2F6059E7 DCFD35E0BF8CA7344752DE8B6FB21E8933C60243
# Sat, 05 Nov 2022 01:39:54 GMT
ENV TOMCAT_MAJOR=9
# Tue, 15 Nov 2022 03:06:43 GMT
ENV TOMCAT_VERSION=9.0.69
# Tue, 15 Nov 2022 03:06:43 GMT
ENV TOMCAT_SHA512=8c883c54ce9ce43eba37756a6404cdf3477879883a3e6d146dc8a7aa5e0425f487466afe6b6da4a895927cb7cb59177b9379cec18000f2de12785be57408c779
# Tue, 15 Nov 2022 03:06:44 GMT
COPY dir:b1a33aa3993dbbfbebb33bd9aa546b60c2f2191abf1227f453d4e830f6deb35f in /usr/local/tomcat 
# Tue, 15 Nov 2022 03:06:48 GMT
RUN set -eux; 	apt-get update; 	xargs -rt apt-get install -y --no-install-recommends < "$TOMCAT_NATIVE_LIBDIR/.dependencies.txt"; 	rm -rf /var/lib/apt/lists/*
# Tue, 15 Nov 2022 03:06:49 GMT
RUN set -eux; 	nativeLines="$(catalina.sh configtest 2>&1)"; 	nativeLines="$(echo "$nativeLines" | grep 'Apache Tomcat Native')"; 	nativeLines="$(echo "$nativeLines" | sort -u)"; 	if ! echo "$nativeLines" | grep -E 'INFO: Loaded( APR based)? Apache Tomcat Native library' >&2; then 		echo >&2 "$nativeLines"; 		exit 1; 	fi
# Tue, 15 Nov 2022 03:06:49 GMT
EXPOSE 8080
# Tue, 15 Nov 2022 03:06:49 GMT
CMD ["catalina.sh" "run"]
# Wed, 11 Jan 2023 02:47:03 GMT
LABEL org.opencontainers.image.authors=XWiki Development Team <committers@xwiki.org>
# Wed, 11 Jan 2023 02:47:03 GMT
LABEL org.opencontainers.image.url=https://hub.docker.com/_/xwiki
# Wed, 11 Jan 2023 02:47:03 GMT
LABEL org.opencontainers.image.documentation=https://hub.docker.com/_/xwiki
# Wed, 11 Jan 2023 02:47:03 GMT
LABEL org.opencontainers.image.source=https://github.com/xwiki/xwiki-docker.git
# Wed, 11 Jan 2023 02:47:04 GMT
LABEL org.opencontainers.image.vendor=xwiki.org
# Wed, 11 Jan 2023 02:47:04 GMT
LABEL org.opencontainers.image.licenses=LGPL-2.1
# Wed, 11 Jan 2023 02:49:03 GMT
RUN apt-get update &&   apt-get --no-install-recommends -y install     curl     libreoffice     unzip     procps &&   rm -rf /var/lib/apt/lists/*
# Tue, 31 Jan 2023 00:20:17 GMT
ENV XWIKI_VERSION=15.0
# Tue, 31 Jan 2023 00:20:17 GMT
ENV XWIKI_URL_PREFIX=https://maven.xwiki.org/releases/org/xwiki/platform/xwiki-platform-distribution-war/15.0
# Tue, 31 Jan 2023 00:20:17 GMT
ENV XWIKI_DOWNLOAD_SHA256=79ba0f479bbc49521c113821adc9d91141075a9470d7f9bbb6994ca59c30d121
# Tue, 31 Jan 2023 00:21:18 GMT
RUN rm -rf /usr/local/tomcat/webapps/* &&   mkdir -p /usr/local/tomcat/temp &&   mkdir -p /usr/local/xwiki/data &&   curl -fSL "${XWIKI_URL_PREFIX}/xwiki-platform-distribution-war-${XWIKI_VERSION}.war" -o xwiki.war &&   echo "$XWIKI_DOWNLOAD_SHA256 xwiki.war" | sha256sum -c - &&   unzip -d /usr/local/tomcat/webapps/ROOT xwiki.war &&   rm -f xwiki.war
# Tue, 31 Jan 2023 00:21:19 GMT
ENV MYSQL_JDBC_VERSION=8.0.31
# Tue, 31 Jan 2023 00:21:19 GMT
ENV MYSQL_JDBC_SHA256=5249e3dc6d6531b37790e3f61845b96db5e41e891d3d8edb0e2e3a1b53ca2f4f
# Tue, 31 Jan 2023 00:21:19 GMT
ENV MYSQL_JDBC_PREFIX=https://repo1.maven.org/maven2/com/mysql/mysql-connector-j/8.0.31
# Tue, 31 Jan 2023 00:21:19 GMT
ENV MYSQL_JDBC_ARTIFACT=mysql-connector-j-8.0.31.jar
# Tue, 31 Jan 2023 00:21:19 GMT
ENV MYSQL_JDBC_TARGET=/usr/local/tomcat/webapps/ROOT/WEB-INF/lib/mysql-connector-j-8.0.31.jar
# Tue, 31 Jan 2023 00:21:20 GMT
RUN curl -fSL "${MYSQL_JDBC_PREFIX}/${MYSQL_JDBC_ARTIFACT}" -o $MYSQL_JDBC_TARGET &&   echo "$MYSQL_JDBC_SHA256 $MYSQL_JDBC_TARGET" | sha256sum -c -
# Tue, 31 Jan 2023 00:21:21 GMT
COPY file:0a1be11e2eb610a1dbcd415404e3a592641110b93090030cb831e3a19a163017 in /usr/local/tomcat/bin/ 
# Tue, 31 Jan 2023 00:21:21 GMT
COPY file:1b8409986f3e4eb79a7a0b18472cb2692a61d504fb5ef34292bc997b79fd760d in /usr/local/tomcat/webapps/ROOT/WEB-INF/hibernate.cfg.xml 
# Tue, 31 Jan 2023 00:21:21 GMT
RUN sed -i 's/<id>org.xwiki.platform:xwiki-platform-distribution-war/<id>org.xwiki.platform:xwiki-platform-distribution-docker/'   /usr/local/tomcat/webapps/ROOT/META-INF/extension.xed
# Tue, 31 Jan 2023 00:21:21 GMT
COPY file:a47c4dcd87c9dad97aff38c49188357e6193bcad50757e516cfb08a60d4de611 in /usr/local/bin/docker-entrypoint.sh 
# Tue, 31 Jan 2023 00:21:22 GMT
VOLUME [/usr/local/xwiki]
# Tue, 31 Jan 2023 00:21:22 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 31 Jan 2023 00:21:22 GMT
CMD ["xwiki"]
```

-	Layers:
	-	`sha256:e96e057aae67380a4ddb16c337c5c3669d97fdff69ec537f02aa2cc30d814281`  
		Last Modified: Wed, 02 Nov 2022 03:03:36 GMT  
		Size: 30.4 MB (30425607 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4ced2591451da3a02e2b6bb44752b9e3f00d77789921be4df5082fb9f9880ad0`  
		Last Modified: Wed, 02 Nov 2022 18:48:43 GMT  
		Size: 12.4 MB (12439006 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:df8f874ae8c08a9e69e5fbe6c5a64200a45386132a3203d1a9a7f1146d94cfbc`  
		Last Modified: Fri, 04 Nov 2022 23:29:33 GMT  
		Size: 46.6 MB (46629936 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:111b6c7486426c4b6989102c2ee5be856e8a58e20ab0a350b24a905d536e8e7f`  
		Last Modified: Fri, 04 Nov 2022 23:29:26 GMT  
		Size: 161.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e6f84dce457c6d4f7b7291fce05f8e77998a3a7722a54125a1f1d52ca83043b4`  
		Last Modified: Sat, 05 Nov 2022 01:50:51 GMT  
		Size: 173.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a6c26749ee782392e38845ee2ba79b0da586ef6a45d8e7f29c7af14612278547`  
		Last Modified: Tue, 15 Nov 2022 03:19:57 GMT  
		Size: 12.2 MB (12200249 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4dddc6d9fa6024025b3fcfe729cab2dc544fb25476eca6e80b1af8e8d93bb0ee`  
		Last Modified: Tue, 15 Nov 2022 03:19:56 GMT  
		Size: 452.7 KB (452680 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:06637eebe5e72c8ad9019ad4eb4cdde1f11f7d4c24c7ed7374cf8966343aa2fb`  
		Last Modified: Tue, 15 Nov 2022 03:19:56 GMT  
		Size: 131.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b276fb8390410a8208724033e325715ea26000d5a1a762d4c3699b927884fbfe`  
		Last Modified: Wed, 11 Jan 2023 02:52:45 GMT  
		Size: 178.8 MB (178805608 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:156ca91198173149698aa0396648a9608b6ab1f2bc2666800843ce33c9f85b6e`  
		Last Modified: Tue, 31 Jan 2023 00:24:09 GMT  
		Size: 307.1 MB (307117069 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4c8b70d250c6d507901857473b0dcb67132d7b2a30ce9a69b07b1036853df738`  
		Last Modified: Tue, 31 Jan 2023 00:23:52 GMT  
		Size: 2.4 MB (2377191 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a9681fd36be674d25231c69d6a39f9e8fa65034eeaef5d1bd885fdbeac7f0f6b`  
		Last Modified: Tue, 31 Jan 2023 00:23:51 GMT  
		Size: 1.3 KB (1346 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a9d0d5da840f4d7da9943942b38cd092fae11f41dc6c19afd58d655cd6192d66`  
		Last Modified: Tue, 31 Jan 2023 00:23:51 GMT  
		Size: 2.3 KB (2312 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d65610da4f1da86fea8fbec0189b066afd4b86e4e8f7d049e3c4bc6ade9ba90a`  
		Last Modified: Tue, 31 Jan 2023 00:23:51 GMT  
		Size: 6.0 KB (6009 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3d41686284d7675eaa0f92c9cc27ebe73b4c30768c8eef9f23ee3b1ad06da00a`  
		Last Modified: Tue, 31 Jan 2023 00:23:51 GMT  
		Size: 2.5 KB (2504 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `xwiki:15.0-mysql-tomcat` - linux; arm64 variant v8

```console
$ docker pull xwiki@sha256:6bf63d9025b07b69d744200c05efd4ffb8a52f3c38380f5d59a0b48514203cd2
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **581.7 MB (581709921 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:6600f2bb05836c703d53944bbcb5399d509a9813a27a35e99ff717becc308330`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["xwiki"]`

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
# Wed, 02 Nov 2022 19:44:32 GMT
RUN apt-get update     && DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends tzdata curl wget ca-certificates fontconfig locales     && echo "en_US.UTF-8 UTF-8" >> /etc/locale.gen     && locale-gen en_US.UTF-8     && rm -rf /var/lib/apt/lists/*
# Fri, 04 Nov 2022 22:40:54 GMT
ENV JAVA_VERSION=jdk-11.0.17+8
# Fri, 04 Nov 2022 22:41:33 GMT
RUN set -eux;     ARCH="$(dpkg --print-architecture)";     case "${ARCH}" in        aarch64|arm64)          ESUM='bd6efe3290c8b5a42f695a55a26f3e3c9c284288574879d4b7089f31f5114177';          BINARY_URL='https://github.com/adoptium/temurin11-binaries/releases/download/jdk-11.0.17%2B8/OpenJDK11U-jre_aarch64_linux_hotspot_11.0.17_8.tar.gz';          ;;        armhf|arm)          ESUM='8cf113d3d7fa808895c8d2e41bb890af21c47e38c2460e0588147a4bb8fc658d';          BINARY_URL='https://github.com/adoptium/temurin11-binaries/releases/download/jdk-11.0.17%2B8/OpenJDK11U-jre_arm_linux_hotspot_11.0.17_8.tar.gz';          ;;        ppc64el|powerpc:common64)          ESUM='0ca3d806131ab5834c501f9c625bb0248cd528af361c704503348e9c9605bedf';          BINARY_URL='https://github.com/adoptium/temurin11-binaries/releases/download/jdk-11.0.17%2B8/OpenJDK11U-jre_ppc64le_linux_hotspot_11.0.17_8.tar.gz';          ;;        s390x|s390:64-bit)          ESUM='dd3b159a374086e65cb07c4ccb226c90f9c02ef929cba6f0b642171d7ed97fa4';          BINARY_URL='https://github.com/adoptium/temurin11-binaries/releases/download/jdk-11.0.17%2B8/OpenJDK11U-jre_s390x_linux_hotspot_11.0.17_8.tar.gz';          ;;        amd64|i386:x86-64)          ESUM='752616097e09d7f60a3ad8bd312f90eaf50ac72577e55df229fe6e8091148f79';          BINARY_URL='https://github.com/adoptium/temurin11-binaries/releases/download/jdk-11.0.17%2B8/OpenJDK11U-jre_x64_linux_hotspot_11.0.17_8.tar.gz';          ;;        *)          echo "Unsupported arch: ${ARCH}";          exit 1;          ;;     esac; 	  wget -O /tmp/openjdk.tar.gz ${BINARY_URL}; 	  echo "${ESUM} */tmp/openjdk.tar.gz" | sha256sum -c -; 	  mkdir -p "$JAVA_HOME"; 	  tar --extract 	      --file /tmp/openjdk.tar.gz 	      --directory "$JAVA_HOME" 	      --strip-components 1 	      --no-same-owner 	  ;     rm /tmp/openjdk.tar.gz;     find "$JAVA_HOME/lib" -name '*.so' -exec dirname '{}' ';' | sort -u > /etc/ld.so.conf.d/docker-openjdk.conf;     ldconfig;     java -Xshare:dump;
# Fri, 04 Nov 2022 22:41:34 GMT
RUN echo Verifying install ...     && fileEncoding="$(echo 'System.out.println(System.getProperty("file.encoding"))' | jshell -s -)"; [ "$fileEncoding" = 'UTF-8' ]; rm -rf ~/.java     && echo java --version && java --version     && echo Complete.
# Fri, 04 Nov 2022 23:48:38 GMT
ENV CATALINA_HOME=/usr/local/tomcat
# Fri, 04 Nov 2022 23:48:38 GMT
ENV PATH=/usr/local/tomcat/bin:/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Fri, 04 Nov 2022 23:48:38 GMT
RUN mkdir -p "$CATALINA_HOME"
# Fri, 04 Nov 2022 23:48:39 GMT
WORKDIR /usr/local/tomcat
# Fri, 04 Nov 2022 23:48:39 GMT
ENV TOMCAT_NATIVE_LIBDIR=/usr/local/tomcat/native-jni-lib
# Fri, 04 Nov 2022 23:48:39 GMT
ENV LD_LIBRARY_PATH=/usr/local/tomcat/native-jni-lib
# Fri, 04 Nov 2022 23:53:12 GMT
ENV GPG_KEYS=48F8E69F6390C9F25CFEDCD268248959359E722B A9C5DF4D22E99998D9875A5110C01C5A2F6059E7 DCFD35E0BF8CA7344752DE8B6FB21E8933C60243
# Fri, 04 Nov 2022 23:53:12 GMT
ENV TOMCAT_MAJOR=9
# Tue, 15 Nov 2022 04:57:22 GMT
ENV TOMCAT_VERSION=9.0.69
# Tue, 15 Nov 2022 04:57:22 GMT
ENV TOMCAT_SHA512=8c883c54ce9ce43eba37756a6404cdf3477879883a3e6d146dc8a7aa5e0425f487466afe6b6da4a895927cb7cb59177b9379cec18000f2de12785be57408c779
# Tue, 15 Nov 2022 04:57:22 GMT
COPY dir:096b403a5f78b17e6b4bff63128a9c93941b97f22470991610dd641633d977f1 in /usr/local/tomcat 
# Tue, 15 Nov 2022 04:57:25 GMT
RUN set -eux; 	apt-get update; 	xargs -rt apt-get install -y --no-install-recommends < "$TOMCAT_NATIVE_LIBDIR/.dependencies.txt"; 	rm -rf /var/lib/apt/lists/*
# Tue, 15 Nov 2022 04:57:26 GMT
RUN set -eux; 	nativeLines="$(catalina.sh configtest 2>&1)"; 	nativeLines="$(echo "$nativeLines" | grep 'Apache Tomcat Native')"; 	nativeLines="$(echo "$nativeLines" | sort -u)"; 	if ! echo "$nativeLines" | grep -E 'INFO: Loaded( APR based)? Apache Tomcat Native library' >&2; then 		echo >&2 "$nativeLines"; 		exit 1; 	fi
# Tue, 15 Nov 2022 04:57:26 GMT
EXPOSE 8080
# Tue, 15 Nov 2022 04:57:27 GMT
CMD ["catalina.sh" "run"]
# Wed, 11 Jan 2023 03:05:10 GMT
LABEL org.opencontainers.image.authors=XWiki Development Team <committers@xwiki.org>
# Wed, 11 Jan 2023 03:05:10 GMT
LABEL org.opencontainers.image.url=https://hub.docker.com/_/xwiki
# Wed, 11 Jan 2023 03:05:10 GMT
LABEL org.opencontainers.image.documentation=https://hub.docker.com/_/xwiki
# Wed, 11 Jan 2023 03:05:10 GMT
LABEL org.opencontainers.image.source=https://github.com/xwiki/xwiki-docker.git
# Wed, 11 Jan 2023 03:05:11 GMT
LABEL org.opencontainers.image.vendor=xwiki.org
# Wed, 11 Jan 2023 03:05:11 GMT
LABEL org.opencontainers.image.licenses=LGPL-2.1
# Wed, 11 Jan 2023 03:07:37 GMT
RUN apt-get update &&   apt-get --no-install-recommends -y install     curl     libreoffice     unzip     procps &&   rm -rf /var/lib/apt/lists/*
# Tue, 31 Jan 2023 00:47:12 GMT
ENV XWIKI_VERSION=15.0
# Tue, 31 Jan 2023 00:47:12 GMT
ENV XWIKI_URL_PREFIX=https://maven.xwiki.org/releases/org/xwiki/platform/xwiki-platform-distribution-war/15.0
# Tue, 31 Jan 2023 00:47:12 GMT
ENV XWIKI_DOWNLOAD_SHA256=79ba0f479bbc49521c113821adc9d91141075a9470d7f9bbb6994ca59c30d121
# Tue, 31 Jan 2023 00:47:58 GMT
RUN rm -rf /usr/local/tomcat/webapps/* &&   mkdir -p /usr/local/tomcat/temp &&   mkdir -p /usr/local/xwiki/data &&   curl -fSL "${XWIKI_URL_PREFIX}/xwiki-platform-distribution-war-${XWIKI_VERSION}.war" -o xwiki.war &&   echo "$XWIKI_DOWNLOAD_SHA256 xwiki.war" | sha256sum -c - &&   unzip -d /usr/local/tomcat/webapps/ROOT xwiki.war &&   rm -f xwiki.war
# Tue, 31 Jan 2023 00:48:01 GMT
ENV MYSQL_JDBC_VERSION=8.0.31
# Tue, 31 Jan 2023 00:48:01 GMT
ENV MYSQL_JDBC_SHA256=5249e3dc6d6531b37790e3f61845b96db5e41e891d3d8edb0e2e3a1b53ca2f4f
# Tue, 31 Jan 2023 00:48:01 GMT
ENV MYSQL_JDBC_PREFIX=https://repo1.maven.org/maven2/com/mysql/mysql-connector-j/8.0.31
# Tue, 31 Jan 2023 00:48:01 GMT
ENV MYSQL_JDBC_ARTIFACT=mysql-connector-j-8.0.31.jar
# Tue, 31 Jan 2023 00:48:01 GMT
ENV MYSQL_JDBC_TARGET=/usr/local/tomcat/webapps/ROOT/WEB-INF/lib/mysql-connector-j-8.0.31.jar
# Tue, 31 Jan 2023 00:48:02 GMT
RUN curl -fSL "${MYSQL_JDBC_PREFIX}/${MYSQL_JDBC_ARTIFACT}" -o $MYSQL_JDBC_TARGET &&   echo "$MYSQL_JDBC_SHA256 $MYSQL_JDBC_TARGET" | sha256sum -c -
# Tue, 31 Jan 2023 00:48:02 GMT
COPY file:0a1be11e2eb610a1dbcd415404e3a592641110b93090030cb831e3a19a163017 in /usr/local/tomcat/bin/ 
# Tue, 31 Jan 2023 00:48:02 GMT
COPY file:1b8409986f3e4eb79a7a0b18472cb2692a61d504fb5ef34292bc997b79fd760d in /usr/local/tomcat/webapps/ROOT/WEB-INF/hibernate.cfg.xml 
# Tue, 31 Jan 2023 00:48:03 GMT
RUN sed -i 's/<id>org.xwiki.platform:xwiki-platform-distribution-war/<id>org.xwiki.platform:xwiki-platform-distribution-docker/'   /usr/local/tomcat/webapps/ROOT/META-INF/extension.xed
# Tue, 31 Jan 2023 00:48:03 GMT
COPY file:a47c4dcd87c9dad97aff38c49188357e6193bcad50757e516cfb08a60d4de611 in /usr/local/bin/docker-entrypoint.sh 
# Tue, 31 Jan 2023 00:48:03 GMT
VOLUME [/usr/local/xwiki]
# Tue, 31 Jan 2023 00:48:03 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 31 Jan 2023 00:48:03 GMT
CMD ["xwiki"]
```

-	Layers:
	-	`sha256:0509fae36eb0656f8bdb23f8ae64100d893bcea2563e97468d337e04d2d0410b`  
		Last Modified: Wed, 02 Nov 2022 18:50:21 GMT  
		Size: 28.4 MB (28382154 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e502a1af2bcd98f5f0d2f5e4da1a0e7bbe07a2c548e2662f7d37dce5ae1df46c`  
		Last Modified: Wed, 02 Nov 2022 19:48:28 GMT  
		Size: 12.4 MB (12396330 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bc4598c07dd818f03a0378b0341a4a8e80f0152fbb3e7d5246ca4f466f42e611`  
		Last Modified: Fri, 04 Nov 2022 22:46:46 GMT  
		Size: 45.0 MB (44958470 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:715a937a1066f998b331fcd62256ad01a5571bdf46804e97825afc64f9ebb427`  
		Last Modified: Fri, 04 Nov 2022 22:46:41 GMT  
		Size: 160.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5fb623f082f74b2fa9fc2c4e3f3a4802875cb9753cfa26ed940201ce72bb56cb`  
		Last Modified: Sat, 05 Nov 2022 00:03:40 GMT  
		Size: 172.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:33260b83200262bbd546be371ad3c1f50f5ae7228afb87982d6fa9d6b11bf26f`  
		Last Modified: Tue, 15 Nov 2022 05:10:19 GMT  
		Size: 12.2 MB (12207235 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0955fb697ea9b30a1b4f95385464f646aa1525cb6efba648e22df84ebef6b2ee`  
		Last Modified: Tue, 15 Nov 2022 05:10:18 GMT  
		Size: 452.0 KB (452021 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6eddcf66f2083b1487296a0308e0b058917c97f614f12428d82d89662038dc2e`  
		Last Modified: Tue, 15 Nov 2022 05:10:18 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ae5f60bb64f3fa11da3d15a9639f886186b4c2c021455c3f9db22e0cfe1b1311`  
		Last Modified: Wed, 11 Jan 2023 03:11:14 GMT  
		Size: 173.8 MB (173806827 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1814d85fce571b42f2cfa7c8a904e1a184ee6f49642242a44bbe0037088994a0`  
		Last Modified: Tue, 31 Jan 2023 00:56:04 GMT  
		Size: 307.1 MB (307117070 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8aec0e24b4fa870989f014944c3c7d535355a2371fc8c948b2b11f9b377efe6e`  
		Last Modified: Tue, 31 Jan 2023 00:55:50 GMT  
		Size: 2.4 MB (2377182 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0b65081619aa0114a7f367836ef421eb8d951e559e0f089c7728af7813b1ea62`  
		Last Modified: Tue, 31 Jan 2023 00:55:49 GMT  
		Size: 1.3 KB (1348 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:46ebad072e608146426d8dc30828937049eea36c2e636d7790b4960d6d586977`  
		Last Modified: Tue, 31 Jan 2023 00:55:49 GMT  
		Size: 2.3 KB (2308 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:708fefcedd4ee6c106da247a68c5790f5ab00225d1cdfff8465575265c3a54e6`  
		Last Modified: Tue, 31 Jan 2023 00:55:49 GMT  
		Size: 6.0 KB (6008 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:81e3bf8e20bc921031e7549a41dec1b2d7795cc6da40a0e7096bf654b25c5c3e`  
		Last Modified: Tue, 31 Jan 2023 00:55:49 GMT  
		Size: 2.5 KB (2507 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `xwiki:15.0-postgres-tomcat`

```console
$ docker pull xwiki@sha256:f6739c1133cbbece87973ddea5fbc57222abb9d7d3f8064eee9d2c2c0d46ecfa
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `xwiki:15.0-postgres-tomcat` - linux; amd64

```console
$ docker pull xwiki@sha256:72928baeace929e42f17f01362700392a90c6750b2ec1f84f24bbba1c4ff0236
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **590.0 MB (589959353 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b71f03d7d3a1760e73e6f4370f49317d16a7e0cb22532f49c11c0ee73b2c6262`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["xwiki"]`

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
# Wed, 02 Nov 2022 18:44:10 GMT
RUN apt-get update     && DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends tzdata curl wget ca-certificates fontconfig locales     && echo "en_US.UTF-8 UTF-8" >> /etc/locale.gen     && locale-gen en_US.UTF-8     && rm -rf /var/lib/apt/lists/*
# Fri, 04 Nov 2022 23:21:41 GMT
ENV JAVA_VERSION=jdk-11.0.17+8
# Fri, 04 Nov 2022 23:22:31 GMT
RUN set -eux;     ARCH="$(dpkg --print-architecture)";     case "${ARCH}" in        aarch64|arm64)          ESUM='bd6efe3290c8b5a42f695a55a26f3e3c9c284288574879d4b7089f31f5114177';          BINARY_URL='https://github.com/adoptium/temurin11-binaries/releases/download/jdk-11.0.17%2B8/OpenJDK11U-jre_aarch64_linux_hotspot_11.0.17_8.tar.gz';          ;;        armhf|arm)          ESUM='8cf113d3d7fa808895c8d2e41bb890af21c47e38c2460e0588147a4bb8fc658d';          BINARY_URL='https://github.com/adoptium/temurin11-binaries/releases/download/jdk-11.0.17%2B8/OpenJDK11U-jre_arm_linux_hotspot_11.0.17_8.tar.gz';          ;;        ppc64el|powerpc:common64)          ESUM='0ca3d806131ab5834c501f9c625bb0248cd528af361c704503348e9c9605bedf';          BINARY_URL='https://github.com/adoptium/temurin11-binaries/releases/download/jdk-11.0.17%2B8/OpenJDK11U-jre_ppc64le_linux_hotspot_11.0.17_8.tar.gz';          ;;        s390x|s390:64-bit)          ESUM='dd3b159a374086e65cb07c4ccb226c90f9c02ef929cba6f0b642171d7ed97fa4';          BINARY_URL='https://github.com/adoptium/temurin11-binaries/releases/download/jdk-11.0.17%2B8/OpenJDK11U-jre_s390x_linux_hotspot_11.0.17_8.tar.gz';          ;;        amd64|i386:x86-64)          ESUM='752616097e09d7f60a3ad8bd312f90eaf50ac72577e55df229fe6e8091148f79';          BINARY_URL='https://github.com/adoptium/temurin11-binaries/releases/download/jdk-11.0.17%2B8/OpenJDK11U-jre_x64_linux_hotspot_11.0.17_8.tar.gz';          ;;        *)          echo "Unsupported arch: ${ARCH}";          exit 1;          ;;     esac; 	  wget -O /tmp/openjdk.tar.gz ${BINARY_URL}; 	  echo "${ESUM} */tmp/openjdk.tar.gz" | sha256sum -c -; 	  mkdir -p "$JAVA_HOME"; 	  tar --extract 	      --file /tmp/openjdk.tar.gz 	      --directory "$JAVA_HOME" 	      --strip-components 1 	      --no-same-owner 	  ;     rm /tmp/openjdk.tar.gz;     find "$JAVA_HOME/lib" -name '*.so' -exec dirname '{}' ';' | sort -u > /etc/ld.so.conf.d/docker-openjdk.conf;     ldconfig;     java -Xshare:dump;
# Fri, 04 Nov 2022 23:22:32 GMT
RUN echo Verifying install ...     && fileEncoding="$(echo 'System.out.println(System.getProperty("file.encoding"))' | jshell -s -)"; [ "$fileEncoding" = 'UTF-8' ]; rm -rf ~/.java     && echo java --version && java --version     && echo Complete.
# Sat, 05 Nov 2022 01:35:16 GMT
ENV CATALINA_HOME=/usr/local/tomcat
# Sat, 05 Nov 2022 01:35:16 GMT
ENV PATH=/usr/local/tomcat/bin:/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Sat, 05 Nov 2022 01:35:17 GMT
RUN mkdir -p "$CATALINA_HOME"
# Sat, 05 Nov 2022 01:35:17 GMT
WORKDIR /usr/local/tomcat
# Sat, 05 Nov 2022 01:35:17 GMT
ENV TOMCAT_NATIVE_LIBDIR=/usr/local/tomcat/native-jni-lib
# Sat, 05 Nov 2022 01:35:17 GMT
ENV LD_LIBRARY_PATH=/usr/local/tomcat/native-jni-lib
# Sat, 05 Nov 2022 01:39:54 GMT
ENV GPG_KEYS=48F8E69F6390C9F25CFEDCD268248959359E722B A9C5DF4D22E99998D9875A5110C01C5A2F6059E7 DCFD35E0BF8CA7344752DE8B6FB21E8933C60243
# Sat, 05 Nov 2022 01:39:54 GMT
ENV TOMCAT_MAJOR=9
# Tue, 15 Nov 2022 03:06:43 GMT
ENV TOMCAT_VERSION=9.0.69
# Tue, 15 Nov 2022 03:06:43 GMT
ENV TOMCAT_SHA512=8c883c54ce9ce43eba37756a6404cdf3477879883a3e6d146dc8a7aa5e0425f487466afe6b6da4a895927cb7cb59177b9379cec18000f2de12785be57408c779
# Tue, 15 Nov 2022 03:06:44 GMT
COPY dir:b1a33aa3993dbbfbebb33bd9aa546b60c2f2191abf1227f453d4e830f6deb35f in /usr/local/tomcat 
# Tue, 15 Nov 2022 03:06:48 GMT
RUN set -eux; 	apt-get update; 	xargs -rt apt-get install -y --no-install-recommends < "$TOMCAT_NATIVE_LIBDIR/.dependencies.txt"; 	rm -rf /var/lib/apt/lists/*
# Tue, 15 Nov 2022 03:06:49 GMT
RUN set -eux; 	nativeLines="$(catalina.sh configtest 2>&1)"; 	nativeLines="$(echo "$nativeLines" | grep 'Apache Tomcat Native')"; 	nativeLines="$(echo "$nativeLines" | sort -u)"; 	if ! echo "$nativeLines" | grep -E 'INFO: Loaded( APR based)? Apache Tomcat Native library' >&2; then 		echo >&2 "$nativeLines"; 		exit 1; 	fi
# Tue, 15 Nov 2022 03:06:49 GMT
EXPOSE 8080
# Tue, 15 Nov 2022 03:06:49 GMT
CMD ["catalina.sh" "run"]
# Wed, 11 Jan 2023 02:47:03 GMT
LABEL org.opencontainers.image.authors=XWiki Development Team <committers@xwiki.org>
# Wed, 11 Jan 2023 02:47:03 GMT
LABEL org.opencontainers.image.url=https://hub.docker.com/_/xwiki
# Wed, 11 Jan 2023 02:47:03 GMT
LABEL org.opencontainers.image.documentation=https://hub.docker.com/_/xwiki
# Wed, 11 Jan 2023 02:47:03 GMT
LABEL org.opencontainers.image.source=https://github.com/xwiki/xwiki-docker.git
# Wed, 11 Jan 2023 02:47:04 GMT
LABEL org.opencontainers.image.vendor=xwiki.org
# Wed, 11 Jan 2023 02:47:04 GMT
LABEL org.opencontainers.image.licenses=LGPL-2.1
# Wed, 11 Jan 2023 02:50:25 GMT
RUN apt-get update &&   apt-get --no-install-recommends -y install     curl     libreoffice     unzip     procps     libpostgresql-jdbc-java &&   rm -rf /var/lib/apt/lists/*
# Tue, 31 Jan 2023 00:21:26 GMT
ENV XWIKI_VERSION=15.0
# Tue, 31 Jan 2023 00:21:27 GMT
ENV XWIKI_URL_PREFIX=https://maven.xwiki.org/releases/org/xwiki/platform/xwiki-platform-distribution-war/15.0
# Tue, 31 Jan 2023 00:21:27 GMT
ENV XWIKI_DOWNLOAD_SHA256=79ba0f479bbc49521c113821adc9d91141075a9470d7f9bbb6994ca59c30d121
# Tue, 31 Jan 2023 00:22:39 GMT
RUN rm -rf /usr/local/tomcat/webapps/* &&   mkdir -p /usr/local/tomcat/temp &&   mkdir -p /usr/local/xwiki/data &&   curl -fSL "${XWIKI_URL_PREFIX}/xwiki-platform-distribution-war-${XWIKI_VERSION}.war" -o xwiki.war &&   echo "$XWIKI_DOWNLOAD_SHA256 xwiki.war" | sha256sum -c - &&   unzip -d /usr/local/tomcat/webapps/ROOT xwiki.war &&   rm -f xwiki.war
# Tue, 31 Jan 2023 00:22:40 GMT
RUN cp /usr/share/java/postgresql-jdbc4.jar /usr/local/tomcat/webapps/ROOT/WEB-INF/lib/
# Tue, 31 Jan 2023 00:22:41 GMT
COPY file:0a1be11e2eb610a1dbcd415404e3a592641110b93090030cb831e3a19a163017 in /usr/local/tomcat/bin/ 
# Tue, 31 Jan 2023 00:22:41 GMT
COPY file:4a923f484bb29a26630c19e1d617d3bf6aa6ae7c6c4a5561e97b037bcde0847c in /usr/local/tomcat/webapps/ROOT/WEB-INF/hibernate.cfg.xml 
# Tue, 31 Jan 2023 00:22:41 GMT
RUN sed -i 's/<id>org.xwiki.platform:xwiki-platform-distribution-war/<id>org.xwiki.platform:xwiki-platform-distribution-docker/'   /usr/local/tomcat/webapps/ROOT/META-INF/extension.xed
# Tue, 31 Jan 2023 00:22:41 GMT
COPY file:a47c4dcd87c9dad97aff38c49188357e6193bcad50757e516cfb08a60d4de611 in /usr/local/bin/docker-entrypoint.sh 
# Tue, 31 Jan 2023 00:22:41 GMT
VOLUME [/usr/local/xwiki]
# Tue, 31 Jan 2023 00:22:42 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 31 Jan 2023 00:22:42 GMT
CMD ["xwiki"]
```

-	Layers:
	-	`sha256:e96e057aae67380a4ddb16c337c5c3669d97fdff69ec537f02aa2cc30d814281`  
		Last Modified: Wed, 02 Nov 2022 03:03:36 GMT  
		Size: 30.4 MB (30425607 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4ced2591451da3a02e2b6bb44752b9e3f00d77789921be4df5082fb9f9880ad0`  
		Last Modified: Wed, 02 Nov 2022 18:48:43 GMT  
		Size: 12.4 MB (12439006 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:df8f874ae8c08a9e69e5fbe6c5a64200a45386132a3203d1a9a7f1146d94cfbc`  
		Last Modified: Fri, 04 Nov 2022 23:29:33 GMT  
		Size: 46.6 MB (46629936 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:111b6c7486426c4b6989102c2ee5be856e8a58e20ab0a350b24a905d536e8e7f`  
		Last Modified: Fri, 04 Nov 2022 23:29:26 GMT  
		Size: 161.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e6f84dce457c6d4f7b7291fce05f8e77998a3a7722a54125a1f1d52ca83043b4`  
		Last Modified: Sat, 05 Nov 2022 01:50:51 GMT  
		Size: 173.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a6c26749ee782392e38845ee2ba79b0da586ef6a45d8e7f29c7af14612278547`  
		Last Modified: Tue, 15 Nov 2022 03:19:57 GMT  
		Size: 12.2 MB (12200249 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4dddc6d9fa6024025b3fcfe729cab2dc544fb25476eca6e80b1af8e8d93bb0ee`  
		Last Modified: Tue, 15 Nov 2022 03:19:56 GMT  
		Size: 452.7 KB (452680 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:06637eebe5e72c8ad9019ad4eb4cdde1f11f7d4c24c7ed7374cf8966343aa2fb`  
		Last Modified: Tue, 15 Nov 2022 03:19:56 GMT  
		Size: 131.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b57f6f8bcfb0d93b8e21d3068d1f65d3f08dba05c5fab7d4c36e2359317b18c7`  
		Last Modified: Wed, 11 Jan 2023 02:53:53 GMT  
		Size: 179.7 MB (179745182 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:71a0aee972ff5a36a4c5d67f5bf6416b1b78d06c906ce727c5e8e11098d0dfd1`  
		Last Modified: Tue, 31 Jan 2023 00:25:01 GMT  
		Size: 307.1 MB (307117070 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ccc745f1273896cef68a5af6cd5713c4a2d8704628920a53e318a008f8096426`  
		Last Modified: Tue, 31 Jan 2023 00:24:44 GMT  
		Size: 936.8 KB (936848 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1593979548bc568ed36dc9f5adb8f00d8b7d3eb1fa850fc06426c2c9345b8472`  
		Last Modified: Tue, 31 Jan 2023 00:24:43 GMT  
		Size: 1.3 KB (1345 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e1e58b32c2c2a52907f7e4ad05462d3b2afd11404a9678bc656fb96029b12d8d`  
		Last Modified: Tue, 31 Jan 2023 00:24:43 GMT  
		Size: 2.5 KB (2454 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c43ce01c7b867ce6cda62f86175ba6a53f44000797d61fe604aded86980c4d41`  
		Last Modified: Tue, 31 Jan 2023 00:24:43 GMT  
		Size: 6.0 KB (6006 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6fe6f306aa61d9839a01e62f4c308a9a7d3bd4cd5ce9a58407b6585f6950f054`  
		Last Modified: Tue, 31 Jan 2023 00:24:43 GMT  
		Size: 2.5 KB (2505 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `xwiki:15.0-postgres-tomcat` - linux; arm64 variant v8

```console
$ docker pull xwiki@sha256:ae51c629c7a76aa7c15ebb33fcfdae3e529ef6456ada6d0dbcf9ed8fc5ecf00d
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **581.2 MB (581212250 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:70277ae3ffdca68401bb57e24e6302cc64a403bf36869f0959e54d03216b0005`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["xwiki"]`

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
# Wed, 02 Nov 2022 19:44:32 GMT
RUN apt-get update     && DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends tzdata curl wget ca-certificates fontconfig locales     && echo "en_US.UTF-8 UTF-8" >> /etc/locale.gen     && locale-gen en_US.UTF-8     && rm -rf /var/lib/apt/lists/*
# Fri, 04 Nov 2022 22:40:54 GMT
ENV JAVA_VERSION=jdk-11.0.17+8
# Fri, 04 Nov 2022 22:41:33 GMT
RUN set -eux;     ARCH="$(dpkg --print-architecture)";     case "${ARCH}" in        aarch64|arm64)          ESUM='bd6efe3290c8b5a42f695a55a26f3e3c9c284288574879d4b7089f31f5114177';          BINARY_URL='https://github.com/adoptium/temurin11-binaries/releases/download/jdk-11.0.17%2B8/OpenJDK11U-jre_aarch64_linux_hotspot_11.0.17_8.tar.gz';          ;;        armhf|arm)          ESUM='8cf113d3d7fa808895c8d2e41bb890af21c47e38c2460e0588147a4bb8fc658d';          BINARY_URL='https://github.com/adoptium/temurin11-binaries/releases/download/jdk-11.0.17%2B8/OpenJDK11U-jre_arm_linux_hotspot_11.0.17_8.tar.gz';          ;;        ppc64el|powerpc:common64)          ESUM='0ca3d806131ab5834c501f9c625bb0248cd528af361c704503348e9c9605bedf';          BINARY_URL='https://github.com/adoptium/temurin11-binaries/releases/download/jdk-11.0.17%2B8/OpenJDK11U-jre_ppc64le_linux_hotspot_11.0.17_8.tar.gz';          ;;        s390x|s390:64-bit)          ESUM='dd3b159a374086e65cb07c4ccb226c90f9c02ef929cba6f0b642171d7ed97fa4';          BINARY_URL='https://github.com/adoptium/temurin11-binaries/releases/download/jdk-11.0.17%2B8/OpenJDK11U-jre_s390x_linux_hotspot_11.0.17_8.tar.gz';          ;;        amd64|i386:x86-64)          ESUM='752616097e09d7f60a3ad8bd312f90eaf50ac72577e55df229fe6e8091148f79';          BINARY_URL='https://github.com/adoptium/temurin11-binaries/releases/download/jdk-11.0.17%2B8/OpenJDK11U-jre_x64_linux_hotspot_11.0.17_8.tar.gz';          ;;        *)          echo "Unsupported arch: ${ARCH}";          exit 1;          ;;     esac; 	  wget -O /tmp/openjdk.tar.gz ${BINARY_URL}; 	  echo "${ESUM} */tmp/openjdk.tar.gz" | sha256sum -c -; 	  mkdir -p "$JAVA_HOME"; 	  tar --extract 	      --file /tmp/openjdk.tar.gz 	      --directory "$JAVA_HOME" 	      --strip-components 1 	      --no-same-owner 	  ;     rm /tmp/openjdk.tar.gz;     find "$JAVA_HOME/lib" -name '*.so' -exec dirname '{}' ';' | sort -u > /etc/ld.so.conf.d/docker-openjdk.conf;     ldconfig;     java -Xshare:dump;
# Fri, 04 Nov 2022 22:41:34 GMT
RUN echo Verifying install ...     && fileEncoding="$(echo 'System.out.println(System.getProperty("file.encoding"))' | jshell -s -)"; [ "$fileEncoding" = 'UTF-8' ]; rm -rf ~/.java     && echo java --version && java --version     && echo Complete.
# Fri, 04 Nov 2022 23:48:38 GMT
ENV CATALINA_HOME=/usr/local/tomcat
# Fri, 04 Nov 2022 23:48:38 GMT
ENV PATH=/usr/local/tomcat/bin:/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Fri, 04 Nov 2022 23:48:38 GMT
RUN mkdir -p "$CATALINA_HOME"
# Fri, 04 Nov 2022 23:48:39 GMT
WORKDIR /usr/local/tomcat
# Fri, 04 Nov 2022 23:48:39 GMT
ENV TOMCAT_NATIVE_LIBDIR=/usr/local/tomcat/native-jni-lib
# Fri, 04 Nov 2022 23:48:39 GMT
ENV LD_LIBRARY_PATH=/usr/local/tomcat/native-jni-lib
# Fri, 04 Nov 2022 23:53:12 GMT
ENV GPG_KEYS=48F8E69F6390C9F25CFEDCD268248959359E722B A9C5DF4D22E99998D9875A5110C01C5A2F6059E7 DCFD35E0BF8CA7344752DE8B6FB21E8933C60243
# Fri, 04 Nov 2022 23:53:12 GMT
ENV TOMCAT_MAJOR=9
# Tue, 15 Nov 2022 04:57:22 GMT
ENV TOMCAT_VERSION=9.0.69
# Tue, 15 Nov 2022 04:57:22 GMT
ENV TOMCAT_SHA512=8c883c54ce9ce43eba37756a6404cdf3477879883a3e6d146dc8a7aa5e0425f487466afe6b6da4a895927cb7cb59177b9379cec18000f2de12785be57408c779
# Tue, 15 Nov 2022 04:57:22 GMT
COPY dir:096b403a5f78b17e6b4bff63128a9c93941b97f22470991610dd641633d977f1 in /usr/local/tomcat 
# Tue, 15 Nov 2022 04:57:25 GMT
RUN set -eux; 	apt-get update; 	xargs -rt apt-get install -y --no-install-recommends < "$TOMCAT_NATIVE_LIBDIR/.dependencies.txt"; 	rm -rf /var/lib/apt/lists/*
# Tue, 15 Nov 2022 04:57:26 GMT
RUN set -eux; 	nativeLines="$(catalina.sh configtest 2>&1)"; 	nativeLines="$(echo "$nativeLines" | grep 'Apache Tomcat Native')"; 	nativeLines="$(echo "$nativeLines" | sort -u)"; 	if ! echo "$nativeLines" | grep -E 'INFO: Loaded( APR based)? Apache Tomcat Native library' >&2; then 		echo >&2 "$nativeLines"; 		exit 1; 	fi
# Tue, 15 Nov 2022 04:57:26 GMT
EXPOSE 8080
# Tue, 15 Nov 2022 04:57:27 GMT
CMD ["catalina.sh" "run"]
# Wed, 11 Jan 2023 03:05:10 GMT
LABEL org.opencontainers.image.authors=XWiki Development Team <committers@xwiki.org>
# Wed, 11 Jan 2023 03:05:10 GMT
LABEL org.opencontainers.image.url=https://hub.docker.com/_/xwiki
# Wed, 11 Jan 2023 03:05:10 GMT
LABEL org.opencontainers.image.documentation=https://hub.docker.com/_/xwiki
# Wed, 11 Jan 2023 03:05:10 GMT
LABEL org.opencontainers.image.source=https://github.com/xwiki/xwiki-docker.git
# Wed, 11 Jan 2023 03:05:11 GMT
LABEL org.opencontainers.image.vendor=xwiki.org
# Wed, 11 Jan 2023 03:05:11 GMT
LABEL org.opencontainers.image.licenses=LGPL-2.1
# Wed, 11 Jan 2023 03:08:55 GMT
RUN apt-get update &&   apt-get --no-install-recommends -y install     curl     libreoffice     unzip     procps     libpostgresql-jdbc-java &&   rm -rf /var/lib/apt/lists/*
# Tue, 31 Jan 2023 00:48:10 GMT
ENV XWIKI_VERSION=15.0
# Tue, 31 Jan 2023 00:48:10 GMT
ENV XWIKI_URL_PREFIX=https://maven.xwiki.org/releases/org/xwiki/platform/xwiki-platform-distribution-war/15.0
# Tue, 31 Jan 2023 00:48:10 GMT
ENV XWIKI_DOWNLOAD_SHA256=79ba0f479bbc49521c113821adc9d91141075a9470d7f9bbb6994ca59c30d121
# Tue, 31 Jan 2023 00:54:38 GMT
RUN rm -rf /usr/local/tomcat/webapps/* &&   mkdir -p /usr/local/tomcat/temp &&   mkdir -p /usr/local/xwiki/data &&   curl -fSL "${XWIKI_URL_PREFIX}/xwiki-platform-distribution-war-${XWIKI_VERSION}.war" -o xwiki.war &&   echo "$XWIKI_DOWNLOAD_SHA256 xwiki.war" | sha256sum -c - &&   unzip -d /usr/local/tomcat/webapps/ROOT xwiki.war &&   rm -f xwiki.war
# Tue, 31 Jan 2023 00:54:41 GMT
RUN cp /usr/share/java/postgresql-jdbc4.jar /usr/local/tomcat/webapps/ROOT/WEB-INF/lib/
# Tue, 31 Jan 2023 00:54:41 GMT
COPY file:0a1be11e2eb610a1dbcd415404e3a592641110b93090030cb831e3a19a163017 in /usr/local/tomcat/bin/ 
# Tue, 31 Jan 2023 00:54:41 GMT
COPY file:4a923f484bb29a26630c19e1d617d3bf6aa6ae7c6c4a5561e97b037bcde0847c in /usr/local/tomcat/webapps/ROOT/WEB-INF/hibernate.cfg.xml 
# Tue, 31 Jan 2023 00:54:42 GMT
RUN sed -i 's/<id>org.xwiki.platform:xwiki-platform-distribution-war/<id>org.xwiki.platform:xwiki-platform-distribution-docker/'   /usr/local/tomcat/webapps/ROOT/META-INF/extension.xed
# Tue, 31 Jan 2023 00:54:42 GMT
COPY file:a47c4dcd87c9dad97aff38c49188357e6193bcad50757e516cfb08a60d4de611 in /usr/local/bin/docker-entrypoint.sh 
# Tue, 31 Jan 2023 00:54:42 GMT
VOLUME [/usr/local/xwiki]
# Tue, 31 Jan 2023 00:54:42 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 31 Jan 2023 00:54:42 GMT
CMD ["xwiki"]
```

-	Layers:
	-	`sha256:0509fae36eb0656f8bdb23f8ae64100d893bcea2563e97468d337e04d2d0410b`  
		Last Modified: Wed, 02 Nov 2022 18:50:21 GMT  
		Size: 28.4 MB (28382154 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e502a1af2bcd98f5f0d2f5e4da1a0e7bbe07a2c548e2662f7d37dce5ae1df46c`  
		Last Modified: Wed, 02 Nov 2022 19:48:28 GMT  
		Size: 12.4 MB (12396330 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bc4598c07dd818f03a0378b0341a4a8e80f0152fbb3e7d5246ca4f466f42e611`  
		Last Modified: Fri, 04 Nov 2022 22:46:46 GMT  
		Size: 45.0 MB (44958470 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:715a937a1066f998b331fcd62256ad01a5571bdf46804e97825afc64f9ebb427`  
		Last Modified: Fri, 04 Nov 2022 22:46:41 GMT  
		Size: 160.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5fb623f082f74b2fa9fc2c4e3f3a4802875cb9753cfa26ed940201ce72bb56cb`  
		Last Modified: Sat, 05 Nov 2022 00:03:40 GMT  
		Size: 172.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:33260b83200262bbd546be371ad3c1f50f5ae7228afb87982d6fa9d6b11bf26f`  
		Last Modified: Tue, 15 Nov 2022 05:10:19 GMT  
		Size: 12.2 MB (12207235 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0955fb697ea9b30a1b4f95385464f646aa1525cb6efba648e22df84ebef6b2ee`  
		Last Modified: Tue, 15 Nov 2022 05:10:18 GMT  
		Size: 452.0 KB (452021 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6eddcf66f2083b1487296a0308e0b058917c97f614f12428d82d89662038dc2e`  
		Last Modified: Tue, 15 Nov 2022 05:10:18 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1ae6a8fce0f2cd131007393c1a4eba9ce9d0501da8406af5c5ce9deb5dc187b8`  
		Last Modified: Wed, 11 Jan 2023 03:12:13 GMT  
		Size: 174.7 MB (174749274 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5351c17af011e98fdd3db4781945e719f390748d66dc50d28bef46bb2d6b6418`  
		Last Modified: Tue, 31 Jan 2023 00:56:53 GMT  
		Size: 307.1 MB (307117134 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6b632a2f6afda42ce5dc291920d8f03e04b69034e314687eb551be8eafedd92d`  
		Last Modified: Tue, 31 Jan 2023 00:56:38 GMT  
		Size: 936.9 KB (936854 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cbd6cbb6ae05692db55d5e4f46142d2e20e051631dc2fc44e5b20d3316143305`  
		Last Modified: Tue, 31 Jan 2023 00:56:38 GMT  
		Size: 1.3 KB (1348 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ceb1d88f8fd44412961c0db372cd86a999c6b2619ce80a916a4fe8ca0e63acc9`  
		Last Modified: Tue, 31 Jan 2023 00:56:38 GMT  
		Size: 2.5 KB (2458 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8d0ee5cad12d41a6d530031aabd4a92619995eb0ee20dcd24d2bb9aec6a694db`  
		Last Modified: Tue, 31 Jan 2023 00:56:38 GMT  
		Size: 6.0 KB (6006 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3c980b95519f007aea60be042d36cd33de21e6265aed0e443c5ecf9bb1f40980`  
		Last Modified: Tue, 31 Jan 2023 00:56:38 GMT  
		Size: 2.5 KB (2505 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `xwiki:15.0.0`

```console
$ docker pull xwiki@sha256:33e789838f82ce73efec6664859feb1ced7a5b7605fbfaddb81916716bce524f
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `xwiki:15.0.0` - linux; amd64

```console
$ docker pull xwiki@sha256:481fdb46e8c043a6709d11310e2083ce71d6ba63ee6517f84da3ba06f320598e
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **590.5 MB (590459982 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:bd630aa0aa5c679e23ea7d52cbbdd6b817eab27a820c25d3c50b54eca83b9744`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["xwiki"]`

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
# Wed, 02 Nov 2022 18:44:10 GMT
RUN apt-get update     && DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends tzdata curl wget ca-certificates fontconfig locales     && echo "en_US.UTF-8 UTF-8" >> /etc/locale.gen     && locale-gen en_US.UTF-8     && rm -rf /var/lib/apt/lists/*
# Fri, 04 Nov 2022 23:21:41 GMT
ENV JAVA_VERSION=jdk-11.0.17+8
# Fri, 04 Nov 2022 23:22:31 GMT
RUN set -eux;     ARCH="$(dpkg --print-architecture)";     case "${ARCH}" in        aarch64|arm64)          ESUM='bd6efe3290c8b5a42f695a55a26f3e3c9c284288574879d4b7089f31f5114177';          BINARY_URL='https://github.com/adoptium/temurin11-binaries/releases/download/jdk-11.0.17%2B8/OpenJDK11U-jre_aarch64_linux_hotspot_11.0.17_8.tar.gz';          ;;        armhf|arm)          ESUM='8cf113d3d7fa808895c8d2e41bb890af21c47e38c2460e0588147a4bb8fc658d';          BINARY_URL='https://github.com/adoptium/temurin11-binaries/releases/download/jdk-11.0.17%2B8/OpenJDK11U-jre_arm_linux_hotspot_11.0.17_8.tar.gz';          ;;        ppc64el|powerpc:common64)          ESUM='0ca3d806131ab5834c501f9c625bb0248cd528af361c704503348e9c9605bedf';          BINARY_URL='https://github.com/adoptium/temurin11-binaries/releases/download/jdk-11.0.17%2B8/OpenJDK11U-jre_ppc64le_linux_hotspot_11.0.17_8.tar.gz';          ;;        s390x|s390:64-bit)          ESUM='dd3b159a374086e65cb07c4ccb226c90f9c02ef929cba6f0b642171d7ed97fa4';          BINARY_URL='https://github.com/adoptium/temurin11-binaries/releases/download/jdk-11.0.17%2B8/OpenJDK11U-jre_s390x_linux_hotspot_11.0.17_8.tar.gz';          ;;        amd64|i386:x86-64)          ESUM='752616097e09d7f60a3ad8bd312f90eaf50ac72577e55df229fe6e8091148f79';          BINARY_URL='https://github.com/adoptium/temurin11-binaries/releases/download/jdk-11.0.17%2B8/OpenJDK11U-jre_x64_linux_hotspot_11.0.17_8.tar.gz';          ;;        *)          echo "Unsupported arch: ${ARCH}";          exit 1;          ;;     esac; 	  wget -O /tmp/openjdk.tar.gz ${BINARY_URL}; 	  echo "${ESUM} */tmp/openjdk.tar.gz" | sha256sum -c -; 	  mkdir -p "$JAVA_HOME"; 	  tar --extract 	      --file /tmp/openjdk.tar.gz 	      --directory "$JAVA_HOME" 	      --strip-components 1 	      --no-same-owner 	  ;     rm /tmp/openjdk.tar.gz;     find "$JAVA_HOME/lib" -name '*.so' -exec dirname '{}' ';' | sort -u > /etc/ld.so.conf.d/docker-openjdk.conf;     ldconfig;     java -Xshare:dump;
# Fri, 04 Nov 2022 23:22:32 GMT
RUN echo Verifying install ...     && fileEncoding="$(echo 'System.out.println(System.getProperty("file.encoding"))' | jshell -s -)"; [ "$fileEncoding" = 'UTF-8' ]; rm -rf ~/.java     && echo java --version && java --version     && echo Complete.
# Sat, 05 Nov 2022 01:35:16 GMT
ENV CATALINA_HOME=/usr/local/tomcat
# Sat, 05 Nov 2022 01:35:16 GMT
ENV PATH=/usr/local/tomcat/bin:/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Sat, 05 Nov 2022 01:35:17 GMT
RUN mkdir -p "$CATALINA_HOME"
# Sat, 05 Nov 2022 01:35:17 GMT
WORKDIR /usr/local/tomcat
# Sat, 05 Nov 2022 01:35:17 GMT
ENV TOMCAT_NATIVE_LIBDIR=/usr/local/tomcat/native-jni-lib
# Sat, 05 Nov 2022 01:35:17 GMT
ENV LD_LIBRARY_PATH=/usr/local/tomcat/native-jni-lib
# Sat, 05 Nov 2022 01:39:54 GMT
ENV GPG_KEYS=48F8E69F6390C9F25CFEDCD268248959359E722B A9C5DF4D22E99998D9875A5110C01C5A2F6059E7 DCFD35E0BF8CA7344752DE8B6FB21E8933C60243
# Sat, 05 Nov 2022 01:39:54 GMT
ENV TOMCAT_MAJOR=9
# Tue, 15 Nov 2022 03:06:43 GMT
ENV TOMCAT_VERSION=9.0.69
# Tue, 15 Nov 2022 03:06:43 GMT
ENV TOMCAT_SHA512=8c883c54ce9ce43eba37756a6404cdf3477879883a3e6d146dc8a7aa5e0425f487466afe6b6da4a895927cb7cb59177b9379cec18000f2de12785be57408c779
# Tue, 15 Nov 2022 03:06:44 GMT
COPY dir:b1a33aa3993dbbfbebb33bd9aa546b60c2f2191abf1227f453d4e830f6deb35f in /usr/local/tomcat 
# Tue, 15 Nov 2022 03:06:48 GMT
RUN set -eux; 	apt-get update; 	xargs -rt apt-get install -y --no-install-recommends < "$TOMCAT_NATIVE_LIBDIR/.dependencies.txt"; 	rm -rf /var/lib/apt/lists/*
# Tue, 15 Nov 2022 03:06:49 GMT
RUN set -eux; 	nativeLines="$(catalina.sh configtest 2>&1)"; 	nativeLines="$(echo "$nativeLines" | grep 'Apache Tomcat Native')"; 	nativeLines="$(echo "$nativeLines" | sort -u)"; 	if ! echo "$nativeLines" | grep -E 'INFO: Loaded( APR based)? Apache Tomcat Native library' >&2; then 		echo >&2 "$nativeLines"; 		exit 1; 	fi
# Tue, 15 Nov 2022 03:06:49 GMT
EXPOSE 8080
# Tue, 15 Nov 2022 03:06:49 GMT
CMD ["catalina.sh" "run"]
# Wed, 11 Jan 2023 02:47:03 GMT
LABEL org.opencontainers.image.authors=XWiki Development Team <committers@xwiki.org>
# Wed, 11 Jan 2023 02:47:03 GMT
LABEL org.opencontainers.image.url=https://hub.docker.com/_/xwiki
# Wed, 11 Jan 2023 02:47:03 GMT
LABEL org.opencontainers.image.documentation=https://hub.docker.com/_/xwiki
# Wed, 11 Jan 2023 02:47:03 GMT
LABEL org.opencontainers.image.source=https://github.com/xwiki/xwiki-docker.git
# Wed, 11 Jan 2023 02:47:04 GMT
LABEL org.opencontainers.image.vendor=xwiki.org
# Wed, 11 Jan 2023 02:47:04 GMT
LABEL org.opencontainers.image.licenses=LGPL-2.1
# Wed, 11 Jan 2023 02:49:03 GMT
RUN apt-get update &&   apt-get --no-install-recommends -y install     curl     libreoffice     unzip     procps &&   rm -rf /var/lib/apt/lists/*
# Tue, 31 Jan 2023 00:20:17 GMT
ENV XWIKI_VERSION=15.0
# Tue, 31 Jan 2023 00:20:17 GMT
ENV XWIKI_URL_PREFIX=https://maven.xwiki.org/releases/org/xwiki/platform/xwiki-platform-distribution-war/15.0
# Tue, 31 Jan 2023 00:20:17 GMT
ENV XWIKI_DOWNLOAD_SHA256=79ba0f479bbc49521c113821adc9d91141075a9470d7f9bbb6994ca59c30d121
# Tue, 31 Jan 2023 00:21:18 GMT
RUN rm -rf /usr/local/tomcat/webapps/* &&   mkdir -p /usr/local/tomcat/temp &&   mkdir -p /usr/local/xwiki/data &&   curl -fSL "${XWIKI_URL_PREFIX}/xwiki-platform-distribution-war-${XWIKI_VERSION}.war" -o xwiki.war &&   echo "$XWIKI_DOWNLOAD_SHA256 xwiki.war" | sha256sum -c - &&   unzip -d /usr/local/tomcat/webapps/ROOT xwiki.war &&   rm -f xwiki.war
# Tue, 31 Jan 2023 00:21:19 GMT
ENV MYSQL_JDBC_VERSION=8.0.31
# Tue, 31 Jan 2023 00:21:19 GMT
ENV MYSQL_JDBC_SHA256=5249e3dc6d6531b37790e3f61845b96db5e41e891d3d8edb0e2e3a1b53ca2f4f
# Tue, 31 Jan 2023 00:21:19 GMT
ENV MYSQL_JDBC_PREFIX=https://repo1.maven.org/maven2/com/mysql/mysql-connector-j/8.0.31
# Tue, 31 Jan 2023 00:21:19 GMT
ENV MYSQL_JDBC_ARTIFACT=mysql-connector-j-8.0.31.jar
# Tue, 31 Jan 2023 00:21:19 GMT
ENV MYSQL_JDBC_TARGET=/usr/local/tomcat/webapps/ROOT/WEB-INF/lib/mysql-connector-j-8.0.31.jar
# Tue, 31 Jan 2023 00:21:20 GMT
RUN curl -fSL "${MYSQL_JDBC_PREFIX}/${MYSQL_JDBC_ARTIFACT}" -o $MYSQL_JDBC_TARGET &&   echo "$MYSQL_JDBC_SHA256 $MYSQL_JDBC_TARGET" | sha256sum -c -
# Tue, 31 Jan 2023 00:21:21 GMT
COPY file:0a1be11e2eb610a1dbcd415404e3a592641110b93090030cb831e3a19a163017 in /usr/local/tomcat/bin/ 
# Tue, 31 Jan 2023 00:21:21 GMT
COPY file:1b8409986f3e4eb79a7a0b18472cb2692a61d504fb5ef34292bc997b79fd760d in /usr/local/tomcat/webapps/ROOT/WEB-INF/hibernate.cfg.xml 
# Tue, 31 Jan 2023 00:21:21 GMT
RUN sed -i 's/<id>org.xwiki.platform:xwiki-platform-distribution-war/<id>org.xwiki.platform:xwiki-platform-distribution-docker/'   /usr/local/tomcat/webapps/ROOT/META-INF/extension.xed
# Tue, 31 Jan 2023 00:21:21 GMT
COPY file:a47c4dcd87c9dad97aff38c49188357e6193bcad50757e516cfb08a60d4de611 in /usr/local/bin/docker-entrypoint.sh 
# Tue, 31 Jan 2023 00:21:22 GMT
VOLUME [/usr/local/xwiki]
# Tue, 31 Jan 2023 00:21:22 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 31 Jan 2023 00:21:22 GMT
CMD ["xwiki"]
```

-	Layers:
	-	`sha256:e96e057aae67380a4ddb16c337c5c3669d97fdff69ec537f02aa2cc30d814281`  
		Last Modified: Wed, 02 Nov 2022 03:03:36 GMT  
		Size: 30.4 MB (30425607 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4ced2591451da3a02e2b6bb44752b9e3f00d77789921be4df5082fb9f9880ad0`  
		Last Modified: Wed, 02 Nov 2022 18:48:43 GMT  
		Size: 12.4 MB (12439006 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:df8f874ae8c08a9e69e5fbe6c5a64200a45386132a3203d1a9a7f1146d94cfbc`  
		Last Modified: Fri, 04 Nov 2022 23:29:33 GMT  
		Size: 46.6 MB (46629936 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:111b6c7486426c4b6989102c2ee5be856e8a58e20ab0a350b24a905d536e8e7f`  
		Last Modified: Fri, 04 Nov 2022 23:29:26 GMT  
		Size: 161.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e6f84dce457c6d4f7b7291fce05f8e77998a3a7722a54125a1f1d52ca83043b4`  
		Last Modified: Sat, 05 Nov 2022 01:50:51 GMT  
		Size: 173.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a6c26749ee782392e38845ee2ba79b0da586ef6a45d8e7f29c7af14612278547`  
		Last Modified: Tue, 15 Nov 2022 03:19:57 GMT  
		Size: 12.2 MB (12200249 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4dddc6d9fa6024025b3fcfe729cab2dc544fb25476eca6e80b1af8e8d93bb0ee`  
		Last Modified: Tue, 15 Nov 2022 03:19:56 GMT  
		Size: 452.7 KB (452680 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:06637eebe5e72c8ad9019ad4eb4cdde1f11f7d4c24c7ed7374cf8966343aa2fb`  
		Last Modified: Tue, 15 Nov 2022 03:19:56 GMT  
		Size: 131.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b276fb8390410a8208724033e325715ea26000d5a1a762d4c3699b927884fbfe`  
		Last Modified: Wed, 11 Jan 2023 02:52:45 GMT  
		Size: 178.8 MB (178805608 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:156ca91198173149698aa0396648a9608b6ab1f2bc2666800843ce33c9f85b6e`  
		Last Modified: Tue, 31 Jan 2023 00:24:09 GMT  
		Size: 307.1 MB (307117069 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4c8b70d250c6d507901857473b0dcb67132d7b2a30ce9a69b07b1036853df738`  
		Last Modified: Tue, 31 Jan 2023 00:23:52 GMT  
		Size: 2.4 MB (2377191 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a9681fd36be674d25231c69d6a39f9e8fa65034eeaef5d1bd885fdbeac7f0f6b`  
		Last Modified: Tue, 31 Jan 2023 00:23:51 GMT  
		Size: 1.3 KB (1346 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a9d0d5da840f4d7da9943942b38cd092fae11f41dc6c19afd58d655cd6192d66`  
		Last Modified: Tue, 31 Jan 2023 00:23:51 GMT  
		Size: 2.3 KB (2312 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d65610da4f1da86fea8fbec0189b066afd4b86e4e8f7d049e3c4bc6ade9ba90a`  
		Last Modified: Tue, 31 Jan 2023 00:23:51 GMT  
		Size: 6.0 KB (6009 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3d41686284d7675eaa0f92c9cc27ebe73b4c30768c8eef9f23ee3b1ad06da00a`  
		Last Modified: Tue, 31 Jan 2023 00:23:51 GMT  
		Size: 2.5 KB (2504 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `xwiki:15.0.0` - linux; arm64 variant v8

```console
$ docker pull xwiki@sha256:6bf63d9025b07b69d744200c05efd4ffb8a52f3c38380f5d59a0b48514203cd2
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **581.7 MB (581709921 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:6600f2bb05836c703d53944bbcb5399d509a9813a27a35e99ff717becc308330`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["xwiki"]`

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
# Wed, 02 Nov 2022 19:44:32 GMT
RUN apt-get update     && DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends tzdata curl wget ca-certificates fontconfig locales     && echo "en_US.UTF-8 UTF-8" >> /etc/locale.gen     && locale-gen en_US.UTF-8     && rm -rf /var/lib/apt/lists/*
# Fri, 04 Nov 2022 22:40:54 GMT
ENV JAVA_VERSION=jdk-11.0.17+8
# Fri, 04 Nov 2022 22:41:33 GMT
RUN set -eux;     ARCH="$(dpkg --print-architecture)";     case "${ARCH}" in        aarch64|arm64)          ESUM='bd6efe3290c8b5a42f695a55a26f3e3c9c284288574879d4b7089f31f5114177';          BINARY_URL='https://github.com/adoptium/temurin11-binaries/releases/download/jdk-11.0.17%2B8/OpenJDK11U-jre_aarch64_linux_hotspot_11.0.17_8.tar.gz';          ;;        armhf|arm)          ESUM='8cf113d3d7fa808895c8d2e41bb890af21c47e38c2460e0588147a4bb8fc658d';          BINARY_URL='https://github.com/adoptium/temurin11-binaries/releases/download/jdk-11.0.17%2B8/OpenJDK11U-jre_arm_linux_hotspot_11.0.17_8.tar.gz';          ;;        ppc64el|powerpc:common64)          ESUM='0ca3d806131ab5834c501f9c625bb0248cd528af361c704503348e9c9605bedf';          BINARY_URL='https://github.com/adoptium/temurin11-binaries/releases/download/jdk-11.0.17%2B8/OpenJDK11U-jre_ppc64le_linux_hotspot_11.0.17_8.tar.gz';          ;;        s390x|s390:64-bit)          ESUM='dd3b159a374086e65cb07c4ccb226c90f9c02ef929cba6f0b642171d7ed97fa4';          BINARY_URL='https://github.com/adoptium/temurin11-binaries/releases/download/jdk-11.0.17%2B8/OpenJDK11U-jre_s390x_linux_hotspot_11.0.17_8.tar.gz';          ;;        amd64|i386:x86-64)          ESUM='752616097e09d7f60a3ad8bd312f90eaf50ac72577e55df229fe6e8091148f79';          BINARY_URL='https://github.com/adoptium/temurin11-binaries/releases/download/jdk-11.0.17%2B8/OpenJDK11U-jre_x64_linux_hotspot_11.0.17_8.tar.gz';          ;;        *)          echo "Unsupported arch: ${ARCH}";          exit 1;          ;;     esac; 	  wget -O /tmp/openjdk.tar.gz ${BINARY_URL}; 	  echo "${ESUM} */tmp/openjdk.tar.gz" | sha256sum -c -; 	  mkdir -p "$JAVA_HOME"; 	  tar --extract 	      --file /tmp/openjdk.tar.gz 	      --directory "$JAVA_HOME" 	      --strip-components 1 	      --no-same-owner 	  ;     rm /tmp/openjdk.tar.gz;     find "$JAVA_HOME/lib" -name '*.so' -exec dirname '{}' ';' | sort -u > /etc/ld.so.conf.d/docker-openjdk.conf;     ldconfig;     java -Xshare:dump;
# Fri, 04 Nov 2022 22:41:34 GMT
RUN echo Verifying install ...     && fileEncoding="$(echo 'System.out.println(System.getProperty("file.encoding"))' | jshell -s -)"; [ "$fileEncoding" = 'UTF-8' ]; rm -rf ~/.java     && echo java --version && java --version     && echo Complete.
# Fri, 04 Nov 2022 23:48:38 GMT
ENV CATALINA_HOME=/usr/local/tomcat
# Fri, 04 Nov 2022 23:48:38 GMT
ENV PATH=/usr/local/tomcat/bin:/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Fri, 04 Nov 2022 23:48:38 GMT
RUN mkdir -p "$CATALINA_HOME"
# Fri, 04 Nov 2022 23:48:39 GMT
WORKDIR /usr/local/tomcat
# Fri, 04 Nov 2022 23:48:39 GMT
ENV TOMCAT_NATIVE_LIBDIR=/usr/local/tomcat/native-jni-lib
# Fri, 04 Nov 2022 23:48:39 GMT
ENV LD_LIBRARY_PATH=/usr/local/tomcat/native-jni-lib
# Fri, 04 Nov 2022 23:53:12 GMT
ENV GPG_KEYS=48F8E69F6390C9F25CFEDCD268248959359E722B A9C5DF4D22E99998D9875A5110C01C5A2F6059E7 DCFD35E0BF8CA7344752DE8B6FB21E8933C60243
# Fri, 04 Nov 2022 23:53:12 GMT
ENV TOMCAT_MAJOR=9
# Tue, 15 Nov 2022 04:57:22 GMT
ENV TOMCAT_VERSION=9.0.69
# Tue, 15 Nov 2022 04:57:22 GMT
ENV TOMCAT_SHA512=8c883c54ce9ce43eba37756a6404cdf3477879883a3e6d146dc8a7aa5e0425f487466afe6b6da4a895927cb7cb59177b9379cec18000f2de12785be57408c779
# Tue, 15 Nov 2022 04:57:22 GMT
COPY dir:096b403a5f78b17e6b4bff63128a9c93941b97f22470991610dd641633d977f1 in /usr/local/tomcat 
# Tue, 15 Nov 2022 04:57:25 GMT
RUN set -eux; 	apt-get update; 	xargs -rt apt-get install -y --no-install-recommends < "$TOMCAT_NATIVE_LIBDIR/.dependencies.txt"; 	rm -rf /var/lib/apt/lists/*
# Tue, 15 Nov 2022 04:57:26 GMT
RUN set -eux; 	nativeLines="$(catalina.sh configtest 2>&1)"; 	nativeLines="$(echo "$nativeLines" | grep 'Apache Tomcat Native')"; 	nativeLines="$(echo "$nativeLines" | sort -u)"; 	if ! echo "$nativeLines" | grep -E 'INFO: Loaded( APR based)? Apache Tomcat Native library' >&2; then 		echo >&2 "$nativeLines"; 		exit 1; 	fi
# Tue, 15 Nov 2022 04:57:26 GMT
EXPOSE 8080
# Tue, 15 Nov 2022 04:57:27 GMT
CMD ["catalina.sh" "run"]
# Wed, 11 Jan 2023 03:05:10 GMT
LABEL org.opencontainers.image.authors=XWiki Development Team <committers@xwiki.org>
# Wed, 11 Jan 2023 03:05:10 GMT
LABEL org.opencontainers.image.url=https://hub.docker.com/_/xwiki
# Wed, 11 Jan 2023 03:05:10 GMT
LABEL org.opencontainers.image.documentation=https://hub.docker.com/_/xwiki
# Wed, 11 Jan 2023 03:05:10 GMT
LABEL org.opencontainers.image.source=https://github.com/xwiki/xwiki-docker.git
# Wed, 11 Jan 2023 03:05:11 GMT
LABEL org.opencontainers.image.vendor=xwiki.org
# Wed, 11 Jan 2023 03:05:11 GMT
LABEL org.opencontainers.image.licenses=LGPL-2.1
# Wed, 11 Jan 2023 03:07:37 GMT
RUN apt-get update &&   apt-get --no-install-recommends -y install     curl     libreoffice     unzip     procps &&   rm -rf /var/lib/apt/lists/*
# Tue, 31 Jan 2023 00:47:12 GMT
ENV XWIKI_VERSION=15.0
# Tue, 31 Jan 2023 00:47:12 GMT
ENV XWIKI_URL_PREFIX=https://maven.xwiki.org/releases/org/xwiki/platform/xwiki-platform-distribution-war/15.0
# Tue, 31 Jan 2023 00:47:12 GMT
ENV XWIKI_DOWNLOAD_SHA256=79ba0f479bbc49521c113821adc9d91141075a9470d7f9bbb6994ca59c30d121
# Tue, 31 Jan 2023 00:47:58 GMT
RUN rm -rf /usr/local/tomcat/webapps/* &&   mkdir -p /usr/local/tomcat/temp &&   mkdir -p /usr/local/xwiki/data &&   curl -fSL "${XWIKI_URL_PREFIX}/xwiki-platform-distribution-war-${XWIKI_VERSION}.war" -o xwiki.war &&   echo "$XWIKI_DOWNLOAD_SHA256 xwiki.war" | sha256sum -c - &&   unzip -d /usr/local/tomcat/webapps/ROOT xwiki.war &&   rm -f xwiki.war
# Tue, 31 Jan 2023 00:48:01 GMT
ENV MYSQL_JDBC_VERSION=8.0.31
# Tue, 31 Jan 2023 00:48:01 GMT
ENV MYSQL_JDBC_SHA256=5249e3dc6d6531b37790e3f61845b96db5e41e891d3d8edb0e2e3a1b53ca2f4f
# Tue, 31 Jan 2023 00:48:01 GMT
ENV MYSQL_JDBC_PREFIX=https://repo1.maven.org/maven2/com/mysql/mysql-connector-j/8.0.31
# Tue, 31 Jan 2023 00:48:01 GMT
ENV MYSQL_JDBC_ARTIFACT=mysql-connector-j-8.0.31.jar
# Tue, 31 Jan 2023 00:48:01 GMT
ENV MYSQL_JDBC_TARGET=/usr/local/tomcat/webapps/ROOT/WEB-INF/lib/mysql-connector-j-8.0.31.jar
# Tue, 31 Jan 2023 00:48:02 GMT
RUN curl -fSL "${MYSQL_JDBC_PREFIX}/${MYSQL_JDBC_ARTIFACT}" -o $MYSQL_JDBC_TARGET &&   echo "$MYSQL_JDBC_SHA256 $MYSQL_JDBC_TARGET" | sha256sum -c -
# Tue, 31 Jan 2023 00:48:02 GMT
COPY file:0a1be11e2eb610a1dbcd415404e3a592641110b93090030cb831e3a19a163017 in /usr/local/tomcat/bin/ 
# Tue, 31 Jan 2023 00:48:02 GMT
COPY file:1b8409986f3e4eb79a7a0b18472cb2692a61d504fb5ef34292bc997b79fd760d in /usr/local/tomcat/webapps/ROOT/WEB-INF/hibernate.cfg.xml 
# Tue, 31 Jan 2023 00:48:03 GMT
RUN sed -i 's/<id>org.xwiki.platform:xwiki-platform-distribution-war/<id>org.xwiki.platform:xwiki-platform-distribution-docker/'   /usr/local/tomcat/webapps/ROOT/META-INF/extension.xed
# Tue, 31 Jan 2023 00:48:03 GMT
COPY file:a47c4dcd87c9dad97aff38c49188357e6193bcad50757e516cfb08a60d4de611 in /usr/local/bin/docker-entrypoint.sh 
# Tue, 31 Jan 2023 00:48:03 GMT
VOLUME [/usr/local/xwiki]
# Tue, 31 Jan 2023 00:48:03 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 31 Jan 2023 00:48:03 GMT
CMD ["xwiki"]
```

-	Layers:
	-	`sha256:0509fae36eb0656f8bdb23f8ae64100d893bcea2563e97468d337e04d2d0410b`  
		Last Modified: Wed, 02 Nov 2022 18:50:21 GMT  
		Size: 28.4 MB (28382154 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e502a1af2bcd98f5f0d2f5e4da1a0e7bbe07a2c548e2662f7d37dce5ae1df46c`  
		Last Modified: Wed, 02 Nov 2022 19:48:28 GMT  
		Size: 12.4 MB (12396330 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bc4598c07dd818f03a0378b0341a4a8e80f0152fbb3e7d5246ca4f466f42e611`  
		Last Modified: Fri, 04 Nov 2022 22:46:46 GMT  
		Size: 45.0 MB (44958470 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:715a937a1066f998b331fcd62256ad01a5571bdf46804e97825afc64f9ebb427`  
		Last Modified: Fri, 04 Nov 2022 22:46:41 GMT  
		Size: 160.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5fb623f082f74b2fa9fc2c4e3f3a4802875cb9753cfa26ed940201ce72bb56cb`  
		Last Modified: Sat, 05 Nov 2022 00:03:40 GMT  
		Size: 172.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:33260b83200262bbd546be371ad3c1f50f5ae7228afb87982d6fa9d6b11bf26f`  
		Last Modified: Tue, 15 Nov 2022 05:10:19 GMT  
		Size: 12.2 MB (12207235 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0955fb697ea9b30a1b4f95385464f646aa1525cb6efba648e22df84ebef6b2ee`  
		Last Modified: Tue, 15 Nov 2022 05:10:18 GMT  
		Size: 452.0 KB (452021 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6eddcf66f2083b1487296a0308e0b058917c97f614f12428d82d89662038dc2e`  
		Last Modified: Tue, 15 Nov 2022 05:10:18 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ae5f60bb64f3fa11da3d15a9639f886186b4c2c021455c3f9db22e0cfe1b1311`  
		Last Modified: Wed, 11 Jan 2023 03:11:14 GMT  
		Size: 173.8 MB (173806827 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1814d85fce571b42f2cfa7c8a904e1a184ee6f49642242a44bbe0037088994a0`  
		Last Modified: Tue, 31 Jan 2023 00:56:04 GMT  
		Size: 307.1 MB (307117070 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8aec0e24b4fa870989f014944c3c7d535355a2371fc8c948b2b11f9b377efe6e`  
		Last Modified: Tue, 31 Jan 2023 00:55:50 GMT  
		Size: 2.4 MB (2377182 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0b65081619aa0114a7f367836ef421eb8d951e559e0f089c7728af7813b1ea62`  
		Last Modified: Tue, 31 Jan 2023 00:55:49 GMT  
		Size: 1.3 KB (1348 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:46ebad072e608146426d8dc30828937049eea36c2e636d7790b4960d6d586977`  
		Last Modified: Tue, 31 Jan 2023 00:55:49 GMT  
		Size: 2.3 KB (2308 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:708fefcedd4ee6c106da247a68c5790f5ab00225d1cdfff8465575265c3a54e6`  
		Last Modified: Tue, 31 Jan 2023 00:55:49 GMT  
		Size: 6.0 KB (6008 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:81e3bf8e20bc921031e7549a41dec1b2d7795cc6da40a0e7096bf654b25c5c3e`  
		Last Modified: Tue, 31 Jan 2023 00:55:49 GMT  
		Size: 2.5 KB (2507 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `xwiki:15.0.0-mariadb-tomcat`

```console
$ docker pull xwiki@sha256:725347355967f33745268f1167cc3c1b12fc85e327ccfa96da0848d05e3836c4
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `xwiki:15.0.0-mariadb-tomcat` - linux; amd64

```console
$ docker pull xwiki@sha256:cca1fb53bc2f0240f7f4843b846210e341a6002d7b18a0b90202520ce2f4ead0
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **588.7 MB (588672467 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:0088d72e62c01c9996a75e1b7e2296ba530b2dbd4054be70a006b33295aa4ff9`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["xwiki"]`

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
# Wed, 02 Nov 2022 18:44:10 GMT
RUN apt-get update     && DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends tzdata curl wget ca-certificates fontconfig locales     && echo "en_US.UTF-8 UTF-8" >> /etc/locale.gen     && locale-gen en_US.UTF-8     && rm -rf /var/lib/apt/lists/*
# Fri, 04 Nov 2022 23:21:41 GMT
ENV JAVA_VERSION=jdk-11.0.17+8
# Fri, 04 Nov 2022 23:22:31 GMT
RUN set -eux;     ARCH="$(dpkg --print-architecture)";     case "${ARCH}" in        aarch64|arm64)          ESUM='bd6efe3290c8b5a42f695a55a26f3e3c9c284288574879d4b7089f31f5114177';          BINARY_URL='https://github.com/adoptium/temurin11-binaries/releases/download/jdk-11.0.17%2B8/OpenJDK11U-jre_aarch64_linux_hotspot_11.0.17_8.tar.gz';          ;;        armhf|arm)          ESUM='8cf113d3d7fa808895c8d2e41bb890af21c47e38c2460e0588147a4bb8fc658d';          BINARY_URL='https://github.com/adoptium/temurin11-binaries/releases/download/jdk-11.0.17%2B8/OpenJDK11U-jre_arm_linux_hotspot_11.0.17_8.tar.gz';          ;;        ppc64el|powerpc:common64)          ESUM='0ca3d806131ab5834c501f9c625bb0248cd528af361c704503348e9c9605bedf';          BINARY_URL='https://github.com/adoptium/temurin11-binaries/releases/download/jdk-11.0.17%2B8/OpenJDK11U-jre_ppc64le_linux_hotspot_11.0.17_8.tar.gz';          ;;        s390x|s390:64-bit)          ESUM='dd3b159a374086e65cb07c4ccb226c90f9c02ef929cba6f0b642171d7ed97fa4';          BINARY_URL='https://github.com/adoptium/temurin11-binaries/releases/download/jdk-11.0.17%2B8/OpenJDK11U-jre_s390x_linux_hotspot_11.0.17_8.tar.gz';          ;;        amd64|i386:x86-64)          ESUM='752616097e09d7f60a3ad8bd312f90eaf50ac72577e55df229fe6e8091148f79';          BINARY_URL='https://github.com/adoptium/temurin11-binaries/releases/download/jdk-11.0.17%2B8/OpenJDK11U-jre_x64_linux_hotspot_11.0.17_8.tar.gz';          ;;        *)          echo "Unsupported arch: ${ARCH}";          exit 1;          ;;     esac; 	  wget -O /tmp/openjdk.tar.gz ${BINARY_URL}; 	  echo "${ESUM} */tmp/openjdk.tar.gz" | sha256sum -c -; 	  mkdir -p "$JAVA_HOME"; 	  tar --extract 	      --file /tmp/openjdk.tar.gz 	      --directory "$JAVA_HOME" 	      --strip-components 1 	      --no-same-owner 	  ;     rm /tmp/openjdk.tar.gz;     find "$JAVA_HOME/lib" -name '*.so' -exec dirname '{}' ';' | sort -u > /etc/ld.so.conf.d/docker-openjdk.conf;     ldconfig;     java -Xshare:dump;
# Fri, 04 Nov 2022 23:22:32 GMT
RUN echo Verifying install ...     && fileEncoding="$(echo 'System.out.println(System.getProperty("file.encoding"))' | jshell -s -)"; [ "$fileEncoding" = 'UTF-8' ]; rm -rf ~/.java     && echo java --version && java --version     && echo Complete.
# Sat, 05 Nov 2022 01:35:16 GMT
ENV CATALINA_HOME=/usr/local/tomcat
# Sat, 05 Nov 2022 01:35:16 GMT
ENV PATH=/usr/local/tomcat/bin:/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Sat, 05 Nov 2022 01:35:17 GMT
RUN mkdir -p "$CATALINA_HOME"
# Sat, 05 Nov 2022 01:35:17 GMT
WORKDIR /usr/local/tomcat
# Sat, 05 Nov 2022 01:35:17 GMT
ENV TOMCAT_NATIVE_LIBDIR=/usr/local/tomcat/native-jni-lib
# Sat, 05 Nov 2022 01:35:17 GMT
ENV LD_LIBRARY_PATH=/usr/local/tomcat/native-jni-lib
# Sat, 05 Nov 2022 01:39:54 GMT
ENV GPG_KEYS=48F8E69F6390C9F25CFEDCD268248959359E722B A9C5DF4D22E99998D9875A5110C01C5A2F6059E7 DCFD35E0BF8CA7344752DE8B6FB21E8933C60243
# Sat, 05 Nov 2022 01:39:54 GMT
ENV TOMCAT_MAJOR=9
# Tue, 15 Nov 2022 03:06:43 GMT
ENV TOMCAT_VERSION=9.0.69
# Tue, 15 Nov 2022 03:06:43 GMT
ENV TOMCAT_SHA512=8c883c54ce9ce43eba37756a6404cdf3477879883a3e6d146dc8a7aa5e0425f487466afe6b6da4a895927cb7cb59177b9379cec18000f2de12785be57408c779
# Tue, 15 Nov 2022 03:06:44 GMT
COPY dir:b1a33aa3993dbbfbebb33bd9aa546b60c2f2191abf1227f453d4e830f6deb35f in /usr/local/tomcat 
# Tue, 15 Nov 2022 03:06:48 GMT
RUN set -eux; 	apt-get update; 	xargs -rt apt-get install -y --no-install-recommends < "$TOMCAT_NATIVE_LIBDIR/.dependencies.txt"; 	rm -rf /var/lib/apt/lists/*
# Tue, 15 Nov 2022 03:06:49 GMT
RUN set -eux; 	nativeLines="$(catalina.sh configtest 2>&1)"; 	nativeLines="$(echo "$nativeLines" | grep 'Apache Tomcat Native')"; 	nativeLines="$(echo "$nativeLines" | sort -u)"; 	if ! echo "$nativeLines" | grep -E 'INFO: Loaded( APR based)? Apache Tomcat Native library' >&2; then 		echo >&2 "$nativeLines"; 		exit 1; 	fi
# Tue, 15 Nov 2022 03:06:49 GMT
EXPOSE 8080
# Tue, 15 Nov 2022 03:06:49 GMT
CMD ["catalina.sh" "run"]
# Wed, 11 Jan 2023 02:47:03 GMT
LABEL org.opencontainers.image.authors=XWiki Development Team <committers@xwiki.org>
# Wed, 11 Jan 2023 02:47:03 GMT
LABEL org.opencontainers.image.url=https://hub.docker.com/_/xwiki
# Wed, 11 Jan 2023 02:47:03 GMT
LABEL org.opencontainers.image.documentation=https://hub.docker.com/_/xwiki
# Wed, 11 Jan 2023 02:47:03 GMT
LABEL org.opencontainers.image.source=https://github.com/xwiki/xwiki-docker.git
# Wed, 11 Jan 2023 02:47:04 GMT
LABEL org.opencontainers.image.vendor=xwiki.org
# Wed, 11 Jan 2023 02:47:04 GMT
LABEL org.opencontainers.image.licenses=LGPL-2.1
# Wed, 11 Jan 2023 02:49:03 GMT
RUN apt-get update &&   apt-get --no-install-recommends -y install     curl     libreoffice     unzip     procps &&   rm -rf /var/lib/apt/lists/*
# Tue, 31 Jan 2023 00:20:17 GMT
ENV XWIKI_VERSION=15.0
# Tue, 31 Jan 2023 00:20:17 GMT
ENV XWIKI_URL_PREFIX=https://maven.xwiki.org/releases/org/xwiki/platform/xwiki-platform-distribution-war/15.0
# Tue, 31 Jan 2023 00:20:17 GMT
ENV XWIKI_DOWNLOAD_SHA256=79ba0f479bbc49521c113821adc9d91141075a9470d7f9bbb6994ca59c30d121
# Tue, 31 Jan 2023 00:21:18 GMT
RUN rm -rf /usr/local/tomcat/webapps/* &&   mkdir -p /usr/local/tomcat/temp &&   mkdir -p /usr/local/xwiki/data &&   curl -fSL "${XWIKI_URL_PREFIX}/xwiki-platform-distribution-war-${XWIKI_VERSION}.war" -o xwiki.war &&   echo "$XWIKI_DOWNLOAD_SHA256 xwiki.war" | sha256sum -c - &&   unzip -d /usr/local/tomcat/webapps/ROOT xwiki.war &&   rm -f xwiki.war
# Tue, 31 Jan 2023 00:22:50 GMT
ENV MARIADB_JDBC_VERSION=3.1.1
# Tue, 31 Jan 2023 00:22:50 GMT
ENV MARIADB_JDBC_SHA256=a554541fd88047905fb0c4c10e1d85295f5e38c7bb5fb408b425392a79fc26e3
# Tue, 31 Jan 2023 00:22:50 GMT
ENV MARIADB_JDBC_PREFIX=https://repo1.maven.org/maven2/org/mariadb/jdbc/mariadb-java-client/3.1.1
# Tue, 31 Jan 2023 00:22:50 GMT
ENV MARIADB_JDBC_ARTIFACT=mariadb-java-client-3.1.1.jar
# Tue, 31 Jan 2023 00:22:50 GMT
ENV MARIADB_JDBC_TARGET=/usr/local/tomcat/webapps/ROOT/WEB-INF/lib/mariadb-java-client-3.1.1.jar
# Tue, 31 Jan 2023 00:22:51 GMT
RUN curl -fSL "${MARIADB_JDBC_PREFIX}/${MARIADB_JDBC_ARTIFACT}" -o $MARIADB_JDBC_TARGET &&   echo "$MARIADB_JDBC_SHA256 $MARIADB_JDBC_TARGET" | sha256sum -c -
# Tue, 31 Jan 2023 00:22:51 GMT
COPY file:0a1be11e2eb610a1dbcd415404e3a592641110b93090030cb831e3a19a163017 in /usr/local/tomcat/bin/ 
# Tue, 31 Jan 2023 00:22:51 GMT
COPY file:0e237c3876eeb3b5f3473a064d3e507da2df6c228ca714687930b34e3b687601 in /usr/local/tomcat/webapps/ROOT/WEB-INF/hibernate.cfg.xml 
# Tue, 31 Jan 2023 00:22:52 GMT
RUN sed -i 's/<id>org.xwiki.platform:xwiki-platform-distribution-war/<id>org.xwiki.platform:xwiki-platform-distribution-docker/'   /usr/local/tomcat/webapps/ROOT/META-INF/extension.xed
# Tue, 31 Jan 2023 00:22:52 GMT
COPY file:a47c4dcd87c9dad97aff38c49188357e6193bcad50757e516cfb08a60d4de611 in /usr/local/bin/docker-entrypoint.sh 
# Tue, 31 Jan 2023 00:22:52 GMT
VOLUME [/usr/local/xwiki]
# Tue, 31 Jan 2023 00:22:52 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 31 Jan 2023 00:22:52 GMT
CMD ["xwiki"]
```

-	Layers:
	-	`sha256:e96e057aae67380a4ddb16c337c5c3669d97fdff69ec537f02aa2cc30d814281`  
		Last Modified: Wed, 02 Nov 2022 03:03:36 GMT  
		Size: 30.4 MB (30425607 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4ced2591451da3a02e2b6bb44752b9e3f00d77789921be4df5082fb9f9880ad0`  
		Last Modified: Wed, 02 Nov 2022 18:48:43 GMT  
		Size: 12.4 MB (12439006 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:df8f874ae8c08a9e69e5fbe6c5a64200a45386132a3203d1a9a7f1146d94cfbc`  
		Last Modified: Fri, 04 Nov 2022 23:29:33 GMT  
		Size: 46.6 MB (46629936 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:111b6c7486426c4b6989102c2ee5be856e8a58e20ab0a350b24a905d536e8e7f`  
		Last Modified: Fri, 04 Nov 2022 23:29:26 GMT  
		Size: 161.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e6f84dce457c6d4f7b7291fce05f8e77998a3a7722a54125a1f1d52ca83043b4`  
		Last Modified: Sat, 05 Nov 2022 01:50:51 GMT  
		Size: 173.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a6c26749ee782392e38845ee2ba79b0da586ef6a45d8e7f29c7af14612278547`  
		Last Modified: Tue, 15 Nov 2022 03:19:57 GMT  
		Size: 12.2 MB (12200249 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4dddc6d9fa6024025b3fcfe729cab2dc544fb25476eca6e80b1af8e8d93bb0ee`  
		Last Modified: Tue, 15 Nov 2022 03:19:56 GMT  
		Size: 452.7 KB (452680 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:06637eebe5e72c8ad9019ad4eb4cdde1f11f7d4c24c7ed7374cf8966343aa2fb`  
		Last Modified: Tue, 15 Nov 2022 03:19:56 GMT  
		Size: 131.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b276fb8390410a8208724033e325715ea26000d5a1a762d4c3699b927884fbfe`  
		Last Modified: Wed, 11 Jan 2023 02:52:45 GMT  
		Size: 178.8 MB (178805608 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:156ca91198173149698aa0396648a9608b6ab1f2bc2666800843ce33c9f85b6e`  
		Last Modified: Tue, 31 Jan 2023 00:24:09 GMT  
		Size: 307.1 MB (307117069 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:457b62e39784bb863cc6a7514f591232a9b9442f2f105a85bdbd5e4abb166ad6`  
		Last Modified: Tue, 31 Jan 2023 00:25:23 GMT  
		Size: 589.7 KB (589675 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:30adbbecb36197c3e48c90be60a50c089cb9738a771c968b36240b05b8164a30`  
		Last Modified: Tue, 31 Jan 2023 00:25:22 GMT  
		Size: 1.3 KB (1345 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3bfcc8a896e6e21d5c28da101d5d57167a5cfc49c542a407feabe27f6c355b6f`  
		Last Modified: Tue, 31 Jan 2023 00:25:22 GMT  
		Size: 2.3 KB (2312 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5cbacf6c3ece365f64b683c8ab4fe61301319c8f1bd26d38ea40abbbd15bc7d4`  
		Last Modified: Tue, 31 Jan 2023 00:25:23 GMT  
		Size: 6.0 KB (6008 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6687ecee0e041196fd810c316565d70808b445cdce0b089b2177e6636bffd9fe`  
		Last Modified: Tue, 31 Jan 2023 00:25:23 GMT  
		Size: 2.5 KB (2507 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `xwiki:15.0.0-mariadb-tomcat` - linux; arm64 variant v8

```console
$ docker pull xwiki@sha256:14b1c6df2a5c5c9b549f372fce50719f39fc809b8b02c945d92eb29c29f7bc75
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **579.9 MB (579922416 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d9a728666283f6f4b71f567ce6c5ef1e2dc544facfd01d52fdf1577be95c6b07`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["xwiki"]`

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
# Wed, 02 Nov 2022 19:44:32 GMT
RUN apt-get update     && DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends tzdata curl wget ca-certificates fontconfig locales     && echo "en_US.UTF-8 UTF-8" >> /etc/locale.gen     && locale-gen en_US.UTF-8     && rm -rf /var/lib/apt/lists/*
# Fri, 04 Nov 2022 22:40:54 GMT
ENV JAVA_VERSION=jdk-11.0.17+8
# Fri, 04 Nov 2022 22:41:33 GMT
RUN set -eux;     ARCH="$(dpkg --print-architecture)";     case "${ARCH}" in        aarch64|arm64)          ESUM='bd6efe3290c8b5a42f695a55a26f3e3c9c284288574879d4b7089f31f5114177';          BINARY_URL='https://github.com/adoptium/temurin11-binaries/releases/download/jdk-11.0.17%2B8/OpenJDK11U-jre_aarch64_linux_hotspot_11.0.17_8.tar.gz';          ;;        armhf|arm)          ESUM='8cf113d3d7fa808895c8d2e41bb890af21c47e38c2460e0588147a4bb8fc658d';          BINARY_URL='https://github.com/adoptium/temurin11-binaries/releases/download/jdk-11.0.17%2B8/OpenJDK11U-jre_arm_linux_hotspot_11.0.17_8.tar.gz';          ;;        ppc64el|powerpc:common64)          ESUM='0ca3d806131ab5834c501f9c625bb0248cd528af361c704503348e9c9605bedf';          BINARY_URL='https://github.com/adoptium/temurin11-binaries/releases/download/jdk-11.0.17%2B8/OpenJDK11U-jre_ppc64le_linux_hotspot_11.0.17_8.tar.gz';          ;;        s390x|s390:64-bit)          ESUM='dd3b159a374086e65cb07c4ccb226c90f9c02ef929cba6f0b642171d7ed97fa4';          BINARY_URL='https://github.com/adoptium/temurin11-binaries/releases/download/jdk-11.0.17%2B8/OpenJDK11U-jre_s390x_linux_hotspot_11.0.17_8.tar.gz';          ;;        amd64|i386:x86-64)          ESUM='752616097e09d7f60a3ad8bd312f90eaf50ac72577e55df229fe6e8091148f79';          BINARY_URL='https://github.com/adoptium/temurin11-binaries/releases/download/jdk-11.0.17%2B8/OpenJDK11U-jre_x64_linux_hotspot_11.0.17_8.tar.gz';          ;;        *)          echo "Unsupported arch: ${ARCH}";          exit 1;          ;;     esac; 	  wget -O /tmp/openjdk.tar.gz ${BINARY_URL}; 	  echo "${ESUM} */tmp/openjdk.tar.gz" | sha256sum -c -; 	  mkdir -p "$JAVA_HOME"; 	  tar --extract 	      --file /tmp/openjdk.tar.gz 	      --directory "$JAVA_HOME" 	      --strip-components 1 	      --no-same-owner 	  ;     rm /tmp/openjdk.tar.gz;     find "$JAVA_HOME/lib" -name '*.so' -exec dirname '{}' ';' | sort -u > /etc/ld.so.conf.d/docker-openjdk.conf;     ldconfig;     java -Xshare:dump;
# Fri, 04 Nov 2022 22:41:34 GMT
RUN echo Verifying install ...     && fileEncoding="$(echo 'System.out.println(System.getProperty("file.encoding"))' | jshell -s -)"; [ "$fileEncoding" = 'UTF-8' ]; rm -rf ~/.java     && echo java --version && java --version     && echo Complete.
# Fri, 04 Nov 2022 23:48:38 GMT
ENV CATALINA_HOME=/usr/local/tomcat
# Fri, 04 Nov 2022 23:48:38 GMT
ENV PATH=/usr/local/tomcat/bin:/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Fri, 04 Nov 2022 23:48:38 GMT
RUN mkdir -p "$CATALINA_HOME"
# Fri, 04 Nov 2022 23:48:39 GMT
WORKDIR /usr/local/tomcat
# Fri, 04 Nov 2022 23:48:39 GMT
ENV TOMCAT_NATIVE_LIBDIR=/usr/local/tomcat/native-jni-lib
# Fri, 04 Nov 2022 23:48:39 GMT
ENV LD_LIBRARY_PATH=/usr/local/tomcat/native-jni-lib
# Fri, 04 Nov 2022 23:53:12 GMT
ENV GPG_KEYS=48F8E69F6390C9F25CFEDCD268248959359E722B A9C5DF4D22E99998D9875A5110C01C5A2F6059E7 DCFD35E0BF8CA7344752DE8B6FB21E8933C60243
# Fri, 04 Nov 2022 23:53:12 GMT
ENV TOMCAT_MAJOR=9
# Tue, 15 Nov 2022 04:57:22 GMT
ENV TOMCAT_VERSION=9.0.69
# Tue, 15 Nov 2022 04:57:22 GMT
ENV TOMCAT_SHA512=8c883c54ce9ce43eba37756a6404cdf3477879883a3e6d146dc8a7aa5e0425f487466afe6b6da4a895927cb7cb59177b9379cec18000f2de12785be57408c779
# Tue, 15 Nov 2022 04:57:22 GMT
COPY dir:096b403a5f78b17e6b4bff63128a9c93941b97f22470991610dd641633d977f1 in /usr/local/tomcat 
# Tue, 15 Nov 2022 04:57:25 GMT
RUN set -eux; 	apt-get update; 	xargs -rt apt-get install -y --no-install-recommends < "$TOMCAT_NATIVE_LIBDIR/.dependencies.txt"; 	rm -rf /var/lib/apt/lists/*
# Tue, 15 Nov 2022 04:57:26 GMT
RUN set -eux; 	nativeLines="$(catalina.sh configtest 2>&1)"; 	nativeLines="$(echo "$nativeLines" | grep 'Apache Tomcat Native')"; 	nativeLines="$(echo "$nativeLines" | sort -u)"; 	if ! echo "$nativeLines" | grep -E 'INFO: Loaded( APR based)? Apache Tomcat Native library' >&2; then 		echo >&2 "$nativeLines"; 		exit 1; 	fi
# Tue, 15 Nov 2022 04:57:26 GMT
EXPOSE 8080
# Tue, 15 Nov 2022 04:57:27 GMT
CMD ["catalina.sh" "run"]
# Wed, 11 Jan 2023 03:05:10 GMT
LABEL org.opencontainers.image.authors=XWiki Development Team <committers@xwiki.org>
# Wed, 11 Jan 2023 03:05:10 GMT
LABEL org.opencontainers.image.url=https://hub.docker.com/_/xwiki
# Wed, 11 Jan 2023 03:05:10 GMT
LABEL org.opencontainers.image.documentation=https://hub.docker.com/_/xwiki
# Wed, 11 Jan 2023 03:05:10 GMT
LABEL org.opencontainers.image.source=https://github.com/xwiki/xwiki-docker.git
# Wed, 11 Jan 2023 03:05:11 GMT
LABEL org.opencontainers.image.vendor=xwiki.org
# Wed, 11 Jan 2023 03:05:11 GMT
LABEL org.opencontainers.image.licenses=LGPL-2.1
# Wed, 11 Jan 2023 03:07:37 GMT
RUN apt-get update &&   apt-get --no-install-recommends -y install     curl     libreoffice     unzip     procps &&   rm -rf /var/lib/apt/lists/*
# Tue, 31 Jan 2023 00:47:12 GMT
ENV XWIKI_VERSION=15.0
# Tue, 31 Jan 2023 00:47:12 GMT
ENV XWIKI_URL_PREFIX=https://maven.xwiki.org/releases/org/xwiki/platform/xwiki-platform-distribution-war/15.0
# Tue, 31 Jan 2023 00:47:12 GMT
ENV XWIKI_DOWNLOAD_SHA256=79ba0f479bbc49521c113821adc9d91141075a9470d7f9bbb6994ca59c30d121
# Tue, 31 Jan 2023 00:47:58 GMT
RUN rm -rf /usr/local/tomcat/webapps/* &&   mkdir -p /usr/local/tomcat/temp &&   mkdir -p /usr/local/xwiki/data &&   curl -fSL "${XWIKI_URL_PREFIX}/xwiki-platform-distribution-war-${XWIKI_VERSION}.war" -o xwiki.war &&   echo "$XWIKI_DOWNLOAD_SHA256 xwiki.war" | sha256sum -c - &&   unzip -d /usr/local/tomcat/webapps/ROOT xwiki.war &&   rm -f xwiki.war
# Tue, 31 Jan 2023 00:54:48 GMT
ENV MARIADB_JDBC_VERSION=3.1.1
# Tue, 31 Jan 2023 00:54:48 GMT
ENV MARIADB_JDBC_SHA256=a554541fd88047905fb0c4c10e1d85295f5e38c7bb5fb408b425392a79fc26e3
# Tue, 31 Jan 2023 00:54:48 GMT
ENV MARIADB_JDBC_PREFIX=https://repo1.maven.org/maven2/org/mariadb/jdbc/mariadb-java-client/3.1.1
# Tue, 31 Jan 2023 00:54:48 GMT
ENV MARIADB_JDBC_ARTIFACT=mariadb-java-client-3.1.1.jar
# Tue, 31 Jan 2023 00:54:48 GMT
ENV MARIADB_JDBC_TARGET=/usr/local/tomcat/webapps/ROOT/WEB-INF/lib/mariadb-java-client-3.1.1.jar
# Tue, 31 Jan 2023 00:54:49 GMT
RUN curl -fSL "${MARIADB_JDBC_PREFIX}/${MARIADB_JDBC_ARTIFACT}" -o $MARIADB_JDBC_TARGET &&   echo "$MARIADB_JDBC_SHA256 $MARIADB_JDBC_TARGET" | sha256sum -c -
# Tue, 31 Jan 2023 00:54:49 GMT
COPY file:0a1be11e2eb610a1dbcd415404e3a592641110b93090030cb831e3a19a163017 in /usr/local/tomcat/bin/ 
# Tue, 31 Jan 2023 00:54:49 GMT
COPY file:0e237c3876eeb3b5f3473a064d3e507da2df6c228ca714687930b34e3b687601 in /usr/local/tomcat/webapps/ROOT/WEB-INF/hibernate.cfg.xml 
# Tue, 31 Jan 2023 00:54:49 GMT
RUN sed -i 's/<id>org.xwiki.platform:xwiki-platform-distribution-war/<id>org.xwiki.platform:xwiki-platform-distribution-docker/'   /usr/local/tomcat/webapps/ROOT/META-INF/extension.xed
# Tue, 31 Jan 2023 00:54:49 GMT
COPY file:a47c4dcd87c9dad97aff38c49188357e6193bcad50757e516cfb08a60d4de611 in /usr/local/bin/docker-entrypoint.sh 
# Tue, 31 Jan 2023 00:54:49 GMT
VOLUME [/usr/local/xwiki]
# Tue, 31 Jan 2023 00:54:50 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 31 Jan 2023 00:54:50 GMT
CMD ["xwiki"]
```

-	Layers:
	-	`sha256:0509fae36eb0656f8bdb23f8ae64100d893bcea2563e97468d337e04d2d0410b`  
		Last Modified: Wed, 02 Nov 2022 18:50:21 GMT  
		Size: 28.4 MB (28382154 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e502a1af2bcd98f5f0d2f5e4da1a0e7bbe07a2c548e2662f7d37dce5ae1df46c`  
		Last Modified: Wed, 02 Nov 2022 19:48:28 GMT  
		Size: 12.4 MB (12396330 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bc4598c07dd818f03a0378b0341a4a8e80f0152fbb3e7d5246ca4f466f42e611`  
		Last Modified: Fri, 04 Nov 2022 22:46:46 GMT  
		Size: 45.0 MB (44958470 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:715a937a1066f998b331fcd62256ad01a5571bdf46804e97825afc64f9ebb427`  
		Last Modified: Fri, 04 Nov 2022 22:46:41 GMT  
		Size: 160.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5fb623f082f74b2fa9fc2c4e3f3a4802875cb9753cfa26ed940201ce72bb56cb`  
		Last Modified: Sat, 05 Nov 2022 00:03:40 GMT  
		Size: 172.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:33260b83200262bbd546be371ad3c1f50f5ae7228afb87982d6fa9d6b11bf26f`  
		Last Modified: Tue, 15 Nov 2022 05:10:19 GMT  
		Size: 12.2 MB (12207235 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0955fb697ea9b30a1b4f95385464f646aa1525cb6efba648e22df84ebef6b2ee`  
		Last Modified: Tue, 15 Nov 2022 05:10:18 GMT  
		Size: 452.0 KB (452021 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6eddcf66f2083b1487296a0308e0b058917c97f614f12428d82d89662038dc2e`  
		Last Modified: Tue, 15 Nov 2022 05:10:18 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ae5f60bb64f3fa11da3d15a9639f886186b4c2c021455c3f9db22e0cfe1b1311`  
		Last Modified: Wed, 11 Jan 2023 03:11:14 GMT  
		Size: 173.8 MB (173806827 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1814d85fce571b42f2cfa7c8a904e1a184ee6f49642242a44bbe0037088994a0`  
		Last Modified: Tue, 31 Jan 2023 00:56:04 GMT  
		Size: 307.1 MB (307117070 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e8637677b7ba0da683afa4e56ff0561e4ba77c8782d5a98da785f4ef58d1caf9`  
		Last Modified: Tue, 31 Jan 2023 00:57:14 GMT  
		Size: 589.7 KB (589677 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:61a67398bc888bcce1656edec9bb40409ce0ffc2fe83d0437c28dd64a8f697ce`  
		Last Modified: Tue, 31 Jan 2023 00:57:14 GMT  
		Size: 1.3 KB (1345 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7ebda7e506ea819ce9717c3d0334df81608bc4c7149cd47ebc9a32790141a637`  
		Last Modified: Tue, 31 Jan 2023 00:57:14 GMT  
		Size: 2.3 KB (2313 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2ceebbf08640e235a928c9df650ca3ab8d0c6b506faa158ecde5fdde34bf8813`  
		Last Modified: Tue, 31 Jan 2023 00:57:14 GMT  
		Size: 6.0 KB (6007 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:12b1d23eae23b1a09ecd4185941d43f13d4ad633d4c6257ab8107a8eebd5fb12`  
		Last Modified: Tue, 31 Jan 2023 00:57:14 GMT  
		Size: 2.5 KB (2506 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `xwiki:15.0.0-mysql-tomcat`

```console
$ docker pull xwiki@sha256:33e789838f82ce73efec6664859feb1ced7a5b7605fbfaddb81916716bce524f
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `xwiki:15.0.0-mysql-tomcat` - linux; amd64

```console
$ docker pull xwiki@sha256:481fdb46e8c043a6709d11310e2083ce71d6ba63ee6517f84da3ba06f320598e
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **590.5 MB (590459982 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:bd630aa0aa5c679e23ea7d52cbbdd6b817eab27a820c25d3c50b54eca83b9744`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["xwiki"]`

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
# Wed, 02 Nov 2022 18:44:10 GMT
RUN apt-get update     && DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends tzdata curl wget ca-certificates fontconfig locales     && echo "en_US.UTF-8 UTF-8" >> /etc/locale.gen     && locale-gen en_US.UTF-8     && rm -rf /var/lib/apt/lists/*
# Fri, 04 Nov 2022 23:21:41 GMT
ENV JAVA_VERSION=jdk-11.0.17+8
# Fri, 04 Nov 2022 23:22:31 GMT
RUN set -eux;     ARCH="$(dpkg --print-architecture)";     case "${ARCH}" in        aarch64|arm64)          ESUM='bd6efe3290c8b5a42f695a55a26f3e3c9c284288574879d4b7089f31f5114177';          BINARY_URL='https://github.com/adoptium/temurin11-binaries/releases/download/jdk-11.0.17%2B8/OpenJDK11U-jre_aarch64_linux_hotspot_11.0.17_8.tar.gz';          ;;        armhf|arm)          ESUM='8cf113d3d7fa808895c8d2e41bb890af21c47e38c2460e0588147a4bb8fc658d';          BINARY_URL='https://github.com/adoptium/temurin11-binaries/releases/download/jdk-11.0.17%2B8/OpenJDK11U-jre_arm_linux_hotspot_11.0.17_8.tar.gz';          ;;        ppc64el|powerpc:common64)          ESUM='0ca3d806131ab5834c501f9c625bb0248cd528af361c704503348e9c9605bedf';          BINARY_URL='https://github.com/adoptium/temurin11-binaries/releases/download/jdk-11.0.17%2B8/OpenJDK11U-jre_ppc64le_linux_hotspot_11.0.17_8.tar.gz';          ;;        s390x|s390:64-bit)          ESUM='dd3b159a374086e65cb07c4ccb226c90f9c02ef929cba6f0b642171d7ed97fa4';          BINARY_URL='https://github.com/adoptium/temurin11-binaries/releases/download/jdk-11.0.17%2B8/OpenJDK11U-jre_s390x_linux_hotspot_11.0.17_8.tar.gz';          ;;        amd64|i386:x86-64)          ESUM='752616097e09d7f60a3ad8bd312f90eaf50ac72577e55df229fe6e8091148f79';          BINARY_URL='https://github.com/adoptium/temurin11-binaries/releases/download/jdk-11.0.17%2B8/OpenJDK11U-jre_x64_linux_hotspot_11.0.17_8.tar.gz';          ;;        *)          echo "Unsupported arch: ${ARCH}";          exit 1;          ;;     esac; 	  wget -O /tmp/openjdk.tar.gz ${BINARY_URL}; 	  echo "${ESUM} */tmp/openjdk.tar.gz" | sha256sum -c -; 	  mkdir -p "$JAVA_HOME"; 	  tar --extract 	      --file /tmp/openjdk.tar.gz 	      --directory "$JAVA_HOME" 	      --strip-components 1 	      --no-same-owner 	  ;     rm /tmp/openjdk.tar.gz;     find "$JAVA_HOME/lib" -name '*.so' -exec dirname '{}' ';' | sort -u > /etc/ld.so.conf.d/docker-openjdk.conf;     ldconfig;     java -Xshare:dump;
# Fri, 04 Nov 2022 23:22:32 GMT
RUN echo Verifying install ...     && fileEncoding="$(echo 'System.out.println(System.getProperty("file.encoding"))' | jshell -s -)"; [ "$fileEncoding" = 'UTF-8' ]; rm -rf ~/.java     && echo java --version && java --version     && echo Complete.
# Sat, 05 Nov 2022 01:35:16 GMT
ENV CATALINA_HOME=/usr/local/tomcat
# Sat, 05 Nov 2022 01:35:16 GMT
ENV PATH=/usr/local/tomcat/bin:/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Sat, 05 Nov 2022 01:35:17 GMT
RUN mkdir -p "$CATALINA_HOME"
# Sat, 05 Nov 2022 01:35:17 GMT
WORKDIR /usr/local/tomcat
# Sat, 05 Nov 2022 01:35:17 GMT
ENV TOMCAT_NATIVE_LIBDIR=/usr/local/tomcat/native-jni-lib
# Sat, 05 Nov 2022 01:35:17 GMT
ENV LD_LIBRARY_PATH=/usr/local/tomcat/native-jni-lib
# Sat, 05 Nov 2022 01:39:54 GMT
ENV GPG_KEYS=48F8E69F6390C9F25CFEDCD268248959359E722B A9C5DF4D22E99998D9875A5110C01C5A2F6059E7 DCFD35E0BF8CA7344752DE8B6FB21E8933C60243
# Sat, 05 Nov 2022 01:39:54 GMT
ENV TOMCAT_MAJOR=9
# Tue, 15 Nov 2022 03:06:43 GMT
ENV TOMCAT_VERSION=9.0.69
# Tue, 15 Nov 2022 03:06:43 GMT
ENV TOMCAT_SHA512=8c883c54ce9ce43eba37756a6404cdf3477879883a3e6d146dc8a7aa5e0425f487466afe6b6da4a895927cb7cb59177b9379cec18000f2de12785be57408c779
# Tue, 15 Nov 2022 03:06:44 GMT
COPY dir:b1a33aa3993dbbfbebb33bd9aa546b60c2f2191abf1227f453d4e830f6deb35f in /usr/local/tomcat 
# Tue, 15 Nov 2022 03:06:48 GMT
RUN set -eux; 	apt-get update; 	xargs -rt apt-get install -y --no-install-recommends < "$TOMCAT_NATIVE_LIBDIR/.dependencies.txt"; 	rm -rf /var/lib/apt/lists/*
# Tue, 15 Nov 2022 03:06:49 GMT
RUN set -eux; 	nativeLines="$(catalina.sh configtest 2>&1)"; 	nativeLines="$(echo "$nativeLines" | grep 'Apache Tomcat Native')"; 	nativeLines="$(echo "$nativeLines" | sort -u)"; 	if ! echo "$nativeLines" | grep -E 'INFO: Loaded( APR based)? Apache Tomcat Native library' >&2; then 		echo >&2 "$nativeLines"; 		exit 1; 	fi
# Tue, 15 Nov 2022 03:06:49 GMT
EXPOSE 8080
# Tue, 15 Nov 2022 03:06:49 GMT
CMD ["catalina.sh" "run"]
# Wed, 11 Jan 2023 02:47:03 GMT
LABEL org.opencontainers.image.authors=XWiki Development Team <committers@xwiki.org>
# Wed, 11 Jan 2023 02:47:03 GMT
LABEL org.opencontainers.image.url=https://hub.docker.com/_/xwiki
# Wed, 11 Jan 2023 02:47:03 GMT
LABEL org.opencontainers.image.documentation=https://hub.docker.com/_/xwiki
# Wed, 11 Jan 2023 02:47:03 GMT
LABEL org.opencontainers.image.source=https://github.com/xwiki/xwiki-docker.git
# Wed, 11 Jan 2023 02:47:04 GMT
LABEL org.opencontainers.image.vendor=xwiki.org
# Wed, 11 Jan 2023 02:47:04 GMT
LABEL org.opencontainers.image.licenses=LGPL-2.1
# Wed, 11 Jan 2023 02:49:03 GMT
RUN apt-get update &&   apt-get --no-install-recommends -y install     curl     libreoffice     unzip     procps &&   rm -rf /var/lib/apt/lists/*
# Tue, 31 Jan 2023 00:20:17 GMT
ENV XWIKI_VERSION=15.0
# Tue, 31 Jan 2023 00:20:17 GMT
ENV XWIKI_URL_PREFIX=https://maven.xwiki.org/releases/org/xwiki/platform/xwiki-platform-distribution-war/15.0
# Tue, 31 Jan 2023 00:20:17 GMT
ENV XWIKI_DOWNLOAD_SHA256=79ba0f479bbc49521c113821adc9d91141075a9470d7f9bbb6994ca59c30d121
# Tue, 31 Jan 2023 00:21:18 GMT
RUN rm -rf /usr/local/tomcat/webapps/* &&   mkdir -p /usr/local/tomcat/temp &&   mkdir -p /usr/local/xwiki/data &&   curl -fSL "${XWIKI_URL_PREFIX}/xwiki-platform-distribution-war-${XWIKI_VERSION}.war" -o xwiki.war &&   echo "$XWIKI_DOWNLOAD_SHA256 xwiki.war" | sha256sum -c - &&   unzip -d /usr/local/tomcat/webapps/ROOT xwiki.war &&   rm -f xwiki.war
# Tue, 31 Jan 2023 00:21:19 GMT
ENV MYSQL_JDBC_VERSION=8.0.31
# Tue, 31 Jan 2023 00:21:19 GMT
ENV MYSQL_JDBC_SHA256=5249e3dc6d6531b37790e3f61845b96db5e41e891d3d8edb0e2e3a1b53ca2f4f
# Tue, 31 Jan 2023 00:21:19 GMT
ENV MYSQL_JDBC_PREFIX=https://repo1.maven.org/maven2/com/mysql/mysql-connector-j/8.0.31
# Tue, 31 Jan 2023 00:21:19 GMT
ENV MYSQL_JDBC_ARTIFACT=mysql-connector-j-8.0.31.jar
# Tue, 31 Jan 2023 00:21:19 GMT
ENV MYSQL_JDBC_TARGET=/usr/local/tomcat/webapps/ROOT/WEB-INF/lib/mysql-connector-j-8.0.31.jar
# Tue, 31 Jan 2023 00:21:20 GMT
RUN curl -fSL "${MYSQL_JDBC_PREFIX}/${MYSQL_JDBC_ARTIFACT}" -o $MYSQL_JDBC_TARGET &&   echo "$MYSQL_JDBC_SHA256 $MYSQL_JDBC_TARGET" | sha256sum -c -
# Tue, 31 Jan 2023 00:21:21 GMT
COPY file:0a1be11e2eb610a1dbcd415404e3a592641110b93090030cb831e3a19a163017 in /usr/local/tomcat/bin/ 
# Tue, 31 Jan 2023 00:21:21 GMT
COPY file:1b8409986f3e4eb79a7a0b18472cb2692a61d504fb5ef34292bc997b79fd760d in /usr/local/tomcat/webapps/ROOT/WEB-INF/hibernate.cfg.xml 
# Tue, 31 Jan 2023 00:21:21 GMT
RUN sed -i 's/<id>org.xwiki.platform:xwiki-platform-distribution-war/<id>org.xwiki.platform:xwiki-platform-distribution-docker/'   /usr/local/tomcat/webapps/ROOT/META-INF/extension.xed
# Tue, 31 Jan 2023 00:21:21 GMT
COPY file:a47c4dcd87c9dad97aff38c49188357e6193bcad50757e516cfb08a60d4de611 in /usr/local/bin/docker-entrypoint.sh 
# Tue, 31 Jan 2023 00:21:22 GMT
VOLUME [/usr/local/xwiki]
# Tue, 31 Jan 2023 00:21:22 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 31 Jan 2023 00:21:22 GMT
CMD ["xwiki"]
```

-	Layers:
	-	`sha256:e96e057aae67380a4ddb16c337c5c3669d97fdff69ec537f02aa2cc30d814281`  
		Last Modified: Wed, 02 Nov 2022 03:03:36 GMT  
		Size: 30.4 MB (30425607 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4ced2591451da3a02e2b6bb44752b9e3f00d77789921be4df5082fb9f9880ad0`  
		Last Modified: Wed, 02 Nov 2022 18:48:43 GMT  
		Size: 12.4 MB (12439006 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:df8f874ae8c08a9e69e5fbe6c5a64200a45386132a3203d1a9a7f1146d94cfbc`  
		Last Modified: Fri, 04 Nov 2022 23:29:33 GMT  
		Size: 46.6 MB (46629936 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:111b6c7486426c4b6989102c2ee5be856e8a58e20ab0a350b24a905d536e8e7f`  
		Last Modified: Fri, 04 Nov 2022 23:29:26 GMT  
		Size: 161.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e6f84dce457c6d4f7b7291fce05f8e77998a3a7722a54125a1f1d52ca83043b4`  
		Last Modified: Sat, 05 Nov 2022 01:50:51 GMT  
		Size: 173.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a6c26749ee782392e38845ee2ba79b0da586ef6a45d8e7f29c7af14612278547`  
		Last Modified: Tue, 15 Nov 2022 03:19:57 GMT  
		Size: 12.2 MB (12200249 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4dddc6d9fa6024025b3fcfe729cab2dc544fb25476eca6e80b1af8e8d93bb0ee`  
		Last Modified: Tue, 15 Nov 2022 03:19:56 GMT  
		Size: 452.7 KB (452680 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:06637eebe5e72c8ad9019ad4eb4cdde1f11f7d4c24c7ed7374cf8966343aa2fb`  
		Last Modified: Tue, 15 Nov 2022 03:19:56 GMT  
		Size: 131.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b276fb8390410a8208724033e325715ea26000d5a1a762d4c3699b927884fbfe`  
		Last Modified: Wed, 11 Jan 2023 02:52:45 GMT  
		Size: 178.8 MB (178805608 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:156ca91198173149698aa0396648a9608b6ab1f2bc2666800843ce33c9f85b6e`  
		Last Modified: Tue, 31 Jan 2023 00:24:09 GMT  
		Size: 307.1 MB (307117069 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4c8b70d250c6d507901857473b0dcb67132d7b2a30ce9a69b07b1036853df738`  
		Last Modified: Tue, 31 Jan 2023 00:23:52 GMT  
		Size: 2.4 MB (2377191 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a9681fd36be674d25231c69d6a39f9e8fa65034eeaef5d1bd885fdbeac7f0f6b`  
		Last Modified: Tue, 31 Jan 2023 00:23:51 GMT  
		Size: 1.3 KB (1346 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a9d0d5da840f4d7da9943942b38cd092fae11f41dc6c19afd58d655cd6192d66`  
		Last Modified: Tue, 31 Jan 2023 00:23:51 GMT  
		Size: 2.3 KB (2312 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d65610da4f1da86fea8fbec0189b066afd4b86e4e8f7d049e3c4bc6ade9ba90a`  
		Last Modified: Tue, 31 Jan 2023 00:23:51 GMT  
		Size: 6.0 KB (6009 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3d41686284d7675eaa0f92c9cc27ebe73b4c30768c8eef9f23ee3b1ad06da00a`  
		Last Modified: Tue, 31 Jan 2023 00:23:51 GMT  
		Size: 2.5 KB (2504 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `xwiki:15.0.0-mysql-tomcat` - linux; arm64 variant v8

```console
$ docker pull xwiki@sha256:6bf63d9025b07b69d744200c05efd4ffb8a52f3c38380f5d59a0b48514203cd2
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **581.7 MB (581709921 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:6600f2bb05836c703d53944bbcb5399d509a9813a27a35e99ff717becc308330`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["xwiki"]`

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
# Wed, 02 Nov 2022 19:44:32 GMT
RUN apt-get update     && DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends tzdata curl wget ca-certificates fontconfig locales     && echo "en_US.UTF-8 UTF-8" >> /etc/locale.gen     && locale-gen en_US.UTF-8     && rm -rf /var/lib/apt/lists/*
# Fri, 04 Nov 2022 22:40:54 GMT
ENV JAVA_VERSION=jdk-11.0.17+8
# Fri, 04 Nov 2022 22:41:33 GMT
RUN set -eux;     ARCH="$(dpkg --print-architecture)";     case "${ARCH}" in        aarch64|arm64)          ESUM='bd6efe3290c8b5a42f695a55a26f3e3c9c284288574879d4b7089f31f5114177';          BINARY_URL='https://github.com/adoptium/temurin11-binaries/releases/download/jdk-11.0.17%2B8/OpenJDK11U-jre_aarch64_linux_hotspot_11.0.17_8.tar.gz';          ;;        armhf|arm)          ESUM='8cf113d3d7fa808895c8d2e41bb890af21c47e38c2460e0588147a4bb8fc658d';          BINARY_URL='https://github.com/adoptium/temurin11-binaries/releases/download/jdk-11.0.17%2B8/OpenJDK11U-jre_arm_linux_hotspot_11.0.17_8.tar.gz';          ;;        ppc64el|powerpc:common64)          ESUM='0ca3d806131ab5834c501f9c625bb0248cd528af361c704503348e9c9605bedf';          BINARY_URL='https://github.com/adoptium/temurin11-binaries/releases/download/jdk-11.0.17%2B8/OpenJDK11U-jre_ppc64le_linux_hotspot_11.0.17_8.tar.gz';          ;;        s390x|s390:64-bit)          ESUM='dd3b159a374086e65cb07c4ccb226c90f9c02ef929cba6f0b642171d7ed97fa4';          BINARY_URL='https://github.com/adoptium/temurin11-binaries/releases/download/jdk-11.0.17%2B8/OpenJDK11U-jre_s390x_linux_hotspot_11.0.17_8.tar.gz';          ;;        amd64|i386:x86-64)          ESUM='752616097e09d7f60a3ad8bd312f90eaf50ac72577e55df229fe6e8091148f79';          BINARY_URL='https://github.com/adoptium/temurin11-binaries/releases/download/jdk-11.0.17%2B8/OpenJDK11U-jre_x64_linux_hotspot_11.0.17_8.tar.gz';          ;;        *)          echo "Unsupported arch: ${ARCH}";          exit 1;          ;;     esac; 	  wget -O /tmp/openjdk.tar.gz ${BINARY_URL}; 	  echo "${ESUM} */tmp/openjdk.tar.gz" | sha256sum -c -; 	  mkdir -p "$JAVA_HOME"; 	  tar --extract 	      --file /tmp/openjdk.tar.gz 	      --directory "$JAVA_HOME" 	      --strip-components 1 	      --no-same-owner 	  ;     rm /tmp/openjdk.tar.gz;     find "$JAVA_HOME/lib" -name '*.so' -exec dirname '{}' ';' | sort -u > /etc/ld.so.conf.d/docker-openjdk.conf;     ldconfig;     java -Xshare:dump;
# Fri, 04 Nov 2022 22:41:34 GMT
RUN echo Verifying install ...     && fileEncoding="$(echo 'System.out.println(System.getProperty("file.encoding"))' | jshell -s -)"; [ "$fileEncoding" = 'UTF-8' ]; rm -rf ~/.java     && echo java --version && java --version     && echo Complete.
# Fri, 04 Nov 2022 23:48:38 GMT
ENV CATALINA_HOME=/usr/local/tomcat
# Fri, 04 Nov 2022 23:48:38 GMT
ENV PATH=/usr/local/tomcat/bin:/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Fri, 04 Nov 2022 23:48:38 GMT
RUN mkdir -p "$CATALINA_HOME"
# Fri, 04 Nov 2022 23:48:39 GMT
WORKDIR /usr/local/tomcat
# Fri, 04 Nov 2022 23:48:39 GMT
ENV TOMCAT_NATIVE_LIBDIR=/usr/local/tomcat/native-jni-lib
# Fri, 04 Nov 2022 23:48:39 GMT
ENV LD_LIBRARY_PATH=/usr/local/tomcat/native-jni-lib
# Fri, 04 Nov 2022 23:53:12 GMT
ENV GPG_KEYS=48F8E69F6390C9F25CFEDCD268248959359E722B A9C5DF4D22E99998D9875A5110C01C5A2F6059E7 DCFD35E0BF8CA7344752DE8B6FB21E8933C60243
# Fri, 04 Nov 2022 23:53:12 GMT
ENV TOMCAT_MAJOR=9
# Tue, 15 Nov 2022 04:57:22 GMT
ENV TOMCAT_VERSION=9.0.69
# Tue, 15 Nov 2022 04:57:22 GMT
ENV TOMCAT_SHA512=8c883c54ce9ce43eba37756a6404cdf3477879883a3e6d146dc8a7aa5e0425f487466afe6b6da4a895927cb7cb59177b9379cec18000f2de12785be57408c779
# Tue, 15 Nov 2022 04:57:22 GMT
COPY dir:096b403a5f78b17e6b4bff63128a9c93941b97f22470991610dd641633d977f1 in /usr/local/tomcat 
# Tue, 15 Nov 2022 04:57:25 GMT
RUN set -eux; 	apt-get update; 	xargs -rt apt-get install -y --no-install-recommends < "$TOMCAT_NATIVE_LIBDIR/.dependencies.txt"; 	rm -rf /var/lib/apt/lists/*
# Tue, 15 Nov 2022 04:57:26 GMT
RUN set -eux; 	nativeLines="$(catalina.sh configtest 2>&1)"; 	nativeLines="$(echo "$nativeLines" | grep 'Apache Tomcat Native')"; 	nativeLines="$(echo "$nativeLines" | sort -u)"; 	if ! echo "$nativeLines" | grep -E 'INFO: Loaded( APR based)? Apache Tomcat Native library' >&2; then 		echo >&2 "$nativeLines"; 		exit 1; 	fi
# Tue, 15 Nov 2022 04:57:26 GMT
EXPOSE 8080
# Tue, 15 Nov 2022 04:57:27 GMT
CMD ["catalina.sh" "run"]
# Wed, 11 Jan 2023 03:05:10 GMT
LABEL org.opencontainers.image.authors=XWiki Development Team <committers@xwiki.org>
# Wed, 11 Jan 2023 03:05:10 GMT
LABEL org.opencontainers.image.url=https://hub.docker.com/_/xwiki
# Wed, 11 Jan 2023 03:05:10 GMT
LABEL org.opencontainers.image.documentation=https://hub.docker.com/_/xwiki
# Wed, 11 Jan 2023 03:05:10 GMT
LABEL org.opencontainers.image.source=https://github.com/xwiki/xwiki-docker.git
# Wed, 11 Jan 2023 03:05:11 GMT
LABEL org.opencontainers.image.vendor=xwiki.org
# Wed, 11 Jan 2023 03:05:11 GMT
LABEL org.opencontainers.image.licenses=LGPL-2.1
# Wed, 11 Jan 2023 03:07:37 GMT
RUN apt-get update &&   apt-get --no-install-recommends -y install     curl     libreoffice     unzip     procps &&   rm -rf /var/lib/apt/lists/*
# Tue, 31 Jan 2023 00:47:12 GMT
ENV XWIKI_VERSION=15.0
# Tue, 31 Jan 2023 00:47:12 GMT
ENV XWIKI_URL_PREFIX=https://maven.xwiki.org/releases/org/xwiki/platform/xwiki-platform-distribution-war/15.0
# Tue, 31 Jan 2023 00:47:12 GMT
ENV XWIKI_DOWNLOAD_SHA256=79ba0f479bbc49521c113821adc9d91141075a9470d7f9bbb6994ca59c30d121
# Tue, 31 Jan 2023 00:47:58 GMT
RUN rm -rf /usr/local/tomcat/webapps/* &&   mkdir -p /usr/local/tomcat/temp &&   mkdir -p /usr/local/xwiki/data &&   curl -fSL "${XWIKI_URL_PREFIX}/xwiki-platform-distribution-war-${XWIKI_VERSION}.war" -o xwiki.war &&   echo "$XWIKI_DOWNLOAD_SHA256 xwiki.war" | sha256sum -c - &&   unzip -d /usr/local/tomcat/webapps/ROOT xwiki.war &&   rm -f xwiki.war
# Tue, 31 Jan 2023 00:48:01 GMT
ENV MYSQL_JDBC_VERSION=8.0.31
# Tue, 31 Jan 2023 00:48:01 GMT
ENV MYSQL_JDBC_SHA256=5249e3dc6d6531b37790e3f61845b96db5e41e891d3d8edb0e2e3a1b53ca2f4f
# Tue, 31 Jan 2023 00:48:01 GMT
ENV MYSQL_JDBC_PREFIX=https://repo1.maven.org/maven2/com/mysql/mysql-connector-j/8.0.31
# Tue, 31 Jan 2023 00:48:01 GMT
ENV MYSQL_JDBC_ARTIFACT=mysql-connector-j-8.0.31.jar
# Tue, 31 Jan 2023 00:48:01 GMT
ENV MYSQL_JDBC_TARGET=/usr/local/tomcat/webapps/ROOT/WEB-INF/lib/mysql-connector-j-8.0.31.jar
# Tue, 31 Jan 2023 00:48:02 GMT
RUN curl -fSL "${MYSQL_JDBC_PREFIX}/${MYSQL_JDBC_ARTIFACT}" -o $MYSQL_JDBC_TARGET &&   echo "$MYSQL_JDBC_SHA256 $MYSQL_JDBC_TARGET" | sha256sum -c -
# Tue, 31 Jan 2023 00:48:02 GMT
COPY file:0a1be11e2eb610a1dbcd415404e3a592641110b93090030cb831e3a19a163017 in /usr/local/tomcat/bin/ 
# Tue, 31 Jan 2023 00:48:02 GMT
COPY file:1b8409986f3e4eb79a7a0b18472cb2692a61d504fb5ef34292bc997b79fd760d in /usr/local/tomcat/webapps/ROOT/WEB-INF/hibernate.cfg.xml 
# Tue, 31 Jan 2023 00:48:03 GMT
RUN sed -i 's/<id>org.xwiki.platform:xwiki-platform-distribution-war/<id>org.xwiki.platform:xwiki-platform-distribution-docker/'   /usr/local/tomcat/webapps/ROOT/META-INF/extension.xed
# Tue, 31 Jan 2023 00:48:03 GMT
COPY file:a47c4dcd87c9dad97aff38c49188357e6193bcad50757e516cfb08a60d4de611 in /usr/local/bin/docker-entrypoint.sh 
# Tue, 31 Jan 2023 00:48:03 GMT
VOLUME [/usr/local/xwiki]
# Tue, 31 Jan 2023 00:48:03 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 31 Jan 2023 00:48:03 GMT
CMD ["xwiki"]
```

-	Layers:
	-	`sha256:0509fae36eb0656f8bdb23f8ae64100d893bcea2563e97468d337e04d2d0410b`  
		Last Modified: Wed, 02 Nov 2022 18:50:21 GMT  
		Size: 28.4 MB (28382154 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e502a1af2bcd98f5f0d2f5e4da1a0e7bbe07a2c548e2662f7d37dce5ae1df46c`  
		Last Modified: Wed, 02 Nov 2022 19:48:28 GMT  
		Size: 12.4 MB (12396330 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bc4598c07dd818f03a0378b0341a4a8e80f0152fbb3e7d5246ca4f466f42e611`  
		Last Modified: Fri, 04 Nov 2022 22:46:46 GMT  
		Size: 45.0 MB (44958470 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:715a937a1066f998b331fcd62256ad01a5571bdf46804e97825afc64f9ebb427`  
		Last Modified: Fri, 04 Nov 2022 22:46:41 GMT  
		Size: 160.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5fb623f082f74b2fa9fc2c4e3f3a4802875cb9753cfa26ed940201ce72bb56cb`  
		Last Modified: Sat, 05 Nov 2022 00:03:40 GMT  
		Size: 172.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:33260b83200262bbd546be371ad3c1f50f5ae7228afb87982d6fa9d6b11bf26f`  
		Last Modified: Tue, 15 Nov 2022 05:10:19 GMT  
		Size: 12.2 MB (12207235 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0955fb697ea9b30a1b4f95385464f646aa1525cb6efba648e22df84ebef6b2ee`  
		Last Modified: Tue, 15 Nov 2022 05:10:18 GMT  
		Size: 452.0 KB (452021 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6eddcf66f2083b1487296a0308e0b058917c97f614f12428d82d89662038dc2e`  
		Last Modified: Tue, 15 Nov 2022 05:10:18 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ae5f60bb64f3fa11da3d15a9639f886186b4c2c021455c3f9db22e0cfe1b1311`  
		Last Modified: Wed, 11 Jan 2023 03:11:14 GMT  
		Size: 173.8 MB (173806827 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1814d85fce571b42f2cfa7c8a904e1a184ee6f49642242a44bbe0037088994a0`  
		Last Modified: Tue, 31 Jan 2023 00:56:04 GMT  
		Size: 307.1 MB (307117070 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8aec0e24b4fa870989f014944c3c7d535355a2371fc8c948b2b11f9b377efe6e`  
		Last Modified: Tue, 31 Jan 2023 00:55:50 GMT  
		Size: 2.4 MB (2377182 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0b65081619aa0114a7f367836ef421eb8d951e559e0f089c7728af7813b1ea62`  
		Last Modified: Tue, 31 Jan 2023 00:55:49 GMT  
		Size: 1.3 KB (1348 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:46ebad072e608146426d8dc30828937049eea36c2e636d7790b4960d6d586977`  
		Last Modified: Tue, 31 Jan 2023 00:55:49 GMT  
		Size: 2.3 KB (2308 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:708fefcedd4ee6c106da247a68c5790f5ab00225d1cdfff8465575265c3a54e6`  
		Last Modified: Tue, 31 Jan 2023 00:55:49 GMT  
		Size: 6.0 KB (6008 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:81e3bf8e20bc921031e7549a41dec1b2d7795cc6da40a0e7096bf654b25c5c3e`  
		Last Modified: Tue, 31 Jan 2023 00:55:49 GMT  
		Size: 2.5 KB (2507 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `xwiki:15.0.0-postgres-tomcat`

```console
$ docker pull xwiki@sha256:f6739c1133cbbece87973ddea5fbc57222abb9d7d3f8064eee9d2c2c0d46ecfa
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `xwiki:15.0.0-postgres-tomcat` - linux; amd64

```console
$ docker pull xwiki@sha256:72928baeace929e42f17f01362700392a90c6750b2ec1f84f24bbba1c4ff0236
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **590.0 MB (589959353 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b71f03d7d3a1760e73e6f4370f49317d16a7e0cb22532f49c11c0ee73b2c6262`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["xwiki"]`

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
# Wed, 02 Nov 2022 18:44:10 GMT
RUN apt-get update     && DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends tzdata curl wget ca-certificates fontconfig locales     && echo "en_US.UTF-8 UTF-8" >> /etc/locale.gen     && locale-gen en_US.UTF-8     && rm -rf /var/lib/apt/lists/*
# Fri, 04 Nov 2022 23:21:41 GMT
ENV JAVA_VERSION=jdk-11.0.17+8
# Fri, 04 Nov 2022 23:22:31 GMT
RUN set -eux;     ARCH="$(dpkg --print-architecture)";     case "${ARCH}" in        aarch64|arm64)          ESUM='bd6efe3290c8b5a42f695a55a26f3e3c9c284288574879d4b7089f31f5114177';          BINARY_URL='https://github.com/adoptium/temurin11-binaries/releases/download/jdk-11.0.17%2B8/OpenJDK11U-jre_aarch64_linux_hotspot_11.0.17_8.tar.gz';          ;;        armhf|arm)          ESUM='8cf113d3d7fa808895c8d2e41bb890af21c47e38c2460e0588147a4bb8fc658d';          BINARY_URL='https://github.com/adoptium/temurin11-binaries/releases/download/jdk-11.0.17%2B8/OpenJDK11U-jre_arm_linux_hotspot_11.0.17_8.tar.gz';          ;;        ppc64el|powerpc:common64)          ESUM='0ca3d806131ab5834c501f9c625bb0248cd528af361c704503348e9c9605bedf';          BINARY_URL='https://github.com/adoptium/temurin11-binaries/releases/download/jdk-11.0.17%2B8/OpenJDK11U-jre_ppc64le_linux_hotspot_11.0.17_8.tar.gz';          ;;        s390x|s390:64-bit)          ESUM='dd3b159a374086e65cb07c4ccb226c90f9c02ef929cba6f0b642171d7ed97fa4';          BINARY_URL='https://github.com/adoptium/temurin11-binaries/releases/download/jdk-11.0.17%2B8/OpenJDK11U-jre_s390x_linux_hotspot_11.0.17_8.tar.gz';          ;;        amd64|i386:x86-64)          ESUM='752616097e09d7f60a3ad8bd312f90eaf50ac72577e55df229fe6e8091148f79';          BINARY_URL='https://github.com/adoptium/temurin11-binaries/releases/download/jdk-11.0.17%2B8/OpenJDK11U-jre_x64_linux_hotspot_11.0.17_8.tar.gz';          ;;        *)          echo "Unsupported arch: ${ARCH}";          exit 1;          ;;     esac; 	  wget -O /tmp/openjdk.tar.gz ${BINARY_URL}; 	  echo "${ESUM} */tmp/openjdk.tar.gz" | sha256sum -c -; 	  mkdir -p "$JAVA_HOME"; 	  tar --extract 	      --file /tmp/openjdk.tar.gz 	      --directory "$JAVA_HOME" 	      --strip-components 1 	      --no-same-owner 	  ;     rm /tmp/openjdk.tar.gz;     find "$JAVA_HOME/lib" -name '*.so' -exec dirname '{}' ';' | sort -u > /etc/ld.so.conf.d/docker-openjdk.conf;     ldconfig;     java -Xshare:dump;
# Fri, 04 Nov 2022 23:22:32 GMT
RUN echo Verifying install ...     && fileEncoding="$(echo 'System.out.println(System.getProperty("file.encoding"))' | jshell -s -)"; [ "$fileEncoding" = 'UTF-8' ]; rm -rf ~/.java     && echo java --version && java --version     && echo Complete.
# Sat, 05 Nov 2022 01:35:16 GMT
ENV CATALINA_HOME=/usr/local/tomcat
# Sat, 05 Nov 2022 01:35:16 GMT
ENV PATH=/usr/local/tomcat/bin:/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Sat, 05 Nov 2022 01:35:17 GMT
RUN mkdir -p "$CATALINA_HOME"
# Sat, 05 Nov 2022 01:35:17 GMT
WORKDIR /usr/local/tomcat
# Sat, 05 Nov 2022 01:35:17 GMT
ENV TOMCAT_NATIVE_LIBDIR=/usr/local/tomcat/native-jni-lib
# Sat, 05 Nov 2022 01:35:17 GMT
ENV LD_LIBRARY_PATH=/usr/local/tomcat/native-jni-lib
# Sat, 05 Nov 2022 01:39:54 GMT
ENV GPG_KEYS=48F8E69F6390C9F25CFEDCD268248959359E722B A9C5DF4D22E99998D9875A5110C01C5A2F6059E7 DCFD35E0BF8CA7344752DE8B6FB21E8933C60243
# Sat, 05 Nov 2022 01:39:54 GMT
ENV TOMCAT_MAJOR=9
# Tue, 15 Nov 2022 03:06:43 GMT
ENV TOMCAT_VERSION=9.0.69
# Tue, 15 Nov 2022 03:06:43 GMT
ENV TOMCAT_SHA512=8c883c54ce9ce43eba37756a6404cdf3477879883a3e6d146dc8a7aa5e0425f487466afe6b6da4a895927cb7cb59177b9379cec18000f2de12785be57408c779
# Tue, 15 Nov 2022 03:06:44 GMT
COPY dir:b1a33aa3993dbbfbebb33bd9aa546b60c2f2191abf1227f453d4e830f6deb35f in /usr/local/tomcat 
# Tue, 15 Nov 2022 03:06:48 GMT
RUN set -eux; 	apt-get update; 	xargs -rt apt-get install -y --no-install-recommends < "$TOMCAT_NATIVE_LIBDIR/.dependencies.txt"; 	rm -rf /var/lib/apt/lists/*
# Tue, 15 Nov 2022 03:06:49 GMT
RUN set -eux; 	nativeLines="$(catalina.sh configtest 2>&1)"; 	nativeLines="$(echo "$nativeLines" | grep 'Apache Tomcat Native')"; 	nativeLines="$(echo "$nativeLines" | sort -u)"; 	if ! echo "$nativeLines" | grep -E 'INFO: Loaded( APR based)? Apache Tomcat Native library' >&2; then 		echo >&2 "$nativeLines"; 		exit 1; 	fi
# Tue, 15 Nov 2022 03:06:49 GMT
EXPOSE 8080
# Tue, 15 Nov 2022 03:06:49 GMT
CMD ["catalina.sh" "run"]
# Wed, 11 Jan 2023 02:47:03 GMT
LABEL org.opencontainers.image.authors=XWiki Development Team <committers@xwiki.org>
# Wed, 11 Jan 2023 02:47:03 GMT
LABEL org.opencontainers.image.url=https://hub.docker.com/_/xwiki
# Wed, 11 Jan 2023 02:47:03 GMT
LABEL org.opencontainers.image.documentation=https://hub.docker.com/_/xwiki
# Wed, 11 Jan 2023 02:47:03 GMT
LABEL org.opencontainers.image.source=https://github.com/xwiki/xwiki-docker.git
# Wed, 11 Jan 2023 02:47:04 GMT
LABEL org.opencontainers.image.vendor=xwiki.org
# Wed, 11 Jan 2023 02:47:04 GMT
LABEL org.opencontainers.image.licenses=LGPL-2.1
# Wed, 11 Jan 2023 02:50:25 GMT
RUN apt-get update &&   apt-get --no-install-recommends -y install     curl     libreoffice     unzip     procps     libpostgresql-jdbc-java &&   rm -rf /var/lib/apt/lists/*
# Tue, 31 Jan 2023 00:21:26 GMT
ENV XWIKI_VERSION=15.0
# Tue, 31 Jan 2023 00:21:27 GMT
ENV XWIKI_URL_PREFIX=https://maven.xwiki.org/releases/org/xwiki/platform/xwiki-platform-distribution-war/15.0
# Tue, 31 Jan 2023 00:21:27 GMT
ENV XWIKI_DOWNLOAD_SHA256=79ba0f479bbc49521c113821adc9d91141075a9470d7f9bbb6994ca59c30d121
# Tue, 31 Jan 2023 00:22:39 GMT
RUN rm -rf /usr/local/tomcat/webapps/* &&   mkdir -p /usr/local/tomcat/temp &&   mkdir -p /usr/local/xwiki/data &&   curl -fSL "${XWIKI_URL_PREFIX}/xwiki-platform-distribution-war-${XWIKI_VERSION}.war" -o xwiki.war &&   echo "$XWIKI_DOWNLOAD_SHA256 xwiki.war" | sha256sum -c - &&   unzip -d /usr/local/tomcat/webapps/ROOT xwiki.war &&   rm -f xwiki.war
# Tue, 31 Jan 2023 00:22:40 GMT
RUN cp /usr/share/java/postgresql-jdbc4.jar /usr/local/tomcat/webapps/ROOT/WEB-INF/lib/
# Tue, 31 Jan 2023 00:22:41 GMT
COPY file:0a1be11e2eb610a1dbcd415404e3a592641110b93090030cb831e3a19a163017 in /usr/local/tomcat/bin/ 
# Tue, 31 Jan 2023 00:22:41 GMT
COPY file:4a923f484bb29a26630c19e1d617d3bf6aa6ae7c6c4a5561e97b037bcde0847c in /usr/local/tomcat/webapps/ROOT/WEB-INF/hibernate.cfg.xml 
# Tue, 31 Jan 2023 00:22:41 GMT
RUN sed -i 's/<id>org.xwiki.platform:xwiki-platform-distribution-war/<id>org.xwiki.platform:xwiki-platform-distribution-docker/'   /usr/local/tomcat/webapps/ROOT/META-INF/extension.xed
# Tue, 31 Jan 2023 00:22:41 GMT
COPY file:a47c4dcd87c9dad97aff38c49188357e6193bcad50757e516cfb08a60d4de611 in /usr/local/bin/docker-entrypoint.sh 
# Tue, 31 Jan 2023 00:22:41 GMT
VOLUME [/usr/local/xwiki]
# Tue, 31 Jan 2023 00:22:42 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 31 Jan 2023 00:22:42 GMT
CMD ["xwiki"]
```

-	Layers:
	-	`sha256:e96e057aae67380a4ddb16c337c5c3669d97fdff69ec537f02aa2cc30d814281`  
		Last Modified: Wed, 02 Nov 2022 03:03:36 GMT  
		Size: 30.4 MB (30425607 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4ced2591451da3a02e2b6bb44752b9e3f00d77789921be4df5082fb9f9880ad0`  
		Last Modified: Wed, 02 Nov 2022 18:48:43 GMT  
		Size: 12.4 MB (12439006 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:df8f874ae8c08a9e69e5fbe6c5a64200a45386132a3203d1a9a7f1146d94cfbc`  
		Last Modified: Fri, 04 Nov 2022 23:29:33 GMT  
		Size: 46.6 MB (46629936 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:111b6c7486426c4b6989102c2ee5be856e8a58e20ab0a350b24a905d536e8e7f`  
		Last Modified: Fri, 04 Nov 2022 23:29:26 GMT  
		Size: 161.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e6f84dce457c6d4f7b7291fce05f8e77998a3a7722a54125a1f1d52ca83043b4`  
		Last Modified: Sat, 05 Nov 2022 01:50:51 GMT  
		Size: 173.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a6c26749ee782392e38845ee2ba79b0da586ef6a45d8e7f29c7af14612278547`  
		Last Modified: Tue, 15 Nov 2022 03:19:57 GMT  
		Size: 12.2 MB (12200249 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4dddc6d9fa6024025b3fcfe729cab2dc544fb25476eca6e80b1af8e8d93bb0ee`  
		Last Modified: Tue, 15 Nov 2022 03:19:56 GMT  
		Size: 452.7 KB (452680 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:06637eebe5e72c8ad9019ad4eb4cdde1f11f7d4c24c7ed7374cf8966343aa2fb`  
		Last Modified: Tue, 15 Nov 2022 03:19:56 GMT  
		Size: 131.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b57f6f8bcfb0d93b8e21d3068d1f65d3f08dba05c5fab7d4c36e2359317b18c7`  
		Last Modified: Wed, 11 Jan 2023 02:53:53 GMT  
		Size: 179.7 MB (179745182 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:71a0aee972ff5a36a4c5d67f5bf6416b1b78d06c906ce727c5e8e11098d0dfd1`  
		Last Modified: Tue, 31 Jan 2023 00:25:01 GMT  
		Size: 307.1 MB (307117070 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ccc745f1273896cef68a5af6cd5713c4a2d8704628920a53e318a008f8096426`  
		Last Modified: Tue, 31 Jan 2023 00:24:44 GMT  
		Size: 936.8 KB (936848 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1593979548bc568ed36dc9f5adb8f00d8b7d3eb1fa850fc06426c2c9345b8472`  
		Last Modified: Tue, 31 Jan 2023 00:24:43 GMT  
		Size: 1.3 KB (1345 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e1e58b32c2c2a52907f7e4ad05462d3b2afd11404a9678bc656fb96029b12d8d`  
		Last Modified: Tue, 31 Jan 2023 00:24:43 GMT  
		Size: 2.5 KB (2454 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c43ce01c7b867ce6cda62f86175ba6a53f44000797d61fe604aded86980c4d41`  
		Last Modified: Tue, 31 Jan 2023 00:24:43 GMT  
		Size: 6.0 KB (6006 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6fe6f306aa61d9839a01e62f4c308a9a7d3bd4cd5ce9a58407b6585f6950f054`  
		Last Modified: Tue, 31 Jan 2023 00:24:43 GMT  
		Size: 2.5 KB (2505 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `xwiki:15.0.0-postgres-tomcat` - linux; arm64 variant v8

```console
$ docker pull xwiki@sha256:ae51c629c7a76aa7c15ebb33fcfdae3e529ef6456ada6d0dbcf9ed8fc5ecf00d
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **581.2 MB (581212250 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:70277ae3ffdca68401bb57e24e6302cc64a403bf36869f0959e54d03216b0005`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["xwiki"]`

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
# Wed, 02 Nov 2022 19:44:32 GMT
RUN apt-get update     && DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends tzdata curl wget ca-certificates fontconfig locales     && echo "en_US.UTF-8 UTF-8" >> /etc/locale.gen     && locale-gen en_US.UTF-8     && rm -rf /var/lib/apt/lists/*
# Fri, 04 Nov 2022 22:40:54 GMT
ENV JAVA_VERSION=jdk-11.0.17+8
# Fri, 04 Nov 2022 22:41:33 GMT
RUN set -eux;     ARCH="$(dpkg --print-architecture)";     case "${ARCH}" in        aarch64|arm64)          ESUM='bd6efe3290c8b5a42f695a55a26f3e3c9c284288574879d4b7089f31f5114177';          BINARY_URL='https://github.com/adoptium/temurin11-binaries/releases/download/jdk-11.0.17%2B8/OpenJDK11U-jre_aarch64_linux_hotspot_11.0.17_8.tar.gz';          ;;        armhf|arm)          ESUM='8cf113d3d7fa808895c8d2e41bb890af21c47e38c2460e0588147a4bb8fc658d';          BINARY_URL='https://github.com/adoptium/temurin11-binaries/releases/download/jdk-11.0.17%2B8/OpenJDK11U-jre_arm_linux_hotspot_11.0.17_8.tar.gz';          ;;        ppc64el|powerpc:common64)          ESUM='0ca3d806131ab5834c501f9c625bb0248cd528af361c704503348e9c9605bedf';          BINARY_URL='https://github.com/adoptium/temurin11-binaries/releases/download/jdk-11.0.17%2B8/OpenJDK11U-jre_ppc64le_linux_hotspot_11.0.17_8.tar.gz';          ;;        s390x|s390:64-bit)          ESUM='dd3b159a374086e65cb07c4ccb226c90f9c02ef929cba6f0b642171d7ed97fa4';          BINARY_URL='https://github.com/adoptium/temurin11-binaries/releases/download/jdk-11.0.17%2B8/OpenJDK11U-jre_s390x_linux_hotspot_11.0.17_8.tar.gz';          ;;        amd64|i386:x86-64)          ESUM='752616097e09d7f60a3ad8bd312f90eaf50ac72577e55df229fe6e8091148f79';          BINARY_URL='https://github.com/adoptium/temurin11-binaries/releases/download/jdk-11.0.17%2B8/OpenJDK11U-jre_x64_linux_hotspot_11.0.17_8.tar.gz';          ;;        *)          echo "Unsupported arch: ${ARCH}";          exit 1;          ;;     esac; 	  wget -O /tmp/openjdk.tar.gz ${BINARY_URL}; 	  echo "${ESUM} */tmp/openjdk.tar.gz" | sha256sum -c -; 	  mkdir -p "$JAVA_HOME"; 	  tar --extract 	      --file /tmp/openjdk.tar.gz 	      --directory "$JAVA_HOME" 	      --strip-components 1 	      --no-same-owner 	  ;     rm /tmp/openjdk.tar.gz;     find "$JAVA_HOME/lib" -name '*.so' -exec dirname '{}' ';' | sort -u > /etc/ld.so.conf.d/docker-openjdk.conf;     ldconfig;     java -Xshare:dump;
# Fri, 04 Nov 2022 22:41:34 GMT
RUN echo Verifying install ...     && fileEncoding="$(echo 'System.out.println(System.getProperty("file.encoding"))' | jshell -s -)"; [ "$fileEncoding" = 'UTF-8' ]; rm -rf ~/.java     && echo java --version && java --version     && echo Complete.
# Fri, 04 Nov 2022 23:48:38 GMT
ENV CATALINA_HOME=/usr/local/tomcat
# Fri, 04 Nov 2022 23:48:38 GMT
ENV PATH=/usr/local/tomcat/bin:/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Fri, 04 Nov 2022 23:48:38 GMT
RUN mkdir -p "$CATALINA_HOME"
# Fri, 04 Nov 2022 23:48:39 GMT
WORKDIR /usr/local/tomcat
# Fri, 04 Nov 2022 23:48:39 GMT
ENV TOMCAT_NATIVE_LIBDIR=/usr/local/tomcat/native-jni-lib
# Fri, 04 Nov 2022 23:48:39 GMT
ENV LD_LIBRARY_PATH=/usr/local/tomcat/native-jni-lib
# Fri, 04 Nov 2022 23:53:12 GMT
ENV GPG_KEYS=48F8E69F6390C9F25CFEDCD268248959359E722B A9C5DF4D22E99998D9875A5110C01C5A2F6059E7 DCFD35E0BF8CA7344752DE8B6FB21E8933C60243
# Fri, 04 Nov 2022 23:53:12 GMT
ENV TOMCAT_MAJOR=9
# Tue, 15 Nov 2022 04:57:22 GMT
ENV TOMCAT_VERSION=9.0.69
# Tue, 15 Nov 2022 04:57:22 GMT
ENV TOMCAT_SHA512=8c883c54ce9ce43eba37756a6404cdf3477879883a3e6d146dc8a7aa5e0425f487466afe6b6da4a895927cb7cb59177b9379cec18000f2de12785be57408c779
# Tue, 15 Nov 2022 04:57:22 GMT
COPY dir:096b403a5f78b17e6b4bff63128a9c93941b97f22470991610dd641633d977f1 in /usr/local/tomcat 
# Tue, 15 Nov 2022 04:57:25 GMT
RUN set -eux; 	apt-get update; 	xargs -rt apt-get install -y --no-install-recommends < "$TOMCAT_NATIVE_LIBDIR/.dependencies.txt"; 	rm -rf /var/lib/apt/lists/*
# Tue, 15 Nov 2022 04:57:26 GMT
RUN set -eux; 	nativeLines="$(catalina.sh configtest 2>&1)"; 	nativeLines="$(echo "$nativeLines" | grep 'Apache Tomcat Native')"; 	nativeLines="$(echo "$nativeLines" | sort -u)"; 	if ! echo "$nativeLines" | grep -E 'INFO: Loaded( APR based)? Apache Tomcat Native library' >&2; then 		echo >&2 "$nativeLines"; 		exit 1; 	fi
# Tue, 15 Nov 2022 04:57:26 GMT
EXPOSE 8080
# Tue, 15 Nov 2022 04:57:27 GMT
CMD ["catalina.sh" "run"]
# Wed, 11 Jan 2023 03:05:10 GMT
LABEL org.opencontainers.image.authors=XWiki Development Team <committers@xwiki.org>
# Wed, 11 Jan 2023 03:05:10 GMT
LABEL org.opencontainers.image.url=https://hub.docker.com/_/xwiki
# Wed, 11 Jan 2023 03:05:10 GMT
LABEL org.opencontainers.image.documentation=https://hub.docker.com/_/xwiki
# Wed, 11 Jan 2023 03:05:10 GMT
LABEL org.opencontainers.image.source=https://github.com/xwiki/xwiki-docker.git
# Wed, 11 Jan 2023 03:05:11 GMT
LABEL org.opencontainers.image.vendor=xwiki.org
# Wed, 11 Jan 2023 03:05:11 GMT
LABEL org.opencontainers.image.licenses=LGPL-2.1
# Wed, 11 Jan 2023 03:08:55 GMT
RUN apt-get update &&   apt-get --no-install-recommends -y install     curl     libreoffice     unzip     procps     libpostgresql-jdbc-java &&   rm -rf /var/lib/apt/lists/*
# Tue, 31 Jan 2023 00:48:10 GMT
ENV XWIKI_VERSION=15.0
# Tue, 31 Jan 2023 00:48:10 GMT
ENV XWIKI_URL_PREFIX=https://maven.xwiki.org/releases/org/xwiki/platform/xwiki-platform-distribution-war/15.0
# Tue, 31 Jan 2023 00:48:10 GMT
ENV XWIKI_DOWNLOAD_SHA256=79ba0f479bbc49521c113821adc9d91141075a9470d7f9bbb6994ca59c30d121
# Tue, 31 Jan 2023 00:54:38 GMT
RUN rm -rf /usr/local/tomcat/webapps/* &&   mkdir -p /usr/local/tomcat/temp &&   mkdir -p /usr/local/xwiki/data &&   curl -fSL "${XWIKI_URL_PREFIX}/xwiki-platform-distribution-war-${XWIKI_VERSION}.war" -o xwiki.war &&   echo "$XWIKI_DOWNLOAD_SHA256 xwiki.war" | sha256sum -c - &&   unzip -d /usr/local/tomcat/webapps/ROOT xwiki.war &&   rm -f xwiki.war
# Tue, 31 Jan 2023 00:54:41 GMT
RUN cp /usr/share/java/postgresql-jdbc4.jar /usr/local/tomcat/webapps/ROOT/WEB-INF/lib/
# Tue, 31 Jan 2023 00:54:41 GMT
COPY file:0a1be11e2eb610a1dbcd415404e3a592641110b93090030cb831e3a19a163017 in /usr/local/tomcat/bin/ 
# Tue, 31 Jan 2023 00:54:41 GMT
COPY file:4a923f484bb29a26630c19e1d617d3bf6aa6ae7c6c4a5561e97b037bcde0847c in /usr/local/tomcat/webapps/ROOT/WEB-INF/hibernate.cfg.xml 
# Tue, 31 Jan 2023 00:54:42 GMT
RUN sed -i 's/<id>org.xwiki.platform:xwiki-platform-distribution-war/<id>org.xwiki.platform:xwiki-platform-distribution-docker/'   /usr/local/tomcat/webapps/ROOT/META-INF/extension.xed
# Tue, 31 Jan 2023 00:54:42 GMT
COPY file:a47c4dcd87c9dad97aff38c49188357e6193bcad50757e516cfb08a60d4de611 in /usr/local/bin/docker-entrypoint.sh 
# Tue, 31 Jan 2023 00:54:42 GMT
VOLUME [/usr/local/xwiki]
# Tue, 31 Jan 2023 00:54:42 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 31 Jan 2023 00:54:42 GMT
CMD ["xwiki"]
```

-	Layers:
	-	`sha256:0509fae36eb0656f8bdb23f8ae64100d893bcea2563e97468d337e04d2d0410b`  
		Last Modified: Wed, 02 Nov 2022 18:50:21 GMT  
		Size: 28.4 MB (28382154 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e502a1af2bcd98f5f0d2f5e4da1a0e7bbe07a2c548e2662f7d37dce5ae1df46c`  
		Last Modified: Wed, 02 Nov 2022 19:48:28 GMT  
		Size: 12.4 MB (12396330 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bc4598c07dd818f03a0378b0341a4a8e80f0152fbb3e7d5246ca4f466f42e611`  
		Last Modified: Fri, 04 Nov 2022 22:46:46 GMT  
		Size: 45.0 MB (44958470 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:715a937a1066f998b331fcd62256ad01a5571bdf46804e97825afc64f9ebb427`  
		Last Modified: Fri, 04 Nov 2022 22:46:41 GMT  
		Size: 160.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5fb623f082f74b2fa9fc2c4e3f3a4802875cb9753cfa26ed940201ce72bb56cb`  
		Last Modified: Sat, 05 Nov 2022 00:03:40 GMT  
		Size: 172.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:33260b83200262bbd546be371ad3c1f50f5ae7228afb87982d6fa9d6b11bf26f`  
		Last Modified: Tue, 15 Nov 2022 05:10:19 GMT  
		Size: 12.2 MB (12207235 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0955fb697ea9b30a1b4f95385464f646aa1525cb6efba648e22df84ebef6b2ee`  
		Last Modified: Tue, 15 Nov 2022 05:10:18 GMT  
		Size: 452.0 KB (452021 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6eddcf66f2083b1487296a0308e0b058917c97f614f12428d82d89662038dc2e`  
		Last Modified: Tue, 15 Nov 2022 05:10:18 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1ae6a8fce0f2cd131007393c1a4eba9ce9d0501da8406af5c5ce9deb5dc187b8`  
		Last Modified: Wed, 11 Jan 2023 03:12:13 GMT  
		Size: 174.7 MB (174749274 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5351c17af011e98fdd3db4781945e719f390748d66dc50d28bef46bb2d6b6418`  
		Last Modified: Tue, 31 Jan 2023 00:56:53 GMT  
		Size: 307.1 MB (307117134 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6b632a2f6afda42ce5dc291920d8f03e04b69034e314687eb551be8eafedd92d`  
		Last Modified: Tue, 31 Jan 2023 00:56:38 GMT  
		Size: 936.9 KB (936854 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cbd6cbb6ae05692db55d5e4f46142d2e20e051631dc2fc44e5b20d3316143305`  
		Last Modified: Tue, 31 Jan 2023 00:56:38 GMT  
		Size: 1.3 KB (1348 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ceb1d88f8fd44412961c0db372cd86a999c6b2619ce80a916a4fe8ca0e63acc9`  
		Last Modified: Tue, 31 Jan 2023 00:56:38 GMT  
		Size: 2.5 KB (2458 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8d0ee5cad12d41a6d530031aabd4a92619995eb0ee20dcd24d2bb9aec6a694db`  
		Last Modified: Tue, 31 Jan 2023 00:56:38 GMT  
		Size: 6.0 KB (6006 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3c980b95519f007aea60be042d36cd33de21e6265aed0e443c5ecf9bb1f40980`  
		Last Modified: Tue, 31 Jan 2023 00:56:38 GMT  
		Size: 2.5 KB (2505 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `xwiki:latest`

```console
$ docker pull xwiki@sha256:33e789838f82ce73efec6664859feb1ced7a5b7605fbfaddb81916716bce524f
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `xwiki:latest` - linux; amd64

```console
$ docker pull xwiki@sha256:481fdb46e8c043a6709d11310e2083ce71d6ba63ee6517f84da3ba06f320598e
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **590.5 MB (590459982 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:bd630aa0aa5c679e23ea7d52cbbdd6b817eab27a820c25d3c50b54eca83b9744`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["xwiki"]`

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
# Wed, 02 Nov 2022 18:44:10 GMT
RUN apt-get update     && DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends tzdata curl wget ca-certificates fontconfig locales     && echo "en_US.UTF-8 UTF-8" >> /etc/locale.gen     && locale-gen en_US.UTF-8     && rm -rf /var/lib/apt/lists/*
# Fri, 04 Nov 2022 23:21:41 GMT
ENV JAVA_VERSION=jdk-11.0.17+8
# Fri, 04 Nov 2022 23:22:31 GMT
RUN set -eux;     ARCH="$(dpkg --print-architecture)";     case "${ARCH}" in        aarch64|arm64)          ESUM='bd6efe3290c8b5a42f695a55a26f3e3c9c284288574879d4b7089f31f5114177';          BINARY_URL='https://github.com/adoptium/temurin11-binaries/releases/download/jdk-11.0.17%2B8/OpenJDK11U-jre_aarch64_linux_hotspot_11.0.17_8.tar.gz';          ;;        armhf|arm)          ESUM='8cf113d3d7fa808895c8d2e41bb890af21c47e38c2460e0588147a4bb8fc658d';          BINARY_URL='https://github.com/adoptium/temurin11-binaries/releases/download/jdk-11.0.17%2B8/OpenJDK11U-jre_arm_linux_hotspot_11.0.17_8.tar.gz';          ;;        ppc64el|powerpc:common64)          ESUM='0ca3d806131ab5834c501f9c625bb0248cd528af361c704503348e9c9605bedf';          BINARY_URL='https://github.com/adoptium/temurin11-binaries/releases/download/jdk-11.0.17%2B8/OpenJDK11U-jre_ppc64le_linux_hotspot_11.0.17_8.tar.gz';          ;;        s390x|s390:64-bit)          ESUM='dd3b159a374086e65cb07c4ccb226c90f9c02ef929cba6f0b642171d7ed97fa4';          BINARY_URL='https://github.com/adoptium/temurin11-binaries/releases/download/jdk-11.0.17%2B8/OpenJDK11U-jre_s390x_linux_hotspot_11.0.17_8.tar.gz';          ;;        amd64|i386:x86-64)          ESUM='752616097e09d7f60a3ad8bd312f90eaf50ac72577e55df229fe6e8091148f79';          BINARY_URL='https://github.com/adoptium/temurin11-binaries/releases/download/jdk-11.0.17%2B8/OpenJDK11U-jre_x64_linux_hotspot_11.0.17_8.tar.gz';          ;;        *)          echo "Unsupported arch: ${ARCH}";          exit 1;          ;;     esac; 	  wget -O /tmp/openjdk.tar.gz ${BINARY_URL}; 	  echo "${ESUM} */tmp/openjdk.tar.gz" | sha256sum -c -; 	  mkdir -p "$JAVA_HOME"; 	  tar --extract 	      --file /tmp/openjdk.tar.gz 	      --directory "$JAVA_HOME" 	      --strip-components 1 	      --no-same-owner 	  ;     rm /tmp/openjdk.tar.gz;     find "$JAVA_HOME/lib" -name '*.so' -exec dirname '{}' ';' | sort -u > /etc/ld.so.conf.d/docker-openjdk.conf;     ldconfig;     java -Xshare:dump;
# Fri, 04 Nov 2022 23:22:32 GMT
RUN echo Verifying install ...     && fileEncoding="$(echo 'System.out.println(System.getProperty("file.encoding"))' | jshell -s -)"; [ "$fileEncoding" = 'UTF-8' ]; rm -rf ~/.java     && echo java --version && java --version     && echo Complete.
# Sat, 05 Nov 2022 01:35:16 GMT
ENV CATALINA_HOME=/usr/local/tomcat
# Sat, 05 Nov 2022 01:35:16 GMT
ENV PATH=/usr/local/tomcat/bin:/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Sat, 05 Nov 2022 01:35:17 GMT
RUN mkdir -p "$CATALINA_HOME"
# Sat, 05 Nov 2022 01:35:17 GMT
WORKDIR /usr/local/tomcat
# Sat, 05 Nov 2022 01:35:17 GMT
ENV TOMCAT_NATIVE_LIBDIR=/usr/local/tomcat/native-jni-lib
# Sat, 05 Nov 2022 01:35:17 GMT
ENV LD_LIBRARY_PATH=/usr/local/tomcat/native-jni-lib
# Sat, 05 Nov 2022 01:39:54 GMT
ENV GPG_KEYS=48F8E69F6390C9F25CFEDCD268248959359E722B A9C5DF4D22E99998D9875A5110C01C5A2F6059E7 DCFD35E0BF8CA7344752DE8B6FB21E8933C60243
# Sat, 05 Nov 2022 01:39:54 GMT
ENV TOMCAT_MAJOR=9
# Tue, 15 Nov 2022 03:06:43 GMT
ENV TOMCAT_VERSION=9.0.69
# Tue, 15 Nov 2022 03:06:43 GMT
ENV TOMCAT_SHA512=8c883c54ce9ce43eba37756a6404cdf3477879883a3e6d146dc8a7aa5e0425f487466afe6b6da4a895927cb7cb59177b9379cec18000f2de12785be57408c779
# Tue, 15 Nov 2022 03:06:44 GMT
COPY dir:b1a33aa3993dbbfbebb33bd9aa546b60c2f2191abf1227f453d4e830f6deb35f in /usr/local/tomcat 
# Tue, 15 Nov 2022 03:06:48 GMT
RUN set -eux; 	apt-get update; 	xargs -rt apt-get install -y --no-install-recommends < "$TOMCAT_NATIVE_LIBDIR/.dependencies.txt"; 	rm -rf /var/lib/apt/lists/*
# Tue, 15 Nov 2022 03:06:49 GMT
RUN set -eux; 	nativeLines="$(catalina.sh configtest 2>&1)"; 	nativeLines="$(echo "$nativeLines" | grep 'Apache Tomcat Native')"; 	nativeLines="$(echo "$nativeLines" | sort -u)"; 	if ! echo "$nativeLines" | grep -E 'INFO: Loaded( APR based)? Apache Tomcat Native library' >&2; then 		echo >&2 "$nativeLines"; 		exit 1; 	fi
# Tue, 15 Nov 2022 03:06:49 GMT
EXPOSE 8080
# Tue, 15 Nov 2022 03:06:49 GMT
CMD ["catalina.sh" "run"]
# Wed, 11 Jan 2023 02:47:03 GMT
LABEL org.opencontainers.image.authors=XWiki Development Team <committers@xwiki.org>
# Wed, 11 Jan 2023 02:47:03 GMT
LABEL org.opencontainers.image.url=https://hub.docker.com/_/xwiki
# Wed, 11 Jan 2023 02:47:03 GMT
LABEL org.opencontainers.image.documentation=https://hub.docker.com/_/xwiki
# Wed, 11 Jan 2023 02:47:03 GMT
LABEL org.opencontainers.image.source=https://github.com/xwiki/xwiki-docker.git
# Wed, 11 Jan 2023 02:47:04 GMT
LABEL org.opencontainers.image.vendor=xwiki.org
# Wed, 11 Jan 2023 02:47:04 GMT
LABEL org.opencontainers.image.licenses=LGPL-2.1
# Wed, 11 Jan 2023 02:49:03 GMT
RUN apt-get update &&   apt-get --no-install-recommends -y install     curl     libreoffice     unzip     procps &&   rm -rf /var/lib/apt/lists/*
# Tue, 31 Jan 2023 00:20:17 GMT
ENV XWIKI_VERSION=15.0
# Tue, 31 Jan 2023 00:20:17 GMT
ENV XWIKI_URL_PREFIX=https://maven.xwiki.org/releases/org/xwiki/platform/xwiki-platform-distribution-war/15.0
# Tue, 31 Jan 2023 00:20:17 GMT
ENV XWIKI_DOWNLOAD_SHA256=79ba0f479bbc49521c113821adc9d91141075a9470d7f9bbb6994ca59c30d121
# Tue, 31 Jan 2023 00:21:18 GMT
RUN rm -rf /usr/local/tomcat/webapps/* &&   mkdir -p /usr/local/tomcat/temp &&   mkdir -p /usr/local/xwiki/data &&   curl -fSL "${XWIKI_URL_PREFIX}/xwiki-platform-distribution-war-${XWIKI_VERSION}.war" -o xwiki.war &&   echo "$XWIKI_DOWNLOAD_SHA256 xwiki.war" | sha256sum -c - &&   unzip -d /usr/local/tomcat/webapps/ROOT xwiki.war &&   rm -f xwiki.war
# Tue, 31 Jan 2023 00:21:19 GMT
ENV MYSQL_JDBC_VERSION=8.0.31
# Tue, 31 Jan 2023 00:21:19 GMT
ENV MYSQL_JDBC_SHA256=5249e3dc6d6531b37790e3f61845b96db5e41e891d3d8edb0e2e3a1b53ca2f4f
# Tue, 31 Jan 2023 00:21:19 GMT
ENV MYSQL_JDBC_PREFIX=https://repo1.maven.org/maven2/com/mysql/mysql-connector-j/8.0.31
# Tue, 31 Jan 2023 00:21:19 GMT
ENV MYSQL_JDBC_ARTIFACT=mysql-connector-j-8.0.31.jar
# Tue, 31 Jan 2023 00:21:19 GMT
ENV MYSQL_JDBC_TARGET=/usr/local/tomcat/webapps/ROOT/WEB-INF/lib/mysql-connector-j-8.0.31.jar
# Tue, 31 Jan 2023 00:21:20 GMT
RUN curl -fSL "${MYSQL_JDBC_PREFIX}/${MYSQL_JDBC_ARTIFACT}" -o $MYSQL_JDBC_TARGET &&   echo "$MYSQL_JDBC_SHA256 $MYSQL_JDBC_TARGET" | sha256sum -c -
# Tue, 31 Jan 2023 00:21:21 GMT
COPY file:0a1be11e2eb610a1dbcd415404e3a592641110b93090030cb831e3a19a163017 in /usr/local/tomcat/bin/ 
# Tue, 31 Jan 2023 00:21:21 GMT
COPY file:1b8409986f3e4eb79a7a0b18472cb2692a61d504fb5ef34292bc997b79fd760d in /usr/local/tomcat/webapps/ROOT/WEB-INF/hibernate.cfg.xml 
# Tue, 31 Jan 2023 00:21:21 GMT
RUN sed -i 's/<id>org.xwiki.platform:xwiki-platform-distribution-war/<id>org.xwiki.platform:xwiki-platform-distribution-docker/'   /usr/local/tomcat/webapps/ROOT/META-INF/extension.xed
# Tue, 31 Jan 2023 00:21:21 GMT
COPY file:a47c4dcd87c9dad97aff38c49188357e6193bcad50757e516cfb08a60d4de611 in /usr/local/bin/docker-entrypoint.sh 
# Tue, 31 Jan 2023 00:21:22 GMT
VOLUME [/usr/local/xwiki]
# Tue, 31 Jan 2023 00:21:22 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 31 Jan 2023 00:21:22 GMT
CMD ["xwiki"]
```

-	Layers:
	-	`sha256:e96e057aae67380a4ddb16c337c5c3669d97fdff69ec537f02aa2cc30d814281`  
		Last Modified: Wed, 02 Nov 2022 03:03:36 GMT  
		Size: 30.4 MB (30425607 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4ced2591451da3a02e2b6bb44752b9e3f00d77789921be4df5082fb9f9880ad0`  
		Last Modified: Wed, 02 Nov 2022 18:48:43 GMT  
		Size: 12.4 MB (12439006 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:df8f874ae8c08a9e69e5fbe6c5a64200a45386132a3203d1a9a7f1146d94cfbc`  
		Last Modified: Fri, 04 Nov 2022 23:29:33 GMT  
		Size: 46.6 MB (46629936 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:111b6c7486426c4b6989102c2ee5be856e8a58e20ab0a350b24a905d536e8e7f`  
		Last Modified: Fri, 04 Nov 2022 23:29:26 GMT  
		Size: 161.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e6f84dce457c6d4f7b7291fce05f8e77998a3a7722a54125a1f1d52ca83043b4`  
		Last Modified: Sat, 05 Nov 2022 01:50:51 GMT  
		Size: 173.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a6c26749ee782392e38845ee2ba79b0da586ef6a45d8e7f29c7af14612278547`  
		Last Modified: Tue, 15 Nov 2022 03:19:57 GMT  
		Size: 12.2 MB (12200249 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4dddc6d9fa6024025b3fcfe729cab2dc544fb25476eca6e80b1af8e8d93bb0ee`  
		Last Modified: Tue, 15 Nov 2022 03:19:56 GMT  
		Size: 452.7 KB (452680 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:06637eebe5e72c8ad9019ad4eb4cdde1f11f7d4c24c7ed7374cf8966343aa2fb`  
		Last Modified: Tue, 15 Nov 2022 03:19:56 GMT  
		Size: 131.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b276fb8390410a8208724033e325715ea26000d5a1a762d4c3699b927884fbfe`  
		Last Modified: Wed, 11 Jan 2023 02:52:45 GMT  
		Size: 178.8 MB (178805608 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:156ca91198173149698aa0396648a9608b6ab1f2bc2666800843ce33c9f85b6e`  
		Last Modified: Tue, 31 Jan 2023 00:24:09 GMT  
		Size: 307.1 MB (307117069 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4c8b70d250c6d507901857473b0dcb67132d7b2a30ce9a69b07b1036853df738`  
		Last Modified: Tue, 31 Jan 2023 00:23:52 GMT  
		Size: 2.4 MB (2377191 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a9681fd36be674d25231c69d6a39f9e8fa65034eeaef5d1bd885fdbeac7f0f6b`  
		Last Modified: Tue, 31 Jan 2023 00:23:51 GMT  
		Size: 1.3 KB (1346 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a9d0d5da840f4d7da9943942b38cd092fae11f41dc6c19afd58d655cd6192d66`  
		Last Modified: Tue, 31 Jan 2023 00:23:51 GMT  
		Size: 2.3 KB (2312 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d65610da4f1da86fea8fbec0189b066afd4b86e4e8f7d049e3c4bc6ade9ba90a`  
		Last Modified: Tue, 31 Jan 2023 00:23:51 GMT  
		Size: 6.0 KB (6009 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3d41686284d7675eaa0f92c9cc27ebe73b4c30768c8eef9f23ee3b1ad06da00a`  
		Last Modified: Tue, 31 Jan 2023 00:23:51 GMT  
		Size: 2.5 KB (2504 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `xwiki:latest` - linux; arm64 variant v8

```console
$ docker pull xwiki@sha256:6bf63d9025b07b69d744200c05efd4ffb8a52f3c38380f5d59a0b48514203cd2
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **581.7 MB (581709921 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:6600f2bb05836c703d53944bbcb5399d509a9813a27a35e99ff717becc308330`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["xwiki"]`

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
# Wed, 02 Nov 2022 19:44:32 GMT
RUN apt-get update     && DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends tzdata curl wget ca-certificates fontconfig locales     && echo "en_US.UTF-8 UTF-8" >> /etc/locale.gen     && locale-gen en_US.UTF-8     && rm -rf /var/lib/apt/lists/*
# Fri, 04 Nov 2022 22:40:54 GMT
ENV JAVA_VERSION=jdk-11.0.17+8
# Fri, 04 Nov 2022 22:41:33 GMT
RUN set -eux;     ARCH="$(dpkg --print-architecture)";     case "${ARCH}" in        aarch64|arm64)          ESUM='bd6efe3290c8b5a42f695a55a26f3e3c9c284288574879d4b7089f31f5114177';          BINARY_URL='https://github.com/adoptium/temurin11-binaries/releases/download/jdk-11.0.17%2B8/OpenJDK11U-jre_aarch64_linux_hotspot_11.0.17_8.tar.gz';          ;;        armhf|arm)          ESUM='8cf113d3d7fa808895c8d2e41bb890af21c47e38c2460e0588147a4bb8fc658d';          BINARY_URL='https://github.com/adoptium/temurin11-binaries/releases/download/jdk-11.0.17%2B8/OpenJDK11U-jre_arm_linux_hotspot_11.0.17_8.tar.gz';          ;;        ppc64el|powerpc:common64)          ESUM='0ca3d806131ab5834c501f9c625bb0248cd528af361c704503348e9c9605bedf';          BINARY_URL='https://github.com/adoptium/temurin11-binaries/releases/download/jdk-11.0.17%2B8/OpenJDK11U-jre_ppc64le_linux_hotspot_11.0.17_8.tar.gz';          ;;        s390x|s390:64-bit)          ESUM='dd3b159a374086e65cb07c4ccb226c90f9c02ef929cba6f0b642171d7ed97fa4';          BINARY_URL='https://github.com/adoptium/temurin11-binaries/releases/download/jdk-11.0.17%2B8/OpenJDK11U-jre_s390x_linux_hotspot_11.0.17_8.tar.gz';          ;;        amd64|i386:x86-64)          ESUM='752616097e09d7f60a3ad8bd312f90eaf50ac72577e55df229fe6e8091148f79';          BINARY_URL='https://github.com/adoptium/temurin11-binaries/releases/download/jdk-11.0.17%2B8/OpenJDK11U-jre_x64_linux_hotspot_11.0.17_8.tar.gz';          ;;        *)          echo "Unsupported arch: ${ARCH}";          exit 1;          ;;     esac; 	  wget -O /tmp/openjdk.tar.gz ${BINARY_URL}; 	  echo "${ESUM} */tmp/openjdk.tar.gz" | sha256sum -c -; 	  mkdir -p "$JAVA_HOME"; 	  tar --extract 	      --file /tmp/openjdk.tar.gz 	      --directory "$JAVA_HOME" 	      --strip-components 1 	      --no-same-owner 	  ;     rm /tmp/openjdk.tar.gz;     find "$JAVA_HOME/lib" -name '*.so' -exec dirname '{}' ';' | sort -u > /etc/ld.so.conf.d/docker-openjdk.conf;     ldconfig;     java -Xshare:dump;
# Fri, 04 Nov 2022 22:41:34 GMT
RUN echo Verifying install ...     && fileEncoding="$(echo 'System.out.println(System.getProperty("file.encoding"))' | jshell -s -)"; [ "$fileEncoding" = 'UTF-8' ]; rm -rf ~/.java     && echo java --version && java --version     && echo Complete.
# Fri, 04 Nov 2022 23:48:38 GMT
ENV CATALINA_HOME=/usr/local/tomcat
# Fri, 04 Nov 2022 23:48:38 GMT
ENV PATH=/usr/local/tomcat/bin:/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Fri, 04 Nov 2022 23:48:38 GMT
RUN mkdir -p "$CATALINA_HOME"
# Fri, 04 Nov 2022 23:48:39 GMT
WORKDIR /usr/local/tomcat
# Fri, 04 Nov 2022 23:48:39 GMT
ENV TOMCAT_NATIVE_LIBDIR=/usr/local/tomcat/native-jni-lib
# Fri, 04 Nov 2022 23:48:39 GMT
ENV LD_LIBRARY_PATH=/usr/local/tomcat/native-jni-lib
# Fri, 04 Nov 2022 23:53:12 GMT
ENV GPG_KEYS=48F8E69F6390C9F25CFEDCD268248959359E722B A9C5DF4D22E99998D9875A5110C01C5A2F6059E7 DCFD35E0BF8CA7344752DE8B6FB21E8933C60243
# Fri, 04 Nov 2022 23:53:12 GMT
ENV TOMCAT_MAJOR=9
# Tue, 15 Nov 2022 04:57:22 GMT
ENV TOMCAT_VERSION=9.0.69
# Tue, 15 Nov 2022 04:57:22 GMT
ENV TOMCAT_SHA512=8c883c54ce9ce43eba37756a6404cdf3477879883a3e6d146dc8a7aa5e0425f487466afe6b6da4a895927cb7cb59177b9379cec18000f2de12785be57408c779
# Tue, 15 Nov 2022 04:57:22 GMT
COPY dir:096b403a5f78b17e6b4bff63128a9c93941b97f22470991610dd641633d977f1 in /usr/local/tomcat 
# Tue, 15 Nov 2022 04:57:25 GMT
RUN set -eux; 	apt-get update; 	xargs -rt apt-get install -y --no-install-recommends < "$TOMCAT_NATIVE_LIBDIR/.dependencies.txt"; 	rm -rf /var/lib/apt/lists/*
# Tue, 15 Nov 2022 04:57:26 GMT
RUN set -eux; 	nativeLines="$(catalina.sh configtest 2>&1)"; 	nativeLines="$(echo "$nativeLines" | grep 'Apache Tomcat Native')"; 	nativeLines="$(echo "$nativeLines" | sort -u)"; 	if ! echo "$nativeLines" | grep -E 'INFO: Loaded( APR based)? Apache Tomcat Native library' >&2; then 		echo >&2 "$nativeLines"; 		exit 1; 	fi
# Tue, 15 Nov 2022 04:57:26 GMT
EXPOSE 8080
# Tue, 15 Nov 2022 04:57:27 GMT
CMD ["catalina.sh" "run"]
# Wed, 11 Jan 2023 03:05:10 GMT
LABEL org.opencontainers.image.authors=XWiki Development Team <committers@xwiki.org>
# Wed, 11 Jan 2023 03:05:10 GMT
LABEL org.opencontainers.image.url=https://hub.docker.com/_/xwiki
# Wed, 11 Jan 2023 03:05:10 GMT
LABEL org.opencontainers.image.documentation=https://hub.docker.com/_/xwiki
# Wed, 11 Jan 2023 03:05:10 GMT
LABEL org.opencontainers.image.source=https://github.com/xwiki/xwiki-docker.git
# Wed, 11 Jan 2023 03:05:11 GMT
LABEL org.opencontainers.image.vendor=xwiki.org
# Wed, 11 Jan 2023 03:05:11 GMT
LABEL org.opencontainers.image.licenses=LGPL-2.1
# Wed, 11 Jan 2023 03:07:37 GMT
RUN apt-get update &&   apt-get --no-install-recommends -y install     curl     libreoffice     unzip     procps &&   rm -rf /var/lib/apt/lists/*
# Tue, 31 Jan 2023 00:47:12 GMT
ENV XWIKI_VERSION=15.0
# Tue, 31 Jan 2023 00:47:12 GMT
ENV XWIKI_URL_PREFIX=https://maven.xwiki.org/releases/org/xwiki/platform/xwiki-platform-distribution-war/15.0
# Tue, 31 Jan 2023 00:47:12 GMT
ENV XWIKI_DOWNLOAD_SHA256=79ba0f479bbc49521c113821adc9d91141075a9470d7f9bbb6994ca59c30d121
# Tue, 31 Jan 2023 00:47:58 GMT
RUN rm -rf /usr/local/tomcat/webapps/* &&   mkdir -p /usr/local/tomcat/temp &&   mkdir -p /usr/local/xwiki/data &&   curl -fSL "${XWIKI_URL_PREFIX}/xwiki-platform-distribution-war-${XWIKI_VERSION}.war" -o xwiki.war &&   echo "$XWIKI_DOWNLOAD_SHA256 xwiki.war" | sha256sum -c - &&   unzip -d /usr/local/tomcat/webapps/ROOT xwiki.war &&   rm -f xwiki.war
# Tue, 31 Jan 2023 00:48:01 GMT
ENV MYSQL_JDBC_VERSION=8.0.31
# Tue, 31 Jan 2023 00:48:01 GMT
ENV MYSQL_JDBC_SHA256=5249e3dc6d6531b37790e3f61845b96db5e41e891d3d8edb0e2e3a1b53ca2f4f
# Tue, 31 Jan 2023 00:48:01 GMT
ENV MYSQL_JDBC_PREFIX=https://repo1.maven.org/maven2/com/mysql/mysql-connector-j/8.0.31
# Tue, 31 Jan 2023 00:48:01 GMT
ENV MYSQL_JDBC_ARTIFACT=mysql-connector-j-8.0.31.jar
# Tue, 31 Jan 2023 00:48:01 GMT
ENV MYSQL_JDBC_TARGET=/usr/local/tomcat/webapps/ROOT/WEB-INF/lib/mysql-connector-j-8.0.31.jar
# Tue, 31 Jan 2023 00:48:02 GMT
RUN curl -fSL "${MYSQL_JDBC_PREFIX}/${MYSQL_JDBC_ARTIFACT}" -o $MYSQL_JDBC_TARGET &&   echo "$MYSQL_JDBC_SHA256 $MYSQL_JDBC_TARGET" | sha256sum -c -
# Tue, 31 Jan 2023 00:48:02 GMT
COPY file:0a1be11e2eb610a1dbcd415404e3a592641110b93090030cb831e3a19a163017 in /usr/local/tomcat/bin/ 
# Tue, 31 Jan 2023 00:48:02 GMT
COPY file:1b8409986f3e4eb79a7a0b18472cb2692a61d504fb5ef34292bc997b79fd760d in /usr/local/tomcat/webapps/ROOT/WEB-INF/hibernate.cfg.xml 
# Tue, 31 Jan 2023 00:48:03 GMT
RUN sed -i 's/<id>org.xwiki.platform:xwiki-platform-distribution-war/<id>org.xwiki.platform:xwiki-platform-distribution-docker/'   /usr/local/tomcat/webapps/ROOT/META-INF/extension.xed
# Tue, 31 Jan 2023 00:48:03 GMT
COPY file:a47c4dcd87c9dad97aff38c49188357e6193bcad50757e516cfb08a60d4de611 in /usr/local/bin/docker-entrypoint.sh 
# Tue, 31 Jan 2023 00:48:03 GMT
VOLUME [/usr/local/xwiki]
# Tue, 31 Jan 2023 00:48:03 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 31 Jan 2023 00:48:03 GMT
CMD ["xwiki"]
```

-	Layers:
	-	`sha256:0509fae36eb0656f8bdb23f8ae64100d893bcea2563e97468d337e04d2d0410b`  
		Last Modified: Wed, 02 Nov 2022 18:50:21 GMT  
		Size: 28.4 MB (28382154 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e502a1af2bcd98f5f0d2f5e4da1a0e7bbe07a2c548e2662f7d37dce5ae1df46c`  
		Last Modified: Wed, 02 Nov 2022 19:48:28 GMT  
		Size: 12.4 MB (12396330 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bc4598c07dd818f03a0378b0341a4a8e80f0152fbb3e7d5246ca4f466f42e611`  
		Last Modified: Fri, 04 Nov 2022 22:46:46 GMT  
		Size: 45.0 MB (44958470 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:715a937a1066f998b331fcd62256ad01a5571bdf46804e97825afc64f9ebb427`  
		Last Modified: Fri, 04 Nov 2022 22:46:41 GMT  
		Size: 160.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5fb623f082f74b2fa9fc2c4e3f3a4802875cb9753cfa26ed940201ce72bb56cb`  
		Last Modified: Sat, 05 Nov 2022 00:03:40 GMT  
		Size: 172.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:33260b83200262bbd546be371ad3c1f50f5ae7228afb87982d6fa9d6b11bf26f`  
		Last Modified: Tue, 15 Nov 2022 05:10:19 GMT  
		Size: 12.2 MB (12207235 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0955fb697ea9b30a1b4f95385464f646aa1525cb6efba648e22df84ebef6b2ee`  
		Last Modified: Tue, 15 Nov 2022 05:10:18 GMT  
		Size: 452.0 KB (452021 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6eddcf66f2083b1487296a0308e0b058917c97f614f12428d82d89662038dc2e`  
		Last Modified: Tue, 15 Nov 2022 05:10:18 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ae5f60bb64f3fa11da3d15a9639f886186b4c2c021455c3f9db22e0cfe1b1311`  
		Last Modified: Wed, 11 Jan 2023 03:11:14 GMT  
		Size: 173.8 MB (173806827 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1814d85fce571b42f2cfa7c8a904e1a184ee6f49642242a44bbe0037088994a0`  
		Last Modified: Tue, 31 Jan 2023 00:56:04 GMT  
		Size: 307.1 MB (307117070 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8aec0e24b4fa870989f014944c3c7d535355a2371fc8c948b2b11f9b377efe6e`  
		Last Modified: Tue, 31 Jan 2023 00:55:50 GMT  
		Size: 2.4 MB (2377182 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0b65081619aa0114a7f367836ef421eb8d951e559e0f089c7728af7813b1ea62`  
		Last Modified: Tue, 31 Jan 2023 00:55:49 GMT  
		Size: 1.3 KB (1348 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:46ebad072e608146426d8dc30828937049eea36c2e636d7790b4960d6d586977`  
		Last Modified: Tue, 31 Jan 2023 00:55:49 GMT  
		Size: 2.3 KB (2308 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:708fefcedd4ee6c106da247a68c5790f5ab00225d1cdfff8465575265c3a54e6`  
		Last Modified: Tue, 31 Jan 2023 00:55:49 GMT  
		Size: 6.0 KB (6008 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:81e3bf8e20bc921031e7549a41dec1b2d7795cc6da40a0e7096bf654b25c5c3e`  
		Last Modified: Tue, 31 Jan 2023 00:55:49 GMT  
		Size: 2.5 KB (2507 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `xwiki:lts`

```console
$ docker pull xwiki@sha256:32e51c9775fda50082b0f02856f2af444a67284446679c9a3a13a78c02ec0c4b
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `xwiki:lts` - linux; amd64

```console
$ docker pull xwiki@sha256:a2e996a399fc68cbccfe11eaeb0115a15314bd69f06c483fef3cba244fa07cbf
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **590.4 MB (590449604 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:6b73fd725d5c1dd8044289fdb0e76f973e7e1d4a64e1efc44428235a718b550a`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["xwiki"]`

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
# Wed, 02 Nov 2022 18:44:10 GMT
RUN apt-get update     && DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends tzdata curl wget ca-certificates fontconfig locales     && echo "en_US.UTF-8 UTF-8" >> /etc/locale.gen     && locale-gen en_US.UTF-8     && rm -rf /var/lib/apt/lists/*
# Fri, 04 Nov 2022 23:21:41 GMT
ENV JAVA_VERSION=jdk-11.0.17+8
# Fri, 04 Nov 2022 23:22:31 GMT
RUN set -eux;     ARCH="$(dpkg --print-architecture)";     case "${ARCH}" in        aarch64|arm64)          ESUM='bd6efe3290c8b5a42f695a55a26f3e3c9c284288574879d4b7089f31f5114177';          BINARY_URL='https://github.com/adoptium/temurin11-binaries/releases/download/jdk-11.0.17%2B8/OpenJDK11U-jre_aarch64_linux_hotspot_11.0.17_8.tar.gz';          ;;        armhf|arm)          ESUM='8cf113d3d7fa808895c8d2e41bb890af21c47e38c2460e0588147a4bb8fc658d';          BINARY_URL='https://github.com/adoptium/temurin11-binaries/releases/download/jdk-11.0.17%2B8/OpenJDK11U-jre_arm_linux_hotspot_11.0.17_8.tar.gz';          ;;        ppc64el|powerpc:common64)          ESUM='0ca3d806131ab5834c501f9c625bb0248cd528af361c704503348e9c9605bedf';          BINARY_URL='https://github.com/adoptium/temurin11-binaries/releases/download/jdk-11.0.17%2B8/OpenJDK11U-jre_ppc64le_linux_hotspot_11.0.17_8.tar.gz';          ;;        s390x|s390:64-bit)          ESUM='dd3b159a374086e65cb07c4ccb226c90f9c02ef929cba6f0b642171d7ed97fa4';          BINARY_URL='https://github.com/adoptium/temurin11-binaries/releases/download/jdk-11.0.17%2B8/OpenJDK11U-jre_s390x_linux_hotspot_11.0.17_8.tar.gz';          ;;        amd64|i386:x86-64)          ESUM='752616097e09d7f60a3ad8bd312f90eaf50ac72577e55df229fe6e8091148f79';          BINARY_URL='https://github.com/adoptium/temurin11-binaries/releases/download/jdk-11.0.17%2B8/OpenJDK11U-jre_x64_linux_hotspot_11.0.17_8.tar.gz';          ;;        *)          echo "Unsupported arch: ${ARCH}";          exit 1;          ;;     esac; 	  wget -O /tmp/openjdk.tar.gz ${BINARY_URL}; 	  echo "${ESUM} */tmp/openjdk.tar.gz" | sha256sum -c -; 	  mkdir -p "$JAVA_HOME"; 	  tar --extract 	      --file /tmp/openjdk.tar.gz 	      --directory "$JAVA_HOME" 	      --strip-components 1 	      --no-same-owner 	  ;     rm /tmp/openjdk.tar.gz;     find "$JAVA_HOME/lib" -name '*.so' -exec dirname '{}' ';' | sort -u > /etc/ld.so.conf.d/docker-openjdk.conf;     ldconfig;     java -Xshare:dump;
# Fri, 04 Nov 2022 23:22:32 GMT
RUN echo Verifying install ...     && fileEncoding="$(echo 'System.out.println(System.getProperty("file.encoding"))' | jshell -s -)"; [ "$fileEncoding" = 'UTF-8' ]; rm -rf ~/.java     && echo java --version && java --version     && echo Complete.
# Sat, 05 Nov 2022 01:35:16 GMT
ENV CATALINA_HOME=/usr/local/tomcat
# Sat, 05 Nov 2022 01:35:16 GMT
ENV PATH=/usr/local/tomcat/bin:/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Sat, 05 Nov 2022 01:35:17 GMT
RUN mkdir -p "$CATALINA_HOME"
# Sat, 05 Nov 2022 01:35:17 GMT
WORKDIR /usr/local/tomcat
# Sat, 05 Nov 2022 01:35:17 GMT
ENV TOMCAT_NATIVE_LIBDIR=/usr/local/tomcat/native-jni-lib
# Sat, 05 Nov 2022 01:35:17 GMT
ENV LD_LIBRARY_PATH=/usr/local/tomcat/native-jni-lib
# Sat, 05 Nov 2022 01:39:54 GMT
ENV GPG_KEYS=48F8E69F6390C9F25CFEDCD268248959359E722B A9C5DF4D22E99998D9875A5110C01C5A2F6059E7 DCFD35E0BF8CA7344752DE8B6FB21E8933C60243
# Sat, 05 Nov 2022 01:39:54 GMT
ENV TOMCAT_MAJOR=9
# Tue, 15 Nov 2022 03:06:43 GMT
ENV TOMCAT_VERSION=9.0.69
# Tue, 15 Nov 2022 03:06:43 GMT
ENV TOMCAT_SHA512=8c883c54ce9ce43eba37756a6404cdf3477879883a3e6d146dc8a7aa5e0425f487466afe6b6da4a895927cb7cb59177b9379cec18000f2de12785be57408c779
# Tue, 15 Nov 2022 03:06:44 GMT
COPY dir:b1a33aa3993dbbfbebb33bd9aa546b60c2f2191abf1227f453d4e830f6deb35f in /usr/local/tomcat 
# Tue, 15 Nov 2022 03:06:48 GMT
RUN set -eux; 	apt-get update; 	xargs -rt apt-get install -y --no-install-recommends < "$TOMCAT_NATIVE_LIBDIR/.dependencies.txt"; 	rm -rf /var/lib/apt/lists/*
# Tue, 15 Nov 2022 03:06:49 GMT
RUN set -eux; 	nativeLines="$(catalina.sh configtest 2>&1)"; 	nativeLines="$(echo "$nativeLines" | grep 'Apache Tomcat Native')"; 	nativeLines="$(echo "$nativeLines" | sort -u)"; 	if ! echo "$nativeLines" | grep -E 'INFO: Loaded( APR based)? Apache Tomcat Native library' >&2; then 		echo >&2 "$nativeLines"; 		exit 1; 	fi
# Tue, 15 Nov 2022 03:06:49 GMT
EXPOSE 8080
# Tue, 15 Nov 2022 03:06:49 GMT
CMD ["catalina.sh" "run"]
# Wed, 11 Jan 2023 02:47:03 GMT
LABEL org.opencontainers.image.authors=XWiki Development Team <committers@xwiki.org>
# Wed, 11 Jan 2023 02:47:03 GMT
LABEL org.opencontainers.image.url=https://hub.docker.com/_/xwiki
# Wed, 11 Jan 2023 02:47:03 GMT
LABEL org.opencontainers.image.documentation=https://hub.docker.com/_/xwiki
# Wed, 11 Jan 2023 02:47:03 GMT
LABEL org.opencontainers.image.source=https://github.com/xwiki/xwiki-docker.git
# Wed, 11 Jan 2023 02:47:04 GMT
LABEL org.opencontainers.image.vendor=xwiki.org
# Wed, 11 Jan 2023 02:47:04 GMT
LABEL org.opencontainers.image.licenses=LGPL-2.1
# Wed, 11 Jan 2023 02:49:03 GMT
RUN apt-get update &&   apt-get --no-install-recommends -y install     curl     libreoffice     unzip     procps &&   rm -rf /var/lib/apt/lists/*
# Wed, 22 Feb 2023 18:39:36 GMT
ENV XWIKI_VERSION=14.10.5
# Wed, 22 Feb 2023 18:39:36 GMT
ENV XWIKI_URL_PREFIX=https://maven.xwiki.org/releases/org/xwiki/platform/xwiki-platform-distribution-war/14.10.5
# Wed, 22 Feb 2023 18:39:36 GMT
ENV XWIKI_DOWNLOAD_SHA256=f58465d0869e4c5605ae8375a09c79399d1149c7131fed3cf9959918267eb6a8
# Wed, 22 Feb 2023 18:40:15 GMT
RUN rm -rf /usr/local/tomcat/webapps/* &&   mkdir -p /usr/local/tomcat/temp &&   mkdir -p /usr/local/xwiki/data &&   curl -fSL "${XWIKI_URL_PREFIX}/xwiki-platform-distribution-war-${XWIKI_VERSION}.war" -o xwiki.war &&   echo "$XWIKI_DOWNLOAD_SHA256 xwiki.war" | sha256sum -c - &&   unzip -d /usr/local/tomcat/webapps/ROOT xwiki.war &&   rm -f xwiki.war
# Wed, 22 Feb 2023 18:40:17 GMT
ENV MYSQL_JDBC_VERSION=8.0.32
# Wed, 22 Feb 2023 18:40:17 GMT
ENV MYSQL_JDBC_SHA256=522329fe925980f02e5eb89b59d227245d345415ff0c08932a68c9765c13acc5
# Wed, 22 Feb 2023 18:40:17 GMT
ENV MYSQL_JDBC_PREFIX=https://repo1.maven.org/maven2/com/mysql/mysql-connector-j/8.0.32
# Wed, 22 Feb 2023 18:40:17 GMT
ENV MYSQL_JDBC_ARTIFACT=mysql-connector-j-8.0.32.jar
# Wed, 22 Feb 2023 18:40:17 GMT
ENV MYSQL_JDBC_TARGET=/usr/local/tomcat/webapps/ROOT/WEB-INF/lib/mysql-connector-j-8.0.32.jar
# Wed, 22 Feb 2023 18:40:18 GMT
RUN curl -fSL "${MYSQL_JDBC_PREFIX}/${MYSQL_JDBC_ARTIFACT}" -o $MYSQL_JDBC_TARGET &&   echo "$MYSQL_JDBC_SHA256 $MYSQL_JDBC_TARGET" | sha256sum -c -
# Wed, 22 Feb 2023 18:40:18 GMT
COPY file:0a1be11e2eb610a1dbcd415404e3a592641110b93090030cb831e3a19a163017 in /usr/local/tomcat/bin/ 
# Wed, 22 Feb 2023 18:40:18 GMT
COPY file:1b8409986f3e4eb79a7a0b18472cb2692a61d504fb5ef34292bc997b79fd760d in /usr/local/tomcat/webapps/ROOT/WEB-INF/hibernate.cfg.xml 
# Wed, 22 Feb 2023 18:40:19 GMT
RUN sed -i 's/<id>org.xwiki.platform:xwiki-platform-distribution-war/<id>org.xwiki.platform:xwiki-platform-distribution-docker/'   /usr/local/tomcat/webapps/ROOT/META-INF/extension.xed
# Wed, 22 Feb 2023 18:40:19 GMT
COPY file:a47c4dcd87c9dad97aff38c49188357e6193bcad50757e516cfb08a60d4de611 in /usr/local/bin/docker-entrypoint.sh 
# Wed, 22 Feb 2023 18:40:19 GMT
VOLUME [/usr/local/xwiki]
# Wed, 22 Feb 2023 18:40:19 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 22 Feb 2023 18:40:19 GMT
CMD ["xwiki"]
```

-	Layers:
	-	`sha256:e96e057aae67380a4ddb16c337c5c3669d97fdff69ec537f02aa2cc30d814281`  
		Last Modified: Wed, 02 Nov 2022 03:03:36 GMT  
		Size: 30.4 MB (30425607 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4ced2591451da3a02e2b6bb44752b9e3f00d77789921be4df5082fb9f9880ad0`  
		Last Modified: Wed, 02 Nov 2022 18:48:43 GMT  
		Size: 12.4 MB (12439006 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:df8f874ae8c08a9e69e5fbe6c5a64200a45386132a3203d1a9a7f1146d94cfbc`  
		Last Modified: Fri, 04 Nov 2022 23:29:33 GMT  
		Size: 46.6 MB (46629936 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:111b6c7486426c4b6989102c2ee5be856e8a58e20ab0a350b24a905d536e8e7f`  
		Last Modified: Fri, 04 Nov 2022 23:29:26 GMT  
		Size: 161.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e6f84dce457c6d4f7b7291fce05f8e77998a3a7722a54125a1f1d52ca83043b4`  
		Last Modified: Sat, 05 Nov 2022 01:50:51 GMT  
		Size: 173.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a6c26749ee782392e38845ee2ba79b0da586ef6a45d8e7f29c7af14612278547`  
		Last Modified: Tue, 15 Nov 2022 03:19:57 GMT  
		Size: 12.2 MB (12200249 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4dddc6d9fa6024025b3fcfe729cab2dc544fb25476eca6e80b1af8e8d93bb0ee`  
		Last Modified: Tue, 15 Nov 2022 03:19:56 GMT  
		Size: 452.7 KB (452680 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:06637eebe5e72c8ad9019ad4eb4cdde1f11f7d4c24c7ed7374cf8966343aa2fb`  
		Last Modified: Tue, 15 Nov 2022 03:19:56 GMT  
		Size: 131.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b276fb8390410a8208724033e325715ea26000d5a1a762d4c3699b927884fbfe`  
		Last Modified: Wed, 11 Jan 2023 02:52:45 GMT  
		Size: 178.8 MB (178805608 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:89de9d9e2c09cd5b84430562516cbcd5695a0a3b2347b451e157bde75c2b5619`  
		Last Modified: Wed, 22 Feb 2023 18:42:21 GMT  
		Size: 307.1 MB (307141303 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4a2089179b7c1db514d0502e476e09b8f9313d08d4c4e4f3981be456288fe507`  
		Last Modified: Wed, 22 Feb 2023 18:42:04 GMT  
		Size: 2.3 MB (2342572 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e7c4ef360ff3673244adb3dfc4769b5710fa68fcc1fbe1c08b2f5fa32dbd4976`  
		Last Modified: Wed, 22 Feb 2023 18:42:04 GMT  
		Size: 1.3 KB (1348 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:08441c368d4b01e361491d7fbf1ac579fcc303b8484123c309a8d5a3b6657c46`  
		Last Modified: Wed, 22 Feb 2023 18:42:04 GMT  
		Size: 2.3 KB (2311 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:542b4bb846d438395e458c08de292f72d14d289fae6ffe7eba6fec1cd8518475`  
		Last Modified: Wed, 22 Feb 2023 18:42:04 GMT  
		Size: 6.0 KB (6013 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:039c0305df9e64c69bb546e64f0658dba6e728eee13022cfd682aa1ee76b8b7f`  
		Last Modified: Wed, 22 Feb 2023 18:42:04 GMT  
		Size: 2.5 KB (2506 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `xwiki:lts` - linux; arm64 variant v8

```console
$ docker pull xwiki@sha256:33e36167828fe9bae944e7d4cbbe3b69dd2415595d40610ac2ebcd73f2c2fa7f
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **581.7 MB (581697690 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:44013daf43fd09deb7221eef006c4d30d484a03c433118e5b59da0a44b573f06`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["xwiki"]`

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
# Wed, 02 Nov 2022 19:44:32 GMT
RUN apt-get update     && DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends tzdata curl wget ca-certificates fontconfig locales     && echo "en_US.UTF-8 UTF-8" >> /etc/locale.gen     && locale-gen en_US.UTF-8     && rm -rf /var/lib/apt/lists/*
# Fri, 04 Nov 2022 22:40:54 GMT
ENV JAVA_VERSION=jdk-11.0.17+8
# Fri, 04 Nov 2022 22:41:33 GMT
RUN set -eux;     ARCH="$(dpkg --print-architecture)";     case "${ARCH}" in        aarch64|arm64)          ESUM='bd6efe3290c8b5a42f695a55a26f3e3c9c284288574879d4b7089f31f5114177';          BINARY_URL='https://github.com/adoptium/temurin11-binaries/releases/download/jdk-11.0.17%2B8/OpenJDK11U-jre_aarch64_linux_hotspot_11.0.17_8.tar.gz';          ;;        armhf|arm)          ESUM='8cf113d3d7fa808895c8d2e41bb890af21c47e38c2460e0588147a4bb8fc658d';          BINARY_URL='https://github.com/adoptium/temurin11-binaries/releases/download/jdk-11.0.17%2B8/OpenJDK11U-jre_arm_linux_hotspot_11.0.17_8.tar.gz';          ;;        ppc64el|powerpc:common64)          ESUM='0ca3d806131ab5834c501f9c625bb0248cd528af361c704503348e9c9605bedf';          BINARY_URL='https://github.com/adoptium/temurin11-binaries/releases/download/jdk-11.0.17%2B8/OpenJDK11U-jre_ppc64le_linux_hotspot_11.0.17_8.tar.gz';          ;;        s390x|s390:64-bit)          ESUM='dd3b159a374086e65cb07c4ccb226c90f9c02ef929cba6f0b642171d7ed97fa4';          BINARY_URL='https://github.com/adoptium/temurin11-binaries/releases/download/jdk-11.0.17%2B8/OpenJDK11U-jre_s390x_linux_hotspot_11.0.17_8.tar.gz';          ;;        amd64|i386:x86-64)          ESUM='752616097e09d7f60a3ad8bd312f90eaf50ac72577e55df229fe6e8091148f79';          BINARY_URL='https://github.com/adoptium/temurin11-binaries/releases/download/jdk-11.0.17%2B8/OpenJDK11U-jre_x64_linux_hotspot_11.0.17_8.tar.gz';          ;;        *)          echo "Unsupported arch: ${ARCH}";          exit 1;          ;;     esac; 	  wget -O /tmp/openjdk.tar.gz ${BINARY_URL}; 	  echo "${ESUM} */tmp/openjdk.tar.gz" | sha256sum -c -; 	  mkdir -p "$JAVA_HOME"; 	  tar --extract 	      --file /tmp/openjdk.tar.gz 	      --directory "$JAVA_HOME" 	      --strip-components 1 	      --no-same-owner 	  ;     rm /tmp/openjdk.tar.gz;     find "$JAVA_HOME/lib" -name '*.so' -exec dirname '{}' ';' | sort -u > /etc/ld.so.conf.d/docker-openjdk.conf;     ldconfig;     java -Xshare:dump;
# Fri, 04 Nov 2022 22:41:34 GMT
RUN echo Verifying install ...     && fileEncoding="$(echo 'System.out.println(System.getProperty("file.encoding"))' | jshell -s -)"; [ "$fileEncoding" = 'UTF-8' ]; rm -rf ~/.java     && echo java --version && java --version     && echo Complete.
# Fri, 04 Nov 2022 23:48:38 GMT
ENV CATALINA_HOME=/usr/local/tomcat
# Fri, 04 Nov 2022 23:48:38 GMT
ENV PATH=/usr/local/tomcat/bin:/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Fri, 04 Nov 2022 23:48:38 GMT
RUN mkdir -p "$CATALINA_HOME"
# Fri, 04 Nov 2022 23:48:39 GMT
WORKDIR /usr/local/tomcat
# Fri, 04 Nov 2022 23:48:39 GMT
ENV TOMCAT_NATIVE_LIBDIR=/usr/local/tomcat/native-jni-lib
# Fri, 04 Nov 2022 23:48:39 GMT
ENV LD_LIBRARY_PATH=/usr/local/tomcat/native-jni-lib
# Fri, 04 Nov 2022 23:53:12 GMT
ENV GPG_KEYS=48F8E69F6390C9F25CFEDCD268248959359E722B A9C5DF4D22E99998D9875A5110C01C5A2F6059E7 DCFD35E0BF8CA7344752DE8B6FB21E8933C60243
# Fri, 04 Nov 2022 23:53:12 GMT
ENV TOMCAT_MAJOR=9
# Tue, 15 Nov 2022 04:57:22 GMT
ENV TOMCAT_VERSION=9.0.69
# Tue, 15 Nov 2022 04:57:22 GMT
ENV TOMCAT_SHA512=8c883c54ce9ce43eba37756a6404cdf3477879883a3e6d146dc8a7aa5e0425f487466afe6b6da4a895927cb7cb59177b9379cec18000f2de12785be57408c779
# Tue, 15 Nov 2022 04:57:22 GMT
COPY dir:096b403a5f78b17e6b4bff63128a9c93941b97f22470991610dd641633d977f1 in /usr/local/tomcat 
# Tue, 15 Nov 2022 04:57:25 GMT
RUN set -eux; 	apt-get update; 	xargs -rt apt-get install -y --no-install-recommends < "$TOMCAT_NATIVE_LIBDIR/.dependencies.txt"; 	rm -rf /var/lib/apt/lists/*
# Tue, 15 Nov 2022 04:57:26 GMT
RUN set -eux; 	nativeLines="$(catalina.sh configtest 2>&1)"; 	nativeLines="$(echo "$nativeLines" | grep 'Apache Tomcat Native')"; 	nativeLines="$(echo "$nativeLines" | sort -u)"; 	if ! echo "$nativeLines" | grep -E 'INFO: Loaded( APR based)? Apache Tomcat Native library' >&2; then 		echo >&2 "$nativeLines"; 		exit 1; 	fi
# Tue, 15 Nov 2022 04:57:26 GMT
EXPOSE 8080
# Tue, 15 Nov 2022 04:57:27 GMT
CMD ["catalina.sh" "run"]
# Wed, 11 Jan 2023 03:05:10 GMT
LABEL org.opencontainers.image.authors=XWiki Development Team <committers@xwiki.org>
# Wed, 11 Jan 2023 03:05:10 GMT
LABEL org.opencontainers.image.url=https://hub.docker.com/_/xwiki
# Wed, 11 Jan 2023 03:05:10 GMT
LABEL org.opencontainers.image.documentation=https://hub.docker.com/_/xwiki
# Wed, 11 Jan 2023 03:05:10 GMT
LABEL org.opencontainers.image.source=https://github.com/xwiki/xwiki-docker.git
# Wed, 11 Jan 2023 03:05:11 GMT
LABEL org.opencontainers.image.vendor=xwiki.org
# Wed, 11 Jan 2023 03:05:11 GMT
LABEL org.opencontainers.image.licenses=LGPL-2.1
# Wed, 11 Jan 2023 03:07:37 GMT
RUN apt-get update &&   apt-get --no-install-recommends -y install     curl     libreoffice     unzip     procps &&   rm -rf /var/lib/apt/lists/*
# Wed, 01 Feb 2023 22:26:19 GMT
ENV XWIKI_VERSION=14.10.4
# Wed, 01 Feb 2023 22:26:19 GMT
ENV XWIKI_URL_PREFIX=https://maven.xwiki.org/releases/org/xwiki/platform/xwiki-platform-distribution-war/14.10.4
# Wed, 01 Feb 2023 22:26:19 GMT
ENV XWIKI_DOWNLOAD_SHA256=2fcfb622319172c2e424b9c11848ebfabe27cf8ef69cba39ceb5d124b7ebe713
# Wed, 01 Feb 2023 22:27:00 GMT
RUN rm -rf /usr/local/tomcat/webapps/* &&   mkdir -p /usr/local/tomcat/temp &&   mkdir -p /usr/local/xwiki/data &&   curl -fSL "${XWIKI_URL_PREFIX}/xwiki-platform-distribution-war-${XWIKI_VERSION}.war" -o xwiki.war &&   echo "$XWIKI_DOWNLOAD_SHA256 xwiki.war" | sha256sum -c - &&   unzip -d /usr/local/tomcat/webapps/ROOT xwiki.war &&   rm -f xwiki.war
# Wed, 01 Feb 2023 22:27:03 GMT
ENV MYSQL_JDBC_VERSION=8.0.31
# Wed, 01 Feb 2023 22:27:03 GMT
ENV MYSQL_JDBC_SHA256=5249e3dc6d6531b37790e3f61845b96db5e41e891d3d8edb0e2e3a1b53ca2f4f
# Wed, 01 Feb 2023 22:27:03 GMT
ENV MYSQL_JDBC_PREFIX=https://repo1.maven.org/maven2/com/mysql/mysql-connector-j/8.0.31
# Wed, 01 Feb 2023 22:27:03 GMT
ENV MYSQL_JDBC_ARTIFACT=mysql-connector-j-8.0.31.jar
# Wed, 01 Feb 2023 22:27:03 GMT
ENV MYSQL_JDBC_TARGET=/usr/local/tomcat/webapps/ROOT/WEB-INF/lib/mysql-connector-j-8.0.31.jar
# Wed, 01 Feb 2023 22:27:04 GMT
RUN curl -fSL "${MYSQL_JDBC_PREFIX}/${MYSQL_JDBC_ARTIFACT}" -o $MYSQL_JDBC_TARGET &&   echo "$MYSQL_JDBC_SHA256 $MYSQL_JDBC_TARGET" | sha256sum -c -
# Wed, 01 Feb 2023 22:27:04 GMT
COPY file:0a1be11e2eb610a1dbcd415404e3a592641110b93090030cb831e3a19a163017 in /usr/local/tomcat/bin/ 
# Wed, 01 Feb 2023 22:27:04 GMT
COPY file:1b8409986f3e4eb79a7a0b18472cb2692a61d504fb5ef34292bc997b79fd760d in /usr/local/tomcat/webapps/ROOT/WEB-INF/hibernate.cfg.xml 
# Wed, 01 Feb 2023 22:27:05 GMT
RUN sed -i 's/<id>org.xwiki.platform:xwiki-platform-distribution-war/<id>org.xwiki.platform:xwiki-platform-distribution-docker/'   /usr/local/tomcat/webapps/ROOT/META-INF/extension.xed
# Wed, 01 Feb 2023 22:27:05 GMT
COPY file:a47c4dcd87c9dad97aff38c49188357e6193bcad50757e516cfb08a60d4de611 in /usr/local/bin/docker-entrypoint.sh 
# Wed, 01 Feb 2023 22:27:05 GMT
VOLUME [/usr/local/xwiki]
# Wed, 01 Feb 2023 22:27:05 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 01 Feb 2023 22:27:05 GMT
CMD ["xwiki"]
```

-	Layers:
	-	`sha256:0509fae36eb0656f8bdb23f8ae64100d893bcea2563e97468d337e04d2d0410b`  
		Last Modified: Wed, 02 Nov 2022 18:50:21 GMT  
		Size: 28.4 MB (28382154 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e502a1af2bcd98f5f0d2f5e4da1a0e7bbe07a2c548e2662f7d37dce5ae1df46c`  
		Last Modified: Wed, 02 Nov 2022 19:48:28 GMT  
		Size: 12.4 MB (12396330 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bc4598c07dd818f03a0378b0341a4a8e80f0152fbb3e7d5246ca4f466f42e611`  
		Last Modified: Fri, 04 Nov 2022 22:46:46 GMT  
		Size: 45.0 MB (44958470 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:715a937a1066f998b331fcd62256ad01a5571bdf46804e97825afc64f9ebb427`  
		Last Modified: Fri, 04 Nov 2022 22:46:41 GMT  
		Size: 160.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5fb623f082f74b2fa9fc2c4e3f3a4802875cb9753cfa26ed940201ce72bb56cb`  
		Last Modified: Sat, 05 Nov 2022 00:03:40 GMT  
		Size: 172.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:33260b83200262bbd546be371ad3c1f50f5ae7228afb87982d6fa9d6b11bf26f`  
		Last Modified: Tue, 15 Nov 2022 05:10:19 GMT  
		Size: 12.2 MB (12207235 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0955fb697ea9b30a1b4f95385464f646aa1525cb6efba648e22df84ebef6b2ee`  
		Last Modified: Tue, 15 Nov 2022 05:10:18 GMT  
		Size: 452.0 KB (452021 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6eddcf66f2083b1487296a0308e0b058917c97f614f12428d82d89662038dc2e`  
		Last Modified: Tue, 15 Nov 2022 05:10:18 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ae5f60bb64f3fa11da3d15a9639f886186b4c2c021455c3f9db22e0cfe1b1311`  
		Last Modified: Wed, 11 Jan 2023 03:11:14 GMT  
		Size: 173.8 MB (173806827 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:13334e257ce7313ca9d6028534e3ec6c7858c374c4afedea7f96c51da716806e`  
		Last Modified: Wed, 01 Feb 2023 22:29:16 GMT  
		Size: 307.1 MB (307104849 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ccb59878c7670194b75b6af22dd3908f9ae1a12dc1074f0b5ed156a5e3afdf0a`  
		Last Modified: Wed, 01 Feb 2023 22:29:02 GMT  
		Size: 2.4 MB (2377177 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d3946fb25102529cda96bcad4925905c9b997e442b447675d89066505cbe1026`  
		Last Modified: Wed, 01 Feb 2023 22:29:02 GMT  
		Size: 1.3 KB (1344 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1ba832da71f2ed07bae5269bb37e7ea79724a069ad63032f2af14996893baa37`  
		Last Modified: Wed, 01 Feb 2023 22:29:02 GMT  
		Size: 2.3 KB (2307 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6616193191331001a42a5d452ea69a215bbc414eca5cb00914c359665be5817f`  
		Last Modified: Wed, 01 Feb 2023 22:29:02 GMT  
		Size: 6.0 KB (6009 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6de4b8ce214cd9b76eda5b4955e5abb249a0b0292e8a38d39683e3002d6534bf`  
		Last Modified: Wed, 01 Feb 2023 22:29:03 GMT  
		Size: 2.5 KB (2506 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `xwiki:lts-mariadb`

```console
$ docker pull xwiki@sha256:016ba45d303064d25d04a705c1a307612a6383139366413fb169f42acc0419ee
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `xwiki:lts-mariadb` - linux; amd64

```console
$ docker pull xwiki@sha256:4aec14b2a2ae95584b839238412bbe33a7314bf32edc3e05f34f532d07fdedce
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **588.7 MB (588696916 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f5fbe86c66c7ac80e07663234a80353ce71d1847f409e2e2a603e0eb2a3342bc`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["xwiki"]`

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
# Wed, 02 Nov 2022 18:44:10 GMT
RUN apt-get update     && DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends tzdata curl wget ca-certificates fontconfig locales     && echo "en_US.UTF-8 UTF-8" >> /etc/locale.gen     && locale-gen en_US.UTF-8     && rm -rf /var/lib/apt/lists/*
# Fri, 04 Nov 2022 23:21:41 GMT
ENV JAVA_VERSION=jdk-11.0.17+8
# Fri, 04 Nov 2022 23:22:31 GMT
RUN set -eux;     ARCH="$(dpkg --print-architecture)";     case "${ARCH}" in        aarch64|arm64)          ESUM='bd6efe3290c8b5a42f695a55a26f3e3c9c284288574879d4b7089f31f5114177';          BINARY_URL='https://github.com/adoptium/temurin11-binaries/releases/download/jdk-11.0.17%2B8/OpenJDK11U-jre_aarch64_linux_hotspot_11.0.17_8.tar.gz';          ;;        armhf|arm)          ESUM='8cf113d3d7fa808895c8d2e41bb890af21c47e38c2460e0588147a4bb8fc658d';          BINARY_URL='https://github.com/adoptium/temurin11-binaries/releases/download/jdk-11.0.17%2B8/OpenJDK11U-jre_arm_linux_hotspot_11.0.17_8.tar.gz';          ;;        ppc64el|powerpc:common64)          ESUM='0ca3d806131ab5834c501f9c625bb0248cd528af361c704503348e9c9605bedf';          BINARY_URL='https://github.com/adoptium/temurin11-binaries/releases/download/jdk-11.0.17%2B8/OpenJDK11U-jre_ppc64le_linux_hotspot_11.0.17_8.tar.gz';          ;;        s390x|s390:64-bit)          ESUM='dd3b159a374086e65cb07c4ccb226c90f9c02ef929cba6f0b642171d7ed97fa4';          BINARY_URL='https://github.com/adoptium/temurin11-binaries/releases/download/jdk-11.0.17%2B8/OpenJDK11U-jre_s390x_linux_hotspot_11.0.17_8.tar.gz';          ;;        amd64|i386:x86-64)          ESUM='752616097e09d7f60a3ad8bd312f90eaf50ac72577e55df229fe6e8091148f79';          BINARY_URL='https://github.com/adoptium/temurin11-binaries/releases/download/jdk-11.0.17%2B8/OpenJDK11U-jre_x64_linux_hotspot_11.0.17_8.tar.gz';          ;;        *)          echo "Unsupported arch: ${ARCH}";          exit 1;          ;;     esac; 	  wget -O /tmp/openjdk.tar.gz ${BINARY_URL}; 	  echo "${ESUM} */tmp/openjdk.tar.gz" | sha256sum -c -; 	  mkdir -p "$JAVA_HOME"; 	  tar --extract 	      --file /tmp/openjdk.tar.gz 	      --directory "$JAVA_HOME" 	      --strip-components 1 	      --no-same-owner 	  ;     rm /tmp/openjdk.tar.gz;     find "$JAVA_HOME/lib" -name '*.so' -exec dirname '{}' ';' | sort -u > /etc/ld.so.conf.d/docker-openjdk.conf;     ldconfig;     java -Xshare:dump;
# Fri, 04 Nov 2022 23:22:32 GMT
RUN echo Verifying install ...     && fileEncoding="$(echo 'System.out.println(System.getProperty("file.encoding"))' | jshell -s -)"; [ "$fileEncoding" = 'UTF-8' ]; rm -rf ~/.java     && echo java --version && java --version     && echo Complete.
# Sat, 05 Nov 2022 01:35:16 GMT
ENV CATALINA_HOME=/usr/local/tomcat
# Sat, 05 Nov 2022 01:35:16 GMT
ENV PATH=/usr/local/tomcat/bin:/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Sat, 05 Nov 2022 01:35:17 GMT
RUN mkdir -p "$CATALINA_HOME"
# Sat, 05 Nov 2022 01:35:17 GMT
WORKDIR /usr/local/tomcat
# Sat, 05 Nov 2022 01:35:17 GMT
ENV TOMCAT_NATIVE_LIBDIR=/usr/local/tomcat/native-jni-lib
# Sat, 05 Nov 2022 01:35:17 GMT
ENV LD_LIBRARY_PATH=/usr/local/tomcat/native-jni-lib
# Sat, 05 Nov 2022 01:39:54 GMT
ENV GPG_KEYS=48F8E69F6390C9F25CFEDCD268248959359E722B A9C5DF4D22E99998D9875A5110C01C5A2F6059E7 DCFD35E0BF8CA7344752DE8B6FB21E8933C60243
# Sat, 05 Nov 2022 01:39:54 GMT
ENV TOMCAT_MAJOR=9
# Tue, 15 Nov 2022 03:06:43 GMT
ENV TOMCAT_VERSION=9.0.69
# Tue, 15 Nov 2022 03:06:43 GMT
ENV TOMCAT_SHA512=8c883c54ce9ce43eba37756a6404cdf3477879883a3e6d146dc8a7aa5e0425f487466afe6b6da4a895927cb7cb59177b9379cec18000f2de12785be57408c779
# Tue, 15 Nov 2022 03:06:44 GMT
COPY dir:b1a33aa3993dbbfbebb33bd9aa546b60c2f2191abf1227f453d4e830f6deb35f in /usr/local/tomcat 
# Tue, 15 Nov 2022 03:06:48 GMT
RUN set -eux; 	apt-get update; 	xargs -rt apt-get install -y --no-install-recommends < "$TOMCAT_NATIVE_LIBDIR/.dependencies.txt"; 	rm -rf /var/lib/apt/lists/*
# Tue, 15 Nov 2022 03:06:49 GMT
RUN set -eux; 	nativeLines="$(catalina.sh configtest 2>&1)"; 	nativeLines="$(echo "$nativeLines" | grep 'Apache Tomcat Native')"; 	nativeLines="$(echo "$nativeLines" | sort -u)"; 	if ! echo "$nativeLines" | grep -E 'INFO: Loaded( APR based)? Apache Tomcat Native library' >&2; then 		echo >&2 "$nativeLines"; 		exit 1; 	fi
# Tue, 15 Nov 2022 03:06:49 GMT
EXPOSE 8080
# Tue, 15 Nov 2022 03:06:49 GMT
CMD ["catalina.sh" "run"]
# Wed, 11 Jan 2023 02:47:03 GMT
LABEL org.opencontainers.image.authors=XWiki Development Team <committers@xwiki.org>
# Wed, 11 Jan 2023 02:47:03 GMT
LABEL org.opencontainers.image.url=https://hub.docker.com/_/xwiki
# Wed, 11 Jan 2023 02:47:03 GMT
LABEL org.opencontainers.image.documentation=https://hub.docker.com/_/xwiki
# Wed, 11 Jan 2023 02:47:03 GMT
LABEL org.opencontainers.image.source=https://github.com/xwiki/xwiki-docker.git
# Wed, 11 Jan 2023 02:47:04 GMT
LABEL org.opencontainers.image.vendor=xwiki.org
# Wed, 11 Jan 2023 02:47:04 GMT
LABEL org.opencontainers.image.licenses=LGPL-2.1
# Wed, 11 Jan 2023 02:49:03 GMT
RUN apt-get update &&   apt-get --no-install-recommends -y install     curl     libreoffice     unzip     procps &&   rm -rf /var/lib/apt/lists/*
# Wed, 22 Feb 2023 18:39:36 GMT
ENV XWIKI_VERSION=14.10.5
# Wed, 22 Feb 2023 18:39:36 GMT
ENV XWIKI_URL_PREFIX=https://maven.xwiki.org/releases/org/xwiki/platform/xwiki-platform-distribution-war/14.10.5
# Wed, 22 Feb 2023 18:39:36 GMT
ENV XWIKI_DOWNLOAD_SHA256=f58465d0869e4c5605ae8375a09c79399d1149c7131fed3cf9959918267eb6a8
# Wed, 22 Feb 2023 18:40:15 GMT
RUN rm -rf /usr/local/tomcat/webapps/* &&   mkdir -p /usr/local/tomcat/temp &&   mkdir -p /usr/local/xwiki/data &&   curl -fSL "${XWIKI_URL_PREFIX}/xwiki-platform-distribution-war-${XWIKI_VERSION}.war" -o xwiki.war &&   echo "$XWIKI_DOWNLOAD_SHA256 xwiki.war" | sha256sum -c - &&   unzip -d /usr/local/tomcat/webapps/ROOT xwiki.war &&   rm -f xwiki.war
# Wed, 22 Feb 2023 18:41:14 GMT
ENV MARIADB_JDBC_VERSION=3.1.2
# Wed, 22 Feb 2023 18:41:14 GMT
ENV MARIADB_JDBC_SHA256=aaec1ad348d030a65b25c93c65cdaf472bf8b4b6b314b965e5ba13aec81bc622
# Wed, 22 Feb 2023 18:41:14 GMT
ENV MARIADB_JDBC_PREFIX=https://repo1.maven.org/maven2/org/mariadb/jdbc/mariadb-java-client/3.1.2
# Wed, 22 Feb 2023 18:41:14 GMT
ENV MARIADB_JDBC_ARTIFACT=mariadb-java-client-3.1.2.jar
# Wed, 22 Feb 2023 18:41:14 GMT
ENV MARIADB_JDBC_TARGET=/usr/local/tomcat/webapps/ROOT/WEB-INF/lib/mariadb-java-client-3.1.2.jar
# Wed, 22 Feb 2023 18:41:15 GMT
RUN curl -fSL "${MARIADB_JDBC_PREFIX}/${MARIADB_JDBC_ARTIFACT}" -o $MARIADB_JDBC_TARGET &&   echo "$MARIADB_JDBC_SHA256 $MARIADB_JDBC_TARGET" | sha256sum -c -
# Wed, 22 Feb 2023 18:41:15 GMT
COPY file:0a1be11e2eb610a1dbcd415404e3a592641110b93090030cb831e3a19a163017 in /usr/local/tomcat/bin/ 
# Wed, 22 Feb 2023 18:41:15 GMT
COPY file:0e237c3876eeb3b5f3473a064d3e507da2df6c228ca714687930b34e3b687601 in /usr/local/tomcat/webapps/ROOT/WEB-INF/hibernate.cfg.xml 
# Wed, 22 Feb 2023 18:41:15 GMT
RUN sed -i 's/<id>org.xwiki.platform:xwiki-platform-distribution-war/<id>org.xwiki.platform:xwiki-platform-distribution-docker/'   /usr/local/tomcat/webapps/ROOT/META-INF/extension.xed
# Wed, 22 Feb 2023 18:41:16 GMT
COPY file:a47c4dcd87c9dad97aff38c49188357e6193bcad50757e516cfb08a60d4de611 in /usr/local/bin/docker-entrypoint.sh 
# Wed, 22 Feb 2023 18:41:16 GMT
VOLUME [/usr/local/xwiki]
# Wed, 22 Feb 2023 18:41:16 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 22 Feb 2023 18:41:16 GMT
CMD ["xwiki"]
```

-	Layers:
	-	`sha256:e96e057aae67380a4ddb16c337c5c3669d97fdff69ec537f02aa2cc30d814281`  
		Last Modified: Wed, 02 Nov 2022 03:03:36 GMT  
		Size: 30.4 MB (30425607 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4ced2591451da3a02e2b6bb44752b9e3f00d77789921be4df5082fb9f9880ad0`  
		Last Modified: Wed, 02 Nov 2022 18:48:43 GMT  
		Size: 12.4 MB (12439006 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:df8f874ae8c08a9e69e5fbe6c5a64200a45386132a3203d1a9a7f1146d94cfbc`  
		Last Modified: Fri, 04 Nov 2022 23:29:33 GMT  
		Size: 46.6 MB (46629936 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:111b6c7486426c4b6989102c2ee5be856e8a58e20ab0a350b24a905d536e8e7f`  
		Last Modified: Fri, 04 Nov 2022 23:29:26 GMT  
		Size: 161.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e6f84dce457c6d4f7b7291fce05f8e77998a3a7722a54125a1f1d52ca83043b4`  
		Last Modified: Sat, 05 Nov 2022 01:50:51 GMT  
		Size: 173.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a6c26749ee782392e38845ee2ba79b0da586ef6a45d8e7f29c7af14612278547`  
		Last Modified: Tue, 15 Nov 2022 03:19:57 GMT  
		Size: 12.2 MB (12200249 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4dddc6d9fa6024025b3fcfe729cab2dc544fb25476eca6e80b1af8e8d93bb0ee`  
		Last Modified: Tue, 15 Nov 2022 03:19:56 GMT  
		Size: 452.7 KB (452680 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:06637eebe5e72c8ad9019ad4eb4cdde1f11f7d4c24c7ed7374cf8966343aa2fb`  
		Last Modified: Tue, 15 Nov 2022 03:19:56 GMT  
		Size: 131.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b276fb8390410a8208724033e325715ea26000d5a1a762d4c3699b927884fbfe`  
		Last Modified: Wed, 11 Jan 2023 02:52:45 GMT  
		Size: 178.8 MB (178805608 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:89de9d9e2c09cd5b84430562516cbcd5695a0a3b2347b451e157bde75c2b5619`  
		Last Modified: Wed, 22 Feb 2023 18:42:21 GMT  
		Size: 307.1 MB (307141303 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c34f6e86e4b4ce021fdc5c26a390f8682b638ef5b002596f5d85721a5b4f8b78`  
		Last Modified: Wed, 22 Feb 2023 18:43:25 GMT  
		Size: 589.9 KB (589888 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7c59af828719a4990baaba43861a4b7dfcf7c9301bc8c1c17b1977363ae47d8f`  
		Last Modified: Wed, 22 Feb 2023 18:43:25 GMT  
		Size: 1.3 KB (1345 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a1ce8abe653003fb1cf66551dd2e3daf88c2ec88e42e874179577314bcb129d7`  
		Last Modified: Wed, 22 Feb 2023 18:43:25 GMT  
		Size: 2.3 KB (2312 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:68e8b10875b16f8254c97d2580791e4ed6c27787f670ac843c0508addb3b38b3`  
		Last Modified: Wed, 22 Feb 2023 18:43:25 GMT  
		Size: 6.0 KB (6013 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ed46c896037147ae7b8029b5b7e890b7930132f0eec078e1211ccb92ff45c89e`  
		Last Modified: Wed, 22 Feb 2023 18:43:25 GMT  
		Size: 2.5 KB (2504 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `xwiki:lts-mariadb` - linux; arm64 variant v8

```console
$ docker pull xwiki@sha256:7325fc8b1c018497044befd011b0c006d687105f4227efb007aa304e9a7aae36
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **579.9 MB (579910180 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e16df67b6f15552144570116827b8b364c740abb52e9ca29c35e0c5ed526fe1b`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["xwiki"]`

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
# Wed, 02 Nov 2022 19:44:32 GMT
RUN apt-get update     && DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends tzdata curl wget ca-certificates fontconfig locales     && echo "en_US.UTF-8 UTF-8" >> /etc/locale.gen     && locale-gen en_US.UTF-8     && rm -rf /var/lib/apt/lists/*
# Fri, 04 Nov 2022 22:40:54 GMT
ENV JAVA_VERSION=jdk-11.0.17+8
# Fri, 04 Nov 2022 22:41:33 GMT
RUN set -eux;     ARCH="$(dpkg --print-architecture)";     case "${ARCH}" in        aarch64|arm64)          ESUM='bd6efe3290c8b5a42f695a55a26f3e3c9c284288574879d4b7089f31f5114177';          BINARY_URL='https://github.com/adoptium/temurin11-binaries/releases/download/jdk-11.0.17%2B8/OpenJDK11U-jre_aarch64_linux_hotspot_11.0.17_8.tar.gz';          ;;        armhf|arm)          ESUM='8cf113d3d7fa808895c8d2e41bb890af21c47e38c2460e0588147a4bb8fc658d';          BINARY_URL='https://github.com/adoptium/temurin11-binaries/releases/download/jdk-11.0.17%2B8/OpenJDK11U-jre_arm_linux_hotspot_11.0.17_8.tar.gz';          ;;        ppc64el|powerpc:common64)          ESUM='0ca3d806131ab5834c501f9c625bb0248cd528af361c704503348e9c9605bedf';          BINARY_URL='https://github.com/adoptium/temurin11-binaries/releases/download/jdk-11.0.17%2B8/OpenJDK11U-jre_ppc64le_linux_hotspot_11.0.17_8.tar.gz';          ;;        s390x|s390:64-bit)          ESUM='dd3b159a374086e65cb07c4ccb226c90f9c02ef929cba6f0b642171d7ed97fa4';          BINARY_URL='https://github.com/adoptium/temurin11-binaries/releases/download/jdk-11.0.17%2B8/OpenJDK11U-jre_s390x_linux_hotspot_11.0.17_8.tar.gz';          ;;        amd64|i386:x86-64)          ESUM='752616097e09d7f60a3ad8bd312f90eaf50ac72577e55df229fe6e8091148f79';          BINARY_URL='https://github.com/adoptium/temurin11-binaries/releases/download/jdk-11.0.17%2B8/OpenJDK11U-jre_x64_linux_hotspot_11.0.17_8.tar.gz';          ;;        *)          echo "Unsupported arch: ${ARCH}";          exit 1;          ;;     esac; 	  wget -O /tmp/openjdk.tar.gz ${BINARY_URL}; 	  echo "${ESUM} */tmp/openjdk.tar.gz" | sha256sum -c -; 	  mkdir -p "$JAVA_HOME"; 	  tar --extract 	      --file /tmp/openjdk.tar.gz 	      --directory "$JAVA_HOME" 	      --strip-components 1 	      --no-same-owner 	  ;     rm /tmp/openjdk.tar.gz;     find "$JAVA_HOME/lib" -name '*.so' -exec dirname '{}' ';' | sort -u > /etc/ld.so.conf.d/docker-openjdk.conf;     ldconfig;     java -Xshare:dump;
# Fri, 04 Nov 2022 22:41:34 GMT
RUN echo Verifying install ...     && fileEncoding="$(echo 'System.out.println(System.getProperty("file.encoding"))' | jshell -s -)"; [ "$fileEncoding" = 'UTF-8' ]; rm -rf ~/.java     && echo java --version && java --version     && echo Complete.
# Fri, 04 Nov 2022 23:48:38 GMT
ENV CATALINA_HOME=/usr/local/tomcat
# Fri, 04 Nov 2022 23:48:38 GMT
ENV PATH=/usr/local/tomcat/bin:/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Fri, 04 Nov 2022 23:48:38 GMT
RUN mkdir -p "$CATALINA_HOME"
# Fri, 04 Nov 2022 23:48:39 GMT
WORKDIR /usr/local/tomcat
# Fri, 04 Nov 2022 23:48:39 GMT
ENV TOMCAT_NATIVE_LIBDIR=/usr/local/tomcat/native-jni-lib
# Fri, 04 Nov 2022 23:48:39 GMT
ENV LD_LIBRARY_PATH=/usr/local/tomcat/native-jni-lib
# Fri, 04 Nov 2022 23:53:12 GMT
ENV GPG_KEYS=48F8E69F6390C9F25CFEDCD268248959359E722B A9C5DF4D22E99998D9875A5110C01C5A2F6059E7 DCFD35E0BF8CA7344752DE8B6FB21E8933C60243
# Fri, 04 Nov 2022 23:53:12 GMT
ENV TOMCAT_MAJOR=9
# Tue, 15 Nov 2022 04:57:22 GMT
ENV TOMCAT_VERSION=9.0.69
# Tue, 15 Nov 2022 04:57:22 GMT
ENV TOMCAT_SHA512=8c883c54ce9ce43eba37756a6404cdf3477879883a3e6d146dc8a7aa5e0425f487466afe6b6da4a895927cb7cb59177b9379cec18000f2de12785be57408c779
# Tue, 15 Nov 2022 04:57:22 GMT
COPY dir:096b403a5f78b17e6b4bff63128a9c93941b97f22470991610dd641633d977f1 in /usr/local/tomcat 
# Tue, 15 Nov 2022 04:57:25 GMT
RUN set -eux; 	apt-get update; 	xargs -rt apt-get install -y --no-install-recommends < "$TOMCAT_NATIVE_LIBDIR/.dependencies.txt"; 	rm -rf /var/lib/apt/lists/*
# Tue, 15 Nov 2022 04:57:26 GMT
RUN set -eux; 	nativeLines="$(catalina.sh configtest 2>&1)"; 	nativeLines="$(echo "$nativeLines" | grep 'Apache Tomcat Native')"; 	nativeLines="$(echo "$nativeLines" | sort -u)"; 	if ! echo "$nativeLines" | grep -E 'INFO: Loaded( APR based)? Apache Tomcat Native library' >&2; then 		echo >&2 "$nativeLines"; 		exit 1; 	fi
# Tue, 15 Nov 2022 04:57:26 GMT
EXPOSE 8080
# Tue, 15 Nov 2022 04:57:27 GMT
CMD ["catalina.sh" "run"]
# Wed, 11 Jan 2023 03:05:10 GMT
LABEL org.opencontainers.image.authors=XWiki Development Team <committers@xwiki.org>
# Wed, 11 Jan 2023 03:05:10 GMT
LABEL org.opencontainers.image.url=https://hub.docker.com/_/xwiki
# Wed, 11 Jan 2023 03:05:10 GMT
LABEL org.opencontainers.image.documentation=https://hub.docker.com/_/xwiki
# Wed, 11 Jan 2023 03:05:10 GMT
LABEL org.opencontainers.image.source=https://github.com/xwiki/xwiki-docker.git
# Wed, 11 Jan 2023 03:05:11 GMT
LABEL org.opencontainers.image.vendor=xwiki.org
# Wed, 11 Jan 2023 03:05:11 GMT
LABEL org.opencontainers.image.licenses=LGPL-2.1
# Wed, 11 Jan 2023 03:07:37 GMT
RUN apt-get update &&   apt-get --no-install-recommends -y install     curl     libreoffice     unzip     procps &&   rm -rf /var/lib/apt/lists/*
# Wed, 01 Feb 2023 22:26:19 GMT
ENV XWIKI_VERSION=14.10.4
# Wed, 01 Feb 2023 22:26:19 GMT
ENV XWIKI_URL_PREFIX=https://maven.xwiki.org/releases/org/xwiki/platform/xwiki-platform-distribution-war/14.10.4
# Wed, 01 Feb 2023 22:26:19 GMT
ENV XWIKI_DOWNLOAD_SHA256=2fcfb622319172c2e424b9c11848ebfabe27cf8ef69cba39ceb5d124b7ebe713
# Wed, 01 Feb 2023 22:27:00 GMT
RUN rm -rf /usr/local/tomcat/webapps/* &&   mkdir -p /usr/local/tomcat/temp &&   mkdir -p /usr/local/xwiki/data &&   curl -fSL "${XWIKI_URL_PREFIX}/xwiki-platform-distribution-war-${XWIKI_VERSION}.war" -o xwiki.war &&   echo "$XWIKI_DOWNLOAD_SHA256 xwiki.war" | sha256sum -c - &&   unzip -d /usr/local/tomcat/webapps/ROOT xwiki.war &&   rm -f xwiki.war
# Wed, 01 Feb 2023 22:27:55 GMT
ENV MARIADB_JDBC_VERSION=3.1.1
# Wed, 01 Feb 2023 22:27:55 GMT
ENV MARIADB_JDBC_SHA256=a554541fd88047905fb0c4c10e1d85295f5e38c7bb5fb408b425392a79fc26e3
# Wed, 01 Feb 2023 22:27:55 GMT
ENV MARIADB_JDBC_PREFIX=https://repo1.maven.org/maven2/org/mariadb/jdbc/mariadb-java-client/3.1.1
# Wed, 01 Feb 2023 22:27:55 GMT
ENV MARIADB_JDBC_ARTIFACT=mariadb-java-client-3.1.1.jar
# Wed, 01 Feb 2023 22:27:55 GMT
ENV MARIADB_JDBC_TARGET=/usr/local/tomcat/webapps/ROOT/WEB-INF/lib/mariadb-java-client-3.1.1.jar
# Wed, 01 Feb 2023 22:27:56 GMT
RUN curl -fSL "${MARIADB_JDBC_PREFIX}/${MARIADB_JDBC_ARTIFACT}" -o $MARIADB_JDBC_TARGET &&   echo "$MARIADB_JDBC_SHA256 $MARIADB_JDBC_TARGET" | sha256sum -c -
# Wed, 01 Feb 2023 22:27:56 GMT
COPY file:0a1be11e2eb610a1dbcd415404e3a592641110b93090030cb831e3a19a163017 in /usr/local/tomcat/bin/ 
# Wed, 01 Feb 2023 22:27:56 GMT
COPY file:0e237c3876eeb3b5f3473a064d3e507da2df6c228ca714687930b34e3b687601 in /usr/local/tomcat/webapps/ROOT/WEB-INF/hibernate.cfg.xml 
# Wed, 01 Feb 2023 22:27:57 GMT
RUN sed -i 's/<id>org.xwiki.platform:xwiki-platform-distribution-war/<id>org.xwiki.platform:xwiki-platform-distribution-docker/'   /usr/local/tomcat/webapps/ROOT/META-INF/extension.xed
# Wed, 01 Feb 2023 22:27:57 GMT
COPY file:a47c4dcd87c9dad97aff38c49188357e6193bcad50757e516cfb08a60d4de611 in /usr/local/bin/docker-entrypoint.sh 
# Wed, 01 Feb 2023 22:27:57 GMT
VOLUME [/usr/local/xwiki]
# Wed, 01 Feb 2023 22:27:57 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 01 Feb 2023 22:27:57 GMT
CMD ["xwiki"]
```

-	Layers:
	-	`sha256:0509fae36eb0656f8bdb23f8ae64100d893bcea2563e97468d337e04d2d0410b`  
		Last Modified: Wed, 02 Nov 2022 18:50:21 GMT  
		Size: 28.4 MB (28382154 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e502a1af2bcd98f5f0d2f5e4da1a0e7bbe07a2c548e2662f7d37dce5ae1df46c`  
		Last Modified: Wed, 02 Nov 2022 19:48:28 GMT  
		Size: 12.4 MB (12396330 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bc4598c07dd818f03a0378b0341a4a8e80f0152fbb3e7d5246ca4f466f42e611`  
		Last Modified: Fri, 04 Nov 2022 22:46:46 GMT  
		Size: 45.0 MB (44958470 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:715a937a1066f998b331fcd62256ad01a5571bdf46804e97825afc64f9ebb427`  
		Last Modified: Fri, 04 Nov 2022 22:46:41 GMT  
		Size: 160.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5fb623f082f74b2fa9fc2c4e3f3a4802875cb9753cfa26ed940201ce72bb56cb`  
		Last Modified: Sat, 05 Nov 2022 00:03:40 GMT  
		Size: 172.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:33260b83200262bbd546be371ad3c1f50f5ae7228afb87982d6fa9d6b11bf26f`  
		Last Modified: Tue, 15 Nov 2022 05:10:19 GMT  
		Size: 12.2 MB (12207235 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0955fb697ea9b30a1b4f95385464f646aa1525cb6efba648e22df84ebef6b2ee`  
		Last Modified: Tue, 15 Nov 2022 05:10:18 GMT  
		Size: 452.0 KB (452021 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6eddcf66f2083b1487296a0308e0b058917c97f614f12428d82d89662038dc2e`  
		Last Modified: Tue, 15 Nov 2022 05:10:18 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ae5f60bb64f3fa11da3d15a9639f886186b4c2c021455c3f9db22e0cfe1b1311`  
		Last Modified: Wed, 11 Jan 2023 03:11:14 GMT  
		Size: 173.8 MB (173806827 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:13334e257ce7313ca9d6028534e3ec6c7858c374c4afedea7f96c51da716806e`  
		Last Modified: Wed, 01 Feb 2023 22:29:16 GMT  
		Size: 307.1 MB (307104849 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a825dc0bda4f4de7842c41ce3db12885844733a8717fc3072c599678278e4b9b`  
		Last Modified: Wed, 01 Feb 2023 22:30:19 GMT  
		Size: 589.7 KB (589668 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0d3b831d82d4e981ad4dd1f4ef4cb7a5b16e7e27fff8121997366b1c93b836b7`  
		Last Modified: Wed, 01 Feb 2023 22:30:19 GMT  
		Size: 1.3 KB (1343 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b4b1db4f27135bc027a5f8478949b1118838f79760f5c779a18756553b080ac0`  
		Last Modified: Wed, 01 Feb 2023 22:30:19 GMT  
		Size: 2.3 KB (2309 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7f634a749b61f1dc714bb14b2b20c7fedd422c285161bdce24613edffc1feaca`  
		Last Modified: Wed, 01 Feb 2023 22:30:19 GMT  
		Size: 6.0 KB (6007 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f68b784196e13fd8e6790aa86b2f5a906f53094387165b175a9b981413e22fe1`  
		Last Modified: Wed, 01 Feb 2023 22:30:20 GMT  
		Size: 2.5 KB (2506 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `xwiki:lts-mariadb-tomcat`

```console
$ docker pull xwiki@sha256:016ba45d303064d25d04a705c1a307612a6383139366413fb169f42acc0419ee
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `xwiki:lts-mariadb-tomcat` - linux; amd64

```console
$ docker pull xwiki@sha256:4aec14b2a2ae95584b839238412bbe33a7314bf32edc3e05f34f532d07fdedce
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **588.7 MB (588696916 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f5fbe86c66c7ac80e07663234a80353ce71d1847f409e2e2a603e0eb2a3342bc`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["xwiki"]`

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
# Wed, 02 Nov 2022 18:44:10 GMT
RUN apt-get update     && DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends tzdata curl wget ca-certificates fontconfig locales     && echo "en_US.UTF-8 UTF-8" >> /etc/locale.gen     && locale-gen en_US.UTF-8     && rm -rf /var/lib/apt/lists/*
# Fri, 04 Nov 2022 23:21:41 GMT
ENV JAVA_VERSION=jdk-11.0.17+8
# Fri, 04 Nov 2022 23:22:31 GMT
RUN set -eux;     ARCH="$(dpkg --print-architecture)";     case "${ARCH}" in        aarch64|arm64)          ESUM='bd6efe3290c8b5a42f695a55a26f3e3c9c284288574879d4b7089f31f5114177';          BINARY_URL='https://github.com/adoptium/temurin11-binaries/releases/download/jdk-11.0.17%2B8/OpenJDK11U-jre_aarch64_linux_hotspot_11.0.17_8.tar.gz';          ;;        armhf|arm)          ESUM='8cf113d3d7fa808895c8d2e41bb890af21c47e38c2460e0588147a4bb8fc658d';          BINARY_URL='https://github.com/adoptium/temurin11-binaries/releases/download/jdk-11.0.17%2B8/OpenJDK11U-jre_arm_linux_hotspot_11.0.17_8.tar.gz';          ;;        ppc64el|powerpc:common64)          ESUM='0ca3d806131ab5834c501f9c625bb0248cd528af361c704503348e9c9605bedf';          BINARY_URL='https://github.com/adoptium/temurin11-binaries/releases/download/jdk-11.0.17%2B8/OpenJDK11U-jre_ppc64le_linux_hotspot_11.0.17_8.tar.gz';          ;;        s390x|s390:64-bit)          ESUM='dd3b159a374086e65cb07c4ccb226c90f9c02ef929cba6f0b642171d7ed97fa4';          BINARY_URL='https://github.com/adoptium/temurin11-binaries/releases/download/jdk-11.0.17%2B8/OpenJDK11U-jre_s390x_linux_hotspot_11.0.17_8.tar.gz';          ;;        amd64|i386:x86-64)          ESUM='752616097e09d7f60a3ad8bd312f90eaf50ac72577e55df229fe6e8091148f79';          BINARY_URL='https://github.com/adoptium/temurin11-binaries/releases/download/jdk-11.0.17%2B8/OpenJDK11U-jre_x64_linux_hotspot_11.0.17_8.tar.gz';          ;;        *)          echo "Unsupported arch: ${ARCH}";          exit 1;          ;;     esac; 	  wget -O /tmp/openjdk.tar.gz ${BINARY_URL}; 	  echo "${ESUM} */tmp/openjdk.tar.gz" | sha256sum -c -; 	  mkdir -p "$JAVA_HOME"; 	  tar --extract 	      --file /tmp/openjdk.tar.gz 	      --directory "$JAVA_HOME" 	      --strip-components 1 	      --no-same-owner 	  ;     rm /tmp/openjdk.tar.gz;     find "$JAVA_HOME/lib" -name '*.so' -exec dirname '{}' ';' | sort -u > /etc/ld.so.conf.d/docker-openjdk.conf;     ldconfig;     java -Xshare:dump;
# Fri, 04 Nov 2022 23:22:32 GMT
RUN echo Verifying install ...     && fileEncoding="$(echo 'System.out.println(System.getProperty("file.encoding"))' | jshell -s -)"; [ "$fileEncoding" = 'UTF-8' ]; rm -rf ~/.java     && echo java --version && java --version     && echo Complete.
# Sat, 05 Nov 2022 01:35:16 GMT
ENV CATALINA_HOME=/usr/local/tomcat
# Sat, 05 Nov 2022 01:35:16 GMT
ENV PATH=/usr/local/tomcat/bin:/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Sat, 05 Nov 2022 01:35:17 GMT
RUN mkdir -p "$CATALINA_HOME"
# Sat, 05 Nov 2022 01:35:17 GMT
WORKDIR /usr/local/tomcat
# Sat, 05 Nov 2022 01:35:17 GMT
ENV TOMCAT_NATIVE_LIBDIR=/usr/local/tomcat/native-jni-lib
# Sat, 05 Nov 2022 01:35:17 GMT
ENV LD_LIBRARY_PATH=/usr/local/tomcat/native-jni-lib
# Sat, 05 Nov 2022 01:39:54 GMT
ENV GPG_KEYS=48F8E69F6390C9F25CFEDCD268248959359E722B A9C5DF4D22E99998D9875A5110C01C5A2F6059E7 DCFD35E0BF8CA7344752DE8B6FB21E8933C60243
# Sat, 05 Nov 2022 01:39:54 GMT
ENV TOMCAT_MAJOR=9
# Tue, 15 Nov 2022 03:06:43 GMT
ENV TOMCAT_VERSION=9.0.69
# Tue, 15 Nov 2022 03:06:43 GMT
ENV TOMCAT_SHA512=8c883c54ce9ce43eba37756a6404cdf3477879883a3e6d146dc8a7aa5e0425f487466afe6b6da4a895927cb7cb59177b9379cec18000f2de12785be57408c779
# Tue, 15 Nov 2022 03:06:44 GMT
COPY dir:b1a33aa3993dbbfbebb33bd9aa546b60c2f2191abf1227f453d4e830f6deb35f in /usr/local/tomcat 
# Tue, 15 Nov 2022 03:06:48 GMT
RUN set -eux; 	apt-get update; 	xargs -rt apt-get install -y --no-install-recommends < "$TOMCAT_NATIVE_LIBDIR/.dependencies.txt"; 	rm -rf /var/lib/apt/lists/*
# Tue, 15 Nov 2022 03:06:49 GMT
RUN set -eux; 	nativeLines="$(catalina.sh configtest 2>&1)"; 	nativeLines="$(echo "$nativeLines" | grep 'Apache Tomcat Native')"; 	nativeLines="$(echo "$nativeLines" | sort -u)"; 	if ! echo "$nativeLines" | grep -E 'INFO: Loaded( APR based)? Apache Tomcat Native library' >&2; then 		echo >&2 "$nativeLines"; 		exit 1; 	fi
# Tue, 15 Nov 2022 03:06:49 GMT
EXPOSE 8080
# Tue, 15 Nov 2022 03:06:49 GMT
CMD ["catalina.sh" "run"]
# Wed, 11 Jan 2023 02:47:03 GMT
LABEL org.opencontainers.image.authors=XWiki Development Team <committers@xwiki.org>
# Wed, 11 Jan 2023 02:47:03 GMT
LABEL org.opencontainers.image.url=https://hub.docker.com/_/xwiki
# Wed, 11 Jan 2023 02:47:03 GMT
LABEL org.opencontainers.image.documentation=https://hub.docker.com/_/xwiki
# Wed, 11 Jan 2023 02:47:03 GMT
LABEL org.opencontainers.image.source=https://github.com/xwiki/xwiki-docker.git
# Wed, 11 Jan 2023 02:47:04 GMT
LABEL org.opencontainers.image.vendor=xwiki.org
# Wed, 11 Jan 2023 02:47:04 GMT
LABEL org.opencontainers.image.licenses=LGPL-2.1
# Wed, 11 Jan 2023 02:49:03 GMT
RUN apt-get update &&   apt-get --no-install-recommends -y install     curl     libreoffice     unzip     procps &&   rm -rf /var/lib/apt/lists/*
# Wed, 22 Feb 2023 18:39:36 GMT
ENV XWIKI_VERSION=14.10.5
# Wed, 22 Feb 2023 18:39:36 GMT
ENV XWIKI_URL_PREFIX=https://maven.xwiki.org/releases/org/xwiki/platform/xwiki-platform-distribution-war/14.10.5
# Wed, 22 Feb 2023 18:39:36 GMT
ENV XWIKI_DOWNLOAD_SHA256=f58465d0869e4c5605ae8375a09c79399d1149c7131fed3cf9959918267eb6a8
# Wed, 22 Feb 2023 18:40:15 GMT
RUN rm -rf /usr/local/tomcat/webapps/* &&   mkdir -p /usr/local/tomcat/temp &&   mkdir -p /usr/local/xwiki/data &&   curl -fSL "${XWIKI_URL_PREFIX}/xwiki-platform-distribution-war-${XWIKI_VERSION}.war" -o xwiki.war &&   echo "$XWIKI_DOWNLOAD_SHA256 xwiki.war" | sha256sum -c - &&   unzip -d /usr/local/tomcat/webapps/ROOT xwiki.war &&   rm -f xwiki.war
# Wed, 22 Feb 2023 18:41:14 GMT
ENV MARIADB_JDBC_VERSION=3.1.2
# Wed, 22 Feb 2023 18:41:14 GMT
ENV MARIADB_JDBC_SHA256=aaec1ad348d030a65b25c93c65cdaf472bf8b4b6b314b965e5ba13aec81bc622
# Wed, 22 Feb 2023 18:41:14 GMT
ENV MARIADB_JDBC_PREFIX=https://repo1.maven.org/maven2/org/mariadb/jdbc/mariadb-java-client/3.1.2
# Wed, 22 Feb 2023 18:41:14 GMT
ENV MARIADB_JDBC_ARTIFACT=mariadb-java-client-3.1.2.jar
# Wed, 22 Feb 2023 18:41:14 GMT
ENV MARIADB_JDBC_TARGET=/usr/local/tomcat/webapps/ROOT/WEB-INF/lib/mariadb-java-client-3.1.2.jar
# Wed, 22 Feb 2023 18:41:15 GMT
RUN curl -fSL "${MARIADB_JDBC_PREFIX}/${MARIADB_JDBC_ARTIFACT}" -o $MARIADB_JDBC_TARGET &&   echo "$MARIADB_JDBC_SHA256 $MARIADB_JDBC_TARGET" | sha256sum -c -
# Wed, 22 Feb 2023 18:41:15 GMT
COPY file:0a1be11e2eb610a1dbcd415404e3a592641110b93090030cb831e3a19a163017 in /usr/local/tomcat/bin/ 
# Wed, 22 Feb 2023 18:41:15 GMT
COPY file:0e237c3876eeb3b5f3473a064d3e507da2df6c228ca714687930b34e3b687601 in /usr/local/tomcat/webapps/ROOT/WEB-INF/hibernate.cfg.xml 
# Wed, 22 Feb 2023 18:41:15 GMT
RUN sed -i 's/<id>org.xwiki.platform:xwiki-platform-distribution-war/<id>org.xwiki.platform:xwiki-platform-distribution-docker/'   /usr/local/tomcat/webapps/ROOT/META-INF/extension.xed
# Wed, 22 Feb 2023 18:41:16 GMT
COPY file:a47c4dcd87c9dad97aff38c49188357e6193bcad50757e516cfb08a60d4de611 in /usr/local/bin/docker-entrypoint.sh 
# Wed, 22 Feb 2023 18:41:16 GMT
VOLUME [/usr/local/xwiki]
# Wed, 22 Feb 2023 18:41:16 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 22 Feb 2023 18:41:16 GMT
CMD ["xwiki"]
```

-	Layers:
	-	`sha256:e96e057aae67380a4ddb16c337c5c3669d97fdff69ec537f02aa2cc30d814281`  
		Last Modified: Wed, 02 Nov 2022 03:03:36 GMT  
		Size: 30.4 MB (30425607 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4ced2591451da3a02e2b6bb44752b9e3f00d77789921be4df5082fb9f9880ad0`  
		Last Modified: Wed, 02 Nov 2022 18:48:43 GMT  
		Size: 12.4 MB (12439006 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:df8f874ae8c08a9e69e5fbe6c5a64200a45386132a3203d1a9a7f1146d94cfbc`  
		Last Modified: Fri, 04 Nov 2022 23:29:33 GMT  
		Size: 46.6 MB (46629936 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:111b6c7486426c4b6989102c2ee5be856e8a58e20ab0a350b24a905d536e8e7f`  
		Last Modified: Fri, 04 Nov 2022 23:29:26 GMT  
		Size: 161.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e6f84dce457c6d4f7b7291fce05f8e77998a3a7722a54125a1f1d52ca83043b4`  
		Last Modified: Sat, 05 Nov 2022 01:50:51 GMT  
		Size: 173.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a6c26749ee782392e38845ee2ba79b0da586ef6a45d8e7f29c7af14612278547`  
		Last Modified: Tue, 15 Nov 2022 03:19:57 GMT  
		Size: 12.2 MB (12200249 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4dddc6d9fa6024025b3fcfe729cab2dc544fb25476eca6e80b1af8e8d93bb0ee`  
		Last Modified: Tue, 15 Nov 2022 03:19:56 GMT  
		Size: 452.7 KB (452680 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:06637eebe5e72c8ad9019ad4eb4cdde1f11f7d4c24c7ed7374cf8966343aa2fb`  
		Last Modified: Tue, 15 Nov 2022 03:19:56 GMT  
		Size: 131.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b276fb8390410a8208724033e325715ea26000d5a1a762d4c3699b927884fbfe`  
		Last Modified: Wed, 11 Jan 2023 02:52:45 GMT  
		Size: 178.8 MB (178805608 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:89de9d9e2c09cd5b84430562516cbcd5695a0a3b2347b451e157bde75c2b5619`  
		Last Modified: Wed, 22 Feb 2023 18:42:21 GMT  
		Size: 307.1 MB (307141303 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c34f6e86e4b4ce021fdc5c26a390f8682b638ef5b002596f5d85721a5b4f8b78`  
		Last Modified: Wed, 22 Feb 2023 18:43:25 GMT  
		Size: 589.9 KB (589888 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7c59af828719a4990baaba43861a4b7dfcf7c9301bc8c1c17b1977363ae47d8f`  
		Last Modified: Wed, 22 Feb 2023 18:43:25 GMT  
		Size: 1.3 KB (1345 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a1ce8abe653003fb1cf66551dd2e3daf88c2ec88e42e874179577314bcb129d7`  
		Last Modified: Wed, 22 Feb 2023 18:43:25 GMT  
		Size: 2.3 KB (2312 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:68e8b10875b16f8254c97d2580791e4ed6c27787f670ac843c0508addb3b38b3`  
		Last Modified: Wed, 22 Feb 2023 18:43:25 GMT  
		Size: 6.0 KB (6013 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ed46c896037147ae7b8029b5b7e890b7930132f0eec078e1211ccb92ff45c89e`  
		Last Modified: Wed, 22 Feb 2023 18:43:25 GMT  
		Size: 2.5 KB (2504 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `xwiki:lts-mariadb-tomcat` - linux; arm64 variant v8

```console
$ docker pull xwiki@sha256:7325fc8b1c018497044befd011b0c006d687105f4227efb007aa304e9a7aae36
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **579.9 MB (579910180 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e16df67b6f15552144570116827b8b364c740abb52e9ca29c35e0c5ed526fe1b`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["xwiki"]`

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
# Wed, 02 Nov 2022 19:44:32 GMT
RUN apt-get update     && DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends tzdata curl wget ca-certificates fontconfig locales     && echo "en_US.UTF-8 UTF-8" >> /etc/locale.gen     && locale-gen en_US.UTF-8     && rm -rf /var/lib/apt/lists/*
# Fri, 04 Nov 2022 22:40:54 GMT
ENV JAVA_VERSION=jdk-11.0.17+8
# Fri, 04 Nov 2022 22:41:33 GMT
RUN set -eux;     ARCH="$(dpkg --print-architecture)";     case "${ARCH}" in        aarch64|arm64)          ESUM='bd6efe3290c8b5a42f695a55a26f3e3c9c284288574879d4b7089f31f5114177';          BINARY_URL='https://github.com/adoptium/temurin11-binaries/releases/download/jdk-11.0.17%2B8/OpenJDK11U-jre_aarch64_linux_hotspot_11.0.17_8.tar.gz';          ;;        armhf|arm)          ESUM='8cf113d3d7fa808895c8d2e41bb890af21c47e38c2460e0588147a4bb8fc658d';          BINARY_URL='https://github.com/adoptium/temurin11-binaries/releases/download/jdk-11.0.17%2B8/OpenJDK11U-jre_arm_linux_hotspot_11.0.17_8.tar.gz';          ;;        ppc64el|powerpc:common64)          ESUM='0ca3d806131ab5834c501f9c625bb0248cd528af361c704503348e9c9605bedf';          BINARY_URL='https://github.com/adoptium/temurin11-binaries/releases/download/jdk-11.0.17%2B8/OpenJDK11U-jre_ppc64le_linux_hotspot_11.0.17_8.tar.gz';          ;;        s390x|s390:64-bit)          ESUM='dd3b159a374086e65cb07c4ccb226c90f9c02ef929cba6f0b642171d7ed97fa4';          BINARY_URL='https://github.com/adoptium/temurin11-binaries/releases/download/jdk-11.0.17%2B8/OpenJDK11U-jre_s390x_linux_hotspot_11.0.17_8.tar.gz';          ;;        amd64|i386:x86-64)          ESUM='752616097e09d7f60a3ad8bd312f90eaf50ac72577e55df229fe6e8091148f79';          BINARY_URL='https://github.com/adoptium/temurin11-binaries/releases/download/jdk-11.0.17%2B8/OpenJDK11U-jre_x64_linux_hotspot_11.0.17_8.tar.gz';          ;;        *)          echo "Unsupported arch: ${ARCH}";          exit 1;          ;;     esac; 	  wget -O /tmp/openjdk.tar.gz ${BINARY_URL}; 	  echo "${ESUM} */tmp/openjdk.tar.gz" | sha256sum -c -; 	  mkdir -p "$JAVA_HOME"; 	  tar --extract 	      --file /tmp/openjdk.tar.gz 	      --directory "$JAVA_HOME" 	      --strip-components 1 	      --no-same-owner 	  ;     rm /tmp/openjdk.tar.gz;     find "$JAVA_HOME/lib" -name '*.so' -exec dirname '{}' ';' | sort -u > /etc/ld.so.conf.d/docker-openjdk.conf;     ldconfig;     java -Xshare:dump;
# Fri, 04 Nov 2022 22:41:34 GMT
RUN echo Verifying install ...     && fileEncoding="$(echo 'System.out.println(System.getProperty("file.encoding"))' | jshell -s -)"; [ "$fileEncoding" = 'UTF-8' ]; rm -rf ~/.java     && echo java --version && java --version     && echo Complete.
# Fri, 04 Nov 2022 23:48:38 GMT
ENV CATALINA_HOME=/usr/local/tomcat
# Fri, 04 Nov 2022 23:48:38 GMT
ENV PATH=/usr/local/tomcat/bin:/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Fri, 04 Nov 2022 23:48:38 GMT
RUN mkdir -p "$CATALINA_HOME"
# Fri, 04 Nov 2022 23:48:39 GMT
WORKDIR /usr/local/tomcat
# Fri, 04 Nov 2022 23:48:39 GMT
ENV TOMCAT_NATIVE_LIBDIR=/usr/local/tomcat/native-jni-lib
# Fri, 04 Nov 2022 23:48:39 GMT
ENV LD_LIBRARY_PATH=/usr/local/tomcat/native-jni-lib
# Fri, 04 Nov 2022 23:53:12 GMT
ENV GPG_KEYS=48F8E69F6390C9F25CFEDCD268248959359E722B A9C5DF4D22E99998D9875A5110C01C5A2F6059E7 DCFD35E0BF8CA7344752DE8B6FB21E8933C60243
# Fri, 04 Nov 2022 23:53:12 GMT
ENV TOMCAT_MAJOR=9
# Tue, 15 Nov 2022 04:57:22 GMT
ENV TOMCAT_VERSION=9.0.69
# Tue, 15 Nov 2022 04:57:22 GMT
ENV TOMCAT_SHA512=8c883c54ce9ce43eba37756a6404cdf3477879883a3e6d146dc8a7aa5e0425f487466afe6b6da4a895927cb7cb59177b9379cec18000f2de12785be57408c779
# Tue, 15 Nov 2022 04:57:22 GMT
COPY dir:096b403a5f78b17e6b4bff63128a9c93941b97f22470991610dd641633d977f1 in /usr/local/tomcat 
# Tue, 15 Nov 2022 04:57:25 GMT
RUN set -eux; 	apt-get update; 	xargs -rt apt-get install -y --no-install-recommends < "$TOMCAT_NATIVE_LIBDIR/.dependencies.txt"; 	rm -rf /var/lib/apt/lists/*
# Tue, 15 Nov 2022 04:57:26 GMT
RUN set -eux; 	nativeLines="$(catalina.sh configtest 2>&1)"; 	nativeLines="$(echo "$nativeLines" | grep 'Apache Tomcat Native')"; 	nativeLines="$(echo "$nativeLines" | sort -u)"; 	if ! echo "$nativeLines" | grep -E 'INFO: Loaded( APR based)? Apache Tomcat Native library' >&2; then 		echo >&2 "$nativeLines"; 		exit 1; 	fi
# Tue, 15 Nov 2022 04:57:26 GMT
EXPOSE 8080
# Tue, 15 Nov 2022 04:57:27 GMT
CMD ["catalina.sh" "run"]
# Wed, 11 Jan 2023 03:05:10 GMT
LABEL org.opencontainers.image.authors=XWiki Development Team <committers@xwiki.org>
# Wed, 11 Jan 2023 03:05:10 GMT
LABEL org.opencontainers.image.url=https://hub.docker.com/_/xwiki
# Wed, 11 Jan 2023 03:05:10 GMT
LABEL org.opencontainers.image.documentation=https://hub.docker.com/_/xwiki
# Wed, 11 Jan 2023 03:05:10 GMT
LABEL org.opencontainers.image.source=https://github.com/xwiki/xwiki-docker.git
# Wed, 11 Jan 2023 03:05:11 GMT
LABEL org.opencontainers.image.vendor=xwiki.org
# Wed, 11 Jan 2023 03:05:11 GMT
LABEL org.opencontainers.image.licenses=LGPL-2.1
# Wed, 11 Jan 2023 03:07:37 GMT
RUN apt-get update &&   apt-get --no-install-recommends -y install     curl     libreoffice     unzip     procps &&   rm -rf /var/lib/apt/lists/*
# Wed, 01 Feb 2023 22:26:19 GMT
ENV XWIKI_VERSION=14.10.4
# Wed, 01 Feb 2023 22:26:19 GMT
ENV XWIKI_URL_PREFIX=https://maven.xwiki.org/releases/org/xwiki/platform/xwiki-platform-distribution-war/14.10.4
# Wed, 01 Feb 2023 22:26:19 GMT
ENV XWIKI_DOWNLOAD_SHA256=2fcfb622319172c2e424b9c11848ebfabe27cf8ef69cba39ceb5d124b7ebe713
# Wed, 01 Feb 2023 22:27:00 GMT
RUN rm -rf /usr/local/tomcat/webapps/* &&   mkdir -p /usr/local/tomcat/temp &&   mkdir -p /usr/local/xwiki/data &&   curl -fSL "${XWIKI_URL_PREFIX}/xwiki-platform-distribution-war-${XWIKI_VERSION}.war" -o xwiki.war &&   echo "$XWIKI_DOWNLOAD_SHA256 xwiki.war" | sha256sum -c - &&   unzip -d /usr/local/tomcat/webapps/ROOT xwiki.war &&   rm -f xwiki.war
# Wed, 01 Feb 2023 22:27:55 GMT
ENV MARIADB_JDBC_VERSION=3.1.1
# Wed, 01 Feb 2023 22:27:55 GMT
ENV MARIADB_JDBC_SHA256=a554541fd88047905fb0c4c10e1d85295f5e38c7bb5fb408b425392a79fc26e3
# Wed, 01 Feb 2023 22:27:55 GMT
ENV MARIADB_JDBC_PREFIX=https://repo1.maven.org/maven2/org/mariadb/jdbc/mariadb-java-client/3.1.1
# Wed, 01 Feb 2023 22:27:55 GMT
ENV MARIADB_JDBC_ARTIFACT=mariadb-java-client-3.1.1.jar
# Wed, 01 Feb 2023 22:27:55 GMT
ENV MARIADB_JDBC_TARGET=/usr/local/tomcat/webapps/ROOT/WEB-INF/lib/mariadb-java-client-3.1.1.jar
# Wed, 01 Feb 2023 22:27:56 GMT
RUN curl -fSL "${MARIADB_JDBC_PREFIX}/${MARIADB_JDBC_ARTIFACT}" -o $MARIADB_JDBC_TARGET &&   echo "$MARIADB_JDBC_SHA256 $MARIADB_JDBC_TARGET" | sha256sum -c -
# Wed, 01 Feb 2023 22:27:56 GMT
COPY file:0a1be11e2eb610a1dbcd415404e3a592641110b93090030cb831e3a19a163017 in /usr/local/tomcat/bin/ 
# Wed, 01 Feb 2023 22:27:56 GMT
COPY file:0e237c3876eeb3b5f3473a064d3e507da2df6c228ca714687930b34e3b687601 in /usr/local/tomcat/webapps/ROOT/WEB-INF/hibernate.cfg.xml 
# Wed, 01 Feb 2023 22:27:57 GMT
RUN sed -i 's/<id>org.xwiki.platform:xwiki-platform-distribution-war/<id>org.xwiki.platform:xwiki-platform-distribution-docker/'   /usr/local/tomcat/webapps/ROOT/META-INF/extension.xed
# Wed, 01 Feb 2023 22:27:57 GMT
COPY file:a47c4dcd87c9dad97aff38c49188357e6193bcad50757e516cfb08a60d4de611 in /usr/local/bin/docker-entrypoint.sh 
# Wed, 01 Feb 2023 22:27:57 GMT
VOLUME [/usr/local/xwiki]
# Wed, 01 Feb 2023 22:27:57 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 01 Feb 2023 22:27:57 GMT
CMD ["xwiki"]
```

-	Layers:
	-	`sha256:0509fae36eb0656f8bdb23f8ae64100d893bcea2563e97468d337e04d2d0410b`  
		Last Modified: Wed, 02 Nov 2022 18:50:21 GMT  
		Size: 28.4 MB (28382154 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e502a1af2bcd98f5f0d2f5e4da1a0e7bbe07a2c548e2662f7d37dce5ae1df46c`  
		Last Modified: Wed, 02 Nov 2022 19:48:28 GMT  
		Size: 12.4 MB (12396330 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bc4598c07dd818f03a0378b0341a4a8e80f0152fbb3e7d5246ca4f466f42e611`  
		Last Modified: Fri, 04 Nov 2022 22:46:46 GMT  
		Size: 45.0 MB (44958470 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:715a937a1066f998b331fcd62256ad01a5571bdf46804e97825afc64f9ebb427`  
		Last Modified: Fri, 04 Nov 2022 22:46:41 GMT  
		Size: 160.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5fb623f082f74b2fa9fc2c4e3f3a4802875cb9753cfa26ed940201ce72bb56cb`  
		Last Modified: Sat, 05 Nov 2022 00:03:40 GMT  
		Size: 172.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:33260b83200262bbd546be371ad3c1f50f5ae7228afb87982d6fa9d6b11bf26f`  
		Last Modified: Tue, 15 Nov 2022 05:10:19 GMT  
		Size: 12.2 MB (12207235 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0955fb697ea9b30a1b4f95385464f646aa1525cb6efba648e22df84ebef6b2ee`  
		Last Modified: Tue, 15 Nov 2022 05:10:18 GMT  
		Size: 452.0 KB (452021 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6eddcf66f2083b1487296a0308e0b058917c97f614f12428d82d89662038dc2e`  
		Last Modified: Tue, 15 Nov 2022 05:10:18 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ae5f60bb64f3fa11da3d15a9639f886186b4c2c021455c3f9db22e0cfe1b1311`  
		Last Modified: Wed, 11 Jan 2023 03:11:14 GMT  
		Size: 173.8 MB (173806827 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:13334e257ce7313ca9d6028534e3ec6c7858c374c4afedea7f96c51da716806e`  
		Last Modified: Wed, 01 Feb 2023 22:29:16 GMT  
		Size: 307.1 MB (307104849 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a825dc0bda4f4de7842c41ce3db12885844733a8717fc3072c599678278e4b9b`  
		Last Modified: Wed, 01 Feb 2023 22:30:19 GMT  
		Size: 589.7 KB (589668 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0d3b831d82d4e981ad4dd1f4ef4cb7a5b16e7e27fff8121997366b1c93b836b7`  
		Last Modified: Wed, 01 Feb 2023 22:30:19 GMT  
		Size: 1.3 KB (1343 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b4b1db4f27135bc027a5f8478949b1118838f79760f5c779a18756553b080ac0`  
		Last Modified: Wed, 01 Feb 2023 22:30:19 GMT  
		Size: 2.3 KB (2309 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7f634a749b61f1dc714bb14b2b20c7fedd422c285161bdce24613edffc1feaca`  
		Last Modified: Wed, 01 Feb 2023 22:30:19 GMT  
		Size: 6.0 KB (6007 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f68b784196e13fd8e6790aa86b2f5a906f53094387165b175a9b981413e22fe1`  
		Last Modified: Wed, 01 Feb 2023 22:30:20 GMT  
		Size: 2.5 KB (2506 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `xwiki:lts-mysql`

```console
$ docker pull xwiki@sha256:32e51c9775fda50082b0f02856f2af444a67284446679c9a3a13a78c02ec0c4b
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `xwiki:lts-mysql` - linux; amd64

```console
$ docker pull xwiki@sha256:a2e996a399fc68cbccfe11eaeb0115a15314bd69f06c483fef3cba244fa07cbf
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **590.4 MB (590449604 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:6b73fd725d5c1dd8044289fdb0e76f973e7e1d4a64e1efc44428235a718b550a`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["xwiki"]`

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
# Wed, 02 Nov 2022 18:44:10 GMT
RUN apt-get update     && DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends tzdata curl wget ca-certificates fontconfig locales     && echo "en_US.UTF-8 UTF-8" >> /etc/locale.gen     && locale-gen en_US.UTF-8     && rm -rf /var/lib/apt/lists/*
# Fri, 04 Nov 2022 23:21:41 GMT
ENV JAVA_VERSION=jdk-11.0.17+8
# Fri, 04 Nov 2022 23:22:31 GMT
RUN set -eux;     ARCH="$(dpkg --print-architecture)";     case "${ARCH}" in        aarch64|arm64)          ESUM='bd6efe3290c8b5a42f695a55a26f3e3c9c284288574879d4b7089f31f5114177';          BINARY_URL='https://github.com/adoptium/temurin11-binaries/releases/download/jdk-11.0.17%2B8/OpenJDK11U-jre_aarch64_linux_hotspot_11.0.17_8.tar.gz';          ;;        armhf|arm)          ESUM='8cf113d3d7fa808895c8d2e41bb890af21c47e38c2460e0588147a4bb8fc658d';          BINARY_URL='https://github.com/adoptium/temurin11-binaries/releases/download/jdk-11.0.17%2B8/OpenJDK11U-jre_arm_linux_hotspot_11.0.17_8.tar.gz';          ;;        ppc64el|powerpc:common64)          ESUM='0ca3d806131ab5834c501f9c625bb0248cd528af361c704503348e9c9605bedf';          BINARY_URL='https://github.com/adoptium/temurin11-binaries/releases/download/jdk-11.0.17%2B8/OpenJDK11U-jre_ppc64le_linux_hotspot_11.0.17_8.tar.gz';          ;;        s390x|s390:64-bit)          ESUM='dd3b159a374086e65cb07c4ccb226c90f9c02ef929cba6f0b642171d7ed97fa4';          BINARY_URL='https://github.com/adoptium/temurin11-binaries/releases/download/jdk-11.0.17%2B8/OpenJDK11U-jre_s390x_linux_hotspot_11.0.17_8.tar.gz';          ;;        amd64|i386:x86-64)          ESUM='752616097e09d7f60a3ad8bd312f90eaf50ac72577e55df229fe6e8091148f79';          BINARY_URL='https://github.com/adoptium/temurin11-binaries/releases/download/jdk-11.0.17%2B8/OpenJDK11U-jre_x64_linux_hotspot_11.0.17_8.tar.gz';          ;;        *)          echo "Unsupported arch: ${ARCH}";          exit 1;          ;;     esac; 	  wget -O /tmp/openjdk.tar.gz ${BINARY_URL}; 	  echo "${ESUM} */tmp/openjdk.tar.gz" | sha256sum -c -; 	  mkdir -p "$JAVA_HOME"; 	  tar --extract 	      --file /tmp/openjdk.tar.gz 	      --directory "$JAVA_HOME" 	      --strip-components 1 	      --no-same-owner 	  ;     rm /tmp/openjdk.tar.gz;     find "$JAVA_HOME/lib" -name '*.so' -exec dirname '{}' ';' | sort -u > /etc/ld.so.conf.d/docker-openjdk.conf;     ldconfig;     java -Xshare:dump;
# Fri, 04 Nov 2022 23:22:32 GMT
RUN echo Verifying install ...     && fileEncoding="$(echo 'System.out.println(System.getProperty("file.encoding"))' | jshell -s -)"; [ "$fileEncoding" = 'UTF-8' ]; rm -rf ~/.java     && echo java --version && java --version     && echo Complete.
# Sat, 05 Nov 2022 01:35:16 GMT
ENV CATALINA_HOME=/usr/local/tomcat
# Sat, 05 Nov 2022 01:35:16 GMT
ENV PATH=/usr/local/tomcat/bin:/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Sat, 05 Nov 2022 01:35:17 GMT
RUN mkdir -p "$CATALINA_HOME"
# Sat, 05 Nov 2022 01:35:17 GMT
WORKDIR /usr/local/tomcat
# Sat, 05 Nov 2022 01:35:17 GMT
ENV TOMCAT_NATIVE_LIBDIR=/usr/local/tomcat/native-jni-lib
# Sat, 05 Nov 2022 01:35:17 GMT
ENV LD_LIBRARY_PATH=/usr/local/tomcat/native-jni-lib
# Sat, 05 Nov 2022 01:39:54 GMT
ENV GPG_KEYS=48F8E69F6390C9F25CFEDCD268248959359E722B A9C5DF4D22E99998D9875A5110C01C5A2F6059E7 DCFD35E0BF8CA7344752DE8B6FB21E8933C60243
# Sat, 05 Nov 2022 01:39:54 GMT
ENV TOMCAT_MAJOR=9
# Tue, 15 Nov 2022 03:06:43 GMT
ENV TOMCAT_VERSION=9.0.69
# Tue, 15 Nov 2022 03:06:43 GMT
ENV TOMCAT_SHA512=8c883c54ce9ce43eba37756a6404cdf3477879883a3e6d146dc8a7aa5e0425f487466afe6b6da4a895927cb7cb59177b9379cec18000f2de12785be57408c779
# Tue, 15 Nov 2022 03:06:44 GMT
COPY dir:b1a33aa3993dbbfbebb33bd9aa546b60c2f2191abf1227f453d4e830f6deb35f in /usr/local/tomcat 
# Tue, 15 Nov 2022 03:06:48 GMT
RUN set -eux; 	apt-get update; 	xargs -rt apt-get install -y --no-install-recommends < "$TOMCAT_NATIVE_LIBDIR/.dependencies.txt"; 	rm -rf /var/lib/apt/lists/*
# Tue, 15 Nov 2022 03:06:49 GMT
RUN set -eux; 	nativeLines="$(catalina.sh configtest 2>&1)"; 	nativeLines="$(echo "$nativeLines" | grep 'Apache Tomcat Native')"; 	nativeLines="$(echo "$nativeLines" | sort -u)"; 	if ! echo "$nativeLines" | grep -E 'INFO: Loaded( APR based)? Apache Tomcat Native library' >&2; then 		echo >&2 "$nativeLines"; 		exit 1; 	fi
# Tue, 15 Nov 2022 03:06:49 GMT
EXPOSE 8080
# Tue, 15 Nov 2022 03:06:49 GMT
CMD ["catalina.sh" "run"]
# Wed, 11 Jan 2023 02:47:03 GMT
LABEL org.opencontainers.image.authors=XWiki Development Team <committers@xwiki.org>
# Wed, 11 Jan 2023 02:47:03 GMT
LABEL org.opencontainers.image.url=https://hub.docker.com/_/xwiki
# Wed, 11 Jan 2023 02:47:03 GMT
LABEL org.opencontainers.image.documentation=https://hub.docker.com/_/xwiki
# Wed, 11 Jan 2023 02:47:03 GMT
LABEL org.opencontainers.image.source=https://github.com/xwiki/xwiki-docker.git
# Wed, 11 Jan 2023 02:47:04 GMT
LABEL org.opencontainers.image.vendor=xwiki.org
# Wed, 11 Jan 2023 02:47:04 GMT
LABEL org.opencontainers.image.licenses=LGPL-2.1
# Wed, 11 Jan 2023 02:49:03 GMT
RUN apt-get update &&   apt-get --no-install-recommends -y install     curl     libreoffice     unzip     procps &&   rm -rf /var/lib/apt/lists/*
# Wed, 22 Feb 2023 18:39:36 GMT
ENV XWIKI_VERSION=14.10.5
# Wed, 22 Feb 2023 18:39:36 GMT
ENV XWIKI_URL_PREFIX=https://maven.xwiki.org/releases/org/xwiki/platform/xwiki-platform-distribution-war/14.10.5
# Wed, 22 Feb 2023 18:39:36 GMT
ENV XWIKI_DOWNLOAD_SHA256=f58465d0869e4c5605ae8375a09c79399d1149c7131fed3cf9959918267eb6a8
# Wed, 22 Feb 2023 18:40:15 GMT
RUN rm -rf /usr/local/tomcat/webapps/* &&   mkdir -p /usr/local/tomcat/temp &&   mkdir -p /usr/local/xwiki/data &&   curl -fSL "${XWIKI_URL_PREFIX}/xwiki-platform-distribution-war-${XWIKI_VERSION}.war" -o xwiki.war &&   echo "$XWIKI_DOWNLOAD_SHA256 xwiki.war" | sha256sum -c - &&   unzip -d /usr/local/tomcat/webapps/ROOT xwiki.war &&   rm -f xwiki.war
# Wed, 22 Feb 2023 18:40:17 GMT
ENV MYSQL_JDBC_VERSION=8.0.32
# Wed, 22 Feb 2023 18:40:17 GMT
ENV MYSQL_JDBC_SHA256=522329fe925980f02e5eb89b59d227245d345415ff0c08932a68c9765c13acc5
# Wed, 22 Feb 2023 18:40:17 GMT
ENV MYSQL_JDBC_PREFIX=https://repo1.maven.org/maven2/com/mysql/mysql-connector-j/8.0.32
# Wed, 22 Feb 2023 18:40:17 GMT
ENV MYSQL_JDBC_ARTIFACT=mysql-connector-j-8.0.32.jar
# Wed, 22 Feb 2023 18:40:17 GMT
ENV MYSQL_JDBC_TARGET=/usr/local/tomcat/webapps/ROOT/WEB-INF/lib/mysql-connector-j-8.0.32.jar
# Wed, 22 Feb 2023 18:40:18 GMT
RUN curl -fSL "${MYSQL_JDBC_PREFIX}/${MYSQL_JDBC_ARTIFACT}" -o $MYSQL_JDBC_TARGET &&   echo "$MYSQL_JDBC_SHA256 $MYSQL_JDBC_TARGET" | sha256sum -c -
# Wed, 22 Feb 2023 18:40:18 GMT
COPY file:0a1be11e2eb610a1dbcd415404e3a592641110b93090030cb831e3a19a163017 in /usr/local/tomcat/bin/ 
# Wed, 22 Feb 2023 18:40:18 GMT
COPY file:1b8409986f3e4eb79a7a0b18472cb2692a61d504fb5ef34292bc997b79fd760d in /usr/local/tomcat/webapps/ROOT/WEB-INF/hibernate.cfg.xml 
# Wed, 22 Feb 2023 18:40:19 GMT
RUN sed -i 's/<id>org.xwiki.platform:xwiki-platform-distribution-war/<id>org.xwiki.platform:xwiki-platform-distribution-docker/'   /usr/local/tomcat/webapps/ROOT/META-INF/extension.xed
# Wed, 22 Feb 2023 18:40:19 GMT
COPY file:a47c4dcd87c9dad97aff38c49188357e6193bcad50757e516cfb08a60d4de611 in /usr/local/bin/docker-entrypoint.sh 
# Wed, 22 Feb 2023 18:40:19 GMT
VOLUME [/usr/local/xwiki]
# Wed, 22 Feb 2023 18:40:19 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 22 Feb 2023 18:40:19 GMT
CMD ["xwiki"]
```

-	Layers:
	-	`sha256:e96e057aae67380a4ddb16c337c5c3669d97fdff69ec537f02aa2cc30d814281`  
		Last Modified: Wed, 02 Nov 2022 03:03:36 GMT  
		Size: 30.4 MB (30425607 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4ced2591451da3a02e2b6bb44752b9e3f00d77789921be4df5082fb9f9880ad0`  
		Last Modified: Wed, 02 Nov 2022 18:48:43 GMT  
		Size: 12.4 MB (12439006 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:df8f874ae8c08a9e69e5fbe6c5a64200a45386132a3203d1a9a7f1146d94cfbc`  
		Last Modified: Fri, 04 Nov 2022 23:29:33 GMT  
		Size: 46.6 MB (46629936 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:111b6c7486426c4b6989102c2ee5be856e8a58e20ab0a350b24a905d536e8e7f`  
		Last Modified: Fri, 04 Nov 2022 23:29:26 GMT  
		Size: 161.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e6f84dce457c6d4f7b7291fce05f8e77998a3a7722a54125a1f1d52ca83043b4`  
		Last Modified: Sat, 05 Nov 2022 01:50:51 GMT  
		Size: 173.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a6c26749ee782392e38845ee2ba79b0da586ef6a45d8e7f29c7af14612278547`  
		Last Modified: Tue, 15 Nov 2022 03:19:57 GMT  
		Size: 12.2 MB (12200249 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4dddc6d9fa6024025b3fcfe729cab2dc544fb25476eca6e80b1af8e8d93bb0ee`  
		Last Modified: Tue, 15 Nov 2022 03:19:56 GMT  
		Size: 452.7 KB (452680 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:06637eebe5e72c8ad9019ad4eb4cdde1f11f7d4c24c7ed7374cf8966343aa2fb`  
		Last Modified: Tue, 15 Nov 2022 03:19:56 GMT  
		Size: 131.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b276fb8390410a8208724033e325715ea26000d5a1a762d4c3699b927884fbfe`  
		Last Modified: Wed, 11 Jan 2023 02:52:45 GMT  
		Size: 178.8 MB (178805608 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:89de9d9e2c09cd5b84430562516cbcd5695a0a3b2347b451e157bde75c2b5619`  
		Last Modified: Wed, 22 Feb 2023 18:42:21 GMT  
		Size: 307.1 MB (307141303 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4a2089179b7c1db514d0502e476e09b8f9313d08d4c4e4f3981be456288fe507`  
		Last Modified: Wed, 22 Feb 2023 18:42:04 GMT  
		Size: 2.3 MB (2342572 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e7c4ef360ff3673244adb3dfc4769b5710fa68fcc1fbe1c08b2f5fa32dbd4976`  
		Last Modified: Wed, 22 Feb 2023 18:42:04 GMT  
		Size: 1.3 KB (1348 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:08441c368d4b01e361491d7fbf1ac579fcc303b8484123c309a8d5a3b6657c46`  
		Last Modified: Wed, 22 Feb 2023 18:42:04 GMT  
		Size: 2.3 KB (2311 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:542b4bb846d438395e458c08de292f72d14d289fae6ffe7eba6fec1cd8518475`  
		Last Modified: Wed, 22 Feb 2023 18:42:04 GMT  
		Size: 6.0 KB (6013 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:039c0305df9e64c69bb546e64f0658dba6e728eee13022cfd682aa1ee76b8b7f`  
		Last Modified: Wed, 22 Feb 2023 18:42:04 GMT  
		Size: 2.5 KB (2506 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `xwiki:lts-mysql` - linux; arm64 variant v8

```console
$ docker pull xwiki@sha256:33e36167828fe9bae944e7d4cbbe3b69dd2415595d40610ac2ebcd73f2c2fa7f
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **581.7 MB (581697690 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:44013daf43fd09deb7221eef006c4d30d484a03c433118e5b59da0a44b573f06`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["xwiki"]`

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
# Wed, 02 Nov 2022 19:44:32 GMT
RUN apt-get update     && DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends tzdata curl wget ca-certificates fontconfig locales     && echo "en_US.UTF-8 UTF-8" >> /etc/locale.gen     && locale-gen en_US.UTF-8     && rm -rf /var/lib/apt/lists/*
# Fri, 04 Nov 2022 22:40:54 GMT
ENV JAVA_VERSION=jdk-11.0.17+8
# Fri, 04 Nov 2022 22:41:33 GMT
RUN set -eux;     ARCH="$(dpkg --print-architecture)";     case "${ARCH}" in        aarch64|arm64)          ESUM='bd6efe3290c8b5a42f695a55a26f3e3c9c284288574879d4b7089f31f5114177';          BINARY_URL='https://github.com/adoptium/temurin11-binaries/releases/download/jdk-11.0.17%2B8/OpenJDK11U-jre_aarch64_linux_hotspot_11.0.17_8.tar.gz';          ;;        armhf|arm)          ESUM='8cf113d3d7fa808895c8d2e41bb890af21c47e38c2460e0588147a4bb8fc658d';          BINARY_URL='https://github.com/adoptium/temurin11-binaries/releases/download/jdk-11.0.17%2B8/OpenJDK11U-jre_arm_linux_hotspot_11.0.17_8.tar.gz';          ;;        ppc64el|powerpc:common64)          ESUM='0ca3d806131ab5834c501f9c625bb0248cd528af361c704503348e9c9605bedf';          BINARY_URL='https://github.com/adoptium/temurin11-binaries/releases/download/jdk-11.0.17%2B8/OpenJDK11U-jre_ppc64le_linux_hotspot_11.0.17_8.tar.gz';          ;;        s390x|s390:64-bit)          ESUM='dd3b159a374086e65cb07c4ccb226c90f9c02ef929cba6f0b642171d7ed97fa4';          BINARY_URL='https://github.com/adoptium/temurin11-binaries/releases/download/jdk-11.0.17%2B8/OpenJDK11U-jre_s390x_linux_hotspot_11.0.17_8.tar.gz';          ;;        amd64|i386:x86-64)          ESUM='752616097e09d7f60a3ad8bd312f90eaf50ac72577e55df229fe6e8091148f79';          BINARY_URL='https://github.com/adoptium/temurin11-binaries/releases/download/jdk-11.0.17%2B8/OpenJDK11U-jre_x64_linux_hotspot_11.0.17_8.tar.gz';          ;;        *)          echo "Unsupported arch: ${ARCH}";          exit 1;          ;;     esac; 	  wget -O /tmp/openjdk.tar.gz ${BINARY_URL}; 	  echo "${ESUM} */tmp/openjdk.tar.gz" | sha256sum -c -; 	  mkdir -p "$JAVA_HOME"; 	  tar --extract 	      --file /tmp/openjdk.tar.gz 	      --directory "$JAVA_HOME" 	      --strip-components 1 	      --no-same-owner 	  ;     rm /tmp/openjdk.tar.gz;     find "$JAVA_HOME/lib" -name '*.so' -exec dirname '{}' ';' | sort -u > /etc/ld.so.conf.d/docker-openjdk.conf;     ldconfig;     java -Xshare:dump;
# Fri, 04 Nov 2022 22:41:34 GMT
RUN echo Verifying install ...     && fileEncoding="$(echo 'System.out.println(System.getProperty("file.encoding"))' | jshell -s -)"; [ "$fileEncoding" = 'UTF-8' ]; rm -rf ~/.java     && echo java --version && java --version     && echo Complete.
# Fri, 04 Nov 2022 23:48:38 GMT
ENV CATALINA_HOME=/usr/local/tomcat
# Fri, 04 Nov 2022 23:48:38 GMT
ENV PATH=/usr/local/tomcat/bin:/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Fri, 04 Nov 2022 23:48:38 GMT
RUN mkdir -p "$CATALINA_HOME"
# Fri, 04 Nov 2022 23:48:39 GMT
WORKDIR /usr/local/tomcat
# Fri, 04 Nov 2022 23:48:39 GMT
ENV TOMCAT_NATIVE_LIBDIR=/usr/local/tomcat/native-jni-lib
# Fri, 04 Nov 2022 23:48:39 GMT
ENV LD_LIBRARY_PATH=/usr/local/tomcat/native-jni-lib
# Fri, 04 Nov 2022 23:53:12 GMT
ENV GPG_KEYS=48F8E69F6390C9F25CFEDCD268248959359E722B A9C5DF4D22E99998D9875A5110C01C5A2F6059E7 DCFD35E0BF8CA7344752DE8B6FB21E8933C60243
# Fri, 04 Nov 2022 23:53:12 GMT
ENV TOMCAT_MAJOR=9
# Tue, 15 Nov 2022 04:57:22 GMT
ENV TOMCAT_VERSION=9.0.69
# Tue, 15 Nov 2022 04:57:22 GMT
ENV TOMCAT_SHA512=8c883c54ce9ce43eba37756a6404cdf3477879883a3e6d146dc8a7aa5e0425f487466afe6b6da4a895927cb7cb59177b9379cec18000f2de12785be57408c779
# Tue, 15 Nov 2022 04:57:22 GMT
COPY dir:096b403a5f78b17e6b4bff63128a9c93941b97f22470991610dd641633d977f1 in /usr/local/tomcat 
# Tue, 15 Nov 2022 04:57:25 GMT
RUN set -eux; 	apt-get update; 	xargs -rt apt-get install -y --no-install-recommends < "$TOMCAT_NATIVE_LIBDIR/.dependencies.txt"; 	rm -rf /var/lib/apt/lists/*
# Tue, 15 Nov 2022 04:57:26 GMT
RUN set -eux; 	nativeLines="$(catalina.sh configtest 2>&1)"; 	nativeLines="$(echo "$nativeLines" | grep 'Apache Tomcat Native')"; 	nativeLines="$(echo "$nativeLines" | sort -u)"; 	if ! echo "$nativeLines" | grep -E 'INFO: Loaded( APR based)? Apache Tomcat Native library' >&2; then 		echo >&2 "$nativeLines"; 		exit 1; 	fi
# Tue, 15 Nov 2022 04:57:26 GMT
EXPOSE 8080
# Tue, 15 Nov 2022 04:57:27 GMT
CMD ["catalina.sh" "run"]
# Wed, 11 Jan 2023 03:05:10 GMT
LABEL org.opencontainers.image.authors=XWiki Development Team <committers@xwiki.org>
# Wed, 11 Jan 2023 03:05:10 GMT
LABEL org.opencontainers.image.url=https://hub.docker.com/_/xwiki
# Wed, 11 Jan 2023 03:05:10 GMT
LABEL org.opencontainers.image.documentation=https://hub.docker.com/_/xwiki
# Wed, 11 Jan 2023 03:05:10 GMT
LABEL org.opencontainers.image.source=https://github.com/xwiki/xwiki-docker.git
# Wed, 11 Jan 2023 03:05:11 GMT
LABEL org.opencontainers.image.vendor=xwiki.org
# Wed, 11 Jan 2023 03:05:11 GMT
LABEL org.opencontainers.image.licenses=LGPL-2.1
# Wed, 11 Jan 2023 03:07:37 GMT
RUN apt-get update &&   apt-get --no-install-recommends -y install     curl     libreoffice     unzip     procps &&   rm -rf /var/lib/apt/lists/*
# Wed, 01 Feb 2023 22:26:19 GMT
ENV XWIKI_VERSION=14.10.4
# Wed, 01 Feb 2023 22:26:19 GMT
ENV XWIKI_URL_PREFIX=https://maven.xwiki.org/releases/org/xwiki/platform/xwiki-platform-distribution-war/14.10.4
# Wed, 01 Feb 2023 22:26:19 GMT
ENV XWIKI_DOWNLOAD_SHA256=2fcfb622319172c2e424b9c11848ebfabe27cf8ef69cba39ceb5d124b7ebe713
# Wed, 01 Feb 2023 22:27:00 GMT
RUN rm -rf /usr/local/tomcat/webapps/* &&   mkdir -p /usr/local/tomcat/temp &&   mkdir -p /usr/local/xwiki/data &&   curl -fSL "${XWIKI_URL_PREFIX}/xwiki-platform-distribution-war-${XWIKI_VERSION}.war" -o xwiki.war &&   echo "$XWIKI_DOWNLOAD_SHA256 xwiki.war" | sha256sum -c - &&   unzip -d /usr/local/tomcat/webapps/ROOT xwiki.war &&   rm -f xwiki.war
# Wed, 01 Feb 2023 22:27:03 GMT
ENV MYSQL_JDBC_VERSION=8.0.31
# Wed, 01 Feb 2023 22:27:03 GMT
ENV MYSQL_JDBC_SHA256=5249e3dc6d6531b37790e3f61845b96db5e41e891d3d8edb0e2e3a1b53ca2f4f
# Wed, 01 Feb 2023 22:27:03 GMT
ENV MYSQL_JDBC_PREFIX=https://repo1.maven.org/maven2/com/mysql/mysql-connector-j/8.0.31
# Wed, 01 Feb 2023 22:27:03 GMT
ENV MYSQL_JDBC_ARTIFACT=mysql-connector-j-8.0.31.jar
# Wed, 01 Feb 2023 22:27:03 GMT
ENV MYSQL_JDBC_TARGET=/usr/local/tomcat/webapps/ROOT/WEB-INF/lib/mysql-connector-j-8.0.31.jar
# Wed, 01 Feb 2023 22:27:04 GMT
RUN curl -fSL "${MYSQL_JDBC_PREFIX}/${MYSQL_JDBC_ARTIFACT}" -o $MYSQL_JDBC_TARGET &&   echo "$MYSQL_JDBC_SHA256 $MYSQL_JDBC_TARGET" | sha256sum -c -
# Wed, 01 Feb 2023 22:27:04 GMT
COPY file:0a1be11e2eb610a1dbcd415404e3a592641110b93090030cb831e3a19a163017 in /usr/local/tomcat/bin/ 
# Wed, 01 Feb 2023 22:27:04 GMT
COPY file:1b8409986f3e4eb79a7a0b18472cb2692a61d504fb5ef34292bc997b79fd760d in /usr/local/tomcat/webapps/ROOT/WEB-INF/hibernate.cfg.xml 
# Wed, 01 Feb 2023 22:27:05 GMT
RUN sed -i 's/<id>org.xwiki.platform:xwiki-platform-distribution-war/<id>org.xwiki.platform:xwiki-platform-distribution-docker/'   /usr/local/tomcat/webapps/ROOT/META-INF/extension.xed
# Wed, 01 Feb 2023 22:27:05 GMT
COPY file:a47c4dcd87c9dad97aff38c49188357e6193bcad50757e516cfb08a60d4de611 in /usr/local/bin/docker-entrypoint.sh 
# Wed, 01 Feb 2023 22:27:05 GMT
VOLUME [/usr/local/xwiki]
# Wed, 01 Feb 2023 22:27:05 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 01 Feb 2023 22:27:05 GMT
CMD ["xwiki"]
```

-	Layers:
	-	`sha256:0509fae36eb0656f8bdb23f8ae64100d893bcea2563e97468d337e04d2d0410b`  
		Last Modified: Wed, 02 Nov 2022 18:50:21 GMT  
		Size: 28.4 MB (28382154 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e502a1af2bcd98f5f0d2f5e4da1a0e7bbe07a2c548e2662f7d37dce5ae1df46c`  
		Last Modified: Wed, 02 Nov 2022 19:48:28 GMT  
		Size: 12.4 MB (12396330 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bc4598c07dd818f03a0378b0341a4a8e80f0152fbb3e7d5246ca4f466f42e611`  
		Last Modified: Fri, 04 Nov 2022 22:46:46 GMT  
		Size: 45.0 MB (44958470 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:715a937a1066f998b331fcd62256ad01a5571bdf46804e97825afc64f9ebb427`  
		Last Modified: Fri, 04 Nov 2022 22:46:41 GMT  
		Size: 160.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5fb623f082f74b2fa9fc2c4e3f3a4802875cb9753cfa26ed940201ce72bb56cb`  
		Last Modified: Sat, 05 Nov 2022 00:03:40 GMT  
		Size: 172.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:33260b83200262bbd546be371ad3c1f50f5ae7228afb87982d6fa9d6b11bf26f`  
		Last Modified: Tue, 15 Nov 2022 05:10:19 GMT  
		Size: 12.2 MB (12207235 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0955fb697ea9b30a1b4f95385464f646aa1525cb6efba648e22df84ebef6b2ee`  
		Last Modified: Tue, 15 Nov 2022 05:10:18 GMT  
		Size: 452.0 KB (452021 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6eddcf66f2083b1487296a0308e0b058917c97f614f12428d82d89662038dc2e`  
		Last Modified: Tue, 15 Nov 2022 05:10:18 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ae5f60bb64f3fa11da3d15a9639f886186b4c2c021455c3f9db22e0cfe1b1311`  
		Last Modified: Wed, 11 Jan 2023 03:11:14 GMT  
		Size: 173.8 MB (173806827 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:13334e257ce7313ca9d6028534e3ec6c7858c374c4afedea7f96c51da716806e`  
		Last Modified: Wed, 01 Feb 2023 22:29:16 GMT  
		Size: 307.1 MB (307104849 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ccb59878c7670194b75b6af22dd3908f9ae1a12dc1074f0b5ed156a5e3afdf0a`  
		Last Modified: Wed, 01 Feb 2023 22:29:02 GMT  
		Size: 2.4 MB (2377177 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d3946fb25102529cda96bcad4925905c9b997e442b447675d89066505cbe1026`  
		Last Modified: Wed, 01 Feb 2023 22:29:02 GMT  
		Size: 1.3 KB (1344 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1ba832da71f2ed07bae5269bb37e7ea79724a069ad63032f2af14996893baa37`  
		Last Modified: Wed, 01 Feb 2023 22:29:02 GMT  
		Size: 2.3 KB (2307 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6616193191331001a42a5d452ea69a215bbc414eca5cb00914c359665be5817f`  
		Last Modified: Wed, 01 Feb 2023 22:29:02 GMT  
		Size: 6.0 KB (6009 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6de4b8ce214cd9b76eda5b4955e5abb249a0b0292e8a38d39683e3002d6534bf`  
		Last Modified: Wed, 01 Feb 2023 22:29:03 GMT  
		Size: 2.5 KB (2506 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `xwiki:lts-mysql-tomcat`

```console
$ docker pull xwiki@sha256:32e51c9775fda50082b0f02856f2af444a67284446679c9a3a13a78c02ec0c4b
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `xwiki:lts-mysql-tomcat` - linux; amd64

```console
$ docker pull xwiki@sha256:a2e996a399fc68cbccfe11eaeb0115a15314bd69f06c483fef3cba244fa07cbf
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **590.4 MB (590449604 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:6b73fd725d5c1dd8044289fdb0e76f973e7e1d4a64e1efc44428235a718b550a`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["xwiki"]`

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
# Wed, 02 Nov 2022 18:44:10 GMT
RUN apt-get update     && DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends tzdata curl wget ca-certificates fontconfig locales     && echo "en_US.UTF-8 UTF-8" >> /etc/locale.gen     && locale-gen en_US.UTF-8     && rm -rf /var/lib/apt/lists/*
# Fri, 04 Nov 2022 23:21:41 GMT
ENV JAVA_VERSION=jdk-11.0.17+8
# Fri, 04 Nov 2022 23:22:31 GMT
RUN set -eux;     ARCH="$(dpkg --print-architecture)";     case "${ARCH}" in        aarch64|arm64)          ESUM='bd6efe3290c8b5a42f695a55a26f3e3c9c284288574879d4b7089f31f5114177';          BINARY_URL='https://github.com/adoptium/temurin11-binaries/releases/download/jdk-11.0.17%2B8/OpenJDK11U-jre_aarch64_linux_hotspot_11.0.17_8.tar.gz';          ;;        armhf|arm)          ESUM='8cf113d3d7fa808895c8d2e41bb890af21c47e38c2460e0588147a4bb8fc658d';          BINARY_URL='https://github.com/adoptium/temurin11-binaries/releases/download/jdk-11.0.17%2B8/OpenJDK11U-jre_arm_linux_hotspot_11.0.17_8.tar.gz';          ;;        ppc64el|powerpc:common64)          ESUM='0ca3d806131ab5834c501f9c625bb0248cd528af361c704503348e9c9605bedf';          BINARY_URL='https://github.com/adoptium/temurin11-binaries/releases/download/jdk-11.0.17%2B8/OpenJDK11U-jre_ppc64le_linux_hotspot_11.0.17_8.tar.gz';          ;;        s390x|s390:64-bit)          ESUM='dd3b159a374086e65cb07c4ccb226c90f9c02ef929cba6f0b642171d7ed97fa4';          BINARY_URL='https://github.com/adoptium/temurin11-binaries/releases/download/jdk-11.0.17%2B8/OpenJDK11U-jre_s390x_linux_hotspot_11.0.17_8.tar.gz';          ;;        amd64|i386:x86-64)          ESUM='752616097e09d7f60a3ad8bd312f90eaf50ac72577e55df229fe6e8091148f79';          BINARY_URL='https://github.com/adoptium/temurin11-binaries/releases/download/jdk-11.0.17%2B8/OpenJDK11U-jre_x64_linux_hotspot_11.0.17_8.tar.gz';          ;;        *)          echo "Unsupported arch: ${ARCH}";          exit 1;          ;;     esac; 	  wget -O /tmp/openjdk.tar.gz ${BINARY_URL}; 	  echo "${ESUM} */tmp/openjdk.tar.gz" | sha256sum -c -; 	  mkdir -p "$JAVA_HOME"; 	  tar --extract 	      --file /tmp/openjdk.tar.gz 	      --directory "$JAVA_HOME" 	      --strip-components 1 	      --no-same-owner 	  ;     rm /tmp/openjdk.tar.gz;     find "$JAVA_HOME/lib" -name '*.so' -exec dirname '{}' ';' | sort -u > /etc/ld.so.conf.d/docker-openjdk.conf;     ldconfig;     java -Xshare:dump;
# Fri, 04 Nov 2022 23:22:32 GMT
RUN echo Verifying install ...     && fileEncoding="$(echo 'System.out.println(System.getProperty("file.encoding"))' | jshell -s -)"; [ "$fileEncoding" = 'UTF-8' ]; rm -rf ~/.java     && echo java --version && java --version     && echo Complete.
# Sat, 05 Nov 2022 01:35:16 GMT
ENV CATALINA_HOME=/usr/local/tomcat
# Sat, 05 Nov 2022 01:35:16 GMT
ENV PATH=/usr/local/tomcat/bin:/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Sat, 05 Nov 2022 01:35:17 GMT
RUN mkdir -p "$CATALINA_HOME"
# Sat, 05 Nov 2022 01:35:17 GMT
WORKDIR /usr/local/tomcat
# Sat, 05 Nov 2022 01:35:17 GMT
ENV TOMCAT_NATIVE_LIBDIR=/usr/local/tomcat/native-jni-lib
# Sat, 05 Nov 2022 01:35:17 GMT
ENV LD_LIBRARY_PATH=/usr/local/tomcat/native-jni-lib
# Sat, 05 Nov 2022 01:39:54 GMT
ENV GPG_KEYS=48F8E69F6390C9F25CFEDCD268248959359E722B A9C5DF4D22E99998D9875A5110C01C5A2F6059E7 DCFD35E0BF8CA7344752DE8B6FB21E8933C60243
# Sat, 05 Nov 2022 01:39:54 GMT
ENV TOMCAT_MAJOR=9
# Tue, 15 Nov 2022 03:06:43 GMT
ENV TOMCAT_VERSION=9.0.69
# Tue, 15 Nov 2022 03:06:43 GMT
ENV TOMCAT_SHA512=8c883c54ce9ce43eba37756a6404cdf3477879883a3e6d146dc8a7aa5e0425f487466afe6b6da4a895927cb7cb59177b9379cec18000f2de12785be57408c779
# Tue, 15 Nov 2022 03:06:44 GMT
COPY dir:b1a33aa3993dbbfbebb33bd9aa546b60c2f2191abf1227f453d4e830f6deb35f in /usr/local/tomcat 
# Tue, 15 Nov 2022 03:06:48 GMT
RUN set -eux; 	apt-get update; 	xargs -rt apt-get install -y --no-install-recommends < "$TOMCAT_NATIVE_LIBDIR/.dependencies.txt"; 	rm -rf /var/lib/apt/lists/*
# Tue, 15 Nov 2022 03:06:49 GMT
RUN set -eux; 	nativeLines="$(catalina.sh configtest 2>&1)"; 	nativeLines="$(echo "$nativeLines" | grep 'Apache Tomcat Native')"; 	nativeLines="$(echo "$nativeLines" | sort -u)"; 	if ! echo "$nativeLines" | grep -E 'INFO: Loaded( APR based)? Apache Tomcat Native library' >&2; then 		echo >&2 "$nativeLines"; 		exit 1; 	fi
# Tue, 15 Nov 2022 03:06:49 GMT
EXPOSE 8080
# Tue, 15 Nov 2022 03:06:49 GMT
CMD ["catalina.sh" "run"]
# Wed, 11 Jan 2023 02:47:03 GMT
LABEL org.opencontainers.image.authors=XWiki Development Team <committers@xwiki.org>
# Wed, 11 Jan 2023 02:47:03 GMT
LABEL org.opencontainers.image.url=https://hub.docker.com/_/xwiki
# Wed, 11 Jan 2023 02:47:03 GMT
LABEL org.opencontainers.image.documentation=https://hub.docker.com/_/xwiki
# Wed, 11 Jan 2023 02:47:03 GMT
LABEL org.opencontainers.image.source=https://github.com/xwiki/xwiki-docker.git
# Wed, 11 Jan 2023 02:47:04 GMT
LABEL org.opencontainers.image.vendor=xwiki.org
# Wed, 11 Jan 2023 02:47:04 GMT
LABEL org.opencontainers.image.licenses=LGPL-2.1
# Wed, 11 Jan 2023 02:49:03 GMT
RUN apt-get update &&   apt-get --no-install-recommends -y install     curl     libreoffice     unzip     procps &&   rm -rf /var/lib/apt/lists/*
# Wed, 22 Feb 2023 18:39:36 GMT
ENV XWIKI_VERSION=14.10.5
# Wed, 22 Feb 2023 18:39:36 GMT
ENV XWIKI_URL_PREFIX=https://maven.xwiki.org/releases/org/xwiki/platform/xwiki-platform-distribution-war/14.10.5
# Wed, 22 Feb 2023 18:39:36 GMT
ENV XWIKI_DOWNLOAD_SHA256=f58465d0869e4c5605ae8375a09c79399d1149c7131fed3cf9959918267eb6a8
# Wed, 22 Feb 2023 18:40:15 GMT
RUN rm -rf /usr/local/tomcat/webapps/* &&   mkdir -p /usr/local/tomcat/temp &&   mkdir -p /usr/local/xwiki/data &&   curl -fSL "${XWIKI_URL_PREFIX}/xwiki-platform-distribution-war-${XWIKI_VERSION}.war" -o xwiki.war &&   echo "$XWIKI_DOWNLOAD_SHA256 xwiki.war" | sha256sum -c - &&   unzip -d /usr/local/tomcat/webapps/ROOT xwiki.war &&   rm -f xwiki.war
# Wed, 22 Feb 2023 18:40:17 GMT
ENV MYSQL_JDBC_VERSION=8.0.32
# Wed, 22 Feb 2023 18:40:17 GMT
ENV MYSQL_JDBC_SHA256=522329fe925980f02e5eb89b59d227245d345415ff0c08932a68c9765c13acc5
# Wed, 22 Feb 2023 18:40:17 GMT
ENV MYSQL_JDBC_PREFIX=https://repo1.maven.org/maven2/com/mysql/mysql-connector-j/8.0.32
# Wed, 22 Feb 2023 18:40:17 GMT
ENV MYSQL_JDBC_ARTIFACT=mysql-connector-j-8.0.32.jar
# Wed, 22 Feb 2023 18:40:17 GMT
ENV MYSQL_JDBC_TARGET=/usr/local/tomcat/webapps/ROOT/WEB-INF/lib/mysql-connector-j-8.0.32.jar
# Wed, 22 Feb 2023 18:40:18 GMT
RUN curl -fSL "${MYSQL_JDBC_PREFIX}/${MYSQL_JDBC_ARTIFACT}" -o $MYSQL_JDBC_TARGET &&   echo "$MYSQL_JDBC_SHA256 $MYSQL_JDBC_TARGET" | sha256sum -c -
# Wed, 22 Feb 2023 18:40:18 GMT
COPY file:0a1be11e2eb610a1dbcd415404e3a592641110b93090030cb831e3a19a163017 in /usr/local/tomcat/bin/ 
# Wed, 22 Feb 2023 18:40:18 GMT
COPY file:1b8409986f3e4eb79a7a0b18472cb2692a61d504fb5ef34292bc997b79fd760d in /usr/local/tomcat/webapps/ROOT/WEB-INF/hibernate.cfg.xml 
# Wed, 22 Feb 2023 18:40:19 GMT
RUN sed -i 's/<id>org.xwiki.platform:xwiki-platform-distribution-war/<id>org.xwiki.platform:xwiki-platform-distribution-docker/'   /usr/local/tomcat/webapps/ROOT/META-INF/extension.xed
# Wed, 22 Feb 2023 18:40:19 GMT
COPY file:a47c4dcd87c9dad97aff38c49188357e6193bcad50757e516cfb08a60d4de611 in /usr/local/bin/docker-entrypoint.sh 
# Wed, 22 Feb 2023 18:40:19 GMT
VOLUME [/usr/local/xwiki]
# Wed, 22 Feb 2023 18:40:19 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 22 Feb 2023 18:40:19 GMT
CMD ["xwiki"]
```

-	Layers:
	-	`sha256:e96e057aae67380a4ddb16c337c5c3669d97fdff69ec537f02aa2cc30d814281`  
		Last Modified: Wed, 02 Nov 2022 03:03:36 GMT  
		Size: 30.4 MB (30425607 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4ced2591451da3a02e2b6bb44752b9e3f00d77789921be4df5082fb9f9880ad0`  
		Last Modified: Wed, 02 Nov 2022 18:48:43 GMT  
		Size: 12.4 MB (12439006 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:df8f874ae8c08a9e69e5fbe6c5a64200a45386132a3203d1a9a7f1146d94cfbc`  
		Last Modified: Fri, 04 Nov 2022 23:29:33 GMT  
		Size: 46.6 MB (46629936 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:111b6c7486426c4b6989102c2ee5be856e8a58e20ab0a350b24a905d536e8e7f`  
		Last Modified: Fri, 04 Nov 2022 23:29:26 GMT  
		Size: 161.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e6f84dce457c6d4f7b7291fce05f8e77998a3a7722a54125a1f1d52ca83043b4`  
		Last Modified: Sat, 05 Nov 2022 01:50:51 GMT  
		Size: 173.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a6c26749ee782392e38845ee2ba79b0da586ef6a45d8e7f29c7af14612278547`  
		Last Modified: Tue, 15 Nov 2022 03:19:57 GMT  
		Size: 12.2 MB (12200249 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4dddc6d9fa6024025b3fcfe729cab2dc544fb25476eca6e80b1af8e8d93bb0ee`  
		Last Modified: Tue, 15 Nov 2022 03:19:56 GMT  
		Size: 452.7 KB (452680 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:06637eebe5e72c8ad9019ad4eb4cdde1f11f7d4c24c7ed7374cf8966343aa2fb`  
		Last Modified: Tue, 15 Nov 2022 03:19:56 GMT  
		Size: 131.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b276fb8390410a8208724033e325715ea26000d5a1a762d4c3699b927884fbfe`  
		Last Modified: Wed, 11 Jan 2023 02:52:45 GMT  
		Size: 178.8 MB (178805608 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:89de9d9e2c09cd5b84430562516cbcd5695a0a3b2347b451e157bde75c2b5619`  
		Last Modified: Wed, 22 Feb 2023 18:42:21 GMT  
		Size: 307.1 MB (307141303 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4a2089179b7c1db514d0502e476e09b8f9313d08d4c4e4f3981be456288fe507`  
		Last Modified: Wed, 22 Feb 2023 18:42:04 GMT  
		Size: 2.3 MB (2342572 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e7c4ef360ff3673244adb3dfc4769b5710fa68fcc1fbe1c08b2f5fa32dbd4976`  
		Last Modified: Wed, 22 Feb 2023 18:42:04 GMT  
		Size: 1.3 KB (1348 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:08441c368d4b01e361491d7fbf1ac579fcc303b8484123c309a8d5a3b6657c46`  
		Last Modified: Wed, 22 Feb 2023 18:42:04 GMT  
		Size: 2.3 KB (2311 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:542b4bb846d438395e458c08de292f72d14d289fae6ffe7eba6fec1cd8518475`  
		Last Modified: Wed, 22 Feb 2023 18:42:04 GMT  
		Size: 6.0 KB (6013 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:039c0305df9e64c69bb546e64f0658dba6e728eee13022cfd682aa1ee76b8b7f`  
		Last Modified: Wed, 22 Feb 2023 18:42:04 GMT  
		Size: 2.5 KB (2506 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `xwiki:lts-mysql-tomcat` - linux; arm64 variant v8

```console
$ docker pull xwiki@sha256:33e36167828fe9bae944e7d4cbbe3b69dd2415595d40610ac2ebcd73f2c2fa7f
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **581.7 MB (581697690 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:44013daf43fd09deb7221eef006c4d30d484a03c433118e5b59da0a44b573f06`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["xwiki"]`

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
# Wed, 02 Nov 2022 19:44:32 GMT
RUN apt-get update     && DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends tzdata curl wget ca-certificates fontconfig locales     && echo "en_US.UTF-8 UTF-8" >> /etc/locale.gen     && locale-gen en_US.UTF-8     && rm -rf /var/lib/apt/lists/*
# Fri, 04 Nov 2022 22:40:54 GMT
ENV JAVA_VERSION=jdk-11.0.17+8
# Fri, 04 Nov 2022 22:41:33 GMT
RUN set -eux;     ARCH="$(dpkg --print-architecture)";     case "${ARCH}" in        aarch64|arm64)          ESUM='bd6efe3290c8b5a42f695a55a26f3e3c9c284288574879d4b7089f31f5114177';          BINARY_URL='https://github.com/adoptium/temurin11-binaries/releases/download/jdk-11.0.17%2B8/OpenJDK11U-jre_aarch64_linux_hotspot_11.0.17_8.tar.gz';          ;;        armhf|arm)          ESUM='8cf113d3d7fa808895c8d2e41bb890af21c47e38c2460e0588147a4bb8fc658d';          BINARY_URL='https://github.com/adoptium/temurin11-binaries/releases/download/jdk-11.0.17%2B8/OpenJDK11U-jre_arm_linux_hotspot_11.0.17_8.tar.gz';          ;;        ppc64el|powerpc:common64)          ESUM='0ca3d806131ab5834c501f9c625bb0248cd528af361c704503348e9c9605bedf';          BINARY_URL='https://github.com/adoptium/temurin11-binaries/releases/download/jdk-11.0.17%2B8/OpenJDK11U-jre_ppc64le_linux_hotspot_11.0.17_8.tar.gz';          ;;        s390x|s390:64-bit)          ESUM='dd3b159a374086e65cb07c4ccb226c90f9c02ef929cba6f0b642171d7ed97fa4';          BINARY_URL='https://github.com/adoptium/temurin11-binaries/releases/download/jdk-11.0.17%2B8/OpenJDK11U-jre_s390x_linux_hotspot_11.0.17_8.tar.gz';          ;;        amd64|i386:x86-64)          ESUM='752616097e09d7f60a3ad8bd312f90eaf50ac72577e55df229fe6e8091148f79';          BINARY_URL='https://github.com/adoptium/temurin11-binaries/releases/download/jdk-11.0.17%2B8/OpenJDK11U-jre_x64_linux_hotspot_11.0.17_8.tar.gz';          ;;        *)          echo "Unsupported arch: ${ARCH}";          exit 1;          ;;     esac; 	  wget -O /tmp/openjdk.tar.gz ${BINARY_URL}; 	  echo "${ESUM} */tmp/openjdk.tar.gz" | sha256sum -c -; 	  mkdir -p "$JAVA_HOME"; 	  tar --extract 	      --file /tmp/openjdk.tar.gz 	      --directory "$JAVA_HOME" 	      --strip-components 1 	      --no-same-owner 	  ;     rm /tmp/openjdk.tar.gz;     find "$JAVA_HOME/lib" -name '*.so' -exec dirname '{}' ';' | sort -u > /etc/ld.so.conf.d/docker-openjdk.conf;     ldconfig;     java -Xshare:dump;
# Fri, 04 Nov 2022 22:41:34 GMT
RUN echo Verifying install ...     && fileEncoding="$(echo 'System.out.println(System.getProperty("file.encoding"))' | jshell -s -)"; [ "$fileEncoding" = 'UTF-8' ]; rm -rf ~/.java     && echo java --version && java --version     && echo Complete.
# Fri, 04 Nov 2022 23:48:38 GMT
ENV CATALINA_HOME=/usr/local/tomcat
# Fri, 04 Nov 2022 23:48:38 GMT
ENV PATH=/usr/local/tomcat/bin:/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Fri, 04 Nov 2022 23:48:38 GMT
RUN mkdir -p "$CATALINA_HOME"
# Fri, 04 Nov 2022 23:48:39 GMT
WORKDIR /usr/local/tomcat
# Fri, 04 Nov 2022 23:48:39 GMT
ENV TOMCAT_NATIVE_LIBDIR=/usr/local/tomcat/native-jni-lib
# Fri, 04 Nov 2022 23:48:39 GMT
ENV LD_LIBRARY_PATH=/usr/local/tomcat/native-jni-lib
# Fri, 04 Nov 2022 23:53:12 GMT
ENV GPG_KEYS=48F8E69F6390C9F25CFEDCD268248959359E722B A9C5DF4D22E99998D9875A5110C01C5A2F6059E7 DCFD35E0BF8CA7344752DE8B6FB21E8933C60243
# Fri, 04 Nov 2022 23:53:12 GMT
ENV TOMCAT_MAJOR=9
# Tue, 15 Nov 2022 04:57:22 GMT
ENV TOMCAT_VERSION=9.0.69
# Tue, 15 Nov 2022 04:57:22 GMT
ENV TOMCAT_SHA512=8c883c54ce9ce43eba37756a6404cdf3477879883a3e6d146dc8a7aa5e0425f487466afe6b6da4a895927cb7cb59177b9379cec18000f2de12785be57408c779
# Tue, 15 Nov 2022 04:57:22 GMT
COPY dir:096b403a5f78b17e6b4bff63128a9c93941b97f22470991610dd641633d977f1 in /usr/local/tomcat 
# Tue, 15 Nov 2022 04:57:25 GMT
RUN set -eux; 	apt-get update; 	xargs -rt apt-get install -y --no-install-recommends < "$TOMCAT_NATIVE_LIBDIR/.dependencies.txt"; 	rm -rf /var/lib/apt/lists/*
# Tue, 15 Nov 2022 04:57:26 GMT
RUN set -eux; 	nativeLines="$(catalina.sh configtest 2>&1)"; 	nativeLines="$(echo "$nativeLines" | grep 'Apache Tomcat Native')"; 	nativeLines="$(echo "$nativeLines" | sort -u)"; 	if ! echo "$nativeLines" | grep -E 'INFO: Loaded( APR based)? Apache Tomcat Native library' >&2; then 		echo >&2 "$nativeLines"; 		exit 1; 	fi
# Tue, 15 Nov 2022 04:57:26 GMT
EXPOSE 8080
# Tue, 15 Nov 2022 04:57:27 GMT
CMD ["catalina.sh" "run"]
# Wed, 11 Jan 2023 03:05:10 GMT
LABEL org.opencontainers.image.authors=XWiki Development Team <committers@xwiki.org>
# Wed, 11 Jan 2023 03:05:10 GMT
LABEL org.opencontainers.image.url=https://hub.docker.com/_/xwiki
# Wed, 11 Jan 2023 03:05:10 GMT
LABEL org.opencontainers.image.documentation=https://hub.docker.com/_/xwiki
# Wed, 11 Jan 2023 03:05:10 GMT
LABEL org.opencontainers.image.source=https://github.com/xwiki/xwiki-docker.git
# Wed, 11 Jan 2023 03:05:11 GMT
LABEL org.opencontainers.image.vendor=xwiki.org
# Wed, 11 Jan 2023 03:05:11 GMT
LABEL org.opencontainers.image.licenses=LGPL-2.1
# Wed, 11 Jan 2023 03:07:37 GMT
RUN apt-get update &&   apt-get --no-install-recommends -y install     curl     libreoffice     unzip     procps &&   rm -rf /var/lib/apt/lists/*
# Wed, 01 Feb 2023 22:26:19 GMT
ENV XWIKI_VERSION=14.10.4
# Wed, 01 Feb 2023 22:26:19 GMT
ENV XWIKI_URL_PREFIX=https://maven.xwiki.org/releases/org/xwiki/platform/xwiki-platform-distribution-war/14.10.4
# Wed, 01 Feb 2023 22:26:19 GMT
ENV XWIKI_DOWNLOAD_SHA256=2fcfb622319172c2e424b9c11848ebfabe27cf8ef69cba39ceb5d124b7ebe713
# Wed, 01 Feb 2023 22:27:00 GMT
RUN rm -rf /usr/local/tomcat/webapps/* &&   mkdir -p /usr/local/tomcat/temp &&   mkdir -p /usr/local/xwiki/data &&   curl -fSL "${XWIKI_URL_PREFIX}/xwiki-platform-distribution-war-${XWIKI_VERSION}.war" -o xwiki.war &&   echo "$XWIKI_DOWNLOAD_SHA256 xwiki.war" | sha256sum -c - &&   unzip -d /usr/local/tomcat/webapps/ROOT xwiki.war &&   rm -f xwiki.war
# Wed, 01 Feb 2023 22:27:03 GMT
ENV MYSQL_JDBC_VERSION=8.0.31
# Wed, 01 Feb 2023 22:27:03 GMT
ENV MYSQL_JDBC_SHA256=5249e3dc6d6531b37790e3f61845b96db5e41e891d3d8edb0e2e3a1b53ca2f4f
# Wed, 01 Feb 2023 22:27:03 GMT
ENV MYSQL_JDBC_PREFIX=https://repo1.maven.org/maven2/com/mysql/mysql-connector-j/8.0.31
# Wed, 01 Feb 2023 22:27:03 GMT
ENV MYSQL_JDBC_ARTIFACT=mysql-connector-j-8.0.31.jar
# Wed, 01 Feb 2023 22:27:03 GMT
ENV MYSQL_JDBC_TARGET=/usr/local/tomcat/webapps/ROOT/WEB-INF/lib/mysql-connector-j-8.0.31.jar
# Wed, 01 Feb 2023 22:27:04 GMT
RUN curl -fSL "${MYSQL_JDBC_PREFIX}/${MYSQL_JDBC_ARTIFACT}" -o $MYSQL_JDBC_TARGET &&   echo "$MYSQL_JDBC_SHA256 $MYSQL_JDBC_TARGET" | sha256sum -c -
# Wed, 01 Feb 2023 22:27:04 GMT
COPY file:0a1be11e2eb610a1dbcd415404e3a592641110b93090030cb831e3a19a163017 in /usr/local/tomcat/bin/ 
# Wed, 01 Feb 2023 22:27:04 GMT
COPY file:1b8409986f3e4eb79a7a0b18472cb2692a61d504fb5ef34292bc997b79fd760d in /usr/local/tomcat/webapps/ROOT/WEB-INF/hibernate.cfg.xml 
# Wed, 01 Feb 2023 22:27:05 GMT
RUN sed -i 's/<id>org.xwiki.platform:xwiki-platform-distribution-war/<id>org.xwiki.platform:xwiki-platform-distribution-docker/'   /usr/local/tomcat/webapps/ROOT/META-INF/extension.xed
# Wed, 01 Feb 2023 22:27:05 GMT
COPY file:a47c4dcd87c9dad97aff38c49188357e6193bcad50757e516cfb08a60d4de611 in /usr/local/bin/docker-entrypoint.sh 
# Wed, 01 Feb 2023 22:27:05 GMT
VOLUME [/usr/local/xwiki]
# Wed, 01 Feb 2023 22:27:05 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 01 Feb 2023 22:27:05 GMT
CMD ["xwiki"]
```

-	Layers:
	-	`sha256:0509fae36eb0656f8bdb23f8ae64100d893bcea2563e97468d337e04d2d0410b`  
		Last Modified: Wed, 02 Nov 2022 18:50:21 GMT  
		Size: 28.4 MB (28382154 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e502a1af2bcd98f5f0d2f5e4da1a0e7bbe07a2c548e2662f7d37dce5ae1df46c`  
		Last Modified: Wed, 02 Nov 2022 19:48:28 GMT  
		Size: 12.4 MB (12396330 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bc4598c07dd818f03a0378b0341a4a8e80f0152fbb3e7d5246ca4f466f42e611`  
		Last Modified: Fri, 04 Nov 2022 22:46:46 GMT  
		Size: 45.0 MB (44958470 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:715a937a1066f998b331fcd62256ad01a5571bdf46804e97825afc64f9ebb427`  
		Last Modified: Fri, 04 Nov 2022 22:46:41 GMT  
		Size: 160.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5fb623f082f74b2fa9fc2c4e3f3a4802875cb9753cfa26ed940201ce72bb56cb`  
		Last Modified: Sat, 05 Nov 2022 00:03:40 GMT  
		Size: 172.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:33260b83200262bbd546be371ad3c1f50f5ae7228afb87982d6fa9d6b11bf26f`  
		Last Modified: Tue, 15 Nov 2022 05:10:19 GMT  
		Size: 12.2 MB (12207235 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0955fb697ea9b30a1b4f95385464f646aa1525cb6efba648e22df84ebef6b2ee`  
		Last Modified: Tue, 15 Nov 2022 05:10:18 GMT  
		Size: 452.0 KB (452021 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6eddcf66f2083b1487296a0308e0b058917c97f614f12428d82d89662038dc2e`  
		Last Modified: Tue, 15 Nov 2022 05:10:18 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ae5f60bb64f3fa11da3d15a9639f886186b4c2c021455c3f9db22e0cfe1b1311`  
		Last Modified: Wed, 11 Jan 2023 03:11:14 GMT  
		Size: 173.8 MB (173806827 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:13334e257ce7313ca9d6028534e3ec6c7858c374c4afedea7f96c51da716806e`  
		Last Modified: Wed, 01 Feb 2023 22:29:16 GMT  
		Size: 307.1 MB (307104849 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ccb59878c7670194b75b6af22dd3908f9ae1a12dc1074f0b5ed156a5e3afdf0a`  
		Last Modified: Wed, 01 Feb 2023 22:29:02 GMT  
		Size: 2.4 MB (2377177 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d3946fb25102529cda96bcad4925905c9b997e442b447675d89066505cbe1026`  
		Last Modified: Wed, 01 Feb 2023 22:29:02 GMT  
		Size: 1.3 KB (1344 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1ba832da71f2ed07bae5269bb37e7ea79724a069ad63032f2af14996893baa37`  
		Last Modified: Wed, 01 Feb 2023 22:29:02 GMT  
		Size: 2.3 KB (2307 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6616193191331001a42a5d452ea69a215bbc414eca5cb00914c359665be5817f`  
		Last Modified: Wed, 01 Feb 2023 22:29:02 GMT  
		Size: 6.0 KB (6009 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6de4b8ce214cd9b76eda5b4955e5abb249a0b0292e8a38d39683e3002d6534bf`  
		Last Modified: Wed, 01 Feb 2023 22:29:03 GMT  
		Size: 2.5 KB (2506 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `xwiki:lts-postgres`

```console
$ docker pull xwiki@sha256:48a8c82a2dcfa36f6d55a5f3e75d3e2b3aca3f80de56276b35838dc7bcb6a4a6
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `xwiki:lts-postgres` - linux; amd64

```console
$ docker pull xwiki@sha256:5cd23e4200b4eed664a61d05e3d436d0e372a3e4e985e29cb866dd9dbb573713
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **590.0 MB (589983532 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ab0dc70572c5101e5837a6281e7cb29a2b4dbf26ad0b9c91860a748aeb3360e1`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["xwiki"]`

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
# Wed, 02 Nov 2022 18:44:10 GMT
RUN apt-get update     && DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends tzdata curl wget ca-certificates fontconfig locales     && echo "en_US.UTF-8 UTF-8" >> /etc/locale.gen     && locale-gen en_US.UTF-8     && rm -rf /var/lib/apt/lists/*
# Fri, 04 Nov 2022 23:21:41 GMT
ENV JAVA_VERSION=jdk-11.0.17+8
# Fri, 04 Nov 2022 23:22:31 GMT
RUN set -eux;     ARCH="$(dpkg --print-architecture)";     case "${ARCH}" in        aarch64|arm64)          ESUM='bd6efe3290c8b5a42f695a55a26f3e3c9c284288574879d4b7089f31f5114177';          BINARY_URL='https://github.com/adoptium/temurin11-binaries/releases/download/jdk-11.0.17%2B8/OpenJDK11U-jre_aarch64_linux_hotspot_11.0.17_8.tar.gz';          ;;        armhf|arm)          ESUM='8cf113d3d7fa808895c8d2e41bb890af21c47e38c2460e0588147a4bb8fc658d';          BINARY_URL='https://github.com/adoptium/temurin11-binaries/releases/download/jdk-11.0.17%2B8/OpenJDK11U-jre_arm_linux_hotspot_11.0.17_8.tar.gz';          ;;        ppc64el|powerpc:common64)          ESUM='0ca3d806131ab5834c501f9c625bb0248cd528af361c704503348e9c9605bedf';          BINARY_URL='https://github.com/adoptium/temurin11-binaries/releases/download/jdk-11.0.17%2B8/OpenJDK11U-jre_ppc64le_linux_hotspot_11.0.17_8.tar.gz';          ;;        s390x|s390:64-bit)          ESUM='dd3b159a374086e65cb07c4ccb226c90f9c02ef929cba6f0b642171d7ed97fa4';          BINARY_URL='https://github.com/adoptium/temurin11-binaries/releases/download/jdk-11.0.17%2B8/OpenJDK11U-jre_s390x_linux_hotspot_11.0.17_8.tar.gz';          ;;        amd64|i386:x86-64)          ESUM='752616097e09d7f60a3ad8bd312f90eaf50ac72577e55df229fe6e8091148f79';          BINARY_URL='https://github.com/adoptium/temurin11-binaries/releases/download/jdk-11.0.17%2B8/OpenJDK11U-jre_x64_linux_hotspot_11.0.17_8.tar.gz';          ;;        *)          echo "Unsupported arch: ${ARCH}";          exit 1;          ;;     esac; 	  wget -O /tmp/openjdk.tar.gz ${BINARY_URL}; 	  echo "${ESUM} */tmp/openjdk.tar.gz" | sha256sum -c -; 	  mkdir -p "$JAVA_HOME"; 	  tar --extract 	      --file /tmp/openjdk.tar.gz 	      --directory "$JAVA_HOME" 	      --strip-components 1 	      --no-same-owner 	  ;     rm /tmp/openjdk.tar.gz;     find "$JAVA_HOME/lib" -name '*.so' -exec dirname '{}' ';' | sort -u > /etc/ld.so.conf.d/docker-openjdk.conf;     ldconfig;     java -Xshare:dump;
# Fri, 04 Nov 2022 23:22:32 GMT
RUN echo Verifying install ...     && fileEncoding="$(echo 'System.out.println(System.getProperty("file.encoding"))' | jshell -s -)"; [ "$fileEncoding" = 'UTF-8' ]; rm -rf ~/.java     && echo java --version && java --version     && echo Complete.
# Sat, 05 Nov 2022 01:35:16 GMT
ENV CATALINA_HOME=/usr/local/tomcat
# Sat, 05 Nov 2022 01:35:16 GMT
ENV PATH=/usr/local/tomcat/bin:/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Sat, 05 Nov 2022 01:35:17 GMT
RUN mkdir -p "$CATALINA_HOME"
# Sat, 05 Nov 2022 01:35:17 GMT
WORKDIR /usr/local/tomcat
# Sat, 05 Nov 2022 01:35:17 GMT
ENV TOMCAT_NATIVE_LIBDIR=/usr/local/tomcat/native-jni-lib
# Sat, 05 Nov 2022 01:35:17 GMT
ENV LD_LIBRARY_PATH=/usr/local/tomcat/native-jni-lib
# Sat, 05 Nov 2022 01:39:54 GMT
ENV GPG_KEYS=48F8E69F6390C9F25CFEDCD268248959359E722B A9C5DF4D22E99998D9875A5110C01C5A2F6059E7 DCFD35E0BF8CA7344752DE8B6FB21E8933C60243
# Sat, 05 Nov 2022 01:39:54 GMT
ENV TOMCAT_MAJOR=9
# Tue, 15 Nov 2022 03:06:43 GMT
ENV TOMCAT_VERSION=9.0.69
# Tue, 15 Nov 2022 03:06:43 GMT
ENV TOMCAT_SHA512=8c883c54ce9ce43eba37756a6404cdf3477879883a3e6d146dc8a7aa5e0425f487466afe6b6da4a895927cb7cb59177b9379cec18000f2de12785be57408c779
# Tue, 15 Nov 2022 03:06:44 GMT
COPY dir:b1a33aa3993dbbfbebb33bd9aa546b60c2f2191abf1227f453d4e830f6deb35f in /usr/local/tomcat 
# Tue, 15 Nov 2022 03:06:48 GMT
RUN set -eux; 	apt-get update; 	xargs -rt apt-get install -y --no-install-recommends < "$TOMCAT_NATIVE_LIBDIR/.dependencies.txt"; 	rm -rf /var/lib/apt/lists/*
# Tue, 15 Nov 2022 03:06:49 GMT
RUN set -eux; 	nativeLines="$(catalina.sh configtest 2>&1)"; 	nativeLines="$(echo "$nativeLines" | grep 'Apache Tomcat Native')"; 	nativeLines="$(echo "$nativeLines" | sort -u)"; 	if ! echo "$nativeLines" | grep -E 'INFO: Loaded( APR based)? Apache Tomcat Native library' >&2; then 		echo >&2 "$nativeLines"; 		exit 1; 	fi
# Tue, 15 Nov 2022 03:06:49 GMT
EXPOSE 8080
# Tue, 15 Nov 2022 03:06:49 GMT
CMD ["catalina.sh" "run"]
# Wed, 11 Jan 2023 02:47:03 GMT
LABEL org.opencontainers.image.authors=XWiki Development Team <committers@xwiki.org>
# Wed, 11 Jan 2023 02:47:03 GMT
LABEL org.opencontainers.image.url=https://hub.docker.com/_/xwiki
# Wed, 11 Jan 2023 02:47:03 GMT
LABEL org.opencontainers.image.documentation=https://hub.docker.com/_/xwiki
# Wed, 11 Jan 2023 02:47:03 GMT
LABEL org.opencontainers.image.source=https://github.com/xwiki/xwiki-docker.git
# Wed, 11 Jan 2023 02:47:04 GMT
LABEL org.opencontainers.image.vendor=xwiki.org
# Wed, 11 Jan 2023 02:47:04 GMT
LABEL org.opencontainers.image.licenses=LGPL-2.1
# Wed, 11 Jan 2023 02:50:25 GMT
RUN apt-get update &&   apt-get --no-install-recommends -y install     curl     libreoffice     unzip     procps     libpostgresql-jdbc-java &&   rm -rf /var/lib/apt/lists/*
# Wed, 22 Feb 2023 18:40:25 GMT
ENV XWIKI_VERSION=14.10.5
# Wed, 22 Feb 2023 18:40:25 GMT
ENV XWIKI_URL_PREFIX=https://maven.xwiki.org/releases/org/xwiki/platform/xwiki-platform-distribution-war/14.10.5
# Wed, 22 Feb 2023 18:40:25 GMT
ENV XWIKI_DOWNLOAD_SHA256=f58465d0869e4c5605ae8375a09c79399d1149c7131fed3cf9959918267eb6a8
# Wed, 22 Feb 2023 18:41:04 GMT
RUN rm -rf /usr/local/tomcat/webapps/* &&   mkdir -p /usr/local/tomcat/temp &&   mkdir -p /usr/local/xwiki/data &&   curl -fSL "${XWIKI_URL_PREFIX}/xwiki-platform-distribution-war-${XWIKI_VERSION}.war" -o xwiki.war &&   echo "$XWIKI_DOWNLOAD_SHA256 xwiki.war" | sha256sum -c - &&   unzip -d /usr/local/tomcat/webapps/ROOT xwiki.war &&   rm -f xwiki.war
# Wed, 22 Feb 2023 18:41:05 GMT
RUN cp /usr/share/java/postgresql-jdbc4.jar /usr/local/tomcat/webapps/ROOT/WEB-INF/lib/
# Wed, 22 Feb 2023 18:41:05 GMT
COPY file:0a1be11e2eb610a1dbcd415404e3a592641110b93090030cb831e3a19a163017 in /usr/local/tomcat/bin/ 
# Wed, 22 Feb 2023 18:41:05 GMT
COPY file:4a923f484bb29a26630c19e1d617d3bf6aa6ae7c6c4a5561e97b037bcde0847c in /usr/local/tomcat/webapps/ROOT/WEB-INF/hibernate.cfg.xml 
# Wed, 22 Feb 2023 18:41:06 GMT
RUN sed -i 's/<id>org.xwiki.platform:xwiki-platform-distribution-war/<id>org.xwiki.platform:xwiki-platform-distribution-docker/'   /usr/local/tomcat/webapps/ROOT/META-INF/extension.xed
# Wed, 22 Feb 2023 18:41:06 GMT
COPY file:a47c4dcd87c9dad97aff38c49188357e6193bcad50757e516cfb08a60d4de611 in /usr/local/bin/docker-entrypoint.sh 
# Wed, 22 Feb 2023 18:41:06 GMT
VOLUME [/usr/local/xwiki]
# Wed, 22 Feb 2023 18:41:06 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 22 Feb 2023 18:41:06 GMT
CMD ["xwiki"]
```

-	Layers:
	-	`sha256:e96e057aae67380a4ddb16c337c5c3669d97fdff69ec537f02aa2cc30d814281`  
		Last Modified: Wed, 02 Nov 2022 03:03:36 GMT  
		Size: 30.4 MB (30425607 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4ced2591451da3a02e2b6bb44752b9e3f00d77789921be4df5082fb9f9880ad0`  
		Last Modified: Wed, 02 Nov 2022 18:48:43 GMT  
		Size: 12.4 MB (12439006 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:df8f874ae8c08a9e69e5fbe6c5a64200a45386132a3203d1a9a7f1146d94cfbc`  
		Last Modified: Fri, 04 Nov 2022 23:29:33 GMT  
		Size: 46.6 MB (46629936 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:111b6c7486426c4b6989102c2ee5be856e8a58e20ab0a350b24a905d536e8e7f`  
		Last Modified: Fri, 04 Nov 2022 23:29:26 GMT  
		Size: 161.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e6f84dce457c6d4f7b7291fce05f8e77998a3a7722a54125a1f1d52ca83043b4`  
		Last Modified: Sat, 05 Nov 2022 01:50:51 GMT  
		Size: 173.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a6c26749ee782392e38845ee2ba79b0da586ef6a45d8e7f29c7af14612278547`  
		Last Modified: Tue, 15 Nov 2022 03:19:57 GMT  
		Size: 12.2 MB (12200249 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4dddc6d9fa6024025b3fcfe729cab2dc544fb25476eca6e80b1af8e8d93bb0ee`  
		Last Modified: Tue, 15 Nov 2022 03:19:56 GMT  
		Size: 452.7 KB (452680 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:06637eebe5e72c8ad9019ad4eb4cdde1f11f7d4c24c7ed7374cf8966343aa2fb`  
		Last Modified: Tue, 15 Nov 2022 03:19:56 GMT  
		Size: 131.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b57f6f8bcfb0d93b8e21d3068d1f65d3f08dba05c5fab7d4c36e2359317b18c7`  
		Last Modified: Wed, 11 Jan 2023 02:53:53 GMT  
		Size: 179.7 MB (179745182 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b26b00a2f6717a934b9a1b08bac612aaaf57a4cfb4d82db521e7d36755621933`  
		Last Modified: Wed, 22 Feb 2023 18:43:06 GMT  
		Size: 307.1 MB (307141251 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:11801aa48fd913e3278b4d0a512df366a8ef26c1cc3e95a8439a1be90aadfd5a`  
		Last Modified: Wed, 22 Feb 2023 18:42:50 GMT  
		Size: 936.9 KB (936850 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fb4e8755162307a316ff405759f2417dc77e746651f89c83a0477ab19dc7da5d`  
		Last Modified: Wed, 22 Feb 2023 18:42:50 GMT  
		Size: 1.3 KB (1342 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2ba124a3d49367a8e2f46fc2043189f91e2dd282d40a301d9c1f79a705d35e66`  
		Last Modified: Wed, 22 Feb 2023 18:42:50 GMT  
		Size: 2.5 KB (2450 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8f421201132c3966dbb37a473df5922718780304fa03993ef75bb78522d5cafd`  
		Last Modified: Wed, 22 Feb 2023 18:42:50 GMT  
		Size: 6.0 KB (6012 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1b5dc6b32b3d1d9a80058f5ffc684363a0cfadf60ade5875fa37854ec7b46fff`  
		Last Modified: Wed, 22 Feb 2023 18:42:50 GMT  
		Size: 2.5 KB (2502 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `xwiki:lts-postgres` - linux; arm64 variant v8

```console
$ docker pull xwiki@sha256:e04b6d052b479b648834e5d960deff2f28274834a9dc812b628ccb9a624c53ef
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **581.2 MB (581199952 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:4693188024e4d84ad63e783e3377e2d600a040c344f7f36ab1bff14f5630ffe7`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["xwiki"]`

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
# Wed, 02 Nov 2022 19:44:32 GMT
RUN apt-get update     && DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends tzdata curl wget ca-certificates fontconfig locales     && echo "en_US.UTF-8 UTF-8" >> /etc/locale.gen     && locale-gen en_US.UTF-8     && rm -rf /var/lib/apt/lists/*
# Fri, 04 Nov 2022 22:40:54 GMT
ENV JAVA_VERSION=jdk-11.0.17+8
# Fri, 04 Nov 2022 22:41:33 GMT
RUN set -eux;     ARCH="$(dpkg --print-architecture)";     case "${ARCH}" in        aarch64|arm64)          ESUM='bd6efe3290c8b5a42f695a55a26f3e3c9c284288574879d4b7089f31f5114177';          BINARY_URL='https://github.com/adoptium/temurin11-binaries/releases/download/jdk-11.0.17%2B8/OpenJDK11U-jre_aarch64_linux_hotspot_11.0.17_8.tar.gz';          ;;        armhf|arm)          ESUM='8cf113d3d7fa808895c8d2e41bb890af21c47e38c2460e0588147a4bb8fc658d';          BINARY_URL='https://github.com/adoptium/temurin11-binaries/releases/download/jdk-11.0.17%2B8/OpenJDK11U-jre_arm_linux_hotspot_11.0.17_8.tar.gz';          ;;        ppc64el|powerpc:common64)          ESUM='0ca3d806131ab5834c501f9c625bb0248cd528af361c704503348e9c9605bedf';          BINARY_URL='https://github.com/adoptium/temurin11-binaries/releases/download/jdk-11.0.17%2B8/OpenJDK11U-jre_ppc64le_linux_hotspot_11.0.17_8.tar.gz';          ;;        s390x|s390:64-bit)          ESUM='dd3b159a374086e65cb07c4ccb226c90f9c02ef929cba6f0b642171d7ed97fa4';          BINARY_URL='https://github.com/adoptium/temurin11-binaries/releases/download/jdk-11.0.17%2B8/OpenJDK11U-jre_s390x_linux_hotspot_11.0.17_8.tar.gz';          ;;        amd64|i386:x86-64)          ESUM='752616097e09d7f60a3ad8bd312f90eaf50ac72577e55df229fe6e8091148f79';          BINARY_URL='https://github.com/adoptium/temurin11-binaries/releases/download/jdk-11.0.17%2B8/OpenJDK11U-jre_x64_linux_hotspot_11.0.17_8.tar.gz';          ;;        *)          echo "Unsupported arch: ${ARCH}";          exit 1;          ;;     esac; 	  wget -O /tmp/openjdk.tar.gz ${BINARY_URL}; 	  echo "${ESUM} */tmp/openjdk.tar.gz" | sha256sum -c -; 	  mkdir -p "$JAVA_HOME"; 	  tar --extract 	      --file /tmp/openjdk.tar.gz 	      --directory "$JAVA_HOME" 	      --strip-components 1 	      --no-same-owner 	  ;     rm /tmp/openjdk.tar.gz;     find "$JAVA_HOME/lib" -name '*.so' -exec dirname '{}' ';' | sort -u > /etc/ld.so.conf.d/docker-openjdk.conf;     ldconfig;     java -Xshare:dump;
# Fri, 04 Nov 2022 22:41:34 GMT
RUN echo Verifying install ...     && fileEncoding="$(echo 'System.out.println(System.getProperty("file.encoding"))' | jshell -s -)"; [ "$fileEncoding" = 'UTF-8' ]; rm -rf ~/.java     && echo java --version && java --version     && echo Complete.
# Fri, 04 Nov 2022 23:48:38 GMT
ENV CATALINA_HOME=/usr/local/tomcat
# Fri, 04 Nov 2022 23:48:38 GMT
ENV PATH=/usr/local/tomcat/bin:/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Fri, 04 Nov 2022 23:48:38 GMT
RUN mkdir -p "$CATALINA_HOME"
# Fri, 04 Nov 2022 23:48:39 GMT
WORKDIR /usr/local/tomcat
# Fri, 04 Nov 2022 23:48:39 GMT
ENV TOMCAT_NATIVE_LIBDIR=/usr/local/tomcat/native-jni-lib
# Fri, 04 Nov 2022 23:48:39 GMT
ENV LD_LIBRARY_PATH=/usr/local/tomcat/native-jni-lib
# Fri, 04 Nov 2022 23:53:12 GMT
ENV GPG_KEYS=48F8E69F6390C9F25CFEDCD268248959359E722B A9C5DF4D22E99998D9875A5110C01C5A2F6059E7 DCFD35E0BF8CA7344752DE8B6FB21E8933C60243
# Fri, 04 Nov 2022 23:53:12 GMT
ENV TOMCAT_MAJOR=9
# Tue, 15 Nov 2022 04:57:22 GMT
ENV TOMCAT_VERSION=9.0.69
# Tue, 15 Nov 2022 04:57:22 GMT
ENV TOMCAT_SHA512=8c883c54ce9ce43eba37756a6404cdf3477879883a3e6d146dc8a7aa5e0425f487466afe6b6da4a895927cb7cb59177b9379cec18000f2de12785be57408c779
# Tue, 15 Nov 2022 04:57:22 GMT
COPY dir:096b403a5f78b17e6b4bff63128a9c93941b97f22470991610dd641633d977f1 in /usr/local/tomcat 
# Tue, 15 Nov 2022 04:57:25 GMT
RUN set -eux; 	apt-get update; 	xargs -rt apt-get install -y --no-install-recommends < "$TOMCAT_NATIVE_LIBDIR/.dependencies.txt"; 	rm -rf /var/lib/apt/lists/*
# Tue, 15 Nov 2022 04:57:26 GMT
RUN set -eux; 	nativeLines="$(catalina.sh configtest 2>&1)"; 	nativeLines="$(echo "$nativeLines" | grep 'Apache Tomcat Native')"; 	nativeLines="$(echo "$nativeLines" | sort -u)"; 	if ! echo "$nativeLines" | grep -E 'INFO: Loaded( APR based)? Apache Tomcat Native library' >&2; then 		echo >&2 "$nativeLines"; 		exit 1; 	fi
# Tue, 15 Nov 2022 04:57:26 GMT
EXPOSE 8080
# Tue, 15 Nov 2022 04:57:27 GMT
CMD ["catalina.sh" "run"]
# Wed, 11 Jan 2023 03:05:10 GMT
LABEL org.opencontainers.image.authors=XWiki Development Team <committers@xwiki.org>
# Wed, 11 Jan 2023 03:05:10 GMT
LABEL org.opencontainers.image.url=https://hub.docker.com/_/xwiki
# Wed, 11 Jan 2023 03:05:10 GMT
LABEL org.opencontainers.image.documentation=https://hub.docker.com/_/xwiki
# Wed, 11 Jan 2023 03:05:10 GMT
LABEL org.opencontainers.image.source=https://github.com/xwiki/xwiki-docker.git
# Wed, 11 Jan 2023 03:05:11 GMT
LABEL org.opencontainers.image.vendor=xwiki.org
# Wed, 11 Jan 2023 03:05:11 GMT
LABEL org.opencontainers.image.licenses=LGPL-2.1
# Wed, 11 Jan 2023 03:08:55 GMT
RUN apt-get update &&   apt-get --no-install-recommends -y install     curl     libreoffice     unzip     procps     libpostgresql-jdbc-java &&   rm -rf /var/lib/apt/lists/*
# Wed, 01 Feb 2023 22:27:07 GMT
ENV XWIKI_VERSION=14.10.4
# Wed, 01 Feb 2023 22:27:07 GMT
ENV XWIKI_URL_PREFIX=https://maven.xwiki.org/releases/org/xwiki/platform/xwiki-platform-distribution-war/14.10.4
# Wed, 01 Feb 2023 22:27:07 GMT
ENV XWIKI_DOWNLOAD_SHA256=2fcfb622319172c2e424b9c11848ebfabe27cf8ef69cba39ceb5d124b7ebe713
# Wed, 01 Feb 2023 22:27:47 GMT
RUN rm -rf /usr/local/tomcat/webapps/* &&   mkdir -p /usr/local/tomcat/temp &&   mkdir -p /usr/local/xwiki/data &&   curl -fSL "${XWIKI_URL_PREFIX}/xwiki-platform-distribution-war-${XWIKI_VERSION}.war" -o xwiki.war &&   echo "$XWIKI_DOWNLOAD_SHA256 xwiki.war" | sha256sum -c - &&   unzip -d /usr/local/tomcat/webapps/ROOT xwiki.war &&   rm -f xwiki.war
# Wed, 01 Feb 2023 22:27:50 GMT
RUN cp /usr/share/java/postgresql-jdbc4.jar /usr/local/tomcat/webapps/ROOT/WEB-INF/lib/
# Wed, 01 Feb 2023 22:27:50 GMT
COPY file:0a1be11e2eb610a1dbcd415404e3a592641110b93090030cb831e3a19a163017 in /usr/local/tomcat/bin/ 
# Wed, 01 Feb 2023 22:27:50 GMT
COPY file:4a923f484bb29a26630c19e1d617d3bf6aa6ae7c6c4a5561e97b037bcde0847c in /usr/local/tomcat/webapps/ROOT/WEB-INF/hibernate.cfg.xml 
# Wed, 01 Feb 2023 22:27:50 GMT
RUN sed -i 's/<id>org.xwiki.platform:xwiki-platform-distribution-war/<id>org.xwiki.platform:xwiki-platform-distribution-docker/'   /usr/local/tomcat/webapps/ROOT/META-INF/extension.xed
# Wed, 01 Feb 2023 22:27:50 GMT
COPY file:a47c4dcd87c9dad97aff38c49188357e6193bcad50757e516cfb08a60d4de611 in /usr/local/bin/docker-entrypoint.sh 
# Wed, 01 Feb 2023 22:27:50 GMT
VOLUME [/usr/local/xwiki]
# Wed, 01 Feb 2023 22:27:51 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 01 Feb 2023 22:27:51 GMT
CMD ["xwiki"]
```

-	Layers:
	-	`sha256:0509fae36eb0656f8bdb23f8ae64100d893bcea2563e97468d337e04d2d0410b`  
		Last Modified: Wed, 02 Nov 2022 18:50:21 GMT  
		Size: 28.4 MB (28382154 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e502a1af2bcd98f5f0d2f5e4da1a0e7bbe07a2c548e2662f7d37dce5ae1df46c`  
		Last Modified: Wed, 02 Nov 2022 19:48:28 GMT  
		Size: 12.4 MB (12396330 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bc4598c07dd818f03a0378b0341a4a8e80f0152fbb3e7d5246ca4f466f42e611`  
		Last Modified: Fri, 04 Nov 2022 22:46:46 GMT  
		Size: 45.0 MB (44958470 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:715a937a1066f998b331fcd62256ad01a5571bdf46804e97825afc64f9ebb427`  
		Last Modified: Fri, 04 Nov 2022 22:46:41 GMT  
		Size: 160.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5fb623f082f74b2fa9fc2c4e3f3a4802875cb9753cfa26ed940201ce72bb56cb`  
		Last Modified: Sat, 05 Nov 2022 00:03:40 GMT  
		Size: 172.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:33260b83200262bbd546be371ad3c1f50f5ae7228afb87982d6fa9d6b11bf26f`  
		Last Modified: Tue, 15 Nov 2022 05:10:19 GMT  
		Size: 12.2 MB (12207235 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0955fb697ea9b30a1b4f95385464f646aa1525cb6efba648e22df84ebef6b2ee`  
		Last Modified: Tue, 15 Nov 2022 05:10:18 GMT  
		Size: 452.0 KB (452021 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6eddcf66f2083b1487296a0308e0b058917c97f614f12428d82d89662038dc2e`  
		Last Modified: Tue, 15 Nov 2022 05:10:18 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1ae6a8fce0f2cd131007393c1a4eba9ce9d0501da8406af5c5ce9deb5dc187b8`  
		Last Modified: Wed, 11 Jan 2023 03:12:13 GMT  
		Size: 174.7 MB (174749274 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:64fdf9e1ef0289a65afb558897bc408557b353c604c9e3bd5dfe845ddc54ab93`  
		Last Modified: Wed, 01 Feb 2023 22:30:00 GMT  
		Size: 307.1 MB (307104835 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0eee07814c2c9ef72478213f8e0091378d617e777e157e5f5550dbf992e4a8bb`  
		Last Modified: Wed, 01 Feb 2023 22:29:45 GMT  
		Size: 936.9 KB (936853 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:889aa9ab03d69382e94096e25991f58b06afde5b4238b94ac1136db5337d1028`  
		Last Modified: Wed, 01 Feb 2023 22:29:45 GMT  
		Size: 1.3 KB (1347 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d0d21fec462339352953dc0188b312a1e80154e3e38402e546f0e4200627f5dc`  
		Last Modified: Wed, 01 Feb 2023 22:29:45 GMT  
		Size: 2.5 KB (2455 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9c6493af5a9b0ca2b189b7be35d0f796b0243ab70d7f92a34a7eae40d269c8f3`  
		Last Modified: Wed, 01 Feb 2023 22:29:45 GMT  
		Size: 6.0 KB (6011 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3a5f6da30b6a4dcd443e582890b4a323952b0320b4c3474d31c01236b8f4cf5e`  
		Last Modified: Wed, 01 Feb 2023 22:29:45 GMT  
		Size: 2.5 KB (2506 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `xwiki:lts-postgres-tomcat`

```console
$ docker pull xwiki@sha256:48a8c82a2dcfa36f6d55a5f3e75d3e2b3aca3f80de56276b35838dc7bcb6a4a6
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `xwiki:lts-postgres-tomcat` - linux; amd64

```console
$ docker pull xwiki@sha256:5cd23e4200b4eed664a61d05e3d436d0e372a3e4e985e29cb866dd9dbb573713
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **590.0 MB (589983532 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ab0dc70572c5101e5837a6281e7cb29a2b4dbf26ad0b9c91860a748aeb3360e1`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["xwiki"]`

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
# Wed, 02 Nov 2022 18:44:10 GMT
RUN apt-get update     && DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends tzdata curl wget ca-certificates fontconfig locales     && echo "en_US.UTF-8 UTF-8" >> /etc/locale.gen     && locale-gen en_US.UTF-8     && rm -rf /var/lib/apt/lists/*
# Fri, 04 Nov 2022 23:21:41 GMT
ENV JAVA_VERSION=jdk-11.0.17+8
# Fri, 04 Nov 2022 23:22:31 GMT
RUN set -eux;     ARCH="$(dpkg --print-architecture)";     case "${ARCH}" in        aarch64|arm64)          ESUM='bd6efe3290c8b5a42f695a55a26f3e3c9c284288574879d4b7089f31f5114177';          BINARY_URL='https://github.com/adoptium/temurin11-binaries/releases/download/jdk-11.0.17%2B8/OpenJDK11U-jre_aarch64_linux_hotspot_11.0.17_8.tar.gz';          ;;        armhf|arm)          ESUM='8cf113d3d7fa808895c8d2e41bb890af21c47e38c2460e0588147a4bb8fc658d';          BINARY_URL='https://github.com/adoptium/temurin11-binaries/releases/download/jdk-11.0.17%2B8/OpenJDK11U-jre_arm_linux_hotspot_11.0.17_8.tar.gz';          ;;        ppc64el|powerpc:common64)          ESUM='0ca3d806131ab5834c501f9c625bb0248cd528af361c704503348e9c9605bedf';          BINARY_URL='https://github.com/adoptium/temurin11-binaries/releases/download/jdk-11.0.17%2B8/OpenJDK11U-jre_ppc64le_linux_hotspot_11.0.17_8.tar.gz';          ;;        s390x|s390:64-bit)          ESUM='dd3b159a374086e65cb07c4ccb226c90f9c02ef929cba6f0b642171d7ed97fa4';          BINARY_URL='https://github.com/adoptium/temurin11-binaries/releases/download/jdk-11.0.17%2B8/OpenJDK11U-jre_s390x_linux_hotspot_11.0.17_8.tar.gz';          ;;        amd64|i386:x86-64)          ESUM='752616097e09d7f60a3ad8bd312f90eaf50ac72577e55df229fe6e8091148f79';          BINARY_URL='https://github.com/adoptium/temurin11-binaries/releases/download/jdk-11.0.17%2B8/OpenJDK11U-jre_x64_linux_hotspot_11.0.17_8.tar.gz';          ;;        *)          echo "Unsupported arch: ${ARCH}";          exit 1;          ;;     esac; 	  wget -O /tmp/openjdk.tar.gz ${BINARY_URL}; 	  echo "${ESUM} */tmp/openjdk.tar.gz" | sha256sum -c -; 	  mkdir -p "$JAVA_HOME"; 	  tar --extract 	      --file /tmp/openjdk.tar.gz 	      --directory "$JAVA_HOME" 	      --strip-components 1 	      --no-same-owner 	  ;     rm /tmp/openjdk.tar.gz;     find "$JAVA_HOME/lib" -name '*.so' -exec dirname '{}' ';' | sort -u > /etc/ld.so.conf.d/docker-openjdk.conf;     ldconfig;     java -Xshare:dump;
# Fri, 04 Nov 2022 23:22:32 GMT
RUN echo Verifying install ...     && fileEncoding="$(echo 'System.out.println(System.getProperty("file.encoding"))' | jshell -s -)"; [ "$fileEncoding" = 'UTF-8' ]; rm -rf ~/.java     && echo java --version && java --version     && echo Complete.
# Sat, 05 Nov 2022 01:35:16 GMT
ENV CATALINA_HOME=/usr/local/tomcat
# Sat, 05 Nov 2022 01:35:16 GMT
ENV PATH=/usr/local/tomcat/bin:/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Sat, 05 Nov 2022 01:35:17 GMT
RUN mkdir -p "$CATALINA_HOME"
# Sat, 05 Nov 2022 01:35:17 GMT
WORKDIR /usr/local/tomcat
# Sat, 05 Nov 2022 01:35:17 GMT
ENV TOMCAT_NATIVE_LIBDIR=/usr/local/tomcat/native-jni-lib
# Sat, 05 Nov 2022 01:35:17 GMT
ENV LD_LIBRARY_PATH=/usr/local/tomcat/native-jni-lib
# Sat, 05 Nov 2022 01:39:54 GMT
ENV GPG_KEYS=48F8E69F6390C9F25CFEDCD268248959359E722B A9C5DF4D22E99998D9875A5110C01C5A2F6059E7 DCFD35E0BF8CA7344752DE8B6FB21E8933C60243
# Sat, 05 Nov 2022 01:39:54 GMT
ENV TOMCAT_MAJOR=9
# Tue, 15 Nov 2022 03:06:43 GMT
ENV TOMCAT_VERSION=9.0.69
# Tue, 15 Nov 2022 03:06:43 GMT
ENV TOMCAT_SHA512=8c883c54ce9ce43eba37756a6404cdf3477879883a3e6d146dc8a7aa5e0425f487466afe6b6da4a895927cb7cb59177b9379cec18000f2de12785be57408c779
# Tue, 15 Nov 2022 03:06:44 GMT
COPY dir:b1a33aa3993dbbfbebb33bd9aa546b60c2f2191abf1227f453d4e830f6deb35f in /usr/local/tomcat 
# Tue, 15 Nov 2022 03:06:48 GMT
RUN set -eux; 	apt-get update; 	xargs -rt apt-get install -y --no-install-recommends < "$TOMCAT_NATIVE_LIBDIR/.dependencies.txt"; 	rm -rf /var/lib/apt/lists/*
# Tue, 15 Nov 2022 03:06:49 GMT
RUN set -eux; 	nativeLines="$(catalina.sh configtest 2>&1)"; 	nativeLines="$(echo "$nativeLines" | grep 'Apache Tomcat Native')"; 	nativeLines="$(echo "$nativeLines" | sort -u)"; 	if ! echo "$nativeLines" | grep -E 'INFO: Loaded( APR based)? Apache Tomcat Native library' >&2; then 		echo >&2 "$nativeLines"; 		exit 1; 	fi
# Tue, 15 Nov 2022 03:06:49 GMT
EXPOSE 8080
# Tue, 15 Nov 2022 03:06:49 GMT
CMD ["catalina.sh" "run"]
# Wed, 11 Jan 2023 02:47:03 GMT
LABEL org.opencontainers.image.authors=XWiki Development Team <committers@xwiki.org>
# Wed, 11 Jan 2023 02:47:03 GMT
LABEL org.opencontainers.image.url=https://hub.docker.com/_/xwiki
# Wed, 11 Jan 2023 02:47:03 GMT
LABEL org.opencontainers.image.documentation=https://hub.docker.com/_/xwiki
# Wed, 11 Jan 2023 02:47:03 GMT
LABEL org.opencontainers.image.source=https://github.com/xwiki/xwiki-docker.git
# Wed, 11 Jan 2023 02:47:04 GMT
LABEL org.opencontainers.image.vendor=xwiki.org
# Wed, 11 Jan 2023 02:47:04 GMT
LABEL org.opencontainers.image.licenses=LGPL-2.1
# Wed, 11 Jan 2023 02:50:25 GMT
RUN apt-get update &&   apt-get --no-install-recommends -y install     curl     libreoffice     unzip     procps     libpostgresql-jdbc-java &&   rm -rf /var/lib/apt/lists/*
# Wed, 22 Feb 2023 18:40:25 GMT
ENV XWIKI_VERSION=14.10.5
# Wed, 22 Feb 2023 18:40:25 GMT
ENV XWIKI_URL_PREFIX=https://maven.xwiki.org/releases/org/xwiki/platform/xwiki-platform-distribution-war/14.10.5
# Wed, 22 Feb 2023 18:40:25 GMT
ENV XWIKI_DOWNLOAD_SHA256=f58465d0869e4c5605ae8375a09c79399d1149c7131fed3cf9959918267eb6a8
# Wed, 22 Feb 2023 18:41:04 GMT
RUN rm -rf /usr/local/tomcat/webapps/* &&   mkdir -p /usr/local/tomcat/temp &&   mkdir -p /usr/local/xwiki/data &&   curl -fSL "${XWIKI_URL_PREFIX}/xwiki-platform-distribution-war-${XWIKI_VERSION}.war" -o xwiki.war &&   echo "$XWIKI_DOWNLOAD_SHA256 xwiki.war" | sha256sum -c - &&   unzip -d /usr/local/tomcat/webapps/ROOT xwiki.war &&   rm -f xwiki.war
# Wed, 22 Feb 2023 18:41:05 GMT
RUN cp /usr/share/java/postgresql-jdbc4.jar /usr/local/tomcat/webapps/ROOT/WEB-INF/lib/
# Wed, 22 Feb 2023 18:41:05 GMT
COPY file:0a1be11e2eb610a1dbcd415404e3a592641110b93090030cb831e3a19a163017 in /usr/local/tomcat/bin/ 
# Wed, 22 Feb 2023 18:41:05 GMT
COPY file:4a923f484bb29a26630c19e1d617d3bf6aa6ae7c6c4a5561e97b037bcde0847c in /usr/local/tomcat/webapps/ROOT/WEB-INF/hibernate.cfg.xml 
# Wed, 22 Feb 2023 18:41:06 GMT
RUN sed -i 's/<id>org.xwiki.platform:xwiki-platform-distribution-war/<id>org.xwiki.platform:xwiki-platform-distribution-docker/'   /usr/local/tomcat/webapps/ROOT/META-INF/extension.xed
# Wed, 22 Feb 2023 18:41:06 GMT
COPY file:a47c4dcd87c9dad97aff38c49188357e6193bcad50757e516cfb08a60d4de611 in /usr/local/bin/docker-entrypoint.sh 
# Wed, 22 Feb 2023 18:41:06 GMT
VOLUME [/usr/local/xwiki]
# Wed, 22 Feb 2023 18:41:06 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 22 Feb 2023 18:41:06 GMT
CMD ["xwiki"]
```

-	Layers:
	-	`sha256:e96e057aae67380a4ddb16c337c5c3669d97fdff69ec537f02aa2cc30d814281`  
		Last Modified: Wed, 02 Nov 2022 03:03:36 GMT  
		Size: 30.4 MB (30425607 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4ced2591451da3a02e2b6bb44752b9e3f00d77789921be4df5082fb9f9880ad0`  
		Last Modified: Wed, 02 Nov 2022 18:48:43 GMT  
		Size: 12.4 MB (12439006 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:df8f874ae8c08a9e69e5fbe6c5a64200a45386132a3203d1a9a7f1146d94cfbc`  
		Last Modified: Fri, 04 Nov 2022 23:29:33 GMT  
		Size: 46.6 MB (46629936 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:111b6c7486426c4b6989102c2ee5be856e8a58e20ab0a350b24a905d536e8e7f`  
		Last Modified: Fri, 04 Nov 2022 23:29:26 GMT  
		Size: 161.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e6f84dce457c6d4f7b7291fce05f8e77998a3a7722a54125a1f1d52ca83043b4`  
		Last Modified: Sat, 05 Nov 2022 01:50:51 GMT  
		Size: 173.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a6c26749ee782392e38845ee2ba79b0da586ef6a45d8e7f29c7af14612278547`  
		Last Modified: Tue, 15 Nov 2022 03:19:57 GMT  
		Size: 12.2 MB (12200249 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4dddc6d9fa6024025b3fcfe729cab2dc544fb25476eca6e80b1af8e8d93bb0ee`  
		Last Modified: Tue, 15 Nov 2022 03:19:56 GMT  
		Size: 452.7 KB (452680 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:06637eebe5e72c8ad9019ad4eb4cdde1f11f7d4c24c7ed7374cf8966343aa2fb`  
		Last Modified: Tue, 15 Nov 2022 03:19:56 GMT  
		Size: 131.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b57f6f8bcfb0d93b8e21d3068d1f65d3f08dba05c5fab7d4c36e2359317b18c7`  
		Last Modified: Wed, 11 Jan 2023 02:53:53 GMT  
		Size: 179.7 MB (179745182 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b26b00a2f6717a934b9a1b08bac612aaaf57a4cfb4d82db521e7d36755621933`  
		Last Modified: Wed, 22 Feb 2023 18:43:06 GMT  
		Size: 307.1 MB (307141251 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:11801aa48fd913e3278b4d0a512df366a8ef26c1cc3e95a8439a1be90aadfd5a`  
		Last Modified: Wed, 22 Feb 2023 18:42:50 GMT  
		Size: 936.9 KB (936850 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fb4e8755162307a316ff405759f2417dc77e746651f89c83a0477ab19dc7da5d`  
		Last Modified: Wed, 22 Feb 2023 18:42:50 GMT  
		Size: 1.3 KB (1342 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2ba124a3d49367a8e2f46fc2043189f91e2dd282d40a301d9c1f79a705d35e66`  
		Last Modified: Wed, 22 Feb 2023 18:42:50 GMT  
		Size: 2.5 KB (2450 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8f421201132c3966dbb37a473df5922718780304fa03993ef75bb78522d5cafd`  
		Last Modified: Wed, 22 Feb 2023 18:42:50 GMT  
		Size: 6.0 KB (6012 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1b5dc6b32b3d1d9a80058f5ffc684363a0cfadf60ade5875fa37854ec7b46fff`  
		Last Modified: Wed, 22 Feb 2023 18:42:50 GMT  
		Size: 2.5 KB (2502 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `xwiki:lts-postgres-tomcat` - linux; arm64 variant v8

```console
$ docker pull xwiki@sha256:e04b6d052b479b648834e5d960deff2f28274834a9dc812b628ccb9a624c53ef
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **581.2 MB (581199952 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:4693188024e4d84ad63e783e3377e2d600a040c344f7f36ab1bff14f5630ffe7`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["xwiki"]`

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
# Wed, 02 Nov 2022 19:44:32 GMT
RUN apt-get update     && DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends tzdata curl wget ca-certificates fontconfig locales     && echo "en_US.UTF-8 UTF-8" >> /etc/locale.gen     && locale-gen en_US.UTF-8     && rm -rf /var/lib/apt/lists/*
# Fri, 04 Nov 2022 22:40:54 GMT
ENV JAVA_VERSION=jdk-11.0.17+8
# Fri, 04 Nov 2022 22:41:33 GMT
RUN set -eux;     ARCH="$(dpkg --print-architecture)";     case "${ARCH}" in        aarch64|arm64)          ESUM='bd6efe3290c8b5a42f695a55a26f3e3c9c284288574879d4b7089f31f5114177';          BINARY_URL='https://github.com/adoptium/temurin11-binaries/releases/download/jdk-11.0.17%2B8/OpenJDK11U-jre_aarch64_linux_hotspot_11.0.17_8.tar.gz';          ;;        armhf|arm)          ESUM='8cf113d3d7fa808895c8d2e41bb890af21c47e38c2460e0588147a4bb8fc658d';          BINARY_URL='https://github.com/adoptium/temurin11-binaries/releases/download/jdk-11.0.17%2B8/OpenJDK11U-jre_arm_linux_hotspot_11.0.17_8.tar.gz';          ;;        ppc64el|powerpc:common64)          ESUM='0ca3d806131ab5834c501f9c625bb0248cd528af361c704503348e9c9605bedf';          BINARY_URL='https://github.com/adoptium/temurin11-binaries/releases/download/jdk-11.0.17%2B8/OpenJDK11U-jre_ppc64le_linux_hotspot_11.0.17_8.tar.gz';          ;;        s390x|s390:64-bit)          ESUM='dd3b159a374086e65cb07c4ccb226c90f9c02ef929cba6f0b642171d7ed97fa4';          BINARY_URL='https://github.com/adoptium/temurin11-binaries/releases/download/jdk-11.0.17%2B8/OpenJDK11U-jre_s390x_linux_hotspot_11.0.17_8.tar.gz';          ;;        amd64|i386:x86-64)          ESUM='752616097e09d7f60a3ad8bd312f90eaf50ac72577e55df229fe6e8091148f79';          BINARY_URL='https://github.com/adoptium/temurin11-binaries/releases/download/jdk-11.0.17%2B8/OpenJDK11U-jre_x64_linux_hotspot_11.0.17_8.tar.gz';          ;;        *)          echo "Unsupported arch: ${ARCH}";          exit 1;          ;;     esac; 	  wget -O /tmp/openjdk.tar.gz ${BINARY_URL}; 	  echo "${ESUM} */tmp/openjdk.tar.gz" | sha256sum -c -; 	  mkdir -p "$JAVA_HOME"; 	  tar --extract 	      --file /tmp/openjdk.tar.gz 	      --directory "$JAVA_HOME" 	      --strip-components 1 	      --no-same-owner 	  ;     rm /tmp/openjdk.tar.gz;     find "$JAVA_HOME/lib" -name '*.so' -exec dirname '{}' ';' | sort -u > /etc/ld.so.conf.d/docker-openjdk.conf;     ldconfig;     java -Xshare:dump;
# Fri, 04 Nov 2022 22:41:34 GMT
RUN echo Verifying install ...     && fileEncoding="$(echo 'System.out.println(System.getProperty("file.encoding"))' | jshell -s -)"; [ "$fileEncoding" = 'UTF-8' ]; rm -rf ~/.java     && echo java --version && java --version     && echo Complete.
# Fri, 04 Nov 2022 23:48:38 GMT
ENV CATALINA_HOME=/usr/local/tomcat
# Fri, 04 Nov 2022 23:48:38 GMT
ENV PATH=/usr/local/tomcat/bin:/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Fri, 04 Nov 2022 23:48:38 GMT
RUN mkdir -p "$CATALINA_HOME"
# Fri, 04 Nov 2022 23:48:39 GMT
WORKDIR /usr/local/tomcat
# Fri, 04 Nov 2022 23:48:39 GMT
ENV TOMCAT_NATIVE_LIBDIR=/usr/local/tomcat/native-jni-lib
# Fri, 04 Nov 2022 23:48:39 GMT
ENV LD_LIBRARY_PATH=/usr/local/tomcat/native-jni-lib
# Fri, 04 Nov 2022 23:53:12 GMT
ENV GPG_KEYS=48F8E69F6390C9F25CFEDCD268248959359E722B A9C5DF4D22E99998D9875A5110C01C5A2F6059E7 DCFD35E0BF8CA7344752DE8B6FB21E8933C60243
# Fri, 04 Nov 2022 23:53:12 GMT
ENV TOMCAT_MAJOR=9
# Tue, 15 Nov 2022 04:57:22 GMT
ENV TOMCAT_VERSION=9.0.69
# Tue, 15 Nov 2022 04:57:22 GMT
ENV TOMCAT_SHA512=8c883c54ce9ce43eba37756a6404cdf3477879883a3e6d146dc8a7aa5e0425f487466afe6b6da4a895927cb7cb59177b9379cec18000f2de12785be57408c779
# Tue, 15 Nov 2022 04:57:22 GMT
COPY dir:096b403a5f78b17e6b4bff63128a9c93941b97f22470991610dd641633d977f1 in /usr/local/tomcat 
# Tue, 15 Nov 2022 04:57:25 GMT
RUN set -eux; 	apt-get update; 	xargs -rt apt-get install -y --no-install-recommends < "$TOMCAT_NATIVE_LIBDIR/.dependencies.txt"; 	rm -rf /var/lib/apt/lists/*
# Tue, 15 Nov 2022 04:57:26 GMT
RUN set -eux; 	nativeLines="$(catalina.sh configtest 2>&1)"; 	nativeLines="$(echo "$nativeLines" | grep 'Apache Tomcat Native')"; 	nativeLines="$(echo "$nativeLines" | sort -u)"; 	if ! echo "$nativeLines" | grep -E 'INFO: Loaded( APR based)? Apache Tomcat Native library' >&2; then 		echo >&2 "$nativeLines"; 		exit 1; 	fi
# Tue, 15 Nov 2022 04:57:26 GMT
EXPOSE 8080
# Tue, 15 Nov 2022 04:57:27 GMT
CMD ["catalina.sh" "run"]
# Wed, 11 Jan 2023 03:05:10 GMT
LABEL org.opencontainers.image.authors=XWiki Development Team <committers@xwiki.org>
# Wed, 11 Jan 2023 03:05:10 GMT
LABEL org.opencontainers.image.url=https://hub.docker.com/_/xwiki
# Wed, 11 Jan 2023 03:05:10 GMT
LABEL org.opencontainers.image.documentation=https://hub.docker.com/_/xwiki
# Wed, 11 Jan 2023 03:05:10 GMT
LABEL org.opencontainers.image.source=https://github.com/xwiki/xwiki-docker.git
# Wed, 11 Jan 2023 03:05:11 GMT
LABEL org.opencontainers.image.vendor=xwiki.org
# Wed, 11 Jan 2023 03:05:11 GMT
LABEL org.opencontainers.image.licenses=LGPL-2.1
# Wed, 11 Jan 2023 03:08:55 GMT
RUN apt-get update &&   apt-get --no-install-recommends -y install     curl     libreoffice     unzip     procps     libpostgresql-jdbc-java &&   rm -rf /var/lib/apt/lists/*
# Wed, 01 Feb 2023 22:27:07 GMT
ENV XWIKI_VERSION=14.10.4
# Wed, 01 Feb 2023 22:27:07 GMT
ENV XWIKI_URL_PREFIX=https://maven.xwiki.org/releases/org/xwiki/platform/xwiki-platform-distribution-war/14.10.4
# Wed, 01 Feb 2023 22:27:07 GMT
ENV XWIKI_DOWNLOAD_SHA256=2fcfb622319172c2e424b9c11848ebfabe27cf8ef69cba39ceb5d124b7ebe713
# Wed, 01 Feb 2023 22:27:47 GMT
RUN rm -rf /usr/local/tomcat/webapps/* &&   mkdir -p /usr/local/tomcat/temp &&   mkdir -p /usr/local/xwiki/data &&   curl -fSL "${XWIKI_URL_PREFIX}/xwiki-platform-distribution-war-${XWIKI_VERSION}.war" -o xwiki.war &&   echo "$XWIKI_DOWNLOAD_SHA256 xwiki.war" | sha256sum -c - &&   unzip -d /usr/local/tomcat/webapps/ROOT xwiki.war &&   rm -f xwiki.war
# Wed, 01 Feb 2023 22:27:50 GMT
RUN cp /usr/share/java/postgresql-jdbc4.jar /usr/local/tomcat/webapps/ROOT/WEB-INF/lib/
# Wed, 01 Feb 2023 22:27:50 GMT
COPY file:0a1be11e2eb610a1dbcd415404e3a592641110b93090030cb831e3a19a163017 in /usr/local/tomcat/bin/ 
# Wed, 01 Feb 2023 22:27:50 GMT
COPY file:4a923f484bb29a26630c19e1d617d3bf6aa6ae7c6c4a5561e97b037bcde0847c in /usr/local/tomcat/webapps/ROOT/WEB-INF/hibernate.cfg.xml 
# Wed, 01 Feb 2023 22:27:50 GMT
RUN sed -i 's/<id>org.xwiki.platform:xwiki-platform-distribution-war/<id>org.xwiki.platform:xwiki-platform-distribution-docker/'   /usr/local/tomcat/webapps/ROOT/META-INF/extension.xed
# Wed, 01 Feb 2023 22:27:50 GMT
COPY file:a47c4dcd87c9dad97aff38c49188357e6193bcad50757e516cfb08a60d4de611 in /usr/local/bin/docker-entrypoint.sh 
# Wed, 01 Feb 2023 22:27:50 GMT
VOLUME [/usr/local/xwiki]
# Wed, 01 Feb 2023 22:27:51 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 01 Feb 2023 22:27:51 GMT
CMD ["xwiki"]
```

-	Layers:
	-	`sha256:0509fae36eb0656f8bdb23f8ae64100d893bcea2563e97468d337e04d2d0410b`  
		Last Modified: Wed, 02 Nov 2022 18:50:21 GMT  
		Size: 28.4 MB (28382154 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e502a1af2bcd98f5f0d2f5e4da1a0e7bbe07a2c548e2662f7d37dce5ae1df46c`  
		Last Modified: Wed, 02 Nov 2022 19:48:28 GMT  
		Size: 12.4 MB (12396330 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bc4598c07dd818f03a0378b0341a4a8e80f0152fbb3e7d5246ca4f466f42e611`  
		Last Modified: Fri, 04 Nov 2022 22:46:46 GMT  
		Size: 45.0 MB (44958470 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:715a937a1066f998b331fcd62256ad01a5571bdf46804e97825afc64f9ebb427`  
		Last Modified: Fri, 04 Nov 2022 22:46:41 GMT  
		Size: 160.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5fb623f082f74b2fa9fc2c4e3f3a4802875cb9753cfa26ed940201ce72bb56cb`  
		Last Modified: Sat, 05 Nov 2022 00:03:40 GMT  
		Size: 172.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:33260b83200262bbd546be371ad3c1f50f5ae7228afb87982d6fa9d6b11bf26f`  
		Last Modified: Tue, 15 Nov 2022 05:10:19 GMT  
		Size: 12.2 MB (12207235 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0955fb697ea9b30a1b4f95385464f646aa1525cb6efba648e22df84ebef6b2ee`  
		Last Modified: Tue, 15 Nov 2022 05:10:18 GMT  
		Size: 452.0 KB (452021 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6eddcf66f2083b1487296a0308e0b058917c97f614f12428d82d89662038dc2e`  
		Last Modified: Tue, 15 Nov 2022 05:10:18 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1ae6a8fce0f2cd131007393c1a4eba9ce9d0501da8406af5c5ce9deb5dc187b8`  
		Last Modified: Wed, 11 Jan 2023 03:12:13 GMT  
		Size: 174.7 MB (174749274 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:64fdf9e1ef0289a65afb558897bc408557b353c604c9e3bd5dfe845ddc54ab93`  
		Last Modified: Wed, 01 Feb 2023 22:30:00 GMT  
		Size: 307.1 MB (307104835 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0eee07814c2c9ef72478213f8e0091378d617e777e157e5f5550dbf992e4a8bb`  
		Last Modified: Wed, 01 Feb 2023 22:29:45 GMT  
		Size: 936.9 KB (936853 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:889aa9ab03d69382e94096e25991f58b06afde5b4238b94ac1136db5337d1028`  
		Last Modified: Wed, 01 Feb 2023 22:29:45 GMT  
		Size: 1.3 KB (1347 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d0d21fec462339352953dc0188b312a1e80154e3e38402e546f0e4200627f5dc`  
		Last Modified: Wed, 01 Feb 2023 22:29:45 GMT  
		Size: 2.5 KB (2455 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9c6493af5a9b0ca2b189b7be35d0f796b0243ab70d7f92a34a7eae40d269c8f3`  
		Last Modified: Wed, 01 Feb 2023 22:29:45 GMT  
		Size: 6.0 KB (6011 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3a5f6da30b6a4dcd443e582890b4a323952b0320b4c3474d31c01236b8f4cf5e`  
		Last Modified: Wed, 01 Feb 2023 22:29:45 GMT  
		Size: 2.5 KB (2506 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `xwiki:mariadb-tomcat`

```console
$ docker pull xwiki@sha256:725347355967f33745268f1167cc3c1b12fc85e327ccfa96da0848d05e3836c4
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `xwiki:mariadb-tomcat` - linux; amd64

```console
$ docker pull xwiki@sha256:cca1fb53bc2f0240f7f4843b846210e341a6002d7b18a0b90202520ce2f4ead0
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **588.7 MB (588672467 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:0088d72e62c01c9996a75e1b7e2296ba530b2dbd4054be70a006b33295aa4ff9`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["xwiki"]`

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
# Wed, 02 Nov 2022 18:44:10 GMT
RUN apt-get update     && DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends tzdata curl wget ca-certificates fontconfig locales     && echo "en_US.UTF-8 UTF-8" >> /etc/locale.gen     && locale-gen en_US.UTF-8     && rm -rf /var/lib/apt/lists/*
# Fri, 04 Nov 2022 23:21:41 GMT
ENV JAVA_VERSION=jdk-11.0.17+8
# Fri, 04 Nov 2022 23:22:31 GMT
RUN set -eux;     ARCH="$(dpkg --print-architecture)";     case "${ARCH}" in        aarch64|arm64)          ESUM='bd6efe3290c8b5a42f695a55a26f3e3c9c284288574879d4b7089f31f5114177';          BINARY_URL='https://github.com/adoptium/temurin11-binaries/releases/download/jdk-11.0.17%2B8/OpenJDK11U-jre_aarch64_linux_hotspot_11.0.17_8.tar.gz';          ;;        armhf|arm)          ESUM='8cf113d3d7fa808895c8d2e41bb890af21c47e38c2460e0588147a4bb8fc658d';          BINARY_URL='https://github.com/adoptium/temurin11-binaries/releases/download/jdk-11.0.17%2B8/OpenJDK11U-jre_arm_linux_hotspot_11.0.17_8.tar.gz';          ;;        ppc64el|powerpc:common64)          ESUM='0ca3d806131ab5834c501f9c625bb0248cd528af361c704503348e9c9605bedf';          BINARY_URL='https://github.com/adoptium/temurin11-binaries/releases/download/jdk-11.0.17%2B8/OpenJDK11U-jre_ppc64le_linux_hotspot_11.0.17_8.tar.gz';          ;;        s390x|s390:64-bit)          ESUM='dd3b159a374086e65cb07c4ccb226c90f9c02ef929cba6f0b642171d7ed97fa4';          BINARY_URL='https://github.com/adoptium/temurin11-binaries/releases/download/jdk-11.0.17%2B8/OpenJDK11U-jre_s390x_linux_hotspot_11.0.17_8.tar.gz';          ;;        amd64|i386:x86-64)          ESUM='752616097e09d7f60a3ad8bd312f90eaf50ac72577e55df229fe6e8091148f79';          BINARY_URL='https://github.com/adoptium/temurin11-binaries/releases/download/jdk-11.0.17%2B8/OpenJDK11U-jre_x64_linux_hotspot_11.0.17_8.tar.gz';          ;;        *)          echo "Unsupported arch: ${ARCH}";          exit 1;          ;;     esac; 	  wget -O /tmp/openjdk.tar.gz ${BINARY_URL}; 	  echo "${ESUM} */tmp/openjdk.tar.gz" | sha256sum -c -; 	  mkdir -p "$JAVA_HOME"; 	  tar --extract 	      --file /tmp/openjdk.tar.gz 	      --directory "$JAVA_HOME" 	      --strip-components 1 	      --no-same-owner 	  ;     rm /tmp/openjdk.tar.gz;     find "$JAVA_HOME/lib" -name '*.so' -exec dirname '{}' ';' | sort -u > /etc/ld.so.conf.d/docker-openjdk.conf;     ldconfig;     java -Xshare:dump;
# Fri, 04 Nov 2022 23:22:32 GMT
RUN echo Verifying install ...     && fileEncoding="$(echo 'System.out.println(System.getProperty("file.encoding"))' | jshell -s -)"; [ "$fileEncoding" = 'UTF-8' ]; rm -rf ~/.java     && echo java --version && java --version     && echo Complete.
# Sat, 05 Nov 2022 01:35:16 GMT
ENV CATALINA_HOME=/usr/local/tomcat
# Sat, 05 Nov 2022 01:35:16 GMT
ENV PATH=/usr/local/tomcat/bin:/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Sat, 05 Nov 2022 01:35:17 GMT
RUN mkdir -p "$CATALINA_HOME"
# Sat, 05 Nov 2022 01:35:17 GMT
WORKDIR /usr/local/tomcat
# Sat, 05 Nov 2022 01:35:17 GMT
ENV TOMCAT_NATIVE_LIBDIR=/usr/local/tomcat/native-jni-lib
# Sat, 05 Nov 2022 01:35:17 GMT
ENV LD_LIBRARY_PATH=/usr/local/tomcat/native-jni-lib
# Sat, 05 Nov 2022 01:39:54 GMT
ENV GPG_KEYS=48F8E69F6390C9F25CFEDCD268248959359E722B A9C5DF4D22E99998D9875A5110C01C5A2F6059E7 DCFD35E0BF8CA7344752DE8B6FB21E8933C60243
# Sat, 05 Nov 2022 01:39:54 GMT
ENV TOMCAT_MAJOR=9
# Tue, 15 Nov 2022 03:06:43 GMT
ENV TOMCAT_VERSION=9.0.69
# Tue, 15 Nov 2022 03:06:43 GMT
ENV TOMCAT_SHA512=8c883c54ce9ce43eba37756a6404cdf3477879883a3e6d146dc8a7aa5e0425f487466afe6b6da4a895927cb7cb59177b9379cec18000f2de12785be57408c779
# Tue, 15 Nov 2022 03:06:44 GMT
COPY dir:b1a33aa3993dbbfbebb33bd9aa546b60c2f2191abf1227f453d4e830f6deb35f in /usr/local/tomcat 
# Tue, 15 Nov 2022 03:06:48 GMT
RUN set -eux; 	apt-get update; 	xargs -rt apt-get install -y --no-install-recommends < "$TOMCAT_NATIVE_LIBDIR/.dependencies.txt"; 	rm -rf /var/lib/apt/lists/*
# Tue, 15 Nov 2022 03:06:49 GMT
RUN set -eux; 	nativeLines="$(catalina.sh configtest 2>&1)"; 	nativeLines="$(echo "$nativeLines" | grep 'Apache Tomcat Native')"; 	nativeLines="$(echo "$nativeLines" | sort -u)"; 	if ! echo "$nativeLines" | grep -E 'INFO: Loaded( APR based)? Apache Tomcat Native library' >&2; then 		echo >&2 "$nativeLines"; 		exit 1; 	fi
# Tue, 15 Nov 2022 03:06:49 GMT
EXPOSE 8080
# Tue, 15 Nov 2022 03:06:49 GMT
CMD ["catalina.sh" "run"]
# Wed, 11 Jan 2023 02:47:03 GMT
LABEL org.opencontainers.image.authors=XWiki Development Team <committers@xwiki.org>
# Wed, 11 Jan 2023 02:47:03 GMT
LABEL org.opencontainers.image.url=https://hub.docker.com/_/xwiki
# Wed, 11 Jan 2023 02:47:03 GMT
LABEL org.opencontainers.image.documentation=https://hub.docker.com/_/xwiki
# Wed, 11 Jan 2023 02:47:03 GMT
LABEL org.opencontainers.image.source=https://github.com/xwiki/xwiki-docker.git
# Wed, 11 Jan 2023 02:47:04 GMT
LABEL org.opencontainers.image.vendor=xwiki.org
# Wed, 11 Jan 2023 02:47:04 GMT
LABEL org.opencontainers.image.licenses=LGPL-2.1
# Wed, 11 Jan 2023 02:49:03 GMT
RUN apt-get update &&   apt-get --no-install-recommends -y install     curl     libreoffice     unzip     procps &&   rm -rf /var/lib/apt/lists/*
# Tue, 31 Jan 2023 00:20:17 GMT
ENV XWIKI_VERSION=15.0
# Tue, 31 Jan 2023 00:20:17 GMT
ENV XWIKI_URL_PREFIX=https://maven.xwiki.org/releases/org/xwiki/platform/xwiki-platform-distribution-war/15.0
# Tue, 31 Jan 2023 00:20:17 GMT
ENV XWIKI_DOWNLOAD_SHA256=79ba0f479bbc49521c113821adc9d91141075a9470d7f9bbb6994ca59c30d121
# Tue, 31 Jan 2023 00:21:18 GMT
RUN rm -rf /usr/local/tomcat/webapps/* &&   mkdir -p /usr/local/tomcat/temp &&   mkdir -p /usr/local/xwiki/data &&   curl -fSL "${XWIKI_URL_PREFIX}/xwiki-platform-distribution-war-${XWIKI_VERSION}.war" -o xwiki.war &&   echo "$XWIKI_DOWNLOAD_SHA256 xwiki.war" | sha256sum -c - &&   unzip -d /usr/local/tomcat/webapps/ROOT xwiki.war &&   rm -f xwiki.war
# Tue, 31 Jan 2023 00:22:50 GMT
ENV MARIADB_JDBC_VERSION=3.1.1
# Tue, 31 Jan 2023 00:22:50 GMT
ENV MARIADB_JDBC_SHA256=a554541fd88047905fb0c4c10e1d85295f5e38c7bb5fb408b425392a79fc26e3
# Tue, 31 Jan 2023 00:22:50 GMT
ENV MARIADB_JDBC_PREFIX=https://repo1.maven.org/maven2/org/mariadb/jdbc/mariadb-java-client/3.1.1
# Tue, 31 Jan 2023 00:22:50 GMT
ENV MARIADB_JDBC_ARTIFACT=mariadb-java-client-3.1.1.jar
# Tue, 31 Jan 2023 00:22:50 GMT
ENV MARIADB_JDBC_TARGET=/usr/local/tomcat/webapps/ROOT/WEB-INF/lib/mariadb-java-client-3.1.1.jar
# Tue, 31 Jan 2023 00:22:51 GMT
RUN curl -fSL "${MARIADB_JDBC_PREFIX}/${MARIADB_JDBC_ARTIFACT}" -o $MARIADB_JDBC_TARGET &&   echo "$MARIADB_JDBC_SHA256 $MARIADB_JDBC_TARGET" | sha256sum -c -
# Tue, 31 Jan 2023 00:22:51 GMT
COPY file:0a1be11e2eb610a1dbcd415404e3a592641110b93090030cb831e3a19a163017 in /usr/local/tomcat/bin/ 
# Tue, 31 Jan 2023 00:22:51 GMT
COPY file:0e237c3876eeb3b5f3473a064d3e507da2df6c228ca714687930b34e3b687601 in /usr/local/tomcat/webapps/ROOT/WEB-INF/hibernate.cfg.xml 
# Tue, 31 Jan 2023 00:22:52 GMT
RUN sed -i 's/<id>org.xwiki.platform:xwiki-platform-distribution-war/<id>org.xwiki.platform:xwiki-platform-distribution-docker/'   /usr/local/tomcat/webapps/ROOT/META-INF/extension.xed
# Tue, 31 Jan 2023 00:22:52 GMT
COPY file:a47c4dcd87c9dad97aff38c49188357e6193bcad50757e516cfb08a60d4de611 in /usr/local/bin/docker-entrypoint.sh 
# Tue, 31 Jan 2023 00:22:52 GMT
VOLUME [/usr/local/xwiki]
# Tue, 31 Jan 2023 00:22:52 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 31 Jan 2023 00:22:52 GMT
CMD ["xwiki"]
```

-	Layers:
	-	`sha256:e96e057aae67380a4ddb16c337c5c3669d97fdff69ec537f02aa2cc30d814281`  
		Last Modified: Wed, 02 Nov 2022 03:03:36 GMT  
		Size: 30.4 MB (30425607 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4ced2591451da3a02e2b6bb44752b9e3f00d77789921be4df5082fb9f9880ad0`  
		Last Modified: Wed, 02 Nov 2022 18:48:43 GMT  
		Size: 12.4 MB (12439006 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:df8f874ae8c08a9e69e5fbe6c5a64200a45386132a3203d1a9a7f1146d94cfbc`  
		Last Modified: Fri, 04 Nov 2022 23:29:33 GMT  
		Size: 46.6 MB (46629936 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:111b6c7486426c4b6989102c2ee5be856e8a58e20ab0a350b24a905d536e8e7f`  
		Last Modified: Fri, 04 Nov 2022 23:29:26 GMT  
		Size: 161.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e6f84dce457c6d4f7b7291fce05f8e77998a3a7722a54125a1f1d52ca83043b4`  
		Last Modified: Sat, 05 Nov 2022 01:50:51 GMT  
		Size: 173.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a6c26749ee782392e38845ee2ba79b0da586ef6a45d8e7f29c7af14612278547`  
		Last Modified: Tue, 15 Nov 2022 03:19:57 GMT  
		Size: 12.2 MB (12200249 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4dddc6d9fa6024025b3fcfe729cab2dc544fb25476eca6e80b1af8e8d93bb0ee`  
		Last Modified: Tue, 15 Nov 2022 03:19:56 GMT  
		Size: 452.7 KB (452680 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:06637eebe5e72c8ad9019ad4eb4cdde1f11f7d4c24c7ed7374cf8966343aa2fb`  
		Last Modified: Tue, 15 Nov 2022 03:19:56 GMT  
		Size: 131.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b276fb8390410a8208724033e325715ea26000d5a1a762d4c3699b927884fbfe`  
		Last Modified: Wed, 11 Jan 2023 02:52:45 GMT  
		Size: 178.8 MB (178805608 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:156ca91198173149698aa0396648a9608b6ab1f2bc2666800843ce33c9f85b6e`  
		Last Modified: Tue, 31 Jan 2023 00:24:09 GMT  
		Size: 307.1 MB (307117069 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:457b62e39784bb863cc6a7514f591232a9b9442f2f105a85bdbd5e4abb166ad6`  
		Last Modified: Tue, 31 Jan 2023 00:25:23 GMT  
		Size: 589.7 KB (589675 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:30adbbecb36197c3e48c90be60a50c089cb9738a771c968b36240b05b8164a30`  
		Last Modified: Tue, 31 Jan 2023 00:25:22 GMT  
		Size: 1.3 KB (1345 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3bfcc8a896e6e21d5c28da101d5d57167a5cfc49c542a407feabe27f6c355b6f`  
		Last Modified: Tue, 31 Jan 2023 00:25:22 GMT  
		Size: 2.3 KB (2312 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5cbacf6c3ece365f64b683c8ab4fe61301319c8f1bd26d38ea40abbbd15bc7d4`  
		Last Modified: Tue, 31 Jan 2023 00:25:23 GMT  
		Size: 6.0 KB (6008 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6687ecee0e041196fd810c316565d70808b445cdce0b089b2177e6636bffd9fe`  
		Last Modified: Tue, 31 Jan 2023 00:25:23 GMT  
		Size: 2.5 KB (2507 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `xwiki:mariadb-tomcat` - linux; arm64 variant v8

```console
$ docker pull xwiki@sha256:14b1c6df2a5c5c9b549f372fce50719f39fc809b8b02c945d92eb29c29f7bc75
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **579.9 MB (579922416 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d9a728666283f6f4b71f567ce6c5ef1e2dc544facfd01d52fdf1577be95c6b07`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["xwiki"]`

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
# Wed, 02 Nov 2022 19:44:32 GMT
RUN apt-get update     && DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends tzdata curl wget ca-certificates fontconfig locales     && echo "en_US.UTF-8 UTF-8" >> /etc/locale.gen     && locale-gen en_US.UTF-8     && rm -rf /var/lib/apt/lists/*
# Fri, 04 Nov 2022 22:40:54 GMT
ENV JAVA_VERSION=jdk-11.0.17+8
# Fri, 04 Nov 2022 22:41:33 GMT
RUN set -eux;     ARCH="$(dpkg --print-architecture)";     case "${ARCH}" in        aarch64|arm64)          ESUM='bd6efe3290c8b5a42f695a55a26f3e3c9c284288574879d4b7089f31f5114177';          BINARY_URL='https://github.com/adoptium/temurin11-binaries/releases/download/jdk-11.0.17%2B8/OpenJDK11U-jre_aarch64_linux_hotspot_11.0.17_8.tar.gz';          ;;        armhf|arm)          ESUM='8cf113d3d7fa808895c8d2e41bb890af21c47e38c2460e0588147a4bb8fc658d';          BINARY_URL='https://github.com/adoptium/temurin11-binaries/releases/download/jdk-11.0.17%2B8/OpenJDK11U-jre_arm_linux_hotspot_11.0.17_8.tar.gz';          ;;        ppc64el|powerpc:common64)          ESUM='0ca3d806131ab5834c501f9c625bb0248cd528af361c704503348e9c9605bedf';          BINARY_URL='https://github.com/adoptium/temurin11-binaries/releases/download/jdk-11.0.17%2B8/OpenJDK11U-jre_ppc64le_linux_hotspot_11.0.17_8.tar.gz';          ;;        s390x|s390:64-bit)          ESUM='dd3b159a374086e65cb07c4ccb226c90f9c02ef929cba6f0b642171d7ed97fa4';          BINARY_URL='https://github.com/adoptium/temurin11-binaries/releases/download/jdk-11.0.17%2B8/OpenJDK11U-jre_s390x_linux_hotspot_11.0.17_8.tar.gz';          ;;        amd64|i386:x86-64)          ESUM='752616097e09d7f60a3ad8bd312f90eaf50ac72577e55df229fe6e8091148f79';          BINARY_URL='https://github.com/adoptium/temurin11-binaries/releases/download/jdk-11.0.17%2B8/OpenJDK11U-jre_x64_linux_hotspot_11.0.17_8.tar.gz';          ;;        *)          echo "Unsupported arch: ${ARCH}";          exit 1;          ;;     esac; 	  wget -O /tmp/openjdk.tar.gz ${BINARY_URL}; 	  echo "${ESUM} */tmp/openjdk.tar.gz" | sha256sum -c -; 	  mkdir -p "$JAVA_HOME"; 	  tar --extract 	      --file /tmp/openjdk.tar.gz 	      --directory "$JAVA_HOME" 	      --strip-components 1 	      --no-same-owner 	  ;     rm /tmp/openjdk.tar.gz;     find "$JAVA_HOME/lib" -name '*.so' -exec dirname '{}' ';' | sort -u > /etc/ld.so.conf.d/docker-openjdk.conf;     ldconfig;     java -Xshare:dump;
# Fri, 04 Nov 2022 22:41:34 GMT
RUN echo Verifying install ...     && fileEncoding="$(echo 'System.out.println(System.getProperty("file.encoding"))' | jshell -s -)"; [ "$fileEncoding" = 'UTF-8' ]; rm -rf ~/.java     && echo java --version && java --version     && echo Complete.
# Fri, 04 Nov 2022 23:48:38 GMT
ENV CATALINA_HOME=/usr/local/tomcat
# Fri, 04 Nov 2022 23:48:38 GMT
ENV PATH=/usr/local/tomcat/bin:/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Fri, 04 Nov 2022 23:48:38 GMT
RUN mkdir -p "$CATALINA_HOME"
# Fri, 04 Nov 2022 23:48:39 GMT
WORKDIR /usr/local/tomcat
# Fri, 04 Nov 2022 23:48:39 GMT
ENV TOMCAT_NATIVE_LIBDIR=/usr/local/tomcat/native-jni-lib
# Fri, 04 Nov 2022 23:48:39 GMT
ENV LD_LIBRARY_PATH=/usr/local/tomcat/native-jni-lib
# Fri, 04 Nov 2022 23:53:12 GMT
ENV GPG_KEYS=48F8E69F6390C9F25CFEDCD268248959359E722B A9C5DF4D22E99998D9875A5110C01C5A2F6059E7 DCFD35E0BF8CA7344752DE8B6FB21E8933C60243
# Fri, 04 Nov 2022 23:53:12 GMT
ENV TOMCAT_MAJOR=9
# Tue, 15 Nov 2022 04:57:22 GMT
ENV TOMCAT_VERSION=9.0.69
# Tue, 15 Nov 2022 04:57:22 GMT
ENV TOMCAT_SHA512=8c883c54ce9ce43eba37756a6404cdf3477879883a3e6d146dc8a7aa5e0425f487466afe6b6da4a895927cb7cb59177b9379cec18000f2de12785be57408c779
# Tue, 15 Nov 2022 04:57:22 GMT
COPY dir:096b403a5f78b17e6b4bff63128a9c93941b97f22470991610dd641633d977f1 in /usr/local/tomcat 
# Tue, 15 Nov 2022 04:57:25 GMT
RUN set -eux; 	apt-get update; 	xargs -rt apt-get install -y --no-install-recommends < "$TOMCAT_NATIVE_LIBDIR/.dependencies.txt"; 	rm -rf /var/lib/apt/lists/*
# Tue, 15 Nov 2022 04:57:26 GMT
RUN set -eux; 	nativeLines="$(catalina.sh configtest 2>&1)"; 	nativeLines="$(echo "$nativeLines" | grep 'Apache Tomcat Native')"; 	nativeLines="$(echo "$nativeLines" | sort -u)"; 	if ! echo "$nativeLines" | grep -E 'INFO: Loaded( APR based)? Apache Tomcat Native library' >&2; then 		echo >&2 "$nativeLines"; 		exit 1; 	fi
# Tue, 15 Nov 2022 04:57:26 GMT
EXPOSE 8080
# Tue, 15 Nov 2022 04:57:27 GMT
CMD ["catalina.sh" "run"]
# Wed, 11 Jan 2023 03:05:10 GMT
LABEL org.opencontainers.image.authors=XWiki Development Team <committers@xwiki.org>
# Wed, 11 Jan 2023 03:05:10 GMT
LABEL org.opencontainers.image.url=https://hub.docker.com/_/xwiki
# Wed, 11 Jan 2023 03:05:10 GMT
LABEL org.opencontainers.image.documentation=https://hub.docker.com/_/xwiki
# Wed, 11 Jan 2023 03:05:10 GMT
LABEL org.opencontainers.image.source=https://github.com/xwiki/xwiki-docker.git
# Wed, 11 Jan 2023 03:05:11 GMT
LABEL org.opencontainers.image.vendor=xwiki.org
# Wed, 11 Jan 2023 03:05:11 GMT
LABEL org.opencontainers.image.licenses=LGPL-2.1
# Wed, 11 Jan 2023 03:07:37 GMT
RUN apt-get update &&   apt-get --no-install-recommends -y install     curl     libreoffice     unzip     procps &&   rm -rf /var/lib/apt/lists/*
# Tue, 31 Jan 2023 00:47:12 GMT
ENV XWIKI_VERSION=15.0
# Tue, 31 Jan 2023 00:47:12 GMT
ENV XWIKI_URL_PREFIX=https://maven.xwiki.org/releases/org/xwiki/platform/xwiki-platform-distribution-war/15.0
# Tue, 31 Jan 2023 00:47:12 GMT
ENV XWIKI_DOWNLOAD_SHA256=79ba0f479bbc49521c113821adc9d91141075a9470d7f9bbb6994ca59c30d121
# Tue, 31 Jan 2023 00:47:58 GMT
RUN rm -rf /usr/local/tomcat/webapps/* &&   mkdir -p /usr/local/tomcat/temp &&   mkdir -p /usr/local/xwiki/data &&   curl -fSL "${XWIKI_URL_PREFIX}/xwiki-platform-distribution-war-${XWIKI_VERSION}.war" -o xwiki.war &&   echo "$XWIKI_DOWNLOAD_SHA256 xwiki.war" | sha256sum -c - &&   unzip -d /usr/local/tomcat/webapps/ROOT xwiki.war &&   rm -f xwiki.war
# Tue, 31 Jan 2023 00:54:48 GMT
ENV MARIADB_JDBC_VERSION=3.1.1
# Tue, 31 Jan 2023 00:54:48 GMT
ENV MARIADB_JDBC_SHA256=a554541fd88047905fb0c4c10e1d85295f5e38c7bb5fb408b425392a79fc26e3
# Tue, 31 Jan 2023 00:54:48 GMT
ENV MARIADB_JDBC_PREFIX=https://repo1.maven.org/maven2/org/mariadb/jdbc/mariadb-java-client/3.1.1
# Tue, 31 Jan 2023 00:54:48 GMT
ENV MARIADB_JDBC_ARTIFACT=mariadb-java-client-3.1.1.jar
# Tue, 31 Jan 2023 00:54:48 GMT
ENV MARIADB_JDBC_TARGET=/usr/local/tomcat/webapps/ROOT/WEB-INF/lib/mariadb-java-client-3.1.1.jar
# Tue, 31 Jan 2023 00:54:49 GMT
RUN curl -fSL "${MARIADB_JDBC_PREFIX}/${MARIADB_JDBC_ARTIFACT}" -o $MARIADB_JDBC_TARGET &&   echo "$MARIADB_JDBC_SHA256 $MARIADB_JDBC_TARGET" | sha256sum -c -
# Tue, 31 Jan 2023 00:54:49 GMT
COPY file:0a1be11e2eb610a1dbcd415404e3a592641110b93090030cb831e3a19a163017 in /usr/local/tomcat/bin/ 
# Tue, 31 Jan 2023 00:54:49 GMT
COPY file:0e237c3876eeb3b5f3473a064d3e507da2df6c228ca714687930b34e3b687601 in /usr/local/tomcat/webapps/ROOT/WEB-INF/hibernate.cfg.xml 
# Tue, 31 Jan 2023 00:54:49 GMT
RUN sed -i 's/<id>org.xwiki.platform:xwiki-platform-distribution-war/<id>org.xwiki.platform:xwiki-platform-distribution-docker/'   /usr/local/tomcat/webapps/ROOT/META-INF/extension.xed
# Tue, 31 Jan 2023 00:54:49 GMT
COPY file:a47c4dcd87c9dad97aff38c49188357e6193bcad50757e516cfb08a60d4de611 in /usr/local/bin/docker-entrypoint.sh 
# Tue, 31 Jan 2023 00:54:49 GMT
VOLUME [/usr/local/xwiki]
# Tue, 31 Jan 2023 00:54:50 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 31 Jan 2023 00:54:50 GMT
CMD ["xwiki"]
```

-	Layers:
	-	`sha256:0509fae36eb0656f8bdb23f8ae64100d893bcea2563e97468d337e04d2d0410b`  
		Last Modified: Wed, 02 Nov 2022 18:50:21 GMT  
		Size: 28.4 MB (28382154 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e502a1af2bcd98f5f0d2f5e4da1a0e7bbe07a2c548e2662f7d37dce5ae1df46c`  
		Last Modified: Wed, 02 Nov 2022 19:48:28 GMT  
		Size: 12.4 MB (12396330 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bc4598c07dd818f03a0378b0341a4a8e80f0152fbb3e7d5246ca4f466f42e611`  
		Last Modified: Fri, 04 Nov 2022 22:46:46 GMT  
		Size: 45.0 MB (44958470 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:715a937a1066f998b331fcd62256ad01a5571bdf46804e97825afc64f9ebb427`  
		Last Modified: Fri, 04 Nov 2022 22:46:41 GMT  
		Size: 160.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5fb623f082f74b2fa9fc2c4e3f3a4802875cb9753cfa26ed940201ce72bb56cb`  
		Last Modified: Sat, 05 Nov 2022 00:03:40 GMT  
		Size: 172.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:33260b83200262bbd546be371ad3c1f50f5ae7228afb87982d6fa9d6b11bf26f`  
		Last Modified: Tue, 15 Nov 2022 05:10:19 GMT  
		Size: 12.2 MB (12207235 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0955fb697ea9b30a1b4f95385464f646aa1525cb6efba648e22df84ebef6b2ee`  
		Last Modified: Tue, 15 Nov 2022 05:10:18 GMT  
		Size: 452.0 KB (452021 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6eddcf66f2083b1487296a0308e0b058917c97f614f12428d82d89662038dc2e`  
		Last Modified: Tue, 15 Nov 2022 05:10:18 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ae5f60bb64f3fa11da3d15a9639f886186b4c2c021455c3f9db22e0cfe1b1311`  
		Last Modified: Wed, 11 Jan 2023 03:11:14 GMT  
		Size: 173.8 MB (173806827 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1814d85fce571b42f2cfa7c8a904e1a184ee6f49642242a44bbe0037088994a0`  
		Last Modified: Tue, 31 Jan 2023 00:56:04 GMT  
		Size: 307.1 MB (307117070 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e8637677b7ba0da683afa4e56ff0561e4ba77c8782d5a98da785f4ef58d1caf9`  
		Last Modified: Tue, 31 Jan 2023 00:57:14 GMT  
		Size: 589.7 KB (589677 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:61a67398bc888bcce1656edec9bb40409ce0ffc2fe83d0437c28dd64a8f697ce`  
		Last Modified: Tue, 31 Jan 2023 00:57:14 GMT  
		Size: 1.3 KB (1345 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7ebda7e506ea819ce9717c3d0334df81608bc4c7149cd47ebc9a32790141a637`  
		Last Modified: Tue, 31 Jan 2023 00:57:14 GMT  
		Size: 2.3 KB (2313 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2ceebbf08640e235a928c9df650ca3ab8d0c6b506faa158ecde5fdde34bf8813`  
		Last Modified: Tue, 31 Jan 2023 00:57:14 GMT  
		Size: 6.0 KB (6007 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:12b1d23eae23b1a09ecd4185941d43f13d4ad633d4c6257ab8107a8eebd5fb12`  
		Last Modified: Tue, 31 Jan 2023 00:57:14 GMT  
		Size: 2.5 KB (2506 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `xwiki:mysql-tomcat`

```console
$ docker pull xwiki@sha256:33e789838f82ce73efec6664859feb1ced7a5b7605fbfaddb81916716bce524f
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `xwiki:mysql-tomcat` - linux; amd64

```console
$ docker pull xwiki@sha256:481fdb46e8c043a6709d11310e2083ce71d6ba63ee6517f84da3ba06f320598e
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **590.5 MB (590459982 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:bd630aa0aa5c679e23ea7d52cbbdd6b817eab27a820c25d3c50b54eca83b9744`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["xwiki"]`

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
# Wed, 02 Nov 2022 18:44:10 GMT
RUN apt-get update     && DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends tzdata curl wget ca-certificates fontconfig locales     && echo "en_US.UTF-8 UTF-8" >> /etc/locale.gen     && locale-gen en_US.UTF-8     && rm -rf /var/lib/apt/lists/*
# Fri, 04 Nov 2022 23:21:41 GMT
ENV JAVA_VERSION=jdk-11.0.17+8
# Fri, 04 Nov 2022 23:22:31 GMT
RUN set -eux;     ARCH="$(dpkg --print-architecture)";     case "${ARCH}" in        aarch64|arm64)          ESUM='bd6efe3290c8b5a42f695a55a26f3e3c9c284288574879d4b7089f31f5114177';          BINARY_URL='https://github.com/adoptium/temurin11-binaries/releases/download/jdk-11.0.17%2B8/OpenJDK11U-jre_aarch64_linux_hotspot_11.0.17_8.tar.gz';          ;;        armhf|arm)          ESUM='8cf113d3d7fa808895c8d2e41bb890af21c47e38c2460e0588147a4bb8fc658d';          BINARY_URL='https://github.com/adoptium/temurin11-binaries/releases/download/jdk-11.0.17%2B8/OpenJDK11U-jre_arm_linux_hotspot_11.0.17_8.tar.gz';          ;;        ppc64el|powerpc:common64)          ESUM='0ca3d806131ab5834c501f9c625bb0248cd528af361c704503348e9c9605bedf';          BINARY_URL='https://github.com/adoptium/temurin11-binaries/releases/download/jdk-11.0.17%2B8/OpenJDK11U-jre_ppc64le_linux_hotspot_11.0.17_8.tar.gz';          ;;        s390x|s390:64-bit)          ESUM='dd3b159a374086e65cb07c4ccb226c90f9c02ef929cba6f0b642171d7ed97fa4';          BINARY_URL='https://github.com/adoptium/temurin11-binaries/releases/download/jdk-11.0.17%2B8/OpenJDK11U-jre_s390x_linux_hotspot_11.0.17_8.tar.gz';          ;;        amd64|i386:x86-64)          ESUM='752616097e09d7f60a3ad8bd312f90eaf50ac72577e55df229fe6e8091148f79';          BINARY_URL='https://github.com/adoptium/temurin11-binaries/releases/download/jdk-11.0.17%2B8/OpenJDK11U-jre_x64_linux_hotspot_11.0.17_8.tar.gz';          ;;        *)          echo "Unsupported arch: ${ARCH}";          exit 1;          ;;     esac; 	  wget -O /tmp/openjdk.tar.gz ${BINARY_URL}; 	  echo "${ESUM} */tmp/openjdk.tar.gz" | sha256sum -c -; 	  mkdir -p "$JAVA_HOME"; 	  tar --extract 	      --file /tmp/openjdk.tar.gz 	      --directory "$JAVA_HOME" 	      --strip-components 1 	      --no-same-owner 	  ;     rm /tmp/openjdk.tar.gz;     find "$JAVA_HOME/lib" -name '*.so' -exec dirname '{}' ';' | sort -u > /etc/ld.so.conf.d/docker-openjdk.conf;     ldconfig;     java -Xshare:dump;
# Fri, 04 Nov 2022 23:22:32 GMT
RUN echo Verifying install ...     && fileEncoding="$(echo 'System.out.println(System.getProperty("file.encoding"))' | jshell -s -)"; [ "$fileEncoding" = 'UTF-8' ]; rm -rf ~/.java     && echo java --version && java --version     && echo Complete.
# Sat, 05 Nov 2022 01:35:16 GMT
ENV CATALINA_HOME=/usr/local/tomcat
# Sat, 05 Nov 2022 01:35:16 GMT
ENV PATH=/usr/local/tomcat/bin:/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Sat, 05 Nov 2022 01:35:17 GMT
RUN mkdir -p "$CATALINA_HOME"
# Sat, 05 Nov 2022 01:35:17 GMT
WORKDIR /usr/local/tomcat
# Sat, 05 Nov 2022 01:35:17 GMT
ENV TOMCAT_NATIVE_LIBDIR=/usr/local/tomcat/native-jni-lib
# Sat, 05 Nov 2022 01:35:17 GMT
ENV LD_LIBRARY_PATH=/usr/local/tomcat/native-jni-lib
# Sat, 05 Nov 2022 01:39:54 GMT
ENV GPG_KEYS=48F8E69F6390C9F25CFEDCD268248959359E722B A9C5DF4D22E99998D9875A5110C01C5A2F6059E7 DCFD35E0BF8CA7344752DE8B6FB21E8933C60243
# Sat, 05 Nov 2022 01:39:54 GMT
ENV TOMCAT_MAJOR=9
# Tue, 15 Nov 2022 03:06:43 GMT
ENV TOMCAT_VERSION=9.0.69
# Tue, 15 Nov 2022 03:06:43 GMT
ENV TOMCAT_SHA512=8c883c54ce9ce43eba37756a6404cdf3477879883a3e6d146dc8a7aa5e0425f487466afe6b6da4a895927cb7cb59177b9379cec18000f2de12785be57408c779
# Tue, 15 Nov 2022 03:06:44 GMT
COPY dir:b1a33aa3993dbbfbebb33bd9aa546b60c2f2191abf1227f453d4e830f6deb35f in /usr/local/tomcat 
# Tue, 15 Nov 2022 03:06:48 GMT
RUN set -eux; 	apt-get update; 	xargs -rt apt-get install -y --no-install-recommends < "$TOMCAT_NATIVE_LIBDIR/.dependencies.txt"; 	rm -rf /var/lib/apt/lists/*
# Tue, 15 Nov 2022 03:06:49 GMT
RUN set -eux; 	nativeLines="$(catalina.sh configtest 2>&1)"; 	nativeLines="$(echo "$nativeLines" | grep 'Apache Tomcat Native')"; 	nativeLines="$(echo "$nativeLines" | sort -u)"; 	if ! echo "$nativeLines" | grep -E 'INFO: Loaded( APR based)? Apache Tomcat Native library' >&2; then 		echo >&2 "$nativeLines"; 		exit 1; 	fi
# Tue, 15 Nov 2022 03:06:49 GMT
EXPOSE 8080
# Tue, 15 Nov 2022 03:06:49 GMT
CMD ["catalina.sh" "run"]
# Wed, 11 Jan 2023 02:47:03 GMT
LABEL org.opencontainers.image.authors=XWiki Development Team <committers@xwiki.org>
# Wed, 11 Jan 2023 02:47:03 GMT
LABEL org.opencontainers.image.url=https://hub.docker.com/_/xwiki
# Wed, 11 Jan 2023 02:47:03 GMT
LABEL org.opencontainers.image.documentation=https://hub.docker.com/_/xwiki
# Wed, 11 Jan 2023 02:47:03 GMT
LABEL org.opencontainers.image.source=https://github.com/xwiki/xwiki-docker.git
# Wed, 11 Jan 2023 02:47:04 GMT
LABEL org.opencontainers.image.vendor=xwiki.org
# Wed, 11 Jan 2023 02:47:04 GMT
LABEL org.opencontainers.image.licenses=LGPL-2.1
# Wed, 11 Jan 2023 02:49:03 GMT
RUN apt-get update &&   apt-get --no-install-recommends -y install     curl     libreoffice     unzip     procps &&   rm -rf /var/lib/apt/lists/*
# Tue, 31 Jan 2023 00:20:17 GMT
ENV XWIKI_VERSION=15.0
# Tue, 31 Jan 2023 00:20:17 GMT
ENV XWIKI_URL_PREFIX=https://maven.xwiki.org/releases/org/xwiki/platform/xwiki-platform-distribution-war/15.0
# Tue, 31 Jan 2023 00:20:17 GMT
ENV XWIKI_DOWNLOAD_SHA256=79ba0f479bbc49521c113821adc9d91141075a9470d7f9bbb6994ca59c30d121
# Tue, 31 Jan 2023 00:21:18 GMT
RUN rm -rf /usr/local/tomcat/webapps/* &&   mkdir -p /usr/local/tomcat/temp &&   mkdir -p /usr/local/xwiki/data &&   curl -fSL "${XWIKI_URL_PREFIX}/xwiki-platform-distribution-war-${XWIKI_VERSION}.war" -o xwiki.war &&   echo "$XWIKI_DOWNLOAD_SHA256 xwiki.war" | sha256sum -c - &&   unzip -d /usr/local/tomcat/webapps/ROOT xwiki.war &&   rm -f xwiki.war
# Tue, 31 Jan 2023 00:21:19 GMT
ENV MYSQL_JDBC_VERSION=8.0.31
# Tue, 31 Jan 2023 00:21:19 GMT
ENV MYSQL_JDBC_SHA256=5249e3dc6d6531b37790e3f61845b96db5e41e891d3d8edb0e2e3a1b53ca2f4f
# Tue, 31 Jan 2023 00:21:19 GMT
ENV MYSQL_JDBC_PREFIX=https://repo1.maven.org/maven2/com/mysql/mysql-connector-j/8.0.31
# Tue, 31 Jan 2023 00:21:19 GMT
ENV MYSQL_JDBC_ARTIFACT=mysql-connector-j-8.0.31.jar
# Tue, 31 Jan 2023 00:21:19 GMT
ENV MYSQL_JDBC_TARGET=/usr/local/tomcat/webapps/ROOT/WEB-INF/lib/mysql-connector-j-8.0.31.jar
# Tue, 31 Jan 2023 00:21:20 GMT
RUN curl -fSL "${MYSQL_JDBC_PREFIX}/${MYSQL_JDBC_ARTIFACT}" -o $MYSQL_JDBC_TARGET &&   echo "$MYSQL_JDBC_SHA256 $MYSQL_JDBC_TARGET" | sha256sum -c -
# Tue, 31 Jan 2023 00:21:21 GMT
COPY file:0a1be11e2eb610a1dbcd415404e3a592641110b93090030cb831e3a19a163017 in /usr/local/tomcat/bin/ 
# Tue, 31 Jan 2023 00:21:21 GMT
COPY file:1b8409986f3e4eb79a7a0b18472cb2692a61d504fb5ef34292bc997b79fd760d in /usr/local/tomcat/webapps/ROOT/WEB-INF/hibernate.cfg.xml 
# Tue, 31 Jan 2023 00:21:21 GMT
RUN sed -i 's/<id>org.xwiki.platform:xwiki-platform-distribution-war/<id>org.xwiki.platform:xwiki-platform-distribution-docker/'   /usr/local/tomcat/webapps/ROOT/META-INF/extension.xed
# Tue, 31 Jan 2023 00:21:21 GMT
COPY file:a47c4dcd87c9dad97aff38c49188357e6193bcad50757e516cfb08a60d4de611 in /usr/local/bin/docker-entrypoint.sh 
# Tue, 31 Jan 2023 00:21:22 GMT
VOLUME [/usr/local/xwiki]
# Tue, 31 Jan 2023 00:21:22 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 31 Jan 2023 00:21:22 GMT
CMD ["xwiki"]
```

-	Layers:
	-	`sha256:e96e057aae67380a4ddb16c337c5c3669d97fdff69ec537f02aa2cc30d814281`  
		Last Modified: Wed, 02 Nov 2022 03:03:36 GMT  
		Size: 30.4 MB (30425607 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4ced2591451da3a02e2b6bb44752b9e3f00d77789921be4df5082fb9f9880ad0`  
		Last Modified: Wed, 02 Nov 2022 18:48:43 GMT  
		Size: 12.4 MB (12439006 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:df8f874ae8c08a9e69e5fbe6c5a64200a45386132a3203d1a9a7f1146d94cfbc`  
		Last Modified: Fri, 04 Nov 2022 23:29:33 GMT  
		Size: 46.6 MB (46629936 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:111b6c7486426c4b6989102c2ee5be856e8a58e20ab0a350b24a905d536e8e7f`  
		Last Modified: Fri, 04 Nov 2022 23:29:26 GMT  
		Size: 161.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e6f84dce457c6d4f7b7291fce05f8e77998a3a7722a54125a1f1d52ca83043b4`  
		Last Modified: Sat, 05 Nov 2022 01:50:51 GMT  
		Size: 173.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a6c26749ee782392e38845ee2ba79b0da586ef6a45d8e7f29c7af14612278547`  
		Last Modified: Tue, 15 Nov 2022 03:19:57 GMT  
		Size: 12.2 MB (12200249 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4dddc6d9fa6024025b3fcfe729cab2dc544fb25476eca6e80b1af8e8d93bb0ee`  
		Last Modified: Tue, 15 Nov 2022 03:19:56 GMT  
		Size: 452.7 KB (452680 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:06637eebe5e72c8ad9019ad4eb4cdde1f11f7d4c24c7ed7374cf8966343aa2fb`  
		Last Modified: Tue, 15 Nov 2022 03:19:56 GMT  
		Size: 131.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b276fb8390410a8208724033e325715ea26000d5a1a762d4c3699b927884fbfe`  
		Last Modified: Wed, 11 Jan 2023 02:52:45 GMT  
		Size: 178.8 MB (178805608 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:156ca91198173149698aa0396648a9608b6ab1f2bc2666800843ce33c9f85b6e`  
		Last Modified: Tue, 31 Jan 2023 00:24:09 GMT  
		Size: 307.1 MB (307117069 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4c8b70d250c6d507901857473b0dcb67132d7b2a30ce9a69b07b1036853df738`  
		Last Modified: Tue, 31 Jan 2023 00:23:52 GMT  
		Size: 2.4 MB (2377191 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a9681fd36be674d25231c69d6a39f9e8fa65034eeaef5d1bd885fdbeac7f0f6b`  
		Last Modified: Tue, 31 Jan 2023 00:23:51 GMT  
		Size: 1.3 KB (1346 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a9d0d5da840f4d7da9943942b38cd092fae11f41dc6c19afd58d655cd6192d66`  
		Last Modified: Tue, 31 Jan 2023 00:23:51 GMT  
		Size: 2.3 KB (2312 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d65610da4f1da86fea8fbec0189b066afd4b86e4e8f7d049e3c4bc6ade9ba90a`  
		Last Modified: Tue, 31 Jan 2023 00:23:51 GMT  
		Size: 6.0 KB (6009 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3d41686284d7675eaa0f92c9cc27ebe73b4c30768c8eef9f23ee3b1ad06da00a`  
		Last Modified: Tue, 31 Jan 2023 00:23:51 GMT  
		Size: 2.5 KB (2504 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `xwiki:mysql-tomcat` - linux; arm64 variant v8

```console
$ docker pull xwiki@sha256:6bf63d9025b07b69d744200c05efd4ffb8a52f3c38380f5d59a0b48514203cd2
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **581.7 MB (581709921 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:6600f2bb05836c703d53944bbcb5399d509a9813a27a35e99ff717becc308330`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["xwiki"]`

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
# Wed, 02 Nov 2022 19:44:32 GMT
RUN apt-get update     && DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends tzdata curl wget ca-certificates fontconfig locales     && echo "en_US.UTF-8 UTF-8" >> /etc/locale.gen     && locale-gen en_US.UTF-8     && rm -rf /var/lib/apt/lists/*
# Fri, 04 Nov 2022 22:40:54 GMT
ENV JAVA_VERSION=jdk-11.0.17+8
# Fri, 04 Nov 2022 22:41:33 GMT
RUN set -eux;     ARCH="$(dpkg --print-architecture)";     case "${ARCH}" in        aarch64|arm64)          ESUM='bd6efe3290c8b5a42f695a55a26f3e3c9c284288574879d4b7089f31f5114177';          BINARY_URL='https://github.com/adoptium/temurin11-binaries/releases/download/jdk-11.0.17%2B8/OpenJDK11U-jre_aarch64_linux_hotspot_11.0.17_8.tar.gz';          ;;        armhf|arm)          ESUM='8cf113d3d7fa808895c8d2e41bb890af21c47e38c2460e0588147a4bb8fc658d';          BINARY_URL='https://github.com/adoptium/temurin11-binaries/releases/download/jdk-11.0.17%2B8/OpenJDK11U-jre_arm_linux_hotspot_11.0.17_8.tar.gz';          ;;        ppc64el|powerpc:common64)          ESUM='0ca3d806131ab5834c501f9c625bb0248cd528af361c704503348e9c9605bedf';          BINARY_URL='https://github.com/adoptium/temurin11-binaries/releases/download/jdk-11.0.17%2B8/OpenJDK11U-jre_ppc64le_linux_hotspot_11.0.17_8.tar.gz';          ;;        s390x|s390:64-bit)          ESUM='dd3b159a374086e65cb07c4ccb226c90f9c02ef929cba6f0b642171d7ed97fa4';          BINARY_URL='https://github.com/adoptium/temurin11-binaries/releases/download/jdk-11.0.17%2B8/OpenJDK11U-jre_s390x_linux_hotspot_11.0.17_8.tar.gz';          ;;        amd64|i386:x86-64)          ESUM='752616097e09d7f60a3ad8bd312f90eaf50ac72577e55df229fe6e8091148f79';          BINARY_URL='https://github.com/adoptium/temurin11-binaries/releases/download/jdk-11.0.17%2B8/OpenJDK11U-jre_x64_linux_hotspot_11.0.17_8.tar.gz';          ;;        *)          echo "Unsupported arch: ${ARCH}";          exit 1;          ;;     esac; 	  wget -O /tmp/openjdk.tar.gz ${BINARY_URL}; 	  echo "${ESUM} */tmp/openjdk.tar.gz" | sha256sum -c -; 	  mkdir -p "$JAVA_HOME"; 	  tar --extract 	      --file /tmp/openjdk.tar.gz 	      --directory "$JAVA_HOME" 	      --strip-components 1 	      --no-same-owner 	  ;     rm /tmp/openjdk.tar.gz;     find "$JAVA_HOME/lib" -name '*.so' -exec dirname '{}' ';' | sort -u > /etc/ld.so.conf.d/docker-openjdk.conf;     ldconfig;     java -Xshare:dump;
# Fri, 04 Nov 2022 22:41:34 GMT
RUN echo Verifying install ...     && fileEncoding="$(echo 'System.out.println(System.getProperty("file.encoding"))' | jshell -s -)"; [ "$fileEncoding" = 'UTF-8' ]; rm -rf ~/.java     && echo java --version && java --version     && echo Complete.
# Fri, 04 Nov 2022 23:48:38 GMT
ENV CATALINA_HOME=/usr/local/tomcat
# Fri, 04 Nov 2022 23:48:38 GMT
ENV PATH=/usr/local/tomcat/bin:/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Fri, 04 Nov 2022 23:48:38 GMT
RUN mkdir -p "$CATALINA_HOME"
# Fri, 04 Nov 2022 23:48:39 GMT
WORKDIR /usr/local/tomcat
# Fri, 04 Nov 2022 23:48:39 GMT
ENV TOMCAT_NATIVE_LIBDIR=/usr/local/tomcat/native-jni-lib
# Fri, 04 Nov 2022 23:48:39 GMT
ENV LD_LIBRARY_PATH=/usr/local/tomcat/native-jni-lib
# Fri, 04 Nov 2022 23:53:12 GMT
ENV GPG_KEYS=48F8E69F6390C9F25CFEDCD268248959359E722B A9C5DF4D22E99998D9875A5110C01C5A2F6059E7 DCFD35E0BF8CA7344752DE8B6FB21E8933C60243
# Fri, 04 Nov 2022 23:53:12 GMT
ENV TOMCAT_MAJOR=9
# Tue, 15 Nov 2022 04:57:22 GMT
ENV TOMCAT_VERSION=9.0.69
# Tue, 15 Nov 2022 04:57:22 GMT
ENV TOMCAT_SHA512=8c883c54ce9ce43eba37756a6404cdf3477879883a3e6d146dc8a7aa5e0425f487466afe6b6da4a895927cb7cb59177b9379cec18000f2de12785be57408c779
# Tue, 15 Nov 2022 04:57:22 GMT
COPY dir:096b403a5f78b17e6b4bff63128a9c93941b97f22470991610dd641633d977f1 in /usr/local/tomcat 
# Tue, 15 Nov 2022 04:57:25 GMT
RUN set -eux; 	apt-get update; 	xargs -rt apt-get install -y --no-install-recommends < "$TOMCAT_NATIVE_LIBDIR/.dependencies.txt"; 	rm -rf /var/lib/apt/lists/*
# Tue, 15 Nov 2022 04:57:26 GMT
RUN set -eux; 	nativeLines="$(catalina.sh configtest 2>&1)"; 	nativeLines="$(echo "$nativeLines" | grep 'Apache Tomcat Native')"; 	nativeLines="$(echo "$nativeLines" | sort -u)"; 	if ! echo "$nativeLines" | grep -E 'INFO: Loaded( APR based)? Apache Tomcat Native library' >&2; then 		echo >&2 "$nativeLines"; 		exit 1; 	fi
# Tue, 15 Nov 2022 04:57:26 GMT
EXPOSE 8080
# Tue, 15 Nov 2022 04:57:27 GMT
CMD ["catalina.sh" "run"]
# Wed, 11 Jan 2023 03:05:10 GMT
LABEL org.opencontainers.image.authors=XWiki Development Team <committers@xwiki.org>
# Wed, 11 Jan 2023 03:05:10 GMT
LABEL org.opencontainers.image.url=https://hub.docker.com/_/xwiki
# Wed, 11 Jan 2023 03:05:10 GMT
LABEL org.opencontainers.image.documentation=https://hub.docker.com/_/xwiki
# Wed, 11 Jan 2023 03:05:10 GMT
LABEL org.opencontainers.image.source=https://github.com/xwiki/xwiki-docker.git
# Wed, 11 Jan 2023 03:05:11 GMT
LABEL org.opencontainers.image.vendor=xwiki.org
# Wed, 11 Jan 2023 03:05:11 GMT
LABEL org.opencontainers.image.licenses=LGPL-2.1
# Wed, 11 Jan 2023 03:07:37 GMT
RUN apt-get update &&   apt-get --no-install-recommends -y install     curl     libreoffice     unzip     procps &&   rm -rf /var/lib/apt/lists/*
# Tue, 31 Jan 2023 00:47:12 GMT
ENV XWIKI_VERSION=15.0
# Tue, 31 Jan 2023 00:47:12 GMT
ENV XWIKI_URL_PREFIX=https://maven.xwiki.org/releases/org/xwiki/platform/xwiki-platform-distribution-war/15.0
# Tue, 31 Jan 2023 00:47:12 GMT
ENV XWIKI_DOWNLOAD_SHA256=79ba0f479bbc49521c113821adc9d91141075a9470d7f9bbb6994ca59c30d121
# Tue, 31 Jan 2023 00:47:58 GMT
RUN rm -rf /usr/local/tomcat/webapps/* &&   mkdir -p /usr/local/tomcat/temp &&   mkdir -p /usr/local/xwiki/data &&   curl -fSL "${XWIKI_URL_PREFIX}/xwiki-platform-distribution-war-${XWIKI_VERSION}.war" -o xwiki.war &&   echo "$XWIKI_DOWNLOAD_SHA256 xwiki.war" | sha256sum -c - &&   unzip -d /usr/local/tomcat/webapps/ROOT xwiki.war &&   rm -f xwiki.war
# Tue, 31 Jan 2023 00:48:01 GMT
ENV MYSQL_JDBC_VERSION=8.0.31
# Tue, 31 Jan 2023 00:48:01 GMT
ENV MYSQL_JDBC_SHA256=5249e3dc6d6531b37790e3f61845b96db5e41e891d3d8edb0e2e3a1b53ca2f4f
# Tue, 31 Jan 2023 00:48:01 GMT
ENV MYSQL_JDBC_PREFIX=https://repo1.maven.org/maven2/com/mysql/mysql-connector-j/8.0.31
# Tue, 31 Jan 2023 00:48:01 GMT
ENV MYSQL_JDBC_ARTIFACT=mysql-connector-j-8.0.31.jar
# Tue, 31 Jan 2023 00:48:01 GMT
ENV MYSQL_JDBC_TARGET=/usr/local/tomcat/webapps/ROOT/WEB-INF/lib/mysql-connector-j-8.0.31.jar
# Tue, 31 Jan 2023 00:48:02 GMT
RUN curl -fSL "${MYSQL_JDBC_PREFIX}/${MYSQL_JDBC_ARTIFACT}" -o $MYSQL_JDBC_TARGET &&   echo "$MYSQL_JDBC_SHA256 $MYSQL_JDBC_TARGET" | sha256sum -c -
# Tue, 31 Jan 2023 00:48:02 GMT
COPY file:0a1be11e2eb610a1dbcd415404e3a592641110b93090030cb831e3a19a163017 in /usr/local/tomcat/bin/ 
# Tue, 31 Jan 2023 00:48:02 GMT
COPY file:1b8409986f3e4eb79a7a0b18472cb2692a61d504fb5ef34292bc997b79fd760d in /usr/local/tomcat/webapps/ROOT/WEB-INF/hibernate.cfg.xml 
# Tue, 31 Jan 2023 00:48:03 GMT
RUN sed -i 's/<id>org.xwiki.platform:xwiki-platform-distribution-war/<id>org.xwiki.platform:xwiki-platform-distribution-docker/'   /usr/local/tomcat/webapps/ROOT/META-INF/extension.xed
# Tue, 31 Jan 2023 00:48:03 GMT
COPY file:a47c4dcd87c9dad97aff38c49188357e6193bcad50757e516cfb08a60d4de611 in /usr/local/bin/docker-entrypoint.sh 
# Tue, 31 Jan 2023 00:48:03 GMT
VOLUME [/usr/local/xwiki]
# Tue, 31 Jan 2023 00:48:03 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 31 Jan 2023 00:48:03 GMT
CMD ["xwiki"]
```

-	Layers:
	-	`sha256:0509fae36eb0656f8bdb23f8ae64100d893bcea2563e97468d337e04d2d0410b`  
		Last Modified: Wed, 02 Nov 2022 18:50:21 GMT  
		Size: 28.4 MB (28382154 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e502a1af2bcd98f5f0d2f5e4da1a0e7bbe07a2c548e2662f7d37dce5ae1df46c`  
		Last Modified: Wed, 02 Nov 2022 19:48:28 GMT  
		Size: 12.4 MB (12396330 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bc4598c07dd818f03a0378b0341a4a8e80f0152fbb3e7d5246ca4f466f42e611`  
		Last Modified: Fri, 04 Nov 2022 22:46:46 GMT  
		Size: 45.0 MB (44958470 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:715a937a1066f998b331fcd62256ad01a5571bdf46804e97825afc64f9ebb427`  
		Last Modified: Fri, 04 Nov 2022 22:46:41 GMT  
		Size: 160.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5fb623f082f74b2fa9fc2c4e3f3a4802875cb9753cfa26ed940201ce72bb56cb`  
		Last Modified: Sat, 05 Nov 2022 00:03:40 GMT  
		Size: 172.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:33260b83200262bbd546be371ad3c1f50f5ae7228afb87982d6fa9d6b11bf26f`  
		Last Modified: Tue, 15 Nov 2022 05:10:19 GMT  
		Size: 12.2 MB (12207235 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0955fb697ea9b30a1b4f95385464f646aa1525cb6efba648e22df84ebef6b2ee`  
		Last Modified: Tue, 15 Nov 2022 05:10:18 GMT  
		Size: 452.0 KB (452021 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6eddcf66f2083b1487296a0308e0b058917c97f614f12428d82d89662038dc2e`  
		Last Modified: Tue, 15 Nov 2022 05:10:18 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ae5f60bb64f3fa11da3d15a9639f886186b4c2c021455c3f9db22e0cfe1b1311`  
		Last Modified: Wed, 11 Jan 2023 03:11:14 GMT  
		Size: 173.8 MB (173806827 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1814d85fce571b42f2cfa7c8a904e1a184ee6f49642242a44bbe0037088994a0`  
		Last Modified: Tue, 31 Jan 2023 00:56:04 GMT  
		Size: 307.1 MB (307117070 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8aec0e24b4fa870989f014944c3c7d535355a2371fc8c948b2b11f9b377efe6e`  
		Last Modified: Tue, 31 Jan 2023 00:55:50 GMT  
		Size: 2.4 MB (2377182 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0b65081619aa0114a7f367836ef421eb8d951e559e0f089c7728af7813b1ea62`  
		Last Modified: Tue, 31 Jan 2023 00:55:49 GMT  
		Size: 1.3 KB (1348 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:46ebad072e608146426d8dc30828937049eea36c2e636d7790b4960d6d586977`  
		Last Modified: Tue, 31 Jan 2023 00:55:49 GMT  
		Size: 2.3 KB (2308 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:708fefcedd4ee6c106da247a68c5790f5ab00225d1cdfff8465575265c3a54e6`  
		Last Modified: Tue, 31 Jan 2023 00:55:49 GMT  
		Size: 6.0 KB (6008 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:81e3bf8e20bc921031e7549a41dec1b2d7795cc6da40a0e7096bf654b25c5c3e`  
		Last Modified: Tue, 31 Jan 2023 00:55:49 GMT  
		Size: 2.5 KB (2507 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `xwiki:postgres-tomcat`

```console
$ docker pull xwiki@sha256:f6739c1133cbbece87973ddea5fbc57222abb9d7d3f8064eee9d2c2c0d46ecfa
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `xwiki:postgres-tomcat` - linux; amd64

```console
$ docker pull xwiki@sha256:72928baeace929e42f17f01362700392a90c6750b2ec1f84f24bbba1c4ff0236
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **590.0 MB (589959353 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b71f03d7d3a1760e73e6f4370f49317d16a7e0cb22532f49c11c0ee73b2c6262`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["xwiki"]`

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
# Wed, 02 Nov 2022 18:44:10 GMT
RUN apt-get update     && DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends tzdata curl wget ca-certificates fontconfig locales     && echo "en_US.UTF-8 UTF-8" >> /etc/locale.gen     && locale-gen en_US.UTF-8     && rm -rf /var/lib/apt/lists/*
# Fri, 04 Nov 2022 23:21:41 GMT
ENV JAVA_VERSION=jdk-11.0.17+8
# Fri, 04 Nov 2022 23:22:31 GMT
RUN set -eux;     ARCH="$(dpkg --print-architecture)";     case "${ARCH}" in        aarch64|arm64)          ESUM='bd6efe3290c8b5a42f695a55a26f3e3c9c284288574879d4b7089f31f5114177';          BINARY_URL='https://github.com/adoptium/temurin11-binaries/releases/download/jdk-11.0.17%2B8/OpenJDK11U-jre_aarch64_linux_hotspot_11.0.17_8.tar.gz';          ;;        armhf|arm)          ESUM='8cf113d3d7fa808895c8d2e41bb890af21c47e38c2460e0588147a4bb8fc658d';          BINARY_URL='https://github.com/adoptium/temurin11-binaries/releases/download/jdk-11.0.17%2B8/OpenJDK11U-jre_arm_linux_hotspot_11.0.17_8.tar.gz';          ;;        ppc64el|powerpc:common64)          ESUM='0ca3d806131ab5834c501f9c625bb0248cd528af361c704503348e9c9605bedf';          BINARY_URL='https://github.com/adoptium/temurin11-binaries/releases/download/jdk-11.0.17%2B8/OpenJDK11U-jre_ppc64le_linux_hotspot_11.0.17_8.tar.gz';          ;;        s390x|s390:64-bit)          ESUM='dd3b159a374086e65cb07c4ccb226c90f9c02ef929cba6f0b642171d7ed97fa4';          BINARY_URL='https://github.com/adoptium/temurin11-binaries/releases/download/jdk-11.0.17%2B8/OpenJDK11U-jre_s390x_linux_hotspot_11.0.17_8.tar.gz';          ;;        amd64|i386:x86-64)          ESUM='752616097e09d7f60a3ad8bd312f90eaf50ac72577e55df229fe6e8091148f79';          BINARY_URL='https://github.com/adoptium/temurin11-binaries/releases/download/jdk-11.0.17%2B8/OpenJDK11U-jre_x64_linux_hotspot_11.0.17_8.tar.gz';          ;;        *)          echo "Unsupported arch: ${ARCH}";          exit 1;          ;;     esac; 	  wget -O /tmp/openjdk.tar.gz ${BINARY_URL}; 	  echo "${ESUM} */tmp/openjdk.tar.gz" | sha256sum -c -; 	  mkdir -p "$JAVA_HOME"; 	  tar --extract 	      --file /tmp/openjdk.tar.gz 	      --directory "$JAVA_HOME" 	      --strip-components 1 	      --no-same-owner 	  ;     rm /tmp/openjdk.tar.gz;     find "$JAVA_HOME/lib" -name '*.so' -exec dirname '{}' ';' | sort -u > /etc/ld.so.conf.d/docker-openjdk.conf;     ldconfig;     java -Xshare:dump;
# Fri, 04 Nov 2022 23:22:32 GMT
RUN echo Verifying install ...     && fileEncoding="$(echo 'System.out.println(System.getProperty("file.encoding"))' | jshell -s -)"; [ "$fileEncoding" = 'UTF-8' ]; rm -rf ~/.java     && echo java --version && java --version     && echo Complete.
# Sat, 05 Nov 2022 01:35:16 GMT
ENV CATALINA_HOME=/usr/local/tomcat
# Sat, 05 Nov 2022 01:35:16 GMT
ENV PATH=/usr/local/tomcat/bin:/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Sat, 05 Nov 2022 01:35:17 GMT
RUN mkdir -p "$CATALINA_HOME"
# Sat, 05 Nov 2022 01:35:17 GMT
WORKDIR /usr/local/tomcat
# Sat, 05 Nov 2022 01:35:17 GMT
ENV TOMCAT_NATIVE_LIBDIR=/usr/local/tomcat/native-jni-lib
# Sat, 05 Nov 2022 01:35:17 GMT
ENV LD_LIBRARY_PATH=/usr/local/tomcat/native-jni-lib
# Sat, 05 Nov 2022 01:39:54 GMT
ENV GPG_KEYS=48F8E69F6390C9F25CFEDCD268248959359E722B A9C5DF4D22E99998D9875A5110C01C5A2F6059E7 DCFD35E0BF8CA7344752DE8B6FB21E8933C60243
# Sat, 05 Nov 2022 01:39:54 GMT
ENV TOMCAT_MAJOR=9
# Tue, 15 Nov 2022 03:06:43 GMT
ENV TOMCAT_VERSION=9.0.69
# Tue, 15 Nov 2022 03:06:43 GMT
ENV TOMCAT_SHA512=8c883c54ce9ce43eba37756a6404cdf3477879883a3e6d146dc8a7aa5e0425f487466afe6b6da4a895927cb7cb59177b9379cec18000f2de12785be57408c779
# Tue, 15 Nov 2022 03:06:44 GMT
COPY dir:b1a33aa3993dbbfbebb33bd9aa546b60c2f2191abf1227f453d4e830f6deb35f in /usr/local/tomcat 
# Tue, 15 Nov 2022 03:06:48 GMT
RUN set -eux; 	apt-get update; 	xargs -rt apt-get install -y --no-install-recommends < "$TOMCAT_NATIVE_LIBDIR/.dependencies.txt"; 	rm -rf /var/lib/apt/lists/*
# Tue, 15 Nov 2022 03:06:49 GMT
RUN set -eux; 	nativeLines="$(catalina.sh configtest 2>&1)"; 	nativeLines="$(echo "$nativeLines" | grep 'Apache Tomcat Native')"; 	nativeLines="$(echo "$nativeLines" | sort -u)"; 	if ! echo "$nativeLines" | grep -E 'INFO: Loaded( APR based)? Apache Tomcat Native library' >&2; then 		echo >&2 "$nativeLines"; 		exit 1; 	fi
# Tue, 15 Nov 2022 03:06:49 GMT
EXPOSE 8080
# Tue, 15 Nov 2022 03:06:49 GMT
CMD ["catalina.sh" "run"]
# Wed, 11 Jan 2023 02:47:03 GMT
LABEL org.opencontainers.image.authors=XWiki Development Team <committers@xwiki.org>
# Wed, 11 Jan 2023 02:47:03 GMT
LABEL org.opencontainers.image.url=https://hub.docker.com/_/xwiki
# Wed, 11 Jan 2023 02:47:03 GMT
LABEL org.opencontainers.image.documentation=https://hub.docker.com/_/xwiki
# Wed, 11 Jan 2023 02:47:03 GMT
LABEL org.opencontainers.image.source=https://github.com/xwiki/xwiki-docker.git
# Wed, 11 Jan 2023 02:47:04 GMT
LABEL org.opencontainers.image.vendor=xwiki.org
# Wed, 11 Jan 2023 02:47:04 GMT
LABEL org.opencontainers.image.licenses=LGPL-2.1
# Wed, 11 Jan 2023 02:50:25 GMT
RUN apt-get update &&   apt-get --no-install-recommends -y install     curl     libreoffice     unzip     procps     libpostgresql-jdbc-java &&   rm -rf /var/lib/apt/lists/*
# Tue, 31 Jan 2023 00:21:26 GMT
ENV XWIKI_VERSION=15.0
# Tue, 31 Jan 2023 00:21:27 GMT
ENV XWIKI_URL_PREFIX=https://maven.xwiki.org/releases/org/xwiki/platform/xwiki-platform-distribution-war/15.0
# Tue, 31 Jan 2023 00:21:27 GMT
ENV XWIKI_DOWNLOAD_SHA256=79ba0f479bbc49521c113821adc9d91141075a9470d7f9bbb6994ca59c30d121
# Tue, 31 Jan 2023 00:22:39 GMT
RUN rm -rf /usr/local/tomcat/webapps/* &&   mkdir -p /usr/local/tomcat/temp &&   mkdir -p /usr/local/xwiki/data &&   curl -fSL "${XWIKI_URL_PREFIX}/xwiki-platform-distribution-war-${XWIKI_VERSION}.war" -o xwiki.war &&   echo "$XWIKI_DOWNLOAD_SHA256 xwiki.war" | sha256sum -c - &&   unzip -d /usr/local/tomcat/webapps/ROOT xwiki.war &&   rm -f xwiki.war
# Tue, 31 Jan 2023 00:22:40 GMT
RUN cp /usr/share/java/postgresql-jdbc4.jar /usr/local/tomcat/webapps/ROOT/WEB-INF/lib/
# Tue, 31 Jan 2023 00:22:41 GMT
COPY file:0a1be11e2eb610a1dbcd415404e3a592641110b93090030cb831e3a19a163017 in /usr/local/tomcat/bin/ 
# Tue, 31 Jan 2023 00:22:41 GMT
COPY file:4a923f484bb29a26630c19e1d617d3bf6aa6ae7c6c4a5561e97b037bcde0847c in /usr/local/tomcat/webapps/ROOT/WEB-INF/hibernate.cfg.xml 
# Tue, 31 Jan 2023 00:22:41 GMT
RUN sed -i 's/<id>org.xwiki.platform:xwiki-platform-distribution-war/<id>org.xwiki.platform:xwiki-platform-distribution-docker/'   /usr/local/tomcat/webapps/ROOT/META-INF/extension.xed
# Tue, 31 Jan 2023 00:22:41 GMT
COPY file:a47c4dcd87c9dad97aff38c49188357e6193bcad50757e516cfb08a60d4de611 in /usr/local/bin/docker-entrypoint.sh 
# Tue, 31 Jan 2023 00:22:41 GMT
VOLUME [/usr/local/xwiki]
# Tue, 31 Jan 2023 00:22:42 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 31 Jan 2023 00:22:42 GMT
CMD ["xwiki"]
```

-	Layers:
	-	`sha256:e96e057aae67380a4ddb16c337c5c3669d97fdff69ec537f02aa2cc30d814281`  
		Last Modified: Wed, 02 Nov 2022 03:03:36 GMT  
		Size: 30.4 MB (30425607 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4ced2591451da3a02e2b6bb44752b9e3f00d77789921be4df5082fb9f9880ad0`  
		Last Modified: Wed, 02 Nov 2022 18:48:43 GMT  
		Size: 12.4 MB (12439006 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:df8f874ae8c08a9e69e5fbe6c5a64200a45386132a3203d1a9a7f1146d94cfbc`  
		Last Modified: Fri, 04 Nov 2022 23:29:33 GMT  
		Size: 46.6 MB (46629936 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:111b6c7486426c4b6989102c2ee5be856e8a58e20ab0a350b24a905d536e8e7f`  
		Last Modified: Fri, 04 Nov 2022 23:29:26 GMT  
		Size: 161.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e6f84dce457c6d4f7b7291fce05f8e77998a3a7722a54125a1f1d52ca83043b4`  
		Last Modified: Sat, 05 Nov 2022 01:50:51 GMT  
		Size: 173.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a6c26749ee782392e38845ee2ba79b0da586ef6a45d8e7f29c7af14612278547`  
		Last Modified: Tue, 15 Nov 2022 03:19:57 GMT  
		Size: 12.2 MB (12200249 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4dddc6d9fa6024025b3fcfe729cab2dc544fb25476eca6e80b1af8e8d93bb0ee`  
		Last Modified: Tue, 15 Nov 2022 03:19:56 GMT  
		Size: 452.7 KB (452680 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:06637eebe5e72c8ad9019ad4eb4cdde1f11f7d4c24c7ed7374cf8966343aa2fb`  
		Last Modified: Tue, 15 Nov 2022 03:19:56 GMT  
		Size: 131.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b57f6f8bcfb0d93b8e21d3068d1f65d3f08dba05c5fab7d4c36e2359317b18c7`  
		Last Modified: Wed, 11 Jan 2023 02:53:53 GMT  
		Size: 179.7 MB (179745182 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:71a0aee972ff5a36a4c5d67f5bf6416b1b78d06c906ce727c5e8e11098d0dfd1`  
		Last Modified: Tue, 31 Jan 2023 00:25:01 GMT  
		Size: 307.1 MB (307117070 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ccc745f1273896cef68a5af6cd5713c4a2d8704628920a53e318a008f8096426`  
		Last Modified: Tue, 31 Jan 2023 00:24:44 GMT  
		Size: 936.8 KB (936848 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1593979548bc568ed36dc9f5adb8f00d8b7d3eb1fa850fc06426c2c9345b8472`  
		Last Modified: Tue, 31 Jan 2023 00:24:43 GMT  
		Size: 1.3 KB (1345 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e1e58b32c2c2a52907f7e4ad05462d3b2afd11404a9678bc656fb96029b12d8d`  
		Last Modified: Tue, 31 Jan 2023 00:24:43 GMT  
		Size: 2.5 KB (2454 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c43ce01c7b867ce6cda62f86175ba6a53f44000797d61fe604aded86980c4d41`  
		Last Modified: Tue, 31 Jan 2023 00:24:43 GMT  
		Size: 6.0 KB (6006 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6fe6f306aa61d9839a01e62f4c308a9a7d3bd4cd5ce9a58407b6585f6950f054`  
		Last Modified: Tue, 31 Jan 2023 00:24:43 GMT  
		Size: 2.5 KB (2505 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `xwiki:postgres-tomcat` - linux; arm64 variant v8

```console
$ docker pull xwiki@sha256:ae51c629c7a76aa7c15ebb33fcfdae3e529ef6456ada6d0dbcf9ed8fc5ecf00d
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **581.2 MB (581212250 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:70277ae3ffdca68401bb57e24e6302cc64a403bf36869f0959e54d03216b0005`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["xwiki"]`

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
# Wed, 02 Nov 2022 19:44:32 GMT
RUN apt-get update     && DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends tzdata curl wget ca-certificates fontconfig locales     && echo "en_US.UTF-8 UTF-8" >> /etc/locale.gen     && locale-gen en_US.UTF-8     && rm -rf /var/lib/apt/lists/*
# Fri, 04 Nov 2022 22:40:54 GMT
ENV JAVA_VERSION=jdk-11.0.17+8
# Fri, 04 Nov 2022 22:41:33 GMT
RUN set -eux;     ARCH="$(dpkg --print-architecture)";     case "${ARCH}" in        aarch64|arm64)          ESUM='bd6efe3290c8b5a42f695a55a26f3e3c9c284288574879d4b7089f31f5114177';          BINARY_URL='https://github.com/adoptium/temurin11-binaries/releases/download/jdk-11.0.17%2B8/OpenJDK11U-jre_aarch64_linux_hotspot_11.0.17_8.tar.gz';          ;;        armhf|arm)          ESUM='8cf113d3d7fa808895c8d2e41bb890af21c47e38c2460e0588147a4bb8fc658d';          BINARY_URL='https://github.com/adoptium/temurin11-binaries/releases/download/jdk-11.0.17%2B8/OpenJDK11U-jre_arm_linux_hotspot_11.0.17_8.tar.gz';          ;;        ppc64el|powerpc:common64)          ESUM='0ca3d806131ab5834c501f9c625bb0248cd528af361c704503348e9c9605bedf';          BINARY_URL='https://github.com/adoptium/temurin11-binaries/releases/download/jdk-11.0.17%2B8/OpenJDK11U-jre_ppc64le_linux_hotspot_11.0.17_8.tar.gz';          ;;        s390x|s390:64-bit)          ESUM='dd3b159a374086e65cb07c4ccb226c90f9c02ef929cba6f0b642171d7ed97fa4';          BINARY_URL='https://github.com/adoptium/temurin11-binaries/releases/download/jdk-11.0.17%2B8/OpenJDK11U-jre_s390x_linux_hotspot_11.0.17_8.tar.gz';          ;;        amd64|i386:x86-64)          ESUM='752616097e09d7f60a3ad8bd312f90eaf50ac72577e55df229fe6e8091148f79';          BINARY_URL='https://github.com/adoptium/temurin11-binaries/releases/download/jdk-11.0.17%2B8/OpenJDK11U-jre_x64_linux_hotspot_11.0.17_8.tar.gz';          ;;        *)          echo "Unsupported arch: ${ARCH}";          exit 1;          ;;     esac; 	  wget -O /tmp/openjdk.tar.gz ${BINARY_URL}; 	  echo "${ESUM} */tmp/openjdk.tar.gz" | sha256sum -c -; 	  mkdir -p "$JAVA_HOME"; 	  tar --extract 	      --file /tmp/openjdk.tar.gz 	      --directory "$JAVA_HOME" 	      --strip-components 1 	      --no-same-owner 	  ;     rm /tmp/openjdk.tar.gz;     find "$JAVA_HOME/lib" -name '*.so' -exec dirname '{}' ';' | sort -u > /etc/ld.so.conf.d/docker-openjdk.conf;     ldconfig;     java -Xshare:dump;
# Fri, 04 Nov 2022 22:41:34 GMT
RUN echo Verifying install ...     && fileEncoding="$(echo 'System.out.println(System.getProperty("file.encoding"))' | jshell -s -)"; [ "$fileEncoding" = 'UTF-8' ]; rm -rf ~/.java     && echo java --version && java --version     && echo Complete.
# Fri, 04 Nov 2022 23:48:38 GMT
ENV CATALINA_HOME=/usr/local/tomcat
# Fri, 04 Nov 2022 23:48:38 GMT
ENV PATH=/usr/local/tomcat/bin:/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Fri, 04 Nov 2022 23:48:38 GMT
RUN mkdir -p "$CATALINA_HOME"
# Fri, 04 Nov 2022 23:48:39 GMT
WORKDIR /usr/local/tomcat
# Fri, 04 Nov 2022 23:48:39 GMT
ENV TOMCAT_NATIVE_LIBDIR=/usr/local/tomcat/native-jni-lib
# Fri, 04 Nov 2022 23:48:39 GMT
ENV LD_LIBRARY_PATH=/usr/local/tomcat/native-jni-lib
# Fri, 04 Nov 2022 23:53:12 GMT
ENV GPG_KEYS=48F8E69F6390C9F25CFEDCD268248959359E722B A9C5DF4D22E99998D9875A5110C01C5A2F6059E7 DCFD35E0BF8CA7344752DE8B6FB21E8933C60243
# Fri, 04 Nov 2022 23:53:12 GMT
ENV TOMCAT_MAJOR=9
# Tue, 15 Nov 2022 04:57:22 GMT
ENV TOMCAT_VERSION=9.0.69
# Tue, 15 Nov 2022 04:57:22 GMT
ENV TOMCAT_SHA512=8c883c54ce9ce43eba37756a6404cdf3477879883a3e6d146dc8a7aa5e0425f487466afe6b6da4a895927cb7cb59177b9379cec18000f2de12785be57408c779
# Tue, 15 Nov 2022 04:57:22 GMT
COPY dir:096b403a5f78b17e6b4bff63128a9c93941b97f22470991610dd641633d977f1 in /usr/local/tomcat 
# Tue, 15 Nov 2022 04:57:25 GMT
RUN set -eux; 	apt-get update; 	xargs -rt apt-get install -y --no-install-recommends < "$TOMCAT_NATIVE_LIBDIR/.dependencies.txt"; 	rm -rf /var/lib/apt/lists/*
# Tue, 15 Nov 2022 04:57:26 GMT
RUN set -eux; 	nativeLines="$(catalina.sh configtest 2>&1)"; 	nativeLines="$(echo "$nativeLines" | grep 'Apache Tomcat Native')"; 	nativeLines="$(echo "$nativeLines" | sort -u)"; 	if ! echo "$nativeLines" | grep -E 'INFO: Loaded( APR based)? Apache Tomcat Native library' >&2; then 		echo >&2 "$nativeLines"; 		exit 1; 	fi
# Tue, 15 Nov 2022 04:57:26 GMT
EXPOSE 8080
# Tue, 15 Nov 2022 04:57:27 GMT
CMD ["catalina.sh" "run"]
# Wed, 11 Jan 2023 03:05:10 GMT
LABEL org.opencontainers.image.authors=XWiki Development Team <committers@xwiki.org>
# Wed, 11 Jan 2023 03:05:10 GMT
LABEL org.opencontainers.image.url=https://hub.docker.com/_/xwiki
# Wed, 11 Jan 2023 03:05:10 GMT
LABEL org.opencontainers.image.documentation=https://hub.docker.com/_/xwiki
# Wed, 11 Jan 2023 03:05:10 GMT
LABEL org.opencontainers.image.source=https://github.com/xwiki/xwiki-docker.git
# Wed, 11 Jan 2023 03:05:11 GMT
LABEL org.opencontainers.image.vendor=xwiki.org
# Wed, 11 Jan 2023 03:05:11 GMT
LABEL org.opencontainers.image.licenses=LGPL-2.1
# Wed, 11 Jan 2023 03:08:55 GMT
RUN apt-get update &&   apt-get --no-install-recommends -y install     curl     libreoffice     unzip     procps     libpostgresql-jdbc-java &&   rm -rf /var/lib/apt/lists/*
# Tue, 31 Jan 2023 00:48:10 GMT
ENV XWIKI_VERSION=15.0
# Tue, 31 Jan 2023 00:48:10 GMT
ENV XWIKI_URL_PREFIX=https://maven.xwiki.org/releases/org/xwiki/platform/xwiki-platform-distribution-war/15.0
# Tue, 31 Jan 2023 00:48:10 GMT
ENV XWIKI_DOWNLOAD_SHA256=79ba0f479bbc49521c113821adc9d91141075a9470d7f9bbb6994ca59c30d121
# Tue, 31 Jan 2023 00:54:38 GMT
RUN rm -rf /usr/local/tomcat/webapps/* &&   mkdir -p /usr/local/tomcat/temp &&   mkdir -p /usr/local/xwiki/data &&   curl -fSL "${XWIKI_URL_PREFIX}/xwiki-platform-distribution-war-${XWIKI_VERSION}.war" -o xwiki.war &&   echo "$XWIKI_DOWNLOAD_SHA256 xwiki.war" | sha256sum -c - &&   unzip -d /usr/local/tomcat/webapps/ROOT xwiki.war &&   rm -f xwiki.war
# Tue, 31 Jan 2023 00:54:41 GMT
RUN cp /usr/share/java/postgresql-jdbc4.jar /usr/local/tomcat/webapps/ROOT/WEB-INF/lib/
# Tue, 31 Jan 2023 00:54:41 GMT
COPY file:0a1be11e2eb610a1dbcd415404e3a592641110b93090030cb831e3a19a163017 in /usr/local/tomcat/bin/ 
# Tue, 31 Jan 2023 00:54:41 GMT
COPY file:4a923f484bb29a26630c19e1d617d3bf6aa6ae7c6c4a5561e97b037bcde0847c in /usr/local/tomcat/webapps/ROOT/WEB-INF/hibernate.cfg.xml 
# Tue, 31 Jan 2023 00:54:42 GMT
RUN sed -i 's/<id>org.xwiki.platform:xwiki-platform-distribution-war/<id>org.xwiki.platform:xwiki-platform-distribution-docker/'   /usr/local/tomcat/webapps/ROOT/META-INF/extension.xed
# Tue, 31 Jan 2023 00:54:42 GMT
COPY file:a47c4dcd87c9dad97aff38c49188357e6193bcad50757e516cfb08a60d4de611 in /usr/local/bin/docker-entrypoint.sh 
# Tue, 31 Jan 2023 00:54:42 GMT
VOLUME [/usr/local/xwiki]
# Tue, 31 Jan 2023 00:54:42 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 31 Jan 2023 00:54:42 GMT
CMD ["xwiki"]
```

-	Layers:
	-	`sha256:0509fae36eb0656f8bdb23f8ae64100d893bcea2563e97468d337e04d2d0410b`  
		Last Modified: Wed, 02 Nov 2022 18:50:21 GMT  
		Size: 28.4 MB (28382154 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e502a1af2bcd98f5f0d2f5e4da1a0e7bbe07a2c548e2662f7d37dce5ae1df46c`  
		Last Modified: Wed, 02 Nov 2022 19:48:28 GMT  
		Size: 12.4 MB (12396330 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bc4598c07dd818f03a0378b0341a4a8e80f0152fbb3e7d5246ca4f466f42e611`  
		Last Modified: Fri, 04 Nov 2022 22:46:46 GMT  
		Size: 45.0 MB (44958470 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:715a937a1066f998b331fcd62256ad01a5571bdf46804e97825afc64f9ebb427`  
		Last Modified: Fri, 04 Nov 2022 22:46:41 GMT  
		Size: 160.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5fb623f082f74b2fa9fc2c4e3f3a4802875cb9753cfa26ed940201ce72bb56cb`  
		Last Modified: Sat, 05 Nov 2022 00:03:40 GMT  
		Size: 172.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:33260b83200262bbd546be371ad3c1f50f5ae7228afb87982d6fa9d6b11bf26f`  
		Last Modified: Tue, 15 Nov 2022 05:10:19 GMT  
		Size: 12.2 MB (12207235 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0955fb697ea9b30a1b4f95385464f646aa1525cb6efba648e22df84ebef6b2ee`  
		Last Modified: Tue, 15 Nov 2022 05:10:18 GMT  
		Size: 452.0 KB (452021 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6eddcf66f2083b1487296a0308e0b058917c97f614f12428d82d89662038dc2e`  
		Last Modified: Tue, 15 Nov 2022 05:10:18 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1ae6a8fce0f2cd131007393c1a4eba9ce9d0501da8406af5c5ce9deb5dc187b8`  
		Last Modified: Wed, 11 Jan 2023 03:12:13 GMT  
		Size: 174.7 MB (174749274 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5351c17af011e98fdd3db4781945e719f390748d66dc50d28bef46bb2d6b6418`  
		Last Modified: Tue, 31 Jan 2023 00:56:53 GMT  
		Size: 307.1 MB (307117134 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6b632a2f6afda42ce5dc291920d8f03e04b69034e314687eb551be8eafedd92d`  
		Last Modified: Tue, 31 Jan 2023 00:56:38 GMT  
		Size: 936.9 KB (936854 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cbd6cbb6ae05692db55d5e4f46142d2e20e051631dc2fc44e5b20d3316143305`  
		Last Modified: Tue, 31 Jan 2023 00:56:38 GMT  
		Size: 1.3 KB (1348 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ceb1d88f8fd44412961c0db372cd86a999c6b2619ce80a916a4fe8ca0e63acc9`  
		Last Modified: Tue, 31 Jan 2023 00:56:38 GMT  
		Size: 2.5 KB (2458 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8d0ee5cad12d41a6d530031aabd4a92619995eb0ee20dcd24d2bb9aec6a694db`  
		Last Modified: Tue, 31 Jan 2023 00:56:38 GMT  
		Size: 6.0 KB (6006 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3c980b95519f007aea60be042d36cd33de21e6265aed0e443c5ecf9bb1f40980`  
		Last Modified: Tue, 31 Jan 2023 00:56:38 GMT  
		Size: 2.5 KB (2505 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `xwiki:stable`

```console
$ docker pull xwiki@sha256:33e789838f82ce73efec6664859feb1ced7a5b7605fbfaddb81916716bce524f
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `xwiki:stable` - linux; amd64

```console
$ docker pull xwiki@sha256:481fdb46e8c043a6709d11310e2083ce71d6ba63ee6517f84da3ba06f320598e
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **590.5 MB (590459982 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:bd630aa0aa5c679e23ea7d52cbbdd6b817eab27a820c25d3c50b54eca83b9744`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["xwiki"]`

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
# Wed, 02 Nov 2022 18:44:10 GMT
RUN apt-get update     && DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends tzdata curl wget ca-certificates fontconfig locales     && echo "en_US.UTF-8 UTF-8" >> /etc/locale.gen     && locale-gen en_US.UTF-8     && rm -rf /var/lib/apt/lists/*
# Fri, 04 Nov 2022 23:21:41 GMT
ENV JAVA_VERSION=jdk-11.0.17+8
# Fri, 04 Nov 2022 23:22:31 GMT
RUN set -eux;     ARCH="$(dpkg --print-architecture)";     case "${ARCH}" in        aarch64|arm64)          ESUM='bd6efe3290c8b5a42f695a55a26f3e3c9c284288574879d4b7089f31f5114177';          BINARY_URL='https://github.com/adoptium/temurin11-binaries/releases/download/jdk-11.0.17%2B8/OpenJDK11U-jre_aarch64_linux_hotspot_11.0.17_8.tar.gz';          ;;        armhf|arm)          ESUM='8cf113d3d7fa808895c8d2e41bb890af21c47e38c2460e0588147a4bb8fc658d';          BINARY_URL='https://github.com/adoptium/temurin11-binaries/releases/download/jdk-11.0.17%2B8/OpenJDK11U-jre_arm_linux_hotspot_11.0.17_8.tar.gz';          ;;        ppc64el|powerpc:common64)          ESUM='0ca3d806131ab5834c501f9c625bb0248cd528af361c704503348e9c9605bedf';          BINARY_URL='https://github.com/adoptium/temurin11-binaries/releases/download/jdk-11.0.17%2B8/OpenJDK11U-jre_ppc64le_linux_hotspot_11.0.17_8.tar.gz';          ;;        s390x|s390:64-bit)          ESUM='dd3b159a374086e65cb07c4ccb226c90f9c02ef929cba6f0b642171d7ed97fa4';          BINARY_URL='https://github.com/adoptium/temurin11-binaries/releases/download/jdk-11.0.17%2B8/OpenJDK11U-jre_s390x_linux_hotspot_11.0.17_8.tar.gz';          ;;        amd64|i386:x86-64)          ESUM='752616097e09d7f60a3ad8bd312f90eaf50ac72577e55df229fe6e8091148f79';          BINARY_URL='https://github.com/adoptium/temurin11-binaries/releases/download/jdk-11.0.17%2B8/OpenJDK11U-jre_x64_linux_hotspot_11.0.17_8.tar.gz';          ;;        *)          echo "Unsupported arch: ${ARCH}";          exit 1;          ;;     esac; 	  wget -O /tmp/openjdk.tar.gz ${BINARY_URL}; 	  echo "${ESUM} */tmp/openjdk.tar.gz" | sha256sum -c -; 	  mkdir -p "$JAVA_HOME"; 	  tar --extract 	      --file /tmp/openjdk.tar.gz 	      --directory "$JAVA_HOME" 	      --strip-components 1 	      --no-same-owner 	  ;     rm /tmp/openjdk.tar.gz;     find "$JAVA_HOME/lib" -name '*.so' -exec dirname '{}' ';' | sort -u > /etc/ld.so.conf.d/docker-openjdk.conf;     ldconfig;     java -Xshare:dump;
# Fri, 04 Nov 2022 23:22:32 GMT
RUN echo Verifying install ...     && fileEncoding="$(echo 'System.out.println(System.getProperty("file.encoding"))' | jshell -s -)"; [ "$fileEncoding" = 'UTF-8' ]; rm -rf ~/.java     && echo java --version && java --version     && echo Complete.
# Sat, 05 Nov 2022 01:35:16 GMT
ENV CATALINA_HOME=/usr/local/tomcat
# Sat, 05 Nov 2022 01:35:16 GMT
ENV PATH=/usr/local/tomcat/bin:/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Sat, 05 Nov 2022 01:35:17 GMT
RUN mkdir -p "$CATALINA_HOME"
# Sat, 05 Nov 2022 01:35:17 GMT
WORKDIR /usr/local/tomcat
# Sat, 05 Nov 2022 01:35:17 GMT
ENV TOMCAT_NATIVE_LIBDIR=/usr/local/tomcat/native-jni-lib
# Sat, 05 Nov 2022 01:35:17 GMT
ENV LD_LIBRARY_PATH=/usr/local/tomcat/native-jni-lib
# Sat, 05 Nov 2022 01:39:54 GMT
ENV GPG_KEYS=48F8E69F6390C9F25CFEDCD268248959359E722B A9C5DF4D22E99998D9875A5110C01C5A2F6059E7 DCFD35E0BF8CA7344752DE8B6FB21E8933C60243
# Sat, 05 Nov 2022 01:39:54 GMT
ENV TOMCAT_MAJOR=9
# Tue, 15 Nov 2022 03:06:43 GMT
ENV TOMCAT_VERSION=9.0.69
# Tue, 15 Nov 2022 03:06:43 GMT
ENV TOMCAT_SHA512=8c883c54ce9ce43eba37756a6404cdf3477879883a3e6d146dc8a7aa5e0425f487466afe6b6da4a895927cb7cb59177b9379cec18000f2de12785be57408c779
# Tue, 15 Nov 2022 03:06:44 GMT
COPY dir:b1a33aa3993dbbfbebb33bd9aa546b60c2f2191abf1227f453d4e830f6deb35f in /usr/local/tomcat 
# Tue, 15 Nov 2022 03:06:48 GMT
RUN set -eux; 	apt-get update; 	xargs -rt apt-get install -y --no-install-recommends < "$TOMCAT_NATIVE_LIBDIR/.dependencies.txt"; 	rm -rf /var/lib/apt/lists/*
# Tue, 15 Nov 2022 03:06:49 GMT
RUN set -eux; 	nativeLines="$(catalina.sh configtest 2>&1)"; 	nativeLines="$(echo "$nativeLines" | grep 'Apache Tomcat Native')"; 	nativeLines="$(echo "$nativeLines" | sort -u)"; 	if ! echo "$nativeLines" | grep -E 'INFO: Loaded( APR based)? Apache Tomcat Native library' >&2; then 		echo >&2 "$nativeLines"; 		exit 1; 	fi
# Tue, 15 Nov 2022 03:06:49 GMT
EXPOSE 8080
# Tue, 15 Nov 2022 03:06:49 GMT
CMD ["catalina.sh" "run"]
# Wed, 11 Jan 2023 02:47:03 GMT
LABEL org.opencontainers.image.authors=XWiki Development Team <committers@xwiki.org>
# Wed, 11 Jan 2023 02:47:03 GMT
LABEL org.opencontainers.image.url=https://hub.docker.com/_/xwiki
# Wed, 11 Jan 2023 02:47:03 GMT
LABEL org.opencontainers.image.documentation=https://hub.docker.com/_/xwiki
# Wed, 11 Jan 2023 02:47:03 GMT
LABEL org.opencontainers.image.source=https://github.com/xwiki/xwiki-docker.git
# Wed, 11 Jan 2023 02:47:04 GMT
LABEL org.opencontainers.image.vendor=xwiki.org
# Wed, 11 Jan 2023 02:47:04 GMT
LABEL org.opencontainers.image.licenses=LGPL-2.1
# Wed, 11 Jan 2023 02:49:03 GMT
RUN apt-get update &&   apt-get --no-install-recommends -y install     curl     libreoffice     unzip     procps &&   rm -rf /var/lib/apt/lists/*
# Tue, 31 Jan 2023 00:20:17 GMT
ENV XWIKI_VERSION=15.0
# Tue, 31 Jan 2023 00:20:17 GMT
ENV XWIKI_URL_PREFIX=https://maven.xwiki.org/releases/org/xwiki/platform/xwiki-platform-distribution-war/15.0
# Tue, 31 Jan 2023 00:20:17 GMT
ENV XWIKI_DOWNLOAD_SHA256=79ba0f479bbc49521c113821adc9d91141075a9470d7f9bbb6994ca59c30d121
# Tue, 31 Jan 2023 00:21:18 GMT
RUN rm -rf /usr/local/tomcat/webapps/* &&   mkdir -p /usr/local/tomcat/temp &&   mkdir -p /usr/local/xwiki/data &&   curl -fSL "${XWIKI_URL_PREFIX}/xwiki-platform-distribution-war-${XWIKI_VERSION}.war" -o xwiki.war &&   echo "$XWIKI_DOWNLOAD_SHA256 xwiki.war" | sha256sum -c - &&   unzip -d /usr/local/tomcat/webapps/ROOT xwiki.war &&   rm -f xwiki.war
# Tue, 31 Jan 2023 00:21:19 GMT
ENV MYSQL_JDBC_VERSION=8.0.31
# Tue, 31 Jan 2023 00:21:19 GMT
ENV MYSQL_JDBC_SHA256=5249e3dc6d6531b37790e3f61845b96db5e41e891d3d8edb0e2e3a1b53ca2f4f
# Tue, 31 Jan 2023 00:21:19 GMT
ENV MYSQL_JDBC_PREFIX=https://repo1.maven.org/maven2/com/mysql/mysql-connector-j/8.0.31
# Tue, 31 Jan 2023 00:21:19 GMT
ENV MYSQL_JDBC_ARTIFACT=mysql-connector-j-8.0.31.jar
# Tue, 31 Jan 2023 00:21:19 GMT
ENV MYSQL_JDBC_TARGET=/usr/local/tomcat/webapps/ROOT/WEB-INF/lib/mysql-connector-j-8.0.31.jar
# Tue, 31 Jan 2023 00:21:20 GMT
RUN curl -fSL "${MYSQL_JDBC_PREFIX}/${MYSQL_JDBC_ARTIFACT}" -o $MYSQL_JDBC_TARGET &&   echo "$MYSQL_JDBC_SHA256 $MYSQL_JDBC_TARGET" | sha256sum -c -
# Tue, 31 Jan 2023 00:21:21 GMT
COPY file:0a1be11e2eb610a1dbcd415404e3a592641110b93090030cb831e3a19a163017 in /usr/local/tomcat/bin/ 
# Tue, 31 Jan 2023 00:21:21 GMT
COPY file:1b8409986f3e4eb79a7a0b18472cb2692a61d504fb5ef34292bc997b79fd760d in /usr/local/tomcat/webapps/ROOT/WEB-INF/hibernate.cfg.xml 
# Tue, 31 Jan 2023 00:21:21 GMT
RUN sed -i 's/<id>org.xwiki.platform:xwiki-platform-distribution-war/<id>org.xwiki.platform:xwiki-platform-distribution-docker/'   /usr/local/tomcat/webapps/ROOT/META-INF/extension.xed
# Tue, 31 Jan 2023 00:21:21 GMT
COPY file:a47c4dcd87c9dad97aff38c49188357e6193bcad50757e516cfb08a60d4de611 in /usr/local/bin/docker-entrypoint.sh 
# Tue, 31 Jan 2023 00:21:22 GMT
VOLUME [/usr/local/xwiki]
# Tue, 31 Jan 2023 00:21:22 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 31 Jan 2023 00:21:22 GMT
CMD ["xwiki"]
```

-	Layers:
	-	`sha256:e96e057aae67380a4ddb16c337c5c3669d97fdff69ec537f02aa2cc30d814281`  
		Last Modified: Wed, 02 Nov 2022 03:03:36 GMT  
		Size: 30.4 MB (30425607 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4ced2591451da3a02e2b6bb44752b9e3f00d77789921be4df5082fb9f9880ad0`  
		Last Modified: Wed, 02 Nov 2022 18:48:43 GMT  
		Size: 12.4 MB (12439006 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:df8f874ae8c08a9e69e5fbe6c5a64200a45386132a3203d1a9a7f1146d94cfbc`  
		Last Modified: Fri, 04 Nov 2022 23:29:33 GMT  
		Size: 46.6 MB (46629936 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:111b6c7486426c4b6989102c2ee5be856e8a58e20ab0a350b24a905d536e8e7f`  
		Last Modified: Fri, 04 Nov 2022 23:29:26 GMT  
		Size: 161.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e6f84dce457c6d4f7b7291fce05f8e77998a3a7722a54125a1f1d52ca83043b4`  
		Last Modified: Sat, 05 Nov 2022 01:50:51 GMT  
		Size: 173.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a6c26749ee782392e38845ee2ba79b0da586ef6a45d8e7f29c7af14612278547`  
		Last Modified: Tue, 15 Nov 2022 03:19:57 GMT  
		Size: 12.2 MB (12200249 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4dddc6d9fa6024025b3fcfe729cab2dc544fb25476eca6e80b1af8e8d93bb0ee`  
		Last Modified: Tue, 15 Nov 2022 03:19:56 GMT  
		Size: 452.7 KB (452680 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:06637eebe5e72c8ad9019ad4eb4cdde1f11f7d4c24c7ed7374cf8966343aa2fb`  
		Last Modified: Tue, 15 Nov 2022 03:19:56 GMT  
		Size: 131.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b276fb8390410a8208724033e325715ea26000d5a1a762d4c3699b927884fbfe`  
		Last Modified: Wed, 11 Jan 2023 02:52:45 GMT  
		Size: 178.8 MB (178805608 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:156ca91198173149698aa0396648a9608b6ab1f2bc2666800843ce33c9f85b6e`  
		Last Modified: Tue, 31 Jan 2023 00:24:09 GMT  
		Size: 307.1 MB (307117069 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4c8b70d250c6d507901857473b0dcb67132d7b2a30ce9a69b07b1036853df738`  
		Last Modified: Tue, 31 Jan 2023 00:23:52 GMT  
		Size: 2.4 MB (2377191 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a9681fd36be674d25231c69d6a39f9e8fa65034eeaef5d1bd885fdbeac7f0f6b`  
		Last Modified: Tue, 31 Jan 2023 00:23:51 GMT  
		Size: 1.3 KB (1346 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a9d0d5da840f4d7da9943942b38cd092fae11f41dc6c19afd58d655cd6192d66`  
		Last Modified: Tue, 31 Jan 2023 00:23:51 GMT  
		Size: 2.3 KB (2312 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d65610da4f1da86fea8fbec0189b066afd4b86e4e8f7d049e3c4bc6ade9ba90a`  
		Last Modified: Tue, 31 Jan 2023 00:23:51 GMT  
		Size: 6.0 KB (6009 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3d41686284d7675eaa0f92c9cc27ebe73b4c30768c8eef9f23ee3b1ad06da00a`  
		Last Modified: Tue, 31 Jan 2023 00:23:51 GMT  
		Size: 2.5 KB (2504 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `xwiki:stable` - linux; arm64 variant v8

```console
$ docker pull xwiki@sha256:6bf63d9025b07b69d744200c05efd4ffb8a52f3c38380f5d59a0b48514203cd2
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **581.7 MB (581709921 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:6600f2bb05836c703d53944bbcb5399d509a9813a27a35e99ff717becc308330`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["xwiki"]`

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
# Wed, 02 Nov 2022 19:44:32 GMT
RUN apt-get update     && DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends tzdata curl wget ca-certificates fontconfig locales     && echo "en_US.UTF-8 UTF-8" >> /etc/locale.gen     && locale-gen en_US.UTF-8     && rm -rf /var/lib/apt/lists/*
# Fri, 04 Nov 2022 22:40:54 GMT
ENV JAVA_VERSION=jdk-11.0.17+8
# Fri, 04 Nov 2022 22:41:33 GMT
RUN set -eux;     ARCH="$(dpkg --print-architecture)";     case "${ARCH}" in        aarch64|arm64)          ESUM='bd6efe3290c8b5a42f695a55a26f3e3c9c284288574879d4b7089f31f5114177';          BINARY_URL='https://github.com/adoptium/temurin11-binaries/releases/download/jdk-11.0.17%2B8/OpenJDK11U-jre_aarch64_linux_hotspot_11.0.17_8.tar.gz';          ;;        armhf|arm)          ESUM='8cf113d3d7fa808895c8d2e41bb890af21c47e38c2460e0588147a4bb8fc658d';          BINARY_URL='https://github.com/adoptium/temurin11-binaries/releases/download/jdk-11.0.17%2B8/OpenJDK11U-jre_arm_linux_hotspot_11.0.17_8.tar.gz';          ;;        ppc64el|powerpc:common64)          ESUM='0ca3d806131ab5834c501f9c625bb0248cd528af361c704503348e9c9605bedf';          BINARY_URL='https://github.com/adoptium/temurin11-binaries/releases/download/jdk-11.0.17%2B8/OpenJDK11U-jre_ppc64le_linux_hotspot_11.0.17_8.tar.gz';          ;;        s390x|s390:64-bit)          ESUM='dd3b159a374086e65cb07c4ccb226c90f9c02ef929cba6f0b642171d7ed97fa4';          BINARY_URL='https://github.com/adoptium/temurin11-binaries/releases/download/jdk-11.0.17%2B8/OpenJDK11U-jre_s390x_linux_hotspot_11.0.17_8.tar.gz';          ;;        amd64|i386:x86-64)          ESUM='752616097e09d7f60a3ad8bd312f90eaf50ac72577e55df229fe6e8091148f79';          BINARY_URL='https://github.com/adoptium/temurin11-binaries/releases/download/jdk-11.0.17%2B8/OpenJDK11U-jre_x64_linux_hotspot_11.0.17_8.tar.gz';          ;;        *)          echo "Unsupported arch: ${ARCH}";          exit 1;          ;;     esac; 	  wget -O /tmp/openjdk.tar.gz ${BINARY_URL}; 	  echo "${ESUM} */tmp/openjdk.tar.gz" | sha256sum -c -; 	  mkdir -p "$JAVA_HOME"; 	  tar --extract 	      --file /tmp/openjdk.tar.gz 	      --directory "$JAVA_HOME" 	      --strip-components 1 	      --no-same-owner 	  ;     rm /tmp/openjdk.tar.gz;     find "$JAVA_HOME/lib" -name '*.so' -exec dirname '{}' ';' | sort -u > /etc/ld.so.conf.d/docker-openjdk.conf;     ldconfig;     java -Xshare:dump;
# Fri, 04 Nov 2022 22:41:34 GMT
RUN echo Verifying install ...     && fileEncoding="$(echo 'System.out.println(System.getProperty("file.encoding"))' | jshell -s -)"; [ "$fileEncoding" = 'UTF-8' ]; rm -rf ~/.java     && echo java --version && java --version     && echo Complete.
# Fri, 04 Nov 2022 23:48:38 GMT
ENV CATALINA_HOME=/usr/local/tomcat
# Fri, 04 Nov 2022 23:48:38 GMT
ENV PATH=/usr/local/tomcat/bin:/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Fri, 04 Nov 2022 23:48:38 GMT
RUN mkdir -p "$CATALINA_HOME"
# Fri, 04 Nov 2022 23:48:39 GMT
WORKDIR /usr/local/tomcat
# Fri, 04 Nov 2022 23:48:39 GMT
ENV TOMCAT_NATIVE_LIBDIR=/usr/local/tomcat/native-jni-lib
# Fri, 04 Nov 2022 23:48:39 GMT
ENV LD_LIBRARY_PATH=/usr/local/tomcat/native-jni-lib
# Fri, 04 Nov 2022 23:53:12 GMT
ENV GPG_KEYS=48F8E69F6390C9F25CFEDCD268248959359E722B A9C5DF4D22E99998D9875A5110C01C5A2F6059E7 DCFD35E0BF8CA7344752DE8B6FB21E8933C60243
# Fri, 04 Nov 2022 23:53:12 GMT
ENV TOMCAT_MAJOR=9
# Tue, 15 Nov 2022 04:57:22 GMT
ENV TOMCAT_VERSION=9.0.69
# Tue, 15 Nov 2022 04:57:22 GMT
ENV TOMCAT_SHA512=8c883c54ce9ce43eba37756a6404cdf3477879883a3e6d146dc8a7aa5e0425f487466afe6b6da4a895927cb7cb59177b9379cec18000f2de12785be57408c779
# Tue, 15 Nov 2022 04:57:22 GMT
COPY dir:096b403a5f78b17e6b4bff63128a9c93941b97f22470991610dd641633d977f1 in /usr/local/tomcat 
# Tue, 15 Nov 2022 04:57:25 GMT
RUN set -eux; 	apt-get update; 	xargs -rt apt-get install -y --no-install-recommends < "$TOMCAT_NATIVE_LIBDIR/.dependencies.txt"; 	rm -rf /var/lib/apt/lists/*
# Tue, 15 Nov 2022 04:57:26 GMT
RUN set -eux; 	nativeLines="$(catalina.sh configtest 2>&1)"; 	nativeLines="$(echo "$nativeLines" | grep 'Apache Tomcat Native')"; 	nativeLines="$(echo "$nativeLines" | sort -u)"; 	if ! echo "$nativeLines" | grep -E 'INFO: Loaded( APR based)? Apache Tomcat Native library' >&2; then 		echo >&2 "$nativeLines"; 		exit 1; 	fi
# Tue, 15 Nov 2022 04:57:26 GMT
EXPOSE 8080
# Tue, 15 Nov 2022 04:57:27 GMT
CMD ["catalina.sh" "run"]
# Wed, 11 Jan 2023 03:05:10 GMT
LABEL org.opencontainers.image.authors=XWiki Development Team <committers@xwiki.org>
# Wed, 11 Jan 2023 03:05:10 GMT
LABEL org.opencontainers.image.url=https://hub.docker.com/_/xwiki
# Wed, 11 Jan 2023 03:05:10 GMT
LABEL org.opencontainers.image.documentation=https://hub.docker.com/_/xwiki
# Wed, 11 Jan 2023 03:05:10 GMT
LABEL org.opencontainers.image.source=https://github.com/xwiki/xwiki-docker.git
# Wed, 11 Jan 2023 03:05:11 GMT
LABEL org.opencontainers.image.vendor=xwiki.org
# Wed, 11 Jan 2023 03:05:11 GMT
LABEL org.opencontainers.image.licenses=LGPL-2.1
# Wed, 11 Jan 2023 03:07:37 GMT
RUN apt-get update &&   apt-get --no-install-recommends -y install     curl     libreoffice     unzip     procps &&   rm -rf /var/lib/apt/lists/*
# Tue, 31 Jan 2023 00:47:12 GMT
ENV XWIKI_VERSION=15.0
# Tue, 31 Jan 2023 00:47:12 GMT
ENV XWIKI_URL_PREFIX=https://maven.xwiki.org/releases/org/xwiki/platform/xwiki-platform-distribution-war/15.0
# Tue, 31 Jan 2023 00:47:12 GMT
ENV XWIKI_DOWNLOAD_SHA256=79ba0f479bbc49521c113821adc9d91141075a9470d7f9bbb6994ca59c30d121
# Tue, 31 Jan 2023 00:47:58 GMT
RUN rm -rf /usr/local/tomcat/webapps/* &&   mkdir -p /usr/local/tomcat/temp &&   mkdir -p /usr/local/xwiki/data &&   curl -fSL "${XWIKI_URL_PREFIX}/xwiki-platform-distribution-war-${XWIKI_VERSION}.war" -o xwiki.war &&   echo "$XWIKI_DOWNLOAD_SHA256 xwiki.war" | sha256sum -c - &&   unzip -d /usr/local/tomcat/webapps/ROOT xwiki.war &&   rm -f xwiki.war
# Tue, 31 Jan 2023 00:48:01 GMT
ENV MYSQL_JDBC_VERSION=8.0.31
# Tue, 31 Jan 2023 00:48:01 GMT
ENV MYSQL_JDBC_SHA256=5249e3dc6d6531b37790e3f61845b96db5e41e891d3d8edb0e2e3a1b53ca2f4f
# Tue, 31 Jan 2023 00:48:01 GMT
ENV MYSQL_JDBC_PREFIX=https://repo1.maven.org/maven2/com/mysql/mysql-connector-j/8.0.31
# Tue, 31 Jan 2023 00:48:01 GMT
ENV MYSQL_JDBC_ARTIFACT=mysql-connector-j-8.0.31.jar
# Tue, 31 Jan 2023 00:48:01 GMT
ENV MYSQL_JDBC_TARGET=/usr/local/tomcat/webapps/ROOT/WEB-INF/lib/mysql-connector-j-8.0.31.jar
# Tue, 31 Jan 2023 00:48:02 GMT
RUN curl -fSL "${MYSQL_JDBC_PREFIX}/${MYSQL_JDBC_ARTIFACT}" -o $MYSQL_JDBC_TARGET &&   echo "$MYSQL_JDBC_SHA256 $MYSQL_JDBC_TARGET" | sha256sum -c -
# Tue, 31 Jan 2023 00:48:02 GMT
COPY file:0a1be11e2eb610a1dbcd415404e3a592641110b93090030cb831e3a19a163017 in /usr/local/tomcat/bin/ 
# Tue, 31 Jan 2023 00:48:02 GMT
COPY file:1b8409986f3e4eb79a7a0b18472cb2692a61d504fb5ef34292bc997b79fd760d in /usr/local/tomcat/webapps/ROOT/WEB-INF/hibernate.cfg.xml 
# Tue, 31 Jan 2023 00:48:03 GMT
RUN sed -i 's/<id>org.xwiki.platform:xwiki-platform-distribution-war/<id>org.xwiki.platform:xwiki-platform-distribution-docker/'   /usr/local/tomcat/webapps/ROOT/META-INF/extension.xed
# Tue, 31 Jan 2023 00:48:03 GMT
COPY file:a47c4dcd87c9dad97aff38c49188357e6193bcad50757e516cfb08a60d4de611 in /usr/local/bin/docker-entrypoint.sh 
# Tue, 31 Jan 2023 00:48:03 GMT
VOLUME [/usr/local/xwiki]
# Tue, 31 Jan 2023 00:48:03 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 31 Jan 2023 00:48:03 GMT
CMD ["xwiki"]
```

-	Layers:
	-	`sha256:0509fae36eb0656f8bdb23f8ae64100d893bcea2563e97468d337e04d2d0410b`  
		Last Modified: Wed, 02 Nov 2022 18:50:21 GMT  
		Size: 28.4 MB (28382154 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e502a1af2bcd98f5f0d2f5e4da1a0e7bbe07a2c548e2662f7d37dce5ae1df46c`  
		Last Modified: Wed, 02 Nov 2022 19:48:28 GMT  
		Size: 12.4 MB (12396330 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bc4598c07dd818f03a0378b0341a4a8e80f0152fbb3e7d5246ca4f466f42e611`  
		Last Modified: Fri, 04 Nov 2022 22:46:46 GMT  
		Size: 45.0 MB (44958470 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:715a937a1066f998b331fcd62256ad01a5571bdf46804e97825afc64f9ebb427`  
		Last Modified: Fri, 04 Nov 2022 22:46:41 GMT  
		Size: 160.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5fb623f082f74b2fa9fc2c4e3f3a4802875cb9753cfa26ed940201ce72bb56cb`  
		Last Modified: Sat, 05 Nov 2022 00:03:40 GMT  
		Size: 172.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:33260b83200262bbd546be371ad3c1f50f5ae7228afb87982d6fa9d6b11bf26f`  
		Last Modified: Tue, 15 Nov 2022 05:10:19 GMT  
		Size: 12.2 MB (12207235 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0955fb697ea9b30a1b4f95385464f646aa1525cb6efba648e22df84ebef6b2ee`  
		Last Modified: Tue, 15 Nov 2022 05:10:18 GMT  
		Size: 452.0 KB (452021 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6eddcf66f2083b1487296a0308e0b058917c97f614f12428d82d89662038dc2e`  
		Last Modified: Tue, 15 Nov 2022 05:10:18 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ae5f60bb64f3fa11da3d15a9639f886186b4c2c021455c3f9db22e0cfe1b1311`  
		Last Modified: Wed, 11 Jan 2023 03:11:14 GMT  
		Size: 173.8 MB (173806827 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1814d85fce571b42f2cfa7c8a904e1a184ee6f49642242a44bbe0037088994a0`  
		Last Modified: Tue, 31 Jan 2023 00:56:04 GMT  
		Size: 307.1 MB (307117070 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8aec0e24b4fa870989f014944c3c7d535355a2371fc8c948b2b11f9b377efe6e`  
		Last Modified: Tue, 31 Jan 2023 00:55:50 GMT  
		Size: 2.4 MB (2377182 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0b65081619aa0114a7f367836ef421eb8d951e559e0f089c7728af7813b1ea62`  
		Last Modified: Tue, 31 Jan 2023 00:55:49 GMT  
		Size: 1.3 KB (1348 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:46ebad072e608146426d8dc30828937049eea36c2e636d7790b4960d6d586977`  
		Last Modified: Tue, 31 Jan 2023 00:55:49 GMT  
		Size: 2.3 KB (2308 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:708fefcedd4ee6c106da247a68c5790f5ab00225d1cdfff8465575265c3a54e6`  
		Last Modified: Tue, 31 Jan 2023 00:55:49 GMT  
		Size: 6.0 KB (6008 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:81e3bf8e20bc921031e7549a41dec1b2d7795cc6da40a0e7096bf654b25c5c3e`  
		Last Modified: Tue, 31 Jan 2023 00:55:49 GMT  
		Size: 2.5 KB (2507 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `xwiki:stable-mariadb`

```console
$ docker pull xwiki@sha256:725347355967f33745268f1167cc3c1b12fc85e327ccfa96da0848d05e3836c4
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `xwiki:stable-mariadb` - linux; amd64

```console
$ docker pull xwiki@sha256:cca1fb53bc2f0240f7f4843b846210e341a6002d7b18a0b90202520ce2f4ead0
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **588.7 MB (588672467 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:0088d72e62c01c9996a75e1b7e2296ba530b2dbd4054be70a006b33295aa4ff9`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["xwiki"]`

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
# Wed, 02 Nov 2022 18:44:10 GMT
RUN apt-get update     && DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends tzdata curl wget ca-certificates fontconfig locales     && echo "en_US.UTF-8 UTF-8" >> /etc/locale.gen     && locale-gen en_US.UTF-8     && rm -rf /var/lib/apt/lists/*
# Fri, 04 Nov 2022 23:21:41 GMT
ENV JAVA_VERSION=jdk-11.0.17+8
# Fri, 04 Nov 2022 23:22:31 GMT
RUN set -eux;     ARCH="$(dpkg --print-architecture)";     case "${ARCH}" in        aarch64|arm64)          ESUM='bd6efe3290c8b5a42f695a55a26f3e3c9c284288574879d4b7089f31f5114177';          BINARY_URL='https://github.com/adoptium/temurin11-binaries/releases/download/jdk-11.0.17%2B8/OpenJDK11U-jre_aarch64_linux_hotspot_11.0.17_8.tar.gz';          ;;        armhf|arm)          ESUM='8cf113d3d7fa808895c8d2e41bb890af21c47e38c2460e0588147a4bb8fc658d';          BINARY_URL='https://github.com/adoptium/temurin11-binaries/releases/download/jdk-11.0.17%2B8/OpenJDK11U-jre_arm_linux_hotspot_11.0.17_8.tar.gz';          ;;        ppc64el|powerpc:common64)          ESUM='0ca3d806131ab5834c501f9c625bb0248cd528af361c704503348e9c9605bedf';          BINARY_URL='https://github.com/adoptium/temurin11-binaries/releases/download/jdk-11.0.17%2B8/OpenJDK11U-jre_ppc64le_linux_hotspot_11.0.17_8.tar.gz';          ;;        s390x|s390:64-bit)          ESUM='dd3b159a374086e65cb07c4ccb226c90f9c02ef929cba6f0b642171d7ed97fa4';          BINARY_URL='https://github.com/adoptium/temurin11-binaries/releases/download/jdk-11.0.17%2B8/OpenJDK11U-jre_s390x_linux_hotspot_11.0.17_8.tar.gz';          ;;        amd64|i386:x86-64)          ESUM='752616097e09d7f60a3ad8bd312f90eaf50ac72577e55df229fe6e8091148f79';          BINARY_URL='https://github.com/adoptium/temurin11-binaries/releases/download/jdk-11.0.17%2B8/OpenJDK11U-jre_x64_linux_hotspot_11.0.17_8.tar.gz';          ;;        *)          echo "Unsupported arch: ${ARCH}";          exit 1;          ;;     esac; 	  wget -O /tmp/openjdk.tar.gz ${BINARY_URL}; 	  echo "${ESUM} */tmp/openjdk.tar.gz" | sha256sum -c -; 	  mkdir -p "$JAVA_HOME"; 	  tar --extract 	      --file /tmp/openjdk.tar.gz 	      --directory "$JAVA_HOME" 	      --strip-components 1 	      --no-same-owner 	  ;     rm /tmp/openjdk.tar.gz;     find "$JAVA_HOME/lib" -name '*.so' -exec dirname '{}' ';' | sort -u > /etc/ld.so.conf.d/docker-openjdk.conf;     ldconfig;     java -Xshare:dump;
# Fri, 04 Nov 2022 23:22:32 GMT
RUN echo Verifying install ...     && fileEncoding="$(echo 'System.out.println(System.getProperty("file.encoding"))' | jshell -s -)"; [ "$fileEncoding" = 'UTF-8' ]; rm -rf ~/.java     && echo java --version && java --version     && echo Complete.
# Sat, 05 Nov 2022 01:35:16 GMT
ENV CATALINA_HOME=/usr/local/tomcat
# Sat, 05 Nov 2022 01:35:16 GMT
ENV PATH=/usr/local/tomcat/bin:/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Sat, 05 Nov 2022 01:35:17 GMT
RUN mkdir -p "$CATALINA_HOME"
# Sat, 05 Nov 2022 01:35:17 GMT
WORKDIR /usr/local/tomcat
# Sat, 05 Nov 2022 01:35:17 GMT
ENV TOMCAT_NATIVE_LIBDIR=/usr/local/tomcat/native-jni-lib
# Sat, 05 Nov 2022 01:35:17 GMT
ENV LD_LIBRARY_PATH=/usr/local/tomcat/native-jni-lib
# Sat, 05 Nov 2022 01:39:54 GMT
ENV GPG_KEYS=48F8E69F6390C9F25CFEDCD268248959359E722B A9C5DF4D22E99998D9875A5110C01C5A2F6059E7 DCFD35E0BF8CA7344752DE8B6FB21E8933C60243
# Sat, 05 Nov 2022 01:39:54 GMT
ENV TOMCAT_MAJOR=9
# Tue, 15 Nov 2022 03:06:43 GMT
ENV TOMCAT_VERSION=9.0.69
# Tue, 15 Nov 2022 03:06:43 GMT
ENV TOMCAT_SHA512=8c883c54ce9ce43eba37756a6404cdf3477879883a3e6d146dc8a7aa5e0425f487466afe6b6da4a895927cb7cb59177b9379cec18000f2de12785be57408c779
# Tue, 15 Nov 2022 03:06:44 GMT
COPY dir:b1a33aa3993dbbfbebb33bd9aa546b60c2f2191abf1227f453d4e830f6deb35f in /usr/local/tomcat 
# Tue, 15 Nov 2022 03:06:48 GMT
RUN set -eux; 	apt-get update; 	xargs -rt apt-get install -y --no-install-recommends < "$TOMCAT_NATIVE_LIBDIR/.dependencies.txt"; 	rm -rf /var/lib/apt/lists/*
# Tue, 15 Nov 2022 03:06:49 GMT
RUN set -eux; 	nativeLines="$(catalina.sh configtest 2>&1)"; 	nativeLines="$(echo "$nativeLines" | grep 'Apache Tomcat Native')"; 	nativeLines="$(echo "$nativeLines" | sort -u)"; 	if ! echo "$nativeLines" | grep -E 'INFO: Loaded( APR based)? Apache Tomcat Native library' >&2; then 		echo >&2 "$nativeLines"; 		exit 1; 	fi
# Tue, 15 Nov 2022 03:06:49 GMT
EXPOSE 8080
# Tue, 15 Nov 2022 03:06:49 GMT
CMD ["catalina.sh" "run"]
# Wed, 11 Jan 2023 02:47:03 GMT
LABEL org.opencontainers.image.authors=XWiki Development Team <committers@xwiki.org>
# Wed, 11 Jan 2023 02:47:03 GMT
LABEL org.opencontainers.image.url=https://hub.docker.com/_/xwiki
# Wed, 11 Jan 2023 02:47:03 GMT
LABEL org.opencontainers.image.documentation=https://hub.docker.com/_/xwiki
# Wed, 11 Jan 2023 02:47:03 GMT
LABEL org.opencontainers.image.source=https://github.com/xwiki/xwiki-docker.git
# Wed, 11 Jan 2023 02:47:04 GMT
LABEL org.opencontainers.image.vendor=xwiki.org
# Wed, 11 Jan 2023 02:47:04 GMT
LABEL org.opencontainers.image.licenses=LGPL-2.1
# Wed, 11 Jan 2023 02:49:03 GMT
RUN apt-get update &&   apt-get --no-install-recommends -y install     curl     libreoffice     unzip     procps &&   rm -rf /var/lib/apt/lists/*
# Tue, 31 Jan 2023 00:20:17 GMT
ENV XWIKI_VERSION=15.0
# Tue, 31 Jan 2023 00:20:17 GMT
ENV XWIKI_URL_PREFIX=https://maven.xwiki.org/releases/org/xwiki/platform/xwiki-platform-distribution-war/15.0
# Tue, 31 Jan 2023 00:20:17 GMT
ENV XWIKI_DOWNLOAD_SHA256=79ba0f479bbc49521c113821adc9d91141075a9470d7f9bbb6994ca59c30d121
# Tue, 31 Jan 2023 00:21:18 GMT
RUN rm -rf /usr/local/tomcat/webapps/* &&   mkdir -p /usr/local/tomcat/temp &&   mkdir -p /usr/local/xwiki/data &&   curl -fSL "${XWIKI_URL_PREFIX}/xwiki-platform-distribution-war-${XWIKI_VERSION}.war" -o xwiki.war &&   echo "$XWIKI_DOWNLOAD_SHA256 xwiki.war" | sha256sum -c - &&   unzip -d /usr/local/tomcat/webapps/ROOT xwiki.war &&   rm -f xwiki.war
# Tue, 31 Jan 2023 00:22:50 GMT
ENV MARIADB_JDBC_VERSION=3.1.1
# Tue, 31 Jan 2023 00:22:50 GMT
ENV MARIADB_JDBC_SHA256=a554541fd88047905fb0c4c10e1d85295f5e38c7bb5fb408b425392a79fc26e3
# Tue, 31 Jan 2023 00:22:50 GMT
ENV MARIADB_JDBC_PREFIX=https://repo1.maven.org/maven2/org/mariadb/jdbc/mariadb-java-client/3.1.1
# Tue, 31 Jan 2023 00:22:50 GMT
ENV MARIADB_JDBC_ARTIFACT=mariadb-java-client-3.1.1.jar
# Tue, 31 Jan 2023 00:22:50 GMT
ENV MARIADB_JDBC_TARGET=/usr/local/tomcat/webapps/ROOT/WEB-INF/lib/mariadb-java-client-3.1.1.jar
# Tue, 31 Jan 2023 00:22:51 GMT
RUN curl -fSL "${MARIADB_JDBC_PREFIX}/${MARIADB_JDBC_ARTIFACT}" -o $MARIADB_JDBC_TARGET &&   echo "$MARIADB_JDBC_SHA256 $MARIADB_JDBC_TARGET" | sha256sum -c -
# Tue, 31 Jan 2023 00:22:51 GMT
COPY file:0a1be11e2eb610a1dbcd415404e3a592641110b93090030cb831e3a19a163017 in /usr/local/tomcat/bin/ 
# Tue, 31 Jan 2023 00:22:51 GMT
COPY file:0e237c3876eeb3b5f3473a064d3e507da2df6c228ca714687930b34e3b687601 in /usr/local/tomcat/webapps/ROOT/WEB-INF/hibernate.cfg.xml 
# Tue, 31 Jan 2023 00:22:52 GMT
RUN sed -i 's/<id>org.xwiki.platform:xwiki-platform-distribution-war/<id>org.xwiki.platform:xwiki-platform-distribution-docker/'   /usr/local/tomcat/webapps/ROOT/META-INF/extension.xed
# Tue, 31 Jan 2023 00:22:52 GMT
COPY file:a47c4dcd87c9dad97aff38c49188357e6193bcad50757e516cfb08a60d4de611 in /usr/local/bin/docker-entrypoint.sh 
# Tue, 31 Jan 2023 00:22:52 GMT
VOLUME [/usr/local/xwiki]
# Tue, 31 Jan 2023 00:22:52 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 31 Jan 2023 00:22:52 GMT
CMD ["xwiki"]
```

-	Layers:
	-	`sha256:e96e057aae67380a4ddb16c337c5c3669d97fdff69ec537f02aa2cc30d814281`  
		Last Modified: Wed, 02 Nov 2022 03:03:36 GMT  
		Size: 30.4 MB (30425607 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4ced2591451da3a02e2b6bb44752b9e3f00d77789921be4df5082fb9f9880ad0`  
		Last Modified: Wed, 02 Nov 2022 18:48:43 GMT  
		Size: 12.4 MB (12439006 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:df8f874ae8c08a9e69e5fbe6c5a64200a45386132a3203d1a9a7f1146d94cfbc`  
		Last Modified: Fri, 04 Nov 2022 23:29:33 GMT  
		Size: 46.6 MB (46629936 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:111b6c7486426c4b6989102c2ee5be856e8a58e20ab0a350b24a905d536e8e7f`  
		Last Modified: Fri, 04 Nov 2022 23:29:26 GMT  
		Size: 161.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e6f84dce457c6d4f7b7291fce05f8e77998a3a7722a54125a1f1d52ca83043b4`  
		Last Modified: Sat, 05 Nov 2022 01:50:51 GMT  
		Size: 173.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a6c26749ee782392e38845ee2ba79b0da586ef6a45d8e7f29c7af14612278547`  
		Last Modified: Tue, 15 Nov 2022 03:19:57 GMT  
		Size: 12.2 MB (12200249 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4dddc6d9fa6024025b3fcfe729cab2dc544fb25476eca6e80b1af8e8d93bb0ee`  
		Last Modified: Tue, 15 Nov 2022 03:19:56 GMT  
		Size: 452.7 KB (452680 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:06637eebe5e72c8ad9019ad4eb4cdde1f11f7d4c24c7ed7374cf8966343aa2fb`  
		Last Modified: Tue, 15 Nov 2022 03:19:56 GMT  
		Size: 131.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b276fb8390410a8208724033e325715ea26000d5a1a762d4c3699b927884fbfe`  
		Last Modified: Wed, 11 Jan 2023 02:52:45 GMT  
		Size: 178.8 MB (178805608 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:156ca91198173149698aa0396648a9608b6ab1f2bc2666800843ce33c9f85b6e`  
		Last Modified: Tue, 31 Jan 2023 00:24:09 GMT  
		Size: 307.1 MB (307117069 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:457b62e39784bb863cc6a7514f591232a9b9442f2f105a85bdbd5e4abb166ad6`  
		Last Modified: Tue, 31 Jan 2023 00:25:23 GMT  
		Size: 589.7 KB (589675 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:30adbbecb36197c3e48c90be60a50c089cb9738a771c968b36240b05b8164a30`  
		Last Modified: Tue, 31 Jan 2023 00:25:22 GMT  
		Size: 1.3 KB (1345 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3bfcc8a896e6e21d5c28da101d5d57167a5cfc49c542a407feabe27f6c355b6f`  
		Last Modified: Tue, 31 Jan 2023 00:25:22 GMT  
		Size: 2.3 KB (2312 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5cbacf6c3ece365f64b683c8ab4fe61301319c8f1bd26d38ea40abbbd15bc7d4`  
		Last Modified: Tue, 31 Jan 2023 00:25:23 GMT  
		Size: 6.0 KB (6008 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6687ecee0e041196fd810c316565d70808b445cdce0b089b2177e6636bffd9fe`  
		Last Modified: Tue, 31 Jan 2023 00:25:23 GMT  
		Size: 2.5 KB (2507 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `xwiki:stable-mariadb` - linux; arm64 variant v8

```console
$ docker pull xwiki@sha256:14b1c6df2a5c5c9b549f372fce50719f39fc809b8b02c945d92eb29c29f7bc75
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **579.9 MB (579922416 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d9a728666283f6f4b71f567ce6c5ef1e2dc544facfd01d52fdf1577be95c6b07`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["xwiki"]`

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
# Wed, 02 Nov 2022 19:44:32 GMT
RUN apt-get update     && DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends tzdata curl wget ca-certificates fontconfig locales     && echo "en_US.UTF-8 UTF-8" >> /etc/locale.gen     && locale-gen en_US.UTF-8     && rm -rf /var/lib/apt/lists/*
# Fri, 04 Nov 2022 22:40:54 GMT
ENV JAVA_VERSION=jdk-11.0.17+8
# Fri, 04 Nov 2022 22:41:33 GMT
RUN set -eux;     ARCH="$(dpkg --print-architecture)";     case "${ARCH}" in        aarch64|arm64)          ESUM='bd6efe3290c8b5a42f695a55a26f3e3c9c284288574879d4b7089f31f5114177';          BINARY_URL='https://github.com/adoptium/temurin11-binaries/releases/download/jdk-11.0.17%2B8/OpenJDK11U-jre_aarch64_linux_hotspot_11.0.17_8.tar.gz';          ;;        armhf|arm)          ESUM='8cf113d3d7fa808895c8d2e41bb890af21c47e38c2460e0588147a4bb8fc658d';          BINARY_URL='https://github.com/adoptium/temurin11-binaries/releases/download/jdk-11.0.17%2B8/OpenJDK11U-jre_arm_linux_hotspot_11.0.17_8.tar.gz';          ;;        ppc64el|powerpc:common64)          ESUM='0ca3d806131ab5834c501f9c625bb0248cd528af361c704503348e9c9605bedf';          BINARY_URL='https://github.com/adoptium/temurin11-binaries/releases/download/jdk-11.0.17%2B8/OpenJDK11U-jre_ppc64le_linux_hotspot_11.0.17_8.tar.gz';          ;;        s390x|s390:64-bit)          ESUM='dd3b159a374086e65cb07c4ccb226c90f9c02ef929cba6f0b642171d7ed97fa4';          BINARY_URL='https://github.com/adoptium/temurin11-binaries/releases/download/jdk-11.0.17%2B8/OpenJDK11U-jre_s390x_linux_hotspot_11.0.17_8.tar.gz';          ;;        amd64|i386:x86-64)          ESUM='752616097e09d7f60a3ad8bd312f90eaf50ac72577e55df229fe6e8091148f79';          BINARY_URL='https://github.com/adoptium/temurin11-binaries/releases/download/jdk-11.0.17%2B8/OpenJDK11U-jre_x64_linux_hotspot_11.0.17_8.tar.gz';          ;;        *)          echo "Unsupported arch: ${ARCH}";          exit 1;          ;;     esac; 	  wget -O /tmp/openjdk.tar.gz ${BINARY_URL}; 	  echo "${ESUM} */tmp/openjdk.tar.gz" | sha256sum -c -; 	  mkdir -p "$JAVA_HOME"; 	  tar --extract 	      --file /tmp/openjdk.tar.gz 	      --directory "$JAVA_HOME" 	      --strip-components 1 	      --no-same-owner 	  ;     rm /tmp/openjdk.tar.gz;     find "$JAVA_HOME/lib" -name '*.so' -exec dirname '{}' ';' | sort -u > /etc/ld.so.conf.d/docker-openjdk.conf;     ldconfig;     java -Xshare:dump;
# Fri, 04 Nov 2022 22:41:34 GMT
RUN echo Verifying install ...     && fileEncoding="$(echo 'System.out.println(System.getProperty("file.encoding"))' | jshell -s -)"; [ "$fileEncoding" = 'UTF-8' ]; rm -rf ~/.java     && echo java --version && java --version     && echo Complete.
# Fri, 04 Nov 2022 23:48:38 GMT
ENV CATALINA_HOME=/usr/local/tomcat
# Fri, 04 Nov 2022 23:48:38 GMT
ENV PATH=/usr/local/tomcat/bin:/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Fri, 04 Nov 2022 23:48:38 GMT
RUN mkdir -p "$CATALINA_HOME"
# Fri, 04 Nov 2022 23:48:39 GMT
WORKDIR /usr/local/tomcat
# Fri, 04 Nov 2022 23:48:39 GMT
ENV TOMCAT_NATIVE_LIBDIR=/usr/local/tomcat/native-jni-lib
# Fri, 04 Nov 2022 23:48:39 GMT
ENV LD_LIBRARY_PATH=/usr/local/tomcat/native-jni-lib
# Fri, 04 Nov 2022 23:53:12 GMT
ENV GPG_KEYS=48F8E69F6390C9F25CFEDCD268248959359E722B A9C5DF4D22E99998D9875A5110C01C5A2F6059E7 DCFD35E0BF8CA7344752DE8B6FB21E8933C60243
# Fri, 04 Nov 2022 23:53:12 GMT
ENV TOMCAT_MAJOR=9
# Tue, 15 Nov 2022 04:57:22 GMT
ENV TOMCAT_VERSION=9.0.69
# Tue, 15 Nov 2022 04:57:22 GMT
ENV TOMCAT_SHA512=8c883c54ce9ce43eba37756a6404cdf3477879883a3e6d146dc8a7aa5e0425f487466afe6b6da4a895927cb7cb59177b9379cec18000f2de12785be57408c779
# Tue, 15 Nov 2022 04:57:22 GMT
COPY dir:096b403a5f78b17e6b4bff63128a9c93941b97f22470991610dd641633d977f1 in /usr/local/tomcat 
# Tue, 15 Nov 2022 04:57:25 GMT
RUN set -eux; 	apt-get update; 	xargs -rt apt-get install -y --no-install-recommends < "$TOMCAT_NATIVE_LIBDIR/.dependencies.txt"; 	rm -rf /var/lib/apt/lists/*
# Tue, 15 Nov 2022 04:57:26 GMT
RUN set -eux; 	nativeLines="$(catalina.sh configtest 2>&1)"; 	nativeLines="$(echo "$nativeLines" | grep 'Apache Tomcat Native')"; 	nativeLines="$(echo "$nativeLines" | sort -u)"; 	if ! echo "$nativeLines" | grep -E 'INFO: Loaded( APR based)? Apache Tomcat Native library' >&2; then 		echo >&2 "$nativeLines"; 		exit 1; 	fi
# Tue, 15 Nov 2022 04:57:26 GMT
EXPOSE 8080
# Tue, 15 Nov 2022 04:57:27 GMT
CMD ["catalina.sh" "run"]
# Wed, 11 Jan 2023 03:05:10 GMT
LABEL org.opencontainers.image.authors=XWiki Development Team <committers@xwiki.org>
# Wed, 11 Jan 2023 03:05:10 GMT
LABEL org.opencontainers.image.url=https://hub.docker.com/_/xwiki
# Wed, 11 Jan 2023 03:05:10 GMT
LABEL org.opencontainers.image.documentation=https://hub.docker.com/_/xwiki
# Wed, 11 Jan 2023 03:05:10 GMT
LABEL org.opencontainers.image.source=https://github.com/xwiki/xwiki-docker.git
# Wed, 11 Jan 2023 03:05:11 GMT
LABEL org.opencontainers.image.vendor=xwiki.org
# Wed, 11 Jan 2023 03:05:11 GMT
LABEL org.opencontainers.image.licenses=LGPL-2.1
# Wed, 11 Jan 2023 03:07:37 GMT
RUN apt-get update &&   apt-get --no-install-recommends -y install     curl     libreoffice     unzip     procps &&   rm -rf /var/lib/apt/lists/*
# Tue, 31 Jan 2023 00:47:12 GMT
ENV XWIKI_VERSION=15.0
# Tue, 31 Jan 2023 00:47:12 GMT
ENV XWIKI_URL_PREFIX=https://maven.xwiki.org/releases/org/xwiki/platform/xwiki-platform-distribution-war/15.0
# Tue, 31 Jan 2023 00:47:12 GMT
ENV XWIKI_DOWNLOAD_SHA256=79ba0f479bbc49521c113821adc9d91141075a9470d7f9bbb6994ca59c30d121
# Tue, 31 Jan 2023 00:47:58 GMT
RUN rm -rf /usr/local/tomcat/webapps/* &&   mkdir -p /usr/local/tomcat/temp &&   mkdir -p /usr/local/xwiki/data &&   curl -fSL "${XWIKI_URL_PREFIX}/xwiki-platform-distribution-war-${XWIKI_VERSION}.war" -o xwiki.war &&   echo "$XWIKI_DOWNLOAD_SHA256 xwiki.war" | sha256sum -c - &&   unzip -d /usr/local/tomcat/webapps/ROOT xwiki.war &&   rm -f xwiki.war
# Tue, 31 Jan 2023 00:54:48 GMT
ENV MARIADB_JDBC_VERSION=3.1.1
# Tue, 31 Jan 2023 00:54:48 GMT
ENV MARIADB_JDBC_SHA256=a554541fd88047905fb0c4c10e1d85295f5e38c7bb5fb408b425392a79fc26e3
# Tue, 31 Jan 2023 00:54:48 GMT
ENV MARIADB_JDBC_PREFIX=https://repo1.maven.org/maven2/org/mariadb/jdbc/mariadb-java-client/3.1.1
# Tue, 31 Jan 2023 00:54:48 GMT
ENV MARIADB_JDBC_ARTIFACT=mariadb-java-client-3.1.1.jar
# Tue, 31 Jan 2023 00:54:48 GMT
ENV MARIADB_JDBC_TARGET=/usr/local/tomcat/webapps/ROOT/WEB-INF/lib/mariadb-java-client-3.1.1.jar
# Tue, 31 Jan 2023 00:54:49 GMT
RUN curl -fSL "${MARIADB_JDBC_PREFIX}/${MARIADB_JDBC_ARTIFACT}" -o $MARIADB_JDBC_TARGET &&   echo "$MARIADB_JDBC_SHA256 $MARIADB_JDBC_TARGET" | sha256sum -c -
# Tue, 31 Jan 2023 00:54:49 GMT
COPY file:0a1be11e2eb610a1dbcd415404e3a592641110b93090030cb831e3a19a163017 in /usr/local/tomcat/bin/ 
# Tue, 31 Jan 2023 00:54:49 GMT
COPY file:0e237c3876eeb3b5f3473a064d3e507da2df6c228ca714687930b34e3b687601 in /usr/local/tomcat/webapps/ROOT/WEB-INF/hibernate.cfg.xml 
# Tue, 31 Jan 2023 00:54:49 GMT
RUN sed -i 's/<id>org.xwiki.platform:xwiki-platform-distribution-war/<id>org.xwiki.platform:xwiki-platform-distribution-docker/'   /usr/local/tomcat/webapps/ROOT/META-INF/extension.xed
# Tue, 31 Jan 2023 00:54:49 GMT
COPY file:a47c4dcd87c9dad97aff38c49188357e6193bcad50757e516cfb08a60d4de611 in /usr/local/bin/docker-entrypoint.sh 
# Tue, 31 Jan 2023 00:54:49 GMT
VOLUME [/usr/local/xwiki]
# Tue, 31 Jan 2023 00:54:50 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 31 Jan 2023 00:54:50 GMT
CMD ["xwiki"]
```

-	Layers:
	-	`sha256:0509fae36eb0656f8bdb23f8ae64100d893bcea2563e97468d337e04d2d0410b`  
		Last Modified: Wed, 02 Nov 2022 18:50:21 GMT  
		Size: 28.4 MB (28382154 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e502a1af2bcd98f5f0d2f5e4da1a0e7bbe07a2c548e2662f7d37dce5ae1df46c`  
		Last Modified: Wed, 02 Nov 2022 19:48:28 GMT  
		Size: 12.4 MB (12396330 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bc4598c07dd818f03a0378b0341a4a8e80f0152fbb3e7d5246ca4f466f42e611`  
		Last Modified: Fri, 04 Nov 2022 22:46:46 GMT  
		Size: 45.0 MB (44958470 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:715a937a1066f998b331fcd62256ad01a5571bdf46804e97825afc64f9ebb427`  
		Last Modified: Fri, 04 Nov 2022 22:46:41 GMT  
		Size: 160.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5fb623f082f74b2fa9fc2c4e3f3a4802875cb9753cfa26ed940201ce72bb56cb`  
		Last Modified: Sat, 05 Nov 2022 00:03:40 GMT  
		Size: 172.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:33260b83200262bbd546be371ad3c1f50f5ae7228afb87982d6fa9d6b11bf26f`  
		Last Modified: Tue, 15 Nov 2022 05:10:19 GMT  
		Size: 12.2 MB (12207235 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0955fb697ea9b30a1b4f95385464f646aa1525cb6efba648e22df84ebef6b2ee`  
		Last Modified: Tue, 15 Nov 2022 05:10:18 GMT  
		Size: 452.0 KB (452021 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6eddcf66f2083b1487296a0308e0b058917c97f614f12428d82d89662038dc2e`  
		Last Modified: Tue, 15 Nov 2022 05:10:18 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ae5f60bb64f3fa11da3d15a9639f886186b4c2c021455c3f9db22e0cfe1b1311`  
		Last Modified: Wed, 11 Jan 2023 03:11:14 GMT  
		Size: 173.8 MB (173806827 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1814d85fce571b42f2cfa7c8a904e1a184ee6f49642242a44bbe0037088994a0`  
		Last Modified: Tue, 31 Jan 2023 00:56:04 GMT  
		Size: 307.1 MB (307117070 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e8637677b7ba0da683afa4e56ff0561e4ba77c8782d5a98da785f4ef58d1caf9`  
		Last Modified: Tue, 31 Jan 2023 00:57:14 GMT  
		Size: 589.7 KB (589677 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:61a67398bc888bcce1656edec9bb40409ce0ffc2fe83d0437c28dd64a8f697ce`  
		Last Modified: Tue, 31 Jan 2023 00:57:14 GMT  
		Size: 1.3 KB (1345 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7ebda7e506ea819ce9717c3d0334df81608bc4c7149cd47ebc9a32790141a637`  
		Last Modified: Tue, 31 Jan 2023 00:57:14 GMT  
		Size: 2.3 KB (2313 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2ceebbf08640e235a928c9df650ca3ab8d0c6b506faa158ecde5fdde34bf8813`  
		Last Modified: Tue, 31 Jan 2023 00:57:14 GMT  
		Size: 6.0 KB (6007 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:12b1d23eae23b1a09ecd4185941d43f13d4ad633d4c6257ab8107a8eebd5fb12`  
		Last Modified: Tue, 31 Jan 2023 00:57:14 GMT  
		Size: 2.5 KB (2506 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `xwiki:stable-mariadb-tomcat`

```console
$ docker pull xwiki@sha256:725347355967f33745268f1167cc3c1b12fc85e327ccfa96da0848d05e3836c4
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `xwiki:stable-mariadb-tomcat` - linux; amd64

```console
$ docker pull xwiki@sha256:cca1fb53bc2f0240f7f4843b846210e341a6002d7b18a0b90202520ce2f4ead0
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **588.7 MB (588672467 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:0088d72e62c01c9996a75e1b7e2296ba530b2dbd4054be70a006b33295aa4ff9`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["xwiki"]`

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
# Wed, 02 Nov 2022 18:44:10 GMT
RUN apt-get update     && DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends tzdata curl wget ca-certificates fontconfig locales     && echo "en_US.UTF-8 UTF-8" >> /etc/locale.gen     && locale-gen en_US.UTF-8     && rm -rf /var/lib/apt/lists/*
# Fri, 04 Nov 2022 23:21:41 GMT
ENV JAVA_VERSION=jdk-11.0.17+8
# Fri, 04 Nov 2022 23:22:31 GMT
RUN set -eux;     ARCH="$(dpkg --print-architecture)";     case "${ARCH}" in        aarch64|arm64)          ESUM='bd6efe3290c8b5a42f695a55a26f3e3c9c284288574879d4b7089f31f5114177';          BINARY_URL='https://github.com/adoptium/temurin11-binaries/releases/download/jdk-11.0.17%2B8/OpenJDK11U-jre_aarch64_linux_hotspot_11.0.17_8.tar.gz';          ;;        armhf|arm)          ESUM='8cf113d3d7fa808895c8d2e41bb890af21c47e38c2460e0588147a4bb8fc658d';          BINARY_URL='https://github.com/adoptium/temurin11-binaries/releases/download/jdk-11.0.17%2B8/OpenJDK11U-jre_arm_linux_hotspot_11.0.17_8.tar.gz';          ;;        ppc64el|powerpc:common64)          ESUM='0ca3d806131ab5834c501f9c625bb0248cd528af361c704503348e9c9605bedf';          BINARY_URL='https://github.com/adoptium/temurin11-binaries/releases/download/jdk-11.0.17%2B8/OpenJDK11U-jre_ppc64le_linux_hotspot_11.0.17_8.tar.gz';          ;;        s390x|s390:64-bit)          ESUM='dd3b159a374086e65cb07c4ccb226c90f9c02ef929cba6f0b642171d7ed97fa4';          BINARY_URL='https://github.com/adoptium/temurin11-binaries/releases/download/jdk-11.0.17%2B8/OpenJDK11U-jre_s390x_linux_hotspot_11.0.17_8.tar.gz';          ;;        amd64|i386:x86-64)          ESUM='752616097e09d7f60a3ad8bd312f90eaf50ac72577e55df229fe6e8091148f79';          BINARY_URL='https://github.com/adoptium/temurin11-binaries/releases/download/jdk-11.0.17%2B8/OpenJDK11U-jre_x64_linux_hotspot_11.0.17_8.tar.gz';          ;;        *)          echo "Unsupported arch: ${ARCH}";          exit 1;          ;;     esac; 	  wget -O /tmp/openjdk.tar.gz ${BINARY_URL}; 	  echo "${ESUM} */tmp/openjdk.tar.gz" | sha256sum -c -; 	  mkdir -p "$JAVA_HOME"; 	  tar --extract 	      --file /tmp/openjdk.tar.gz 	      --directory "$JAVA_HOME" 	      --strip-components 1 	      --no-same-owner 	  ;     rm /tmp/openjdk.tar.gz;     find "$JAVA_HOME/lib" -name '*.so' -exec dirname '{}' ';' | sort -u > /etc/ld.so.conf.d/docker-openjdk.conf;     ldconfig;     java -Xshare:dump;
# Fri, 04 Nov 2022 23:22:32 GMT
RUN echo Verifying install ...     && fileEncoding="$(echo 'System.out.println(System.getProperty("file.encoding"))' | jshell -s -)"; [ "$fileEncoding" = 'UTF-8' ]; rm -rf ~/.java     && echo java --version && java --version     && echo Complete.
# Sat, 05 Nov 2022 01:35:16 GMT
ENV CATALINA_HOME=/usr/local/tomcat
# Sat, 05 Nov 2022 01:35:16 GMT
ENV PATH=/usr/local/tomcat/bin:/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Sat, 05 Nov 2022 01:35:17 GMT
RUN mkdir -p "$CATALINA_HOME"
# Sat, 05 Nov 2022 01:35:17 GMT
WORKDIR /usr/local/tomcat
# Sat, 05 Nov 2022 01:35:17 GMT
ENV TOMCAT_NATIVE_LIBDIR=/usr/local/tomcat/native-jni-lib
# Sat, 05 Nov 2022 01:35:17 GMT
ENV LD_LIBRARY_PATH=/usr/local/tomcat/native-jni-lib
# Sat, 05 Nov 2022 01:39:54 GMT
ENV GPG_KEYS=48F8E69F6390C9F25CFEDCD268248959359E722B A9C5DF4D22E99998D9875A5110C01C5A2F6059E7 DCFD35E0BF8CA7344752DE8B6FB21E8933C60243
# Sat, 05 Nov 2022 01:39:54 GMT
ENV TOMCAT_MAJOR=9
# Tue, 15 Nov 2022 03:06:43 GMT
ENV TOMCAT_VERSION=9.0.69
# Tue, 15 Nov 2022 03:06:43 GMT
ENV TOMCAT_SHA512=8c883c54ce9ce43eba37756a6404cdf3477879883a3e6d146dc8a7aa5e0425f487466afe6b6da4a895927cb7cb59177b9379cec18000f2de12785be57408c779
# Tue, 15 Nov 2022 03:06:44 GMT
COPY dir:b1a33aa3993dbbfbebb33bd9aa546b60c2f2191abf1227f453d4e830f6deb35f in /usr/local/tomcat 
# Tue, 15 Nov 2022 03:06:48 GMT
RUN set -eux; 	apt-get update; 	xargs -rt apt-get install -y --no-install-recommends < "$TOMCAT_NATIVE_LIBDIR/.dependencies.txt"; 	rm -rf /var/lib/apt/lists/*
# Tue, 15 Nov 2022 03:06:49 GMT
RUN set -eux; 	nativeLines="$(catalina.sh configtest 2>&1)"; 	nativeLines="$(echo "$nativeLines" | grep 'Apache Tomcat Native')"; 	nativeLines="$(echo "$nativeLines" | sort -u)"; 	if ! echo "$nativeLines" | grep -E 'INFO: Loaded( APR based)? Apache Tomcat Native library' >&2; then 		echo >&2 "$nativeLines"; 		exit 1; 	fi
# Tue, 15 Nov 2022 03:06:49 GMT
EXPOSE 8080
# Tue, 15 Nov 2022 03:06:49 GMT
CMD ["catalina.sh" "run"]
# Wed, 11 Jan 2023 02:47:03 GMT
LABEL org.opencontainers.image.authors=XWiki Development Team <committers@xwiki.org>
# Wed, 11 Jan 2023 02:47:03 GMT
LABEL org.opencontainers.image.url=https://hub.docker.com/_/xwiki
# Wed, 11 Jan 2023 02:47:03 GMT
LABEL org.opencontainers.image.documentation=https://hub.docker.com/_/xwiki
# Wed, 11 Jan 2023 02:47:03 GMT
LABEL org.opencontainers.image.source=https://github.com/xwiki/xwiki-docker.git
# Wed, 11 Jan 2023 02:47:04 GMT
LABEL org.opencontainers.image.vendor=xwiki.org
# Wed, 11 Jan 2023 02:47:04 GMT
LABEL org.opencontainers.image.licenses=LGPL-2.1
# Wed, 11 Jan 2023 02:49:03 GMT
RUN apt-get update &&   apt-get --no-install-recommends -y install     curl     libreoffice     unzip     procps &&   rm -rf /var/lib/apt/lists/*
# Tue, 31 Jan 2023 00:20:17 GMT
ENV XWIKI_VERSION=15.0
# Tue, 31 Jan 2023 00:20:17 GMT
ENV XWIKI_URL_PREFIX=https://maven.xwiki.org/releases/org/xwiki/platform/xwiki-platform-distribution-war/15.0
# Tue, 31 Jan 2023 00:20:17 GMT
ENV XWIKI_DOWNLOAD_SHA256=79ba0f479bbc49521c113821adc9d91141075a9470d7f9bbb6994ca59c30d121
# Tue, 31 Jan 2023 00:21:18 GMT
RUN rm -rf /usr/local/tomcat/webapps/* &&   mkdir -p /usr/local/tomcat/temp &&   mkdir -p /usr/local/xwiki/data &&   curl -fSL "${XWIKI_URL_PREFIX}/xwiki-platform-distribution-war-${XWIKI_VERSION}.war" -o xwiki.war &&   echo "$XWIKI_DOWNLOAD_SHA256 xwiki.war" | sha256sum -c - &&   unzip -d /usr/local/tomcat/webapps/ROOT xwiki.war &&   rm -f xwiki.war
# Tue, 31 Jan 2023 00:22:50 GMT
ENV MARIADB_JDBC_VERSION=3.1.1
# Tue, 31 Jan 2023 00:22:50 GMT
ENV MARIADB_JDBC_SHA256=a554541fd88047905fb0c4c10e1d85295f5e38c7bb5fb408b425392a79fc26e3
# Tue, 31 Jan 2023 00:22:50 GMT
ENV MARIADB_JDBC_PREFIX=https://repo1.maven.org/maven2/org/mariadb/jdbc/mariadb-java-client/3.1.1
# Tue, 31 Jan 2023 00:22:50 GMT
ENV MARIADB_JDBC_ARTIFACT=mariadb-java-client-3.1.1.jar
# Tue, 31 Jan 2023 00:22:50 GMT
ENV MARIADB_JDBC_TARGET=/usr/local/tomcat/webapps/ROOT/WEB-INF/lib/mariadb-java-client-3.1.1.jar
# Tue, 31 Jan 2023 00:22:51 GMT
RUN curl -fSL "${MARIADB_JDBC_PREFIX}/${MARIADB_JDBC_ARTIFACT}" -o $MARIADB_JDBC_TARGET &&   echo "$MARIADB_JDBC_SHA256 $MARIADB_JDBC_TARGET" | sha256sum -c -
# Tue, 31 Jan 2023 00:22:51 GMT
COPY file:0a1be11e2eb610a1dbcd415404e3a592641110b93090030cb831e3a19a163017 in /usr/local/tomcat/bin/ 
# Tue, 31 Jan 2023 00:22:51 GMT
COPY file:0e237c3876eeb3b5f3473a064d3e507da2df6c228ca714687930b34e3b687601 in /usr/local/tomcat/webapps/ROOT/WEB-INF/hibernate.cfg.xml 
# Tue, 31 Jan 2023 00:22:52 GMT
RUN sed -i 's/<id>org.xwiki.platform:xwiki-platform-distribution-war/<id>org.xwiki.platform:xwiki-platform-distribution-docker/'   /usr/local/tomcat/webapps/ROOT/META-INF/extension.xed
# Tue, 31 Jan 2023 00:22:52 GMT
COPY file:a47c4dcd87c9dad97aff38c49188357e6193bcad50757e516cfb08a60d4de611 in /usr/local/bin/docker-entrypoint.sh 
# Tue, 31 Jan 2023 00:22:52 GMT
VOLUME [/usr/local/xwiki]
# Tue, 31 Jan 2023 00:22:52 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 31 Jan 2023 00:22:52 GMT
CMD ["xwiki"]
```

-	Layers:
	-	`sha256:e96e057aae67380a4ddb16c337c5c3669d97fdff69ec537f02aa2cc30d814281`  
		Last Modified: Wed, 02 Nov 2022 03:03:36 GMT  
		Size: 30.4 MB (30425607 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4ced2591451da3a02e2b6bb44752b9e3f00d77789921be4df5082fb9f9880ad0`  
		Last Modified: Wed, 02 Nov 2022 18:48:43 GMT  
		Size: 12.4 MB (12439006 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:df8f874ae8c08a9e69e5fbe6c5a64200a45386132a3203d1a9a7f1146d94cfbc`  
		Last Modified: Fri, 04 Nov 2022 23:29:33 GMT  
		Size: 46.6 MB (46629936 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:111b6c7486426c4b6989102c2ee5be856e8a58e20ab0a350b24a905d536e8e7f`  
		Last Modified: Fri, 04 Nov 2022 23:29:26 GMT  
		Size: 161.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e6f84dce457c6d4f7b7291fce05f8e77998a3a7722a54125a1f1d52ca83043b4`  
		Last Modified: Sat, 05 Nov 2022 01:50:51 GMT  
		Size: 173.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a6c26749ee782392e38845ee2ba79b0da586ef6a45d8e7f29c7af14612278547`  
		Last Modified: Tue, 15 Nov 2022 03:19:57 GMT  
		Size: 12.2 MB (12200249 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4dddc6d9fa6024025b3fcfe729cab2dc544fb25476eca6e80b1af8e8d93bb0ee`  
		Last Modified: Tue, 15 Nov 2022 03:19:56 GMT  
		Size: 452.7 KB (452680 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:06637eebe5e72c8ad9019ad4eb4cdde1f11f7d4c24c7ed7374cf8966343aa2fb`  
		Last Modified: Tue, 15 Nov 2022 03:19:56 GMT  
		Size: 131.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b276fb8390410a8208724033e325715ea26000d5a1a762d4c3699b927884fbfe`  
		Last Modified: Wed, 11 Jan 2023 02:52:45 GMT  
		Size: 178.8 MB (178805608 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:156ca91198173149698aa0396648a9608b6ab1f2bc2666800843ce33c9f85b6e`  
		Last Modified: Tue, 31 Jan 2023 00:24:09 GMT  
		Size: 307.1 MB (307117069 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:457b62e39784bb863cc6a7514f591232a9b9442f2f105a85bdbd5e4abb166ad6`  
		Last Modified: Tue, 31 Jan 2023 00:25:23 GMT  
		Size: 589.7 KB (589675 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:30adbbecb36197c3e48c90be60a50c089cb9738a771c968b36240b05b8164a30`  
		Last Modified: Tue, 31 Jan 2023 00:25:22 GMT  
		Size: 1.3 KB (1345 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3bfcc8a896e6e21d5c28da101d5d57167a5cfc49c542a407feabe27f6c355b6f`  
		Last Modified: Tue, 31 Jan 2023 00:25:22 GMT  
		Size: 2.3 KB (2312 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5cbacf6c3ece365f64b683c8ab4fe61301319c8f1bd26d38ea40abbbd15bc7d4`  
		Last Modified: Tue, 31 Jan 2023 00:25:23 GMT  
		Size: 6.0 KB (6008 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6687ecee0e041196fd810c316565d70808b445cdce0b089b2177e6636bffd9fe`  
		Last Modified: Tue, 31 Jan 2023 00:25:23 GMT  
		Size: 2.5 KB (2507 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `xwiki:stable-mariadb-tomcat` - linux; arm64 variant v8

```console
$ docker pull xwiki@sha256:14b1c6df2a5c5c9b549f372fce50719f39fc809b8b02c945d92eb29c29f7bc75
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **579.9 MB (579922416 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d9a728666283f6f4b71f567ce6c5ef1e2dc544facfd01d52fdf1577be95c6b07`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["xwiki"]`

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
# Wed, 02 Nov 2022 19:44:32 GMT
RUN apt-get update     && DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends tzdata curl wget ca-certificates fontconfig locales     && echo "en_US.UTF-8 UTF-8" >> /etc/locale.gen     && locale-gen en_US.UTF-8     && rm -rf /var/lib/apt/lists/*
# Fri, 04 Nov 2022 22:40:54 GMT
ENV JAVA_VERSION=jdk-11.0.17+8
# Fri, 04 Nov 2022 22:41:33 GMT
RUN set -eux;     ARCH="$(dpkg --print-architecture)";     case "${ARCH}" in        aarch64|arm64)          ESUM='bd6efe3290c8b5a42f695a55a26f3e3c9c284288574879d4b7089f31f5114177';          BINARY_URL='https://github.com/adoptium/temurin11-binaries/releases/download/jdk-11.0.17%2B8/OpenJDK11U-jre_aarch64_linux_hotspot_11.0.17_8.tar.gz';          ;;        armhf|arm)          ESUM='8cf113d3d7fa808895c8d2e41bb890af21c47e38c2460e0588147a4bb8fc658d';          BINARY_URL='https://github.com/adoptium/temurin11-binaries/releases/download/jdk-11.0.17%2B8/OpenJDK11U-jre_arm_linux_hotspot_11.0.17_8.tar.gz';          ;;        ppc64el|powerpc:common64)          ESUM='0ca3d806131ab5834c501f9c625bb0248cd528af361c704503348e9c9605bedf';          BINARY_URL='https://github.com/adoptium/temurin11-binaries/releases/download/jdk-11.0.17%2B8/OpenJDK11U-jre_ppc64le_linux_hotspot_11.0.17_8.tar.gz';          ;;        s390x|s390:64-bit)          ESUM='dd3b159a374086e65cb07c4ccb226c90f9c02ef929cba6f0b642171d7ed97fa4';          BINARY_URL='https://github.com/adoptium/temurin11-binaries/releases/download/jdk-11.0.17%2B8/OpenJDK11U-jre_s390x_linux_hotspot_11.0.17_8.tar.gz';          ;;        amd64|i386:x86-64)          ESUM='752616097e09d7f60a3ad8bd312f90eaf50ac72577e55df229fe6e8091148f79';          BINARY_URL='https://github.com/adoptium/temurin11-binaries/releases/download/jdk-11.0.17%2B8/OpenJDK11U-jre_x64_linux_hotspot_11.0.17_8.tar.gz';          ;;        *)          echo "Unsupported arch: ${ARCH}";          exit 1;          ;;     esac; 	  wget -O /tmp/openjdk.tar.gz ${BINARY_URL}; 	  echo "${ESUM} */tmp/openjdk.tar.gz" | sha256sum -c -; 	  mkdir -p "$JAVA_HOME"; 	  tar --extract 	      --file /tmp/openjdk.tar.gz 	      --directory "$JAVA_HOME" 	      --strip-components 1 	      --no-same-owner 	  ;     rm /tmp/openjdk.tar.gz;     find "$JAVA_HOME/lib" -name '*.so' -exec dirname '{}' ';' | sort -u > /etc/ld.so.conf.d/docker-openjdk.conf;     ldconfig;     java -Xshare:dump;
# Fri, 04 Nov 2022 22:41:34 GMT
RUN echo Verifying install ...     && fileEncoding="$(echo 'System.out.println(System.getProperty("file.encoding"))' | jshell -s -)"; [ "$fileEncoding" = 'UTF-8' ]; rm -rf ~/.java     && echo java --version && java --version     && echo Complete.
# Fri, 04 Nov 2022 23:48:38 GMT
ENV CATALINA_HOME=/usr/local/tomcat
# Fri, 04 Nov 2022 23:48:38 GMT
ENV PATH=/usr/local/tomcat/bin:/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Fri, 04 Nov 2022 23:48:38 GMT
RUN mkdir -p "$CATALINA_HOME"
# Fri, 04 Nov 2022 23:48:39 GMT
WORKDIR /usr/local/tomcat
# Fri, 04 Nov 2022 23:48:39 GMT
ENV TOMCAT_NATIVE_LIBDIR=/usr/local/tomcat/native-jni-lib
# Fri, 04 Nov 2022 23:48:39 GMT
ENV LD_LIBRARY_PATH=/usr/local/tomcat/native-jni-lib
# Fri, 04 Nov 2022 23:53:12 GMT
ENV GPG_KEYS=48F8E69F6390C9F25CFEDCD268248959359E722B A9C5DF4D22E99998D9875A5110C01C5A2F6059E7 DCFD35E0BF8CA7344752DE8B6FB21E8933C60243
# Fri, 04 Nov 2022 23:53:12 GMT
ENV TOMCAT_MAJOR=9
# Tue, 15 Nov 2022 04:57:22 GMT
ENV TOMCAT_VERSION=9.0.69
# Tue, 15 Nov 2022 04:57:22 GMT
ENV TOMCAT_SHA512=8c883c54ce9ce43eba37756a6404cdf3477879883a3e6d146dc8a7aa5e0425f487466afe6b6da4a895927cb7cb59177b9379cec18000f2de12785be57408c779
# Tue, 15 Nov 2022 04:57:22 GMT
COPY dir:096b403a5f78b17e6b4bff63128a9c93941b97f22470991610dd641633d977f1 in /usr/local/tomcat 
# Tue, 15 Nov 2022 04:57:25 GMT
RUN set -eux; 	apt-get update; 	xargs -rt apt-get install -y --no-install-recommends < "$TOMCAT_NATIVE_LIBDIR/.dependencies.txt"; 	rm -rf /var/lib/apt/lists/*
# Tue, 15 Nov 2022 04:57:26 GMT
RUN set -eux; 	nativeLines="$(catalina.sh configtest 2>&1)"; 	nativeLines="$(echo "$nativeLines" | grep 'Apache Tomcat Native')"; 	nativeLines="$(echo "$nativeLines" | sort -u)"; 	if ! echo "$nativeLines" | grep -E 'INFO: Loaded( APR based)? Apache Tomcat Native library' >&2; then 		echo >&2 "$nativeLines"; 		exit 1; 	fi
# Tue, 15 Nov 2022 04:57:26 GMT
EXPOSE 8080
# Tue, 15 Nov 2022 04:57:27 GMT
CMD ["catalina.sh" "run"]
# Wed, 11 Jan 2023 03:05:10 GMT
LABEL org.opencontainers.image.authors=XWiki Development Team <committers@xwiki.org>
# Wed, 11 Jan 2023 03:05:10 GMT
LABEL org.opencontainers.image.url=https://hub.docker.com/_/xwiki
# Wed, 11 Jan 2023 03:05:10 GMT
LABEL org.opencontainers.image.documentation=https://hub.docker.com/_/xwiki
# Wed, 11 Jan 2023 03:05:10 GMT
LABEL org.opencontainers.image.source=https://github.com/xwiki/xwiki-docker.git
# Wed, 11 Jan 2023 03:05:11 GMT
LABEL org.opencontainers.image.vendor=xwiki.org
# Wed, 11 Jan 2023 03:05:11 GMT
LABEL org.opencontainers.image.licenses=LGPL-2.1
# Wed, 11 Jan 2023 03:07:37 GMT
RUN apt-get update &&   apt-get --no-install-recommends -y install     curl     libreoffice     unzip     procps &&   rm -rf /var/lib/apt/lists/*
# Tue, 31 Jan 2023 00:47:12 GMT
ENV XWIKI_VERSION=15.0
# Tue, 31 Jan 2023 00:47:12 GMT
ENV XWIKI_URL_PREFIX=https://maven.xwiki.org/releases/org/xwiki/platform/xwiki-platform-distribution-war/15.0
# Tue, 31 Jan 2023 00:47:12 GMT
ENV XWIKI_DOWNLOAD_SHA256=79ba0f479bbc49521c113821adc9d91141075a9470d7f9bbb6994ca59c30d121
# Tue, 31 Jan 2023 00:47:58 GMT
RUN rm -rf /usr/local/tomcat/webapps/* &&   mkdir -p /usr/local/tomcat/temp &&   mkdir -p /usr/local/xwiki/data &&   curl -fSL "${XWIKI_URL_PREFIX}/xwiki-platform-distribution-war-${XWIKI_VERSION}.war" -o xwiki.war &&   echo "$XWIKI_DOWNLOAD_SHA256 xwiki.war" | sha256sum -c - &&   unzip -d /usr/local/tomcat/webapps/ROOT xwiki.war &&   rm -f xwiki.war
# Tue, 31 Jan 2023 00:54:48 GMT
ENV MARIADB_JDBC_VERSION=3.1.1
# Tue, 31 Jan 2023 00:54:48 GMT
ENV MARIADB_JDBC_SHA256=a554541fd88047905fb0c4c10e1d85295f5e38c7bb5fb408b425392a79fc26e3
# Tue, 31 Jan 2023 00:54:48 GMT
ENV MARIADB_JDBC_PREFIX=https://repo1.maven.org/maven2/org/mariadb/jdbc/mariadb-java-client/3.1.1
# Tue, 31 Jan 2023 00:54:48 GMT
ENV MARIADB_JDBC_ARTIFACT=mariadb-java-client-3.1.1.jar
# Tue, 31 Jan 2023 00:54:48 GMT
ENV MARIADB_JDBC_TARGET=/usr/local/tomcat/webapps/ROOT/WEB-INF/lib/mariadb-java-client-3.1.1.jar
# Tue, 31 Jan 2023 00:54:49 GMT
RUN curl -fSL "${MARIADB_JDBC_PREFIX}/${MARIADB_JDBC_ARTIFACT}" -o $MARIADB_JDBC_TARGET &&   echo "$MARIADB_JDBC_SHA256 $MARIADB_JDBC_TARGET" | sha256sum -c -
# Tue, 31 Jan 2023 00:54:49 GMT
COPY file:0a1be11e2eb610a1dbcd415404e3a592641110b93090030cb831e3a19a163017 in /usr/local/tomcat/bin/ 
# Tue, 31 Jan 2023 00:54:49 GMT
COPY file:0e237c3876eeb3b5f3473a064d3e507da2df6c228ca714687930b34e3b687601 in /usr/local/tomcat/webapps/ROOT/WEB-INF/hibernate.cfg.xml 
# Tue, 31 Jan 2023 00:54:49 GMT
RUN sed -i 's/<id>org.xwiki.platform:xwiki-platform-distribution-war/<id>org.xwiki.platform:xwiki-platform-distribution-docker/'   /usr/local/tomcat/webapps/ROOT/META-INF/extension.xed
# Tue, 31 Jan 2023 00:54:49 GMT
COPY file:a47c4dcd87c9dad97aff38c49188357e6193bcad50757e516cfb08a60d4de611 in /usr/local/bin/docker-entrypoint.sh 
# Tue, 31 Jan 2023 00:54:49 GMT
VOLUME [/usr/local/xwiki]
# Tue, 31 Jan 2023 00:54:50 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 31 Jan 2023 00:54:50 GMT
CMD ["xwiki"]
```

-	Layers:
	-	`sha256:0509fae36eb0656f8bdb23f8ae64100d893bcea2563e97468d337e04d2d0410b`  
		Last Modified: Wed, 02 Nov 2022 18:50:21 GMT  
		Size: 28.4 MB (28382154 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e502a1af2bcd98f5f0d2f5e4da1a0e7bbe07a2c548e2662f7d37dce5ae1df46c`  
		Last Modified: Wed, 02 Nov 2022 19:48:28 GMT  
		Size: 12.4 MB (12396330 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bc4598c07dd818f03a0378b0341a4a8e80f0152fbb3e7d5246ca4f466f42e611`  
		Last Modified: Fri, 04 Nov 2022 22:46:46 GMT  
		Size: 45.0 MB (44958470 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:715a937a1066f998b331fcd62256ad01a5571bdf46804e97825afc64f9ebb427`  
		Last Modified: Fri, 04 Nov 2022 22:46:41 GMT  
		Size: 160.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5fb623f082f74b2fa9fc2c4e3f3a4802875cb9753cfa26ed940201ce72bb56cb`  
		Last Modified: Sat, 05 Nov 2022 00:03:40 GMT  
		Size: 172.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:33260b83200262bbd546be371ad3c1f50f5ae7228afb87982d6fa9d6b11bf26f`  
		Last Modified: Tue, 15 Nov 2022 05:10:19 GMT  
		Size: 12.2 MB (12207235 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0955fb697ea9b30a1b4f95385464f646aa1525cb6efba648e22df84ebef6b2ee`  
		Last Modified: Tue, 15 Nov 2022 05:10:18 GMT  
		Size: 452.0 KB (452021 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6eddcf66f2083b1487296a0308e0b058917c97f614f12428d82d89662038dc2e`  
		Last Modified: Tue, 15 Nov 2022 05:10:18 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ae5f60bb64f3fa11da3d15a9639f886186b4c2c021455c3f9db22e0cfe1b1311`  
		Last Modified: Wed, 11 Jan 2023 03:11:14 GMT  
		Size: 173.8 MB (173806827 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1814d85fce571b42f2cfa7c8a904e1a184ee6f49642242a44bbe0037088994a0`  
		Last Modified: Tue, 31 Jan 2023 00:56:04 GMT  
		Size: 307.1 MB (307117070 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e8637677b7ba0da683afa4e56ff0561e4ba77c8782d5a98da785f4ef58d1caf9`  
		Last Modified: Tue, 31 Jan 2023 00:57:14 GMT  
		Size: 589.7 KB (589677 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:61a67398bc888bcce1656edec9bb40409ce0ffc2fe83d0437c28dd64a8f697ce`  
		Last Modified: Tue, 31 Jan 2023 00:57:14 GMT  
		Size: 1.3 KB (1345 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7ebda7e506ea819ce9717c3d0334df81608bc4c7149cd47ebc9a32790141a637`  
		Last Modified: Tue, 31 Jan 2023 00:57:14 GMT  
		Size: 2.3 KB (2313 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2ceebbf08640e235a928c9df650ca3ab8d0c6b506faa158ecde5fdde34bf8813`  
		Last Modified: Tue, 31 Jan 2023 00:57:14 GMT  
		Size: 6.0 KB (6007 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:12b1d23eae23b1a09ecd4185941d43f13d4ad633d4c6257ab8107a8eebd5fb12`  
		Last Modified: Tue, 31 Jan 2023 00:57:14 GMT  
		Size: 2.5 KB (2506 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `xwiki:stable-mysql`

```console
$ docker pull xwiki@sha256:33e789838f82ce73efec6664859feb1ced7a5b7605fbfaddb81916716bce524f
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `xwiki:stable-mysql` - linux; amd64

```console
$ docker pull xwiki@sha256:481fdb46e8c043a6709d11310e2083ce71d6ba63ee6517f84da3ba06f320598e
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **590.5 MB (590459982 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:bd630aa0aa5c679e23ea7d52cbbdd6b817eab27a820c25d3c50b54eca83b9744`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["xwiki"]`

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
# Wed, 02 Nov 2022 18:44:10 GMT
RUN apt-get update     && DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends tzdata curl wget ca-certificates fontconfig locales     && echo "en_US.UTF-8 UTF-8" >> /etc/locale.gen     && locale-gen en_US.UTF-8     && rm -rf /var/lib/apt/lists/*
# Fri, 04 Nov 2022 23:21:41 GMT
ENV JAVA_VERSION=jdk-11.0.17+8
# Fri, 04 Nov 2022 23:22:31 GMT
RUN set -eux;     ARCH="$(dpkg --print-architecture)";     case "${ARCH}" in        aarch64|arm64)          ESUM='bd6efe3290c8b5a42f695a55a26f3e3c9c284288574879d4b7089f31f5114177';          BINARY_URL='https://github.com/adoptium/temurin11-binaries/releases/download/jdk-11.0.17%2B8/OpenJDK11U-jre_aarch64_linux_hotspot_11.0.17_8.tar.gz';          ;;        armhf|arm)          ESUM='8cf113d3d7fa808895c8d2e41bb890af21c47e38c2460e0588147a4bb8fc658d';          BINARY_URL='https://github.com/adoptium/temurin11-binaries/releases/download/jdk-11.0.17%2B8/OpenJDK11U-jre_arm_linux_hotspot_11.0.17_8.tar.gz';          ;;        ppc64el|powerpc:common64)          ESUM='0ca3d806131ab5834c501f9c625bb0248cd528af361c704503348e9c9605bedf';          BINARY_URL='https://github.com/adoptium/temurin11-binaries/releases/download/jdk-11.0.17%2B8/OpenJDK11U-jre_ppc64le_linux_hotspot_11.0.17_8.tar.gz';          ;;        s390x|s390:64-bit)          ESUM='dd3b159a374086e65cb07c4ccb226c90f9c02ef929cba6f0b642171d7ed97fa4';          BINARY_URL='https://github.com/adoptium/temurin11-binaries/releases/download/jdk-11.0.17%2B8/OpenJDK11U-jre_s390x_linux_hotspot_11.0.17_8.tar.gz';          ;;        amd64|i386:x86-64)          ESUM='752616097e09d7f60a3ad8bd312f90eaf50ac72577e55df229fe6e8091148f79';          BINARY_URL='https://github.com/adoptium/temurin11-binaries/releases/download/jdk-11.0.17%2B8/OpenJDK11U-jre_x64_linux_hotspot_11.0.17_8.tar.gz';          ;;        *)          echo "Unsupported arch: ${ARCH}";          exit 1;          ;;     esac; 	  wget -O /tmp/openjdk.tar.gz ${BINARY_URL}; 	  echo "${ESUM} */tmp/openjdk.tar.gz" | sha256sum -c -; 	  mkdir -p "$JAVA_HOME"; 	  tar --extract 	      --file /tmp/openjdk.tar.gz 	      --directory "$JAVA_HOME" 	      --strip-components 1 	      --no-same-owner 	  ;     rm /tmp/openjdk.tar.gz;     find "$JAVA_HOME/lib" -name '*.so' -exec dirname '{}' ';' | sort -u > /etc/ld.so.conf.d/docker-openjdk.conf;     ldconfig;     java -Xshare:dump;
# Fri, 04 Nov 2022 23:22:32 GMT
RUN echo Verifying install ...     && fileEncoding="$(echo 'System.out.println(System.getProperty("file.encoding"))' | jshell -s -)"; [ "$fileEncoding" = 'UTF-8' ]; rm -rf ~/.java     && echo java --version && java --version     && echo Complete.
# Sat, 05 Nov 2022 01:35:16 GMT
ENV CATALINA_HOME=/usr/local/tomcat
# Sat, 05 Nov 2022 01:35:16 GMT
ENV PATH=/usr/local/tomcat/bin:/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Sat, 05 Nov 2022 01:35:17 GMT
RUN mkdir -p "$CATALINA_HOME"
# Sat, 05 Nov 2022 01:35:17 GMT
WORKDIR /usr/local/tomcat
# Sat, 05 Nov 2022 01:35:17 GMT
ENV TOMCAT_NATIVE_LIBDIR=/usr/local/tomcat/native-jni-lib
# Sat, 05 Nov 2022 01:35:17 GMT
ENV LD_LIBRARY_PATH=/usr/local/tomcat/native-jni-lib
# Sat, 05 Nov 2022 01:39:54 GMT
ENV GPG_KEYS=48F8E69F6390C9F25CFEDCD268248959359E722B A9C5DF4D22E99998D9875A5110C01C5A2F6059E7 DCFD35E0BF8CA7344752DE8B6FB21E8933C60243
# Sat, 05 Nov 2022 01:39:54 GMT
ENV TOMCAT_MAJOR=9
# Tue, 15 Nov 2022 03:06:43 GMT
ENV TOMCAT_VERSION=9.0.69
# Tue, 15 Nov 2022 03:06:43 GMT
ENV TOMCAT_SHA512=8c883c54ce9ce43eba37756a6404cdf3477879883a3e6d146dc8a7aa5e0425f487466afe6b6da4a895927cb7cb59177b9379cec18000f2de12785be57408c779
# Tue, 15 Nov 2022 03:06:44 GMT
COPY dir:b1a33aa3993dbbfbebb33bd9aa546b60c2f2191abf1227f453d4e830f6deb35f in /usr/local/tomcat 
# Tue, 15 Nov 2022 03:06:48 GMT
RUN set -eux; 	apt-get update; 	xargs -rt apt-get install -y --no-install-recommends < "$TOMCAT_NATIVE_LIBDIR/.dependencies.txt"; 	rm -rf /var/lib/apt/lists/*
# Tue, 15 Nov 2022 03:06:49 GMT
RUN set -eux; 	nativeLines="$(catalina.sh configtest 2>&1)"; 	nativeLines="$(echo "$nativeLines" | grep 'Apache Tomcat Native')"; 	nativeLines="$(echo "$nativeLines" | sort -u)"; 	if ! echo "$nativeLines" | grep -E 'INFO: Loaded( APR based)? Apache Tomcat Native library' >&2; then 		echo >&2 "$nativeLines"; 		exit 1; 	fi
# Tue, 15 Nov 2022 03:06:49 GMT
EXPOSE 8080
# Tue, 15 Nov 2022 03:06:49 GMT
CMD ["catalina.sh" "run"]
# Wed, 11 Jan 2023 02:47:03 GMT
LABEL org.opencontainers.image.authors=XWiki Development Team <committers@xwiki.org>
# Wed, 11 Jan 2023 02:47:03 GMT
LABEL org.opencontainers.image.url=https://hub.docker.com/_/xwiki
# Wed, 11 Jan 2023 02:47:03 GMT
LABEL org.opencontainers.image.documentation=https://hub.docker.com/_/xwiki
# Wed, 11 Jan 2023 02:47:03 GMT
LABEL org.opencontainers.image.source=https://github.com/xwiki/xwiki-docker.git
# Wed, 11 Jan 2023 02:47:04 GMT
LABEL org.opencontainers.image.vendor=xwiki.org
# Wed, 11 Jan 2023 02:47:04 GMT
LABEL org.opencontainers.image.licenses=LGPL-2.1
# Wed, 11 Jan 2023 02:49:03 GMT
RUN apt-get update &&   apt-get --no-install-recommends -y install     curl     libreoffice     unzip     procps &&   rm -rf /var/lib/apt/lists/*
# Tue, 31 Jan 2023 00:20:17 GMT
ENV XWIKI_VERSION=15.0
# Tue, 31 Jan 2023 00:20:17 GMT
ENV XWIKI_URL_PREFIX=https://maven.xwiki.org/releases/org/xwiki/platform/xwiki-platform-distribution-war/15.0
# Tue, 31 Jan 2023 00:20:17 GMT
ENV XWIKI_DOWNLOAD_SHA256=79ba0f479bbc49521c113821adc9d91141075a9470d7f9bbb6994ca59c30d121
# Tue, 31 Jan 2023 00:21:18 GMT
RUN rm -rf /usr/local/tomcat/webapps/* &&   mkdir -p /usr/local/tomcat/temp &&   mkdir -p /usr/local/xwiki/data &&   curl -fSL "${XWIKI_URL_PREFIX}/xwiki-platform-distribution-war-${XWIKI_VERSION}.war" -o xwiki.war &&   echo "$XWIKI_DOWNLOAD_SHA256 xwiki.war" | sha256sum -c - &&   unzip -d /usr/local/tomcat/webapps/ROOT xwiki.war &&   rm -f xwiki.war
# Tue, 31 Jan 2023 00:21:19 GMT
ENV MYSQL_JDBC_VERSION=8.0.31
# Tue, 31 Jan 2023 00:21:19 GMT
ENV MYSQL_JDBC_SHA256=5249e3dc6d6531b37790e3f61845b96db5e41e891d3d8edb0e2e3a1b53ca2f4f
# Tue, 31 Jan 2023 00:21:19 GMT
ENV MYSQL_JDBC_PREFIX=https://repo1.maven.org/maven2/com/mysql/mysql-connector-j/8.0.31
# Tue, 31 Jan 2023 00:21:19 GMT
ENV MYSQL_JDBC_ARTIFACT=mysql-connector-j-8.0.31.jar
# Tue, 31 Jan 2023 00:21:19 GMT
ENV MYSQL_JDBC_TARGET=/usr/local/tomcat/webapps/ROOT/WEB-INF/lib/mysql-connector-j-8.0.31.jar
# Tue, 31 Jan 2023 00:21:20 GMT
RUN curl -fSL "${MYSQL_JDBC_PREFIX}/${MYSQL_JDBC_ARTIFACT}" -o $MYSQL_JDBC_TARGET &&   echo "$MYSQL_JDBC_SHA256 $MYSQL_JDBC_TARGET" | sha256sum -c -
# Tue, 31 Jan 2023 00:21:21 GMT
COPY file:0a1be11e2eb610a1dbcd415404e3a592641110b93090030cb831e3a19a163017 in /usr/local/tomcat/bin/ 
# Tue, 31 Jan 2023 00:21:21 GMT
COPY file:1b8409986f3e4eb79a7a0b18472cb2692a61d504fb5ef34292bc997b79fd760d in /usr/local/tomcat/webapps/ROOT/WEB-INF/hibernate.cfg.xml 
# Tue, 31 Jan 2023 00:21:21 GMT
RUN sed -i 's/<id>org.xwiki.platform:xwiki-platform-distribution-war/<id>org.xwiki.platform:xwiki-platform-distribution-docker/'   /usr/local/tomcat/webapps/ROOT/META-INF/extension.xed
# Tue, 31 Jan 2023 00:21:21 GMT
COPY file:a47c4dcd87c9dad97aff38c49188357e6193bcad50757e516cfb08a60d4de611 in /usr/local/bin/docker-entrypoint.sh 
# Tue, 31 Jan 2023 00:21:22 GMT
VOLUME [/usr/local/xwiki]
# Tue, 31 Jan 2023 00:21:22 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 31 Jan 2023 00:21:22 GMT
CMD ["xwiki"]
```

-	Layers:
	-	`sha256:e96e057aae67380a4ddb16c337c5c3669d97fdff69ec537f02aa2cc30d814281`  
		Last Modified: Wed, 02 Nov 2022 03:03:36 GMT  
		Size: 30.4 MB (30425607 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4ced2591451da3a02e2b6bb44752b9e3f00d77789921be4df5082fb9f9880ad0`  
		Last Modified: Wed, 02 Nov 2022 18:48:43 GMT  
		Size: 12.4 MB (12439006 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:df8f874ae8c08a9e69e5fbe6c5a64200a45386132a3203d1a9a7f1146d94cfbc`  
		Last Modified: Fri, 04 Nov 2022 23:29:33 GMT  
		Size: 46.6 MB (46629936 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:111b6c7486426c4b6989102c2ee5be856e8a58e20ab0a350b24a905d536e8e7f`  
		Last Modified: Fri, 04 Nov 2022 23:29:26 GMT  
		Size: 161.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e6f84dce457c6d4f7b7291fce05f8e77998a3a7722a54125a1f1d52ca83043b4`  
		Last Modified: Sat, 05 Nov 2022 01:50:51 GMT  
		Size: 173.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a6c26749ee782392e38845ee2ba79b0da586ef6a45d8e7f29c7af14612278547`  
		Last Modified: Tue, 15 Nov 2022 03:19:57 GMT  
		Size: 12.2 MB (12200249 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4dddc6d9fa6024025b3fcfe729cab2dc544fb25476eca6e80b1af8e8d93bb0ee`  
		Last Modified: Tue, 15 Nov 2022 03:19:56 GMT  
		Size: 452.7 KB (452680 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:06637eebe5e72c8ad9019ad4eb4cdde1f11f7d4c24c7ed7374cf8966343aa2fb`  
		Last Modified: Tue, 15 Nov 2022 03:19:56 GMT  
		Size: 131.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b276fb8390410a8208724033e325715ea26000d5a1a762d4c3699b927884fbfe`  
		Last Modified: Wed, 11 Jan 2023 02:52:45 GMT  
		Size: 178.8 MB (178805608 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:156ca91198173149698aa0396648a9608b6ab1f2bc2666800843ce33c9f85b6e`  
		Last Modified: Tue, 31 Jan 2023 00:24:09 GMT  
		Size: 307.1 MB (307117069 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4c8b70d250c6d507901857473b0dcb67132d7b2a30ce9a69b07b1036853df738`  
		Last Modified: Tue, 31 Jan 2023 00:23:52 GMT  
		Size: 2.4 MB (2377191 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a9681fd36be674d25231c69d6a39f9e8fa65034eeaef5d1bd885fdbeac7f0f6b`  
		Last Modified: Tue, 31 Jan 2023 00:23:51 GMT  
		Size: 1.3 KB (1346 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a9d0d5da840f4d7da9943942b38cd092fae11f41dc6c19afd58d655cd6192d66`  
		Last Modified: Tue, 31 Jan 2023 00:23:51 GMT  
		Size: 2.3 KB (2312 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d65610da4f1da86fea8fbec0189b066afd4b86e4e8f7d049e3c4bc6ade9ba90a`  
		Last Modified: Tue, 31 Jan 2023 00:23:51 GMT  
		Size: 6.0 KB (6009 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3d41686284d7675eaa0f92c9cc27ebe73b4c30768c8eef9f23ee3b1ad06da00a`  
		Last Modified: Tue, 31 Jan 2023 00:23:51 GMT  
		Size: 2.5 KB (2504 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `xwiki:stable-mysql` - linux; arm64 variant v8

```console
$ docker pull xwiki@sha256:6bf63d9025b07b69d744200c05efd4ffb8a52f3c38380f5d59a0b48514203cd2
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **581.7 MB (581709921 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:6600f2bb05836c703d53944bbcb5399d509a9813a27a35e99ff717becc308330`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["xwiki"]`

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
# Wed, 02 Nov 2022 19:44:32 GMT
RUN apt-get update     && DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends tzdata curl wget ca-certificates fontconfig locales     && echo "en_US.UTF-8 UTF-8" >> /etc/locale.gen     && locale-gen en_US.UTF-8     && rm -rf /var/lib/apt/lists/*
# Fri, 04 Nov 2022 22:40:54 GMT
ENV JAVA_VERSION=jdk-11.0.17+8
# Fri, 04 Nov 2022 22:41:33 GMT
RUN set -eux;     ARCH="$(dpkg --print-architecture)";     case "${ARCH}" in        aarch64|arm64)          ESUM='bd6efe3290c8b5a42f695a55a26f3e3c9c284288574879d4b7089f31f5114177';          BINARY_URL='https://github.com/adoptium/temurin11-binaries/releases/download/jdk-11.0.17%2B8/OpenJDK11U-jre_aarch64_linux_hotspot_11.0.17_8.tar.gz';          ;;        armhf|arm)          ESUM='8cf113d3d7fa808895c8d2e41bb890af21c47e38c2460e0588147a4bb8fc658d';          BINARY_URL='https://github.com/adoptium/temurin11-binaries/releases/download/jdk-11.0.17%2B8/OpenJDK11U-jre_arm_linux_hotspot_11.0.17_8.tar.gz';          ;;        ppc64el|powerpc:common64)          ESUM='0ca3d806131ab5834c501f9c625bb0248cd528af361c704503348e9c9605bedf';          BINARY_URL='https://github.com/adoptium/temurin11-binaries/releases/download/jdk-11.0.17%2B8/OpenJDK11U-jre_ppc64le_linux_hotspot_11.0.17_8.tar.gz';          ;;        s390x|s390:64-bit)          ESUM='dd3b159a374086e65cb07c4ccb226c90f9c02ef929cba6f0b642171d7ed97fa4';          BINARY_URL='https://github.com/adoptium/temurin11-binaries/releases/download/jdk-11.0.17%2B8/OpenJDK11U-jre_s390x_linux_hotspot_11.0.17_8.tar.gz';          ;;        amd64|i386:x86-64)          ESUM='752616097e09d7f60a3ad8bd312f90eaf50ac72577e55df229fe6e8091148f79';          BINARY_URL='https://github.com/adoptium/temurin11-binaries/releases/download/jdk-11.0.17%2B8/OpenJDK11U-jre_x64_linux_hotspot_11.0.17_8.tar.gz';          ;;        *)          echo "Unsupported arch: ${ARCH}";          exit 1;          ;;     esac; 	  wget -O /tmp/openjdk.tar.gz ${BINARY_URL}; 	  echo "${ESUM} */tmp/openjdk.tar.gz" | sha256sum -c -; 	  mkdir -p "$JAVA_HOME"; 	  tar --extract 	      --file /tmp/openjdk.tar.gz 	      --directory "$JAVA_HOME" 	      --strip-components 1 	      --no-same-owner 	  ;     rm /tmp/openjdk.tar.gz;     find "$JAVA_HOME/lib" -name '*.so' -exec dirname '{}' ';' | sort -u > /etc/ld.so.conf.d/docker-openjdk.conf;     ldconfig;     java -Xshare:dump;
# Fri, 04 Nov 2022 22:41:34 GMT
RUN echo Verifying install ...     && fileEncoding="$(echo 'System.out.println(System.getProperty("file.encoding"))' | jshell -s -)"; [ "$fileEncoding" = 'UTF-8' ]; rm -rf ~/.java     && echo java --version && java --version     && echo Complete.
# Fri, 04 Nov 2022 23:48:38 GMT
ENV CATALINA_HOME=/usr/local/tomcat
# Fri, 04 Nov 2022 23:48:38 GMT
ENV PATH=/usr/local/tomcat/bin:/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Fri, 04 Nov 2022 23:48:38 GMT
RUN mkdir -p "$CATALINA_HOME"
# Fri, 04 Nov 2022 23:48:39 GMT
WORKDIR /usr/local/tomcat
# Fri, 04 Nov 2022 23:48:39 GMT
ENV TOMCAT_NATIVE_LIBDIR=/usr/local/tomcat/native-jni-lib
# Fri, 04 Nov 2022 23:48:39 GMT
ENV LD_LIBRARY_PATH=/usr/local/tomcat/native-jni-lib
# Fri, 04 Nov 2022 23:53:12 GMT
ENV GPG_KEYS=48F8E69F6390C9F25CFEDCD268248959359E722B A9C5DF4D22E99998D9875A5110C01C5A2F6059E7 DCFD35E0BF8CA7344752DE8B6FB21E8933C60243
# Fri, 04 Nov 2022 23:53:12 GMT
ENV TOMCAT_MAJOR=9
# Tue, 15 Nov 2022 04:57:22 GMT
ENV TOMCAT_VERSION=9.0.69
# Tue, 15 Nov 2022 04:57:22 GMT
ENV TOMCAT_SHA512=8c883c54ce9ce43eba37756a6404cdf3477879883a3e6d146dc8a7aa5e0425f487466afe6b6da4a895927cb7cb59177b9379cec18000f2de12785be57408c779
# Tue, 15 Nov 2022 04:57:22 GMT
COPY dir:096b403a5f78b17e6b4bff63128a9c93941b97f22470991610dd641633d977f1 in /usr/local/tomcat 
# Tue, 15 Nov 2022 04:57:25 GMT
RUN set -eux; 	apt-get update; 	xargs -rt apt-get install -y --no-install-recommends < "$TOMCAT_NATIVE_LIBDIR/.dependencies.txt"; 	rm -rf /var/lib/apt/lists/*
# Tue, 15 Nov 2022 04:57:26 GMT
RUN set -eux; 	nativeLines="$(catalina.sh configtest 2>&1)"; 	nativeLines="$(echo "$nativeLines" | grep 'Apache Tomcat Native')"; 	nativeLines="$(echo "$nativeLines" | sort -u)"; 	if ! echo "$nativeLines" | grep -E 'INFO: Loaded( APR based)? Apache Tomcat Native library' >&2; then 		echo >&2 "$nativeLines"; 		exit 1; 	fi
# Tue, 15 Nov 2022 04:57:26 GMT
EXPOSE 8080
# Tue, 15 Nov 2022 04:57:27 GMT
CMD ["catalina.sh" "run"]
# Wed, 11 Jan 2023 03:05:10 GMT
LABEL org.opencontainers.image.authors=XWiki Development Team <committers@xwiki.org>
# Wed, 11 Jan 2023 03:05:10 GMT
LABEL org.opencontainers.image.url=https://hub.docker.com/_/xwiki
# Wed, 11 Jan 2023 03:05:10 GMT
LABEL org.opencontainers.image.documentation=https://hub.docker.com/_/xwiki
# Wed, 11 Jan 2023 03:05:10 GMT
LABEL org.opencontainers.image.source=https://github.com/xwiki/xwiki-docker.git
# Wed, 11 Jan 2023 03:05:11 GMT
LABEL org.opencontainers.image.vendor=xwiki.org
# Wed, 11 Jan 2023 03:05:11 GMT
LABEL org.opencontainers.image.licenses=LGPL-2.1
# Wed, 11 Jan 2023 03:07:37 GMT
RUN apt-get update &&   apt-get --no-install-recommends -y install     curl     libreoffice     unzip     procps &&   rm -rf /var/lib/apt/lists/*
# Tue, 31 Jan 2023 00:47:12 GMT
ENV XWIKI_VERSION=15.0
# Tue, 31 Jan 2023 00:47:12 GMT
ENV XWIKI_URL_PREFIX=https://maven.xwiki.org/releases/org/xwiki/platform/xwiki-platform-distribution-war/15.0
# Tue, 31 Jan 2023 00:47:12 GMT
ENV XWIKI_DOWNLOAD_SHA256=79ba0f479bbc49521c113821adc9d91141075a9470d7f9bbb6994ca59c30d121
# Tue, 31 Jan 2023 00:47:58 GMT
RUN rm -rf /usr/local/tomcat/webapps/* &&   mkdir -p /usr/local/tomcat/temp &&   mkdir -p /usr/local/xwiki/data &&   curl -fSL "${XWIKI_URL_PREFIX}/xwiki-platform-distribution-war-${XWIKI_VERSION}.war" -o xwiki.war &&   echo "$XWIKI_DOWNLOAD_SHA256 xwiki.war" | sha256sum -c - &&   unzip -d /usr/local/tomcat/webapps/ROOT xwiki.war &&   rm -f xwiki.war
# Tue, 31 Jan 2023 00:48:01 GMT
ENV MYSQL_JDBC_VERSION=8.0.31
# Tue, 31 Jan 2023 00:48:01 GMT
ENV MYSQL_JDBC_SHA256=5249e3dc6d6531b37790e3f61845b96db5e41e891d3d8edb0e2e3a1b53ca2f4f
# Tue, 31 Jan 2023 00:48:01 GMT
ENV MYSQL_JDBC_PREFIX=https://repo1.maven.org/maven2/com/mysql/mysql-connector-j/8.0.31
# Tue, 31 Jan 2023 00:48:01 GMT
ENV MYSQL_JDBC_ARTIFACT=mysql-connector-j-8.0.31.jar
# Tue, 31 Jan 2023 00:48:01 GMT
ENV MYSQL_JDBC_TARGET=/usr/local/tomcat/webapps/ROOT/WEB-INF/lib/mysql-connector-j-8.0.31.jar
# Tue, 31 Jan 2023 00:48:02 GMT
RUN curl -fSL "${MYSQL_JDBC_PREFIX}/${MYSQL_JDBC_ARTIFACT}" -o $MYSQL_JDBC_TARGET &&   echo "$MYSQL_JDBC_SHA256 $MYSQL_JDBC_TARGET" | sha256sum -c -
# Tue, 31 Jan 2023 00:48:02 GMT
COPY file:0a1be11e2eb610a1dbcd415404e3a592641110b93090030cb831e3a19a163017 in /usr/local/tomcat/bin/ 
# Tue, 31 Jan 2023 00:48:02 GMT
COPY file:1b8409986f3e4eb79a7a0b18472cb2692a61d504fb5ef34292bc997b79fd760d in /usr/local/tomcat/webapps/ROOT/WEB-INF/hibernate.cfg.xml 
# Tue, 31 Jan 2023 00:48:03 GMT
RUN sed -i 's/<id>org.xwiki.platform:xwiki-platform-distribution-war/<id>org.xwiki.platform:xwiki-platform-distribution-docker/'   /usr/local/tomcat/webapps/ROOT/META-INF/extension.xed
# Tue, 31 Jan 2023 00:48:03 GMT
COPY file:a47c4dcd87c9dad97aff38c49188357e6193bcad50757e516cfb08a60d4de611 in /usr/local/bin/docker-entrypoint.sh 
# Tue, 31 Jan 2023 00:48:03 GMT
VOLUME [/usr/local/xwiki]
# Tue, 31 Jan 2023 00:48:03 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 31 Jan 2023 00:48:03 GMT
CMD ["xwiki"]
```

-	Layers:
	-	`sha256:0509fae36eb0656f8bdb23f8ae64100d893bcea2563e97468d337e04d2d0410b`  
		Last Modified: Wed, 02 Nov 2022 18:50:21 GMT  
		Size: 28.4 MB (28382154 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e502a1af2bcd98f5f0d2f5e4da1a0e7bbe07a2c548e2662f7d37dce5ae1df46c`  
		Last Modified: Wed, 02 Nov 2022 19:48:28 GMT  
		Size: 12.4 MB (12396330 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bc4598c07dd818f03a0378b0341a4a8e80f0152fbb3e7d5246ca4f466f42e611`  
		Last Modified: Fri, 04 Nov 2022 22:46:46 GMT  
		Size: 45.0 MB (44958470 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:715a937a1066f998b331fcd62256ad01a5571bdf46804e97825afc64f9ebb427`  
		Last Modified: Fri, 04 Nov 2022 22:46:41 GMT  
		Size: 160.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5fb623f082f74b2fa9fc2c4e3f3a4802875cb9753cfa26ed940201ce72bb56cb`  
		Last Modified: Sat, 05 Nov 2022 00:03:40 GMT  
		Size: 172.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:33260b83200262bbd546be371ad3c1f50f5ae7228afb87982d6fa9d6b11bf26f`  
		Last Modified: Tue, 15 Nov 2022 05:10:19 GMT  
		Size: 12.2 MB (12207235 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0955fb697ea9b30a1b4f95385464f646aa1525cb6efba648e22df84ebef6b2ee`  
		Last Modified: Tue, 15 Nov 2022 05:10:18 GMT  
		Size: 452.0 KB (452021 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6eddcf66f2083b1487296a0308e0b058917c97f614f12428d82d89662038dc2e`  
		Last Modified: Tue, 15 Nov 2022 05:10:18 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ae5f60bb64f3fa11da3d15a9639f886186b4c2c021455c3f9db22e0cfe1b1311`  
		Last Modified: Wed, 11 Jan 2023 03:11:14 GMT  
		Size: 173.8 MB (173806827 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1814d85fce571b42f2cfa7c8a904e1a184ee6f49642242a44bbe0037088994a0`  
		Last Modified: Tue, 31 Jan 2023 00:56:04 GMT  
		Size: 307.1 MB (307117070 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8aec0e24b4fa870989f014944c3c7d535355a2371fc8c948b2b11f9b377efe6e`  
		Last Modified: Tue, 31 Jan 2023 00:55:50 GMT  
		Size: 2.4 MB (2377182 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0b65081619aa0114a7f367836ef421eb8d951e559e0f089c7728af7813b1ea62`  
		Last Modified: Tue, 31 Jan 2023 00:55:49 GMT  
		Size: 1.3 KB (1348 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:46ebad072e608146426d8dc30828937049eea36c2e636d7790b4960d6d586977`  
		Last Modified: Tue, 31 Jan 2023 00:55:49 GMT  
		Size: 2.3 KB (2308 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:708fefcedd4ee6c106da247a68c5790f5ab00225d1cdfff8465575265c3a54e6`  
		Last Modified: Tue, 31 Jan 2023 00:55:49 GMT  
		Size: 6.0 KB (6008 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:81e3bf8e20bc921031e7549a41dec1b2d7795cc6da40a0e7096bf654b25c5c3e`  
		Last Modified: Tue, 31 Jan 2023 00:55:49 GMT  
		Size: 2.5 KB (2507 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `xwiki:stable-mysql-tomcat`

```console
$ docker pull xwiki@sha256:33e789838f82ce73efec6664859feb1ced7a5b7605fbfaddb81916716bce524f
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `xwiki:stable-mysql-tomcat` - linux; amd64

```console
$ docker pull xwiki@sha256:481fdb46e8c043a6709d11310e2083ce71d6ba63ee6517f84da3ba06f320598e
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **590.5 MB (590459982 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:bd630aa0aa5c679e23ea7d52cbbdd6b817eab27a820c25d3c50b54eca83b9744`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["xwiki"]`

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
# Wed, 02 Nov 2022 18:44:10 GMT
RUN apt-get update     && DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends tzdata curl wget ca-certificates fontconfig locales     && echo "en_US.UTF-8 UTF-8" >> /etc/locale.gen     && locale-gen en_US.UTF-8     && rm -rf /var/lib/apt/lists/*
# Fri, 04 Nov 2022 23:21:41 GMT
ENV JAVA_VERSION=jdk-11.0.17+8
# Fri, 04 Nov 2022 23:22:31 GMT
RUN set -eux;     ARCH="$(dpkg --print-architecture)";     case "${ARCH}" in        aarch64|arm64)          ESUM='bd6efe3290c8b5a42f695a55a26f3e3c9c284288574879d4b7089f31f5114177';          BINARY_URL='https://github.com/adoptium/temurin11-binaries/releases/download/jdk-11.0.17%2B8/OpenJDK11U-jre_aarch64_linux_hotspot_11.0.17_8.tar.gz';          ;;        armhf|arm)          ESUM='8cf113d3d7fa808895c8d2e41bb890af21c47e38c2460e0588147a4bb8fc658d';          BINARY_URL='https://github.com/adoptium/temurin11-binaries/releases/download/jdk-11.0.17%2B8/OpenJDK11U-jre_arm_linux_hotspot_11.0.17_8.tar.gz';          ;;        ppc64el|powerpc:common64)          ESUM='0ca3d806131ab5834c501f9c625bb0248cd528af361c704503348e9c9605bedf';          BINARY_URL='https://github.com/adoptium/temurin11-binaries/releases/download/jdk-11.0.17%2B8/OpenJDK11U-jre_ppc64le_linux_hotspot_11.0.17_8.tar.gz';          ;;        s390x|s390:64-bit)          ESUM='dd3b159a374086e65cb07c4ccb226c90f9c02ef929cba6f0b642171d7ed97fa4';          BINARY_URL='https://github.com/adoptium/temurin11-binaries/releases/download/jdk-11.0.17%2B8/OpenJDK11U-jre_s390x_linux_hotspot_11.0.17_8.tar.gz';          ;;        amd64|i386:x86-64)          ESUM='752616097e09d7f60a3ad8bd312f90eaf50ac72577e55df229fe6e8091148f79';          BINARY_URL='https://github.com/adoptium/temurin11-binaries/releases/download/jdk-11.0.17%2B8/OpenJDK11U-jre_x64_linux_hotspot_11.0.17_8.tar.gz';          ;;        *)          echo "Unsupported arch: ${ARCH}";          exit 1;          ;;     esac; 	  wget -O /tmp/openjdk.tar.gz ${BINARY_URL}; 	  echo "${ESUM} */tmp/openjdk.tar.gz" | sha256sum -c -; 	  mkdir -p "$JAVA_HOME"; 	  tar --extract 	      --file /tmp/openjdk.tar.gz 	      --directory "$JAVA_HOME" 	      --strip-components 1 	      --no-same-owner 	  ;     rm /tmp/openjdk.tar.gz;     find "$JAVA_HOME/lib" -name '*.so' -exec dirname '{}' ';' | sort -u > /etc/ld.so.conf.d/docker-openjdk.conf;     ldconfig;     java -Xshare:dump;
# Fri, 04 Nov 2022 23:22:32 GMT
RUN echo Verifying install ...     && fileEncoding="$(echo 'System.out.println(System.getProperty("file.encoding"))' | jshell -s -)"; [ "$fileEncoding" = 'UTF-8' ]; rm -rf ~/.java     && echo java --version && java --version     && echo Complete.
# Sat, 05 Nov 2022 01:35:16 GMT
ENV CATALINA_HOME=/usr/local/tomcat
# Sat, 05 Nov 2022 01:35:16 GMT
ENV PATH=/usr/local/tomcat/bin:/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Sat, 05 Nov 2022 01:35:17 GMT
RUN mkdir -p "$CATALINA_HOME"
# Sat, 05 Nov 2022 01:35:17 GMT
WORKDIR /usr/local/tomcat
# Sat, 05 Nov 2022 01:35:17 GMT
ENV TOMCAT_NATIVE_LIBDIR=/usr/local/tomcat/native-jni-lib
# Sat, 05 Nov 2022 01:35:17 GMT
ENV LD_LIBRARY_PATH=/usr/local/tomcat/native-jni-lib
# Sat, 05 Nov 2022 01:39:54 GMT
ENV GPG_KEYS=48F8E69F6390C9F25CFEDCD268248959359E722B A9C5DF4D22E99998D9875A5110C01C5A2F6059E7 DCFD35E0BF8CA7344752DE8B6FB21E8933C60243
# Sat, 05 Nov 2022 01:39:54 GMT
ENV TOMCAT_MAJOR=9
# Tue, 15 Nov 2022 03:06:43 GMT
ENV TOMCAT_VERSION=9.0.69
# Tue, 15 Nov 2022 03:06:43 GMT
ENV TOMCAT_SHA512=8c883c54ce9ce43eba37756a6404cdf3477879883a3e6d146dc8a7aa5e0425f487466afe6b6da4a895927cb7cb59177b9379cec18000f2de12785be57408c779
# Tue, 15 Nov 2022 03:06:44 GMT
COPY dir:b1a33aa3993dbbfbebb33bd9aa546b60c2f2191abf1227f453d4e830f6deb35f in /usr/local/tomcat 
# Tue, 15 Nov 2022 03:06:48 GMT
RUN set -eux; 	apt-get update; 	xargs -rt apt-get install -y --no-install-recommends < "$TOMCAT_NATIVE_LIBDIR/.dependencies.txt"; 	rm -rf /var/lib/apt/lists/*
# Tue, 15 Nov 2022 03:06:49 GMT
RUN set -eux; 	nativeLines="$(catalina.sh configtest 2>&1)"; 	nativeLines="$(echo "$nativeLines" | grep 'Apache Tomcat Native')"; 	nativeLines="$(echo "$nativeLines" | sort -u)"; 	if ! echo "$nativeLines" | grep -E 'INFO: Loaded( APR based)? Apache Tomcat Native library' >&2; then 		echo >&2 "$nativeLines"; 		exit 1; 	fi
# Tue, 15 Nov 2022 03:06:49 GMT
EXPOSE 8080
# Tue, 15 Nov 2022 03:06:49 GMT
CMD ["catalina.sh" "run"]
# Wed, 11 Jan 2023 02:47:03 GMT
LABEL org.opencontainers.image.authors=XWiki Development Team <committers@xwiki.org>
# Wed, 11 Jan 2023 02:47:03 GMT
LABEL org.opencontainers.image.url=https://hub.docker.com/_/xwiki
# Wed, 11 Jan 2023 02:47:03 GMT
LABEL org.opencontainers.image.documentation=https://hub.docker.com/_/xwiki
# Wed, 11 Jan 2023 02:47:03 GMT
LABEL org.opencontainers.image.source=https://github.com/xwiki/xwiki-docker.git
# Wed, 11 Jan 2023 02:47:04 GMT
LABEL org.opencontainers.image.vendor=xwiki.org
# Wed, 11 Jan 2023 02:47:04 GMT
LABEL org.opencontainers.image.licenses=LGPL-2.1
# Wed, 11 Jan 2023 02:49:03 GMT
RUN apt-get update &&   apt-get --no-install-recommends -y install     curl     libreoffice     unzip     procps &&   rm -rf /var/lib/apt/lists/*
# Tue, 31 Jan 2023 00:20:17 GMT
ENV XWIKI_VERSION=15.0
# Tue, 31 Jan 2023 00:20:17 GMT
ENV XWIKI_URL_PREFIX=https://maven.xwiki.org/releases/org/xwiki/platform/xwiki-platform-distribution-war/15.0
# Tue, 31 Jan 2023 00:20:17 GMT
ENV XWIKI_DOWNLOAD_SHA256=79ba0f479bbc49521c113821adc9d91141075a9470d7f9bbb6994ca59c30d121
# Tue, 31 Jan 2023 00:21:18 GMT
RUN rm -rf /usr/local/tomcat/webapps/* &&   mkdir -p /usr/local/tomcat/temp &&   mkdir -p /usr/local/xwiki/data &&   curl -fSL "${XWIKI_URL_PREFIX}/xwiki-platform-distribution-war-${XWIKI_VERSION}.war" -o xwiki.war &&   echo "$XWIKI_DOWNLOAD_SHA256 xwiki.war" | sha256sum -c - &&   unzip -d /usr/local/tomcat/webapps/ROOT xwiki.war &&   rm -f xwiki.war
# Tue, 31 Jan 2023 00:21:19 GMT
ENV MYSQL_JDBC_VERSION=8.0.31
# Tue, 31 Jan 2023 00:21:19 GMT
ENV MYSQL_JDBC_SHA256=5249e3dc6d6531b37790e3f61845b96db5e41e891d3d8edb0e2e3a1b53ca2f4f
# Tue, 31 Jan 2023 00:21:19 GMT
ENV MYSQL_JDBC_PREFIX=https://repo1.maven.org/maven2/com/mysql/mysql-connector-j/8.0.31
# Tue, 31 Jan 2023 00:21:19 GMT
ENV MYSQL_JDBC_ARTIFACT=mysql-connector-j-8.0.31.jar
# Tue, 31 Jan 2023 00:21:19 GMT
ENV MYSQL_JDBC_TARGET=/usr/local/tomcat/webapps/ROOT/WEB-INF/lib/mysql-connector-j-8.0.31.jar
# Tue, 31 Jan 2023 00:21:20 GMT
RUN curl -fSL "${MYSQL_JDBC_PREFIX}/${MYSQL_JDBC_ARTIFACT}" -o $MYSQL_JDBC_TARGET &&   echo "$MYSQL_JDBC_SHA256 $MYSQL_JDBC_TARGET" | sha256sum -c -
# Tue, 31 Jan 2023 00:21:21 GMT
COPY file:0a1be11e2eb610a1dbcd415404e3a592641110b93090030cb831e3a19a163017 in /usr/local/tomcat/bin/ 
# Tue, 31 Jan 2023 00:21:21 GMT
COPY file:1b8409986f3e4eb79a7a0b18472cb2692a61d504fb5ef34292bc997b79fd760d in /usr/local/tomcat/webapps/ROOT/WEB-INF/hibernate.cfg.xml 
# Tue, 31 Jan 2023 00:21:21 GMT
RUN sed -i 's/<id>org.xwiki.platform:xwiki-platform-distribution-war/<id>org.xwiki.platform:xwiki-platform-distribution-docker/'   /usr/local/tomcat/webapps/ROOT/META-INF/extension.xed
# Tue, 31 Jan 2023 00:21:21 GMT
COPY file:a47c4dcd87c9dad97aff38c49188357e6193bcad50757e516cfb08a60d4de611 in /usr/local/bin/docker-entrypoint.sh 
# Tue, 31 Jan 2023 00:21:22 GMT
VOLUME [/usr/local/xwiki]
# Tue, 31 Jan 2023 00:21:22 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 31 Jan 2023 00:21:22 GMT
CMD ["xwiki"]
```

-	Layers:
	-	`sha256:e96e057aae67380a4ddb16c337c5c3669d97fdff69ec537f02aa2cc30d814281`  
		Last Modified: Wed, 02 Nov 2022 03:03:36 GMT  
		Size: 30.4 MB (30425607 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4ced2591451da3a02e2b6bb44752b9e3f00d77789921be4df5082fb9f9880ad0`  
		Last Modified: Wed, 02 Nov 2022 18:48:43 GMT  
		Size: 12.4 MB (12439006 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:df8f874ae8c08a9e69e5fbe6c5a64200a45386132a3203d1a9a7f1146d94cfbc`  
		Last Modified: Fri, 04 Nov 2022 23:29:33 GMT  
		Size: 46.6 MB (46629936 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:111b6c7486426c4b6989102c2ee5be856e8a58e20ab0a350b24a905d536e8e7f`  
		Last Modified: Fri, 04 Nov 2022 23:29:26 GMT  
		Size: 161.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e6f84dce457c6d4f7b7291fce05f8e77998a3a7722a54125a1f1d52ca83043b4`  
		Last Modified: Sat, 05 Nov 2022 01:50:51 GMT  
		Size: 173.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a6c26749ee782392e38845ee2ba79b0da586ef6a45d8e7f29c7af14612278547`  
		Last Modified: Tue, 15 Nov 2022 03:19:57 GMT  
		Size: 12.2 MB (12200249 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4dddc6d9fa6024025b3fcfe729cab2dc544fb25476eca6e80b1af8e8d93bb0ee`  
		Last Modified: Tue, 15 Nov 2022 03:19:56 GMT  
		Size: 452.7 KB (452680 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:06637eebe5e72c8ad9019ad4eb4cdde1f11f7d4c24c7ed7374cf8966343aa2fb`  
		Last Modified: Tue, 15 Nov 2022 03:19:56 GMT  
		Size: 131.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b276fb8390410a8208724033e325715ea26000d5a1a762d4c3699b927884fbfe`  
		Last Modified: Wed, 11 Jan 2023 02:52:45 GMT  
		Size: 178.8 MB (178805608 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:156ca91198173149698aa0396648a9608b6ab1f2bc2666800843ce33c9f85b6e`  
		Last Modified: Tue, 31 Jan 2023 00:24:09 GMT  
		Size: 307.1 MB (307117069 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4c8b70d250c6d507901857473b0dcb67132d7b2a30ce9a69b07b1036853df738`  
		Last Modified: Tue, 31 Jan 2023 00:23:52 GMT  
		Size: 2.4 MB (2377191 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a9681fd36be674d25231c69d6a39f9e8fa65034eeaef5d1bd885fdbeac7f0f6b`  
		Last Modified: Tue, 31 Jan 2023 00:23:51 GMT  
		Size: 1.3 KB (1346 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a9d0d5da840f4d7da9943942b38cd092fae11f41dc6c19afd58d655cd6192d66`  
		Last Modified: Tue, 31 Jan 2023 00:23:51 GMT  
		Size: 2.3 KB (2312 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d65610da4f1da86fea8fbec0189b066afd4b86e4e8f7d049e3c4bc6ade9ba90a`  
		Last Modified: Tue, 31 Jan 2023 00:23:51 GMT  
		Size: 6.0 KB (6009 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3d41686284d7675eaa0f92c9cc27ebe73b4c30768c8eef9f23ee3b1ad06da00a`  
		Last Modified: Tue, 31 Jan 2023 00:23:51 GMT  
		Size: 2.5 KB (2504 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `xwiki:stable-mysql-tomcat` - linux; arm64 variant v8

```console
$ docker pull xwiki@sha256:6bf63d9025b07b69d744200c05efd4ffb8a52f3c38380f5d59a0b48514203cd2
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **581.7 MB (581709921 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:6600f2bb05836c703d53944bbcb5399d509a9813a27a35e99ff717becc308330`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["xwiki"]`

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
# Wed, 02 Nov 2022 19:44:32 GMT
RUN apt-get update     && DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends tzdata curl wget ca-certificates fontconfig locales     && echo "en_US.UTF-8 UTF-8" >> /etc/locale.gen     && locale-gen en_US.UTF-8     && rm -rf /var/lib/apt/lists/*
# Fri, 04 Nov 2022 22:40:54 GMT
ENV JAVA_VERSION=jdk-11.0.17+8
# Fri, 04 Nov 2022 22:41:33 GMT
RUN set -eux;     ARCH="$(dpkg --print-architecture)";     case "${ARCH}" in        aarch64|arm64)          ESUM='bd6efe3290c8b5a42f695a55a26f3e3c9c284288574879d4b7089f31f5114177';          BINARY_URL='https://github.com/adoptium/temurin11-binaries/releases/download/jdk-11.0.17%2B8/OpenJDK11U-jre_aarch64_linux_hotspot_11.0.17_8.tar.gz';          ;;        armhf|arm)          ESUM='8cf113d3d7fa808895c8d2e41bb890af21c47e38c2460e0588147a4bb8fc658d';          BINARY_URL='https://github.com/adoptium/temurin11-binaries/releases/download/jdk-11.0.17%2B8/OpenJDK11U-jre_arm_linux_hotspot_11.0.17_8.tar.gz';          ;;        ppc64el|powerpc:common64)          ESUM='0ca3d806131ab5834c501f9c625bb0248cd528af361c704503348e9c9605bedf';          BINARY_URL='https://github.com/adoptium/temurin11-binaries/releases/download/jdk-11.0.17%2B8/OpenJDK11U-jre_ppc64le_linux_hotspot_11.0.17_8.tar.gz';          ;;        s390x|s390:64-bit)          ESUM='dd3b159a374086e65cb07c4ccb226c90f9c02ef929cba6f0b642171d7ed97fa4';          BINARY_URL='https://github.com/adoptium/temurin11-binaries/releases/download/jdk-11.0.17%2B8/OpenJDK11U-jre_s390x_linux_hotspot_11.0.17_8.tar.gz';          ;;        amd64|i386:x86-64)          ESUM='752616097e09d7f60a3ad8bd312f90eaf50ac72577e55df229fe6e8091148f79';          BINARY_URL='https://github.com/adoptium/temurin11-binaries/releases/download/jdk-11.0.17%2B8/OpenJDK11U-jre_x64_linux_hotspot_11.0.17_8.tar.gz';          ;;        *)          echo "Unsupported arch: ${ARCH}";          exit 1;          ;;     esac; 	  wget -O /tmp/openjdk.tar.gz ${BINARY_URL}; 	  echo "${ESUM} */tmp/openjdk.tar.gz" | sha256sum -c -; 	  mkdir -p "$JAVA_HOME"; 	  tar --extract 	      --file /tmp/openjdk.tar.gz 	      --directory "$JAVA_HOME" 	      --strip-components 1 	      --no-same-owner 	  ;     rm /tmp/openjdk.tar.gz;     find "$JAVA_HOME/lib" -name '*.so' -exec dirname '{}' ';' | sort -u > /etc/ld.so.conf.d/docker-openjdk.conf;     ldconfig;     java -Xshare:dump;
# Fri, 04 Nov 2022 22:41:34 GMT
RUN echo Verifying install ...     && fileEncoding="$(echo 'System.out.println(System.getProperty("file.encoding"))' | jshell -s -)"; [ "$fileEncoding" = 'UTF-8' ]; rm -rf ~/.java     && echo java --version && java --version     && echo Complete.
# Fri, 04 Nov 2022 23:48:38 GMT
ENV CATALINA_HOME=/usr/local/tomcat
# Fri, 04 Nov 2022 23:48:38 GMT
ENV PATH=/usr/local/tomcat/bin:/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Fri, 04 Nov 2022 23:48:38 GMT
RUN mkdir -p "$CATALINA_HOME"
# Fri, 04 Nov 2022 23:48:39 GMT
WORKDIR /usr/local/tomcat
# Fri, 04 Nov 2022 23:48:39 GMT
ENV TOMCAT_NATIVE_LIBDIR=/usr/local/tomcat/native-jni-lib
# Fri, 04 Nov 2022 23:48:39 GMT
ENV LD_LIBRARY_PATH=/usr/local/tomcat/native-jni-lib
# Fri, 04 Nov 2022 23:53:12 GMT
ENV GPG_KEYS=48F8E69F6390C9F25CFEDCD268248959359E722B A9C5DF4D22E99998D9875A5110C01C5A2F6059E7 DCFD35E0BF8CA7344752DE8B6FB21E8933C60243
# Fri, 04 Nov 2022 23:53:12 GMT
ENV TOMCAT_MAJOR=9
# Tue, 15 Nov 2022 04:57:22 GMT
ENV TOMCAT_VERSION=9.0.69
# Tue, 15 Nov 2022 04:57:22 GMT
ENV TOMCAT_SHA512=8c883c54ce9ce43eba37756a6404cdf3477879883a3e6d146dc8a7aa5e0425f487466afe6b6da4a895927cb7cb59177b9379cec18000f2de12785be57408c779
# Tue, 15 Nov 2022 04:57:22 GMT
COPY dir:096b403a5f78b17e6b4bff63128a9c93941b97f22470991610dd641633d977f1 in /usr/local/tomcat 
# Tue, 15 Nov 2022 04:57:25 GMT
RUN set -eux; 	apt-get update; 	xargs -rt apt-get install -y --no-install-recommends < "$TOMCAT_NATIVE_LIBDIR/.dependencies.txt"; 	rm -rf /var/lib/apt/lists/*
# Tue, 15 Nov 2022 04:57:26 GMT
RUN set -eux; 	nativeLines="$(catalina.sh configtest 2>&1)"; 	nativeLines="$(echo "$nativeLines" | grep 'Apache Tomcat Native')"; 	nativeLines="$(echo "$nativeLines" | sort -u)"; 	if ! echo "$nativeLines" | grep -E 'INFO: Loaded( APR based)? Apache Tomcat Native library' >&2; then 		echo >&2 "$nativeLines"; 		exit 1; 	fi
# Tue, 15 Nov 2022 04:57:26 GMT
EXPOSE 8080
# Tue, 15 Nov 2022 04:57:27 GMT
CMD ["catalina.sh" "run"]
# Wed, 11 Jan 2023 03:05:10 GMT
LABEL org.opencontainers.image.authors=XWiki Development Team <committers@xwiki.org>
# Wed, 11 Jan 2023 03:05:10 GMT
LABEL org.opencontainers.image.url=https://hub.docker.com/_/xwiki
# Wed, 11 Jan 2023 03:05:10 GMT
LABEL org.opencontainers.image.documentation=https://hub.docker.com/_/xwiki
# Wed, 11 Jan 2023 03:05:10 GMT
LABEL org.opencontainers.image.source=https://github.com/xwiki/xwiki-docker.git
# Wed, 11 Jan 2023 03:05:11 GMT
LABEL org.opencontainers.image.vendor=xwiki.org
# Wed, 11 Jan 2023 03:05:11 GMT
LABEL org.opencontainers.image.licenses=LGPL-2.1
# Wed, 11 Jan 2023 03:07:37 GMT
RUN apt-get update &&   apt-get --no-install-recommends -y install     curl     libreoffice     unzip     procps &&   rm -rf /var/lib/apt/lists/*
# Tue, 31 Jan 2023 00:47:12 GMT
ENV XWIKI_VERSION=15.0
# Tue, 31 Jan 2023 00:47:12 GMT
ENV XWIKI_URL_PREFIX=https://maven.xwiki.org/releases/org/xwiki/platform/xwiki-platform-distribution-war/15.0
# Tue, 31 Jan 2023 00:47:12 GMT
ENV XWIKI_DOWNLOAD_SHA256=79ba0f479bbc49521c113821adc9d91141075a9470d7f9bbb6994ca59c30d121
# Tue, 31 Jan 2023 00:47:58 GMT
RUN rm -rf /usr/local/tomcat/webapps/* &&   mkdir -p /usr/local/tomcat/temp &&   mkdir -p /usr/local/xwiki/data &&   curl -fSL "${XWIKI_URL_PREFIX}/xwiki-platform-distribution-war-${XWIKI_VERSION}.war" -o xwiki.war &&   echo "$XWIKI_DOWNLOAD_SHA256 xwiki.war" | sha256sum -c - &&   unzip -d /usr/local/tomcat/webapps/ROOT xwiki.war &&   rm -f xwiki.war
# Tue, 31 Jan 2023 00:48:01 GMT
ENV MYSQL_JDBC_VERSION=8.0.31
# Tue, 31 Jan 2023 00:48:01 GMT
ENV MYSQL_JDBC_SHA256=5249e3dc6d6531b37790e3f61845b96db5e41e891d3d8edb0e2e3a1b53ca2f4f
# Tue, 31 Jan 2023 00:48:01 GMT
ENV MYSQL_JDBC_PREFIX=https://repo1.maven.org/maven2/com/mysql/mysql-connector-j/8.0.31
# Tue, 31 Jan 2023 00:48:01 GMT
ENV MYSQL_JDBC_ARTIFACT=mysql-connector-j-8.0.31.jar
# Tue, 31 Jan 2023 00:48:01 GMT
ENV MYSQL_JDBC_TARGET=/usr/local/tomcat/webapps/ROOT/WEB-INF/lib/mysql-connector-j-8.0.31.jar
# Tue, 31 Jan 2023 00:48:02 GMT
RUN curl -fSL "${MYSQL_JDBC_PREFIX}/${MYSQL_JDBC_ARTIFACT}" -o $MYSQL_JDBC_TARGET &&   echo "$MYSQL_JDBC_SHA256 $MYSQL_JDBC_TARGET" | sha256sum -c -
# Tue, 31 Jan 2023 00:48:02 GMT
COPY file:0a1be11e2eb610a1dbcd415404e3a592641110b93090030cb831e3a19a163017 in /usr/local/tomcat/bin/ 
# Tue, 31 Jan 2023 00:48:02 GMT
COPY file:1b8409986f3e4eb79a7a0b18472cb2692a61d504fb5ef34292bc997b79fd760d in /usr/local/tomcat/webapps/ROOT/WEB-INF/hibernate.cfg.xml 
# Tue, 31 Jan 2023 00:48:03 GMT
RUN sed -i 's/<id>org.xwiki.platform:xwiki-platform-distribution-war/<id>org.xwiki.platform:xwiki-platform-distribution-docker/'   /usr/local/tomcat/webapps/ROOT/META-INF/extension.xed
# Tue, 31 Jan 2023 00:48:03 GMT
COPY file:a47c4dcd87c9dad97aff38c49188357e6193bcad50757e516cfb08a60d4de611 in /usr/local/bin/docker-entrypoint.sh 
# Tue, 31 Jan 2023 00:48:03 GMT
VOLUME [/usr/local/xwiki]
# Tue, 31 Jan 2023 00:48:03 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 31 Jan 2023 00:48:03 GMT
CMD ["xwiki"]
```

-	Layers:
	-	`sha256:0509fae36eb0656f8bdb23f8ae64100d893bcea2563e97468d337e04d2d0410b`  
		Last Modified: Wed, 02 Nov 2022 18:50:21 GMT  
		Size: 28.4 MB (28382154 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e502a1af2bcd98f5f0d2f5e4da1a0e7bbe07a2c548e2662f7d37dce5ae1df46c`  
		Last Modified: Wed, 02 Nov 2022 19:48:28 GMT  
		Size: 12.4 MB (12396330 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bc4598c07dd818f03a0378b0341a4a8e80f0152fbb3e7d5246ca4f466f42e611`  
		Last Modified: Fri, 04 Nov 2022 22:46:46 GMT  
		Size: 45.0 MB (44958470 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:715a937a1066f998b331fcd62256ad01a5571bdf46804e97825afc64f9ebb427`  
		Last Modified: Fri, 04 Nov 2022 22:46:41 GMT  
		Size: 160.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5fb623f082f74b2fa9fc2c4e3f3a4802875cb9753cfa26ed940201ce72bb56cb`  
		Last Modified: Sat, 05 Nov 2022 00:03:40 GMT  
		Size: 172.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:33260b83200262bbd546be371ad3c1f50f5ae7228afb87982d6fa9d6b11bf26f`  
		Last Modified: Tue, 15 Nov 2022 05:10:19 GMT  
		Size: 12.2 MB (12207235 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0955fb697ea9b30a1b4f95385464f646aa1525cb6efba648e22df84ebef6b2ee`  
		Last Modified: Tue, 15 Nov 2022 05:10:18 GMT  
		Size: 452.0 KB (452021 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6eddcf66f2083b1487296a0308e0b058917c97f614f12428d82d89662038dc2e`  
		Last Modified: Tue, 15 Nov 2022 05:10:18 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ae5f60bb64f3fa11da3d15a9639f886186b4c2c021455c3f9db22e0cfe1b1311`  
		Last Modified: Wed, 11 Jan 2023 03:11:14 GMT  
		Size: 173.8 MB (173806827 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1814d85fce571b42f2cfa7c8a904e1a184ee6f49642242a44bbe0037088994a0`  
		Last Modified: Tue, 31 Jan 2023 00:56:04 GMT  
		Size: 307.1 MB (307117070 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8aec0e24b4fa870989f014944c3c7d535355a2371fc8c948b2b11f9b377efe6e`  
		Last Modified: Tue, 31 Jan 2023 00:55:50 GMT  
		Size: 2.4 MB (2377182 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0b65081619aa0114a7f367836ef421eb8d951e559e0f089c7728af7813b1ea62`  
		Last Modified: Tue, 31 Jan 2023 00:55:49 GMT  
		Size: 1.3 KB (1348 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:46ebad072e608146426d8dc30828937049eea36c2e636d7790b4960d6d586977`  
		Last Modified: Tue, 31 Jan 2023 00:55:49 GMT  
		Size: 2.3 KB (2308 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:708fefcedd4ee6c106da247a68c5790f5ab00225d1cdfff8465575265c3a54e6`  
		Last Modified: Tue, 31 Jan 2023 00:55:49 GMT  
		Size: 6.0 KB (6008 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:81e3bf8e20bc921031e7549a41dec1b2d7795cc6da40a0e7096bf654b25c5c3e`  
		Last Modified: Tue, 31 Jan 2023 00:55:49 GMT  
		Size: 2.5 KB (2507 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `xwiki:stable-postgres`

```console
$ docker pull xwiki@sha256:f6739c1133cbbece87973ddea5fbc57222abb9d7d3f8064eee9d2c2c0d46ecfa
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `xwiki:stable-postgres` - linux; amd64

```console
$ docker pull xwiki@sha256:72928baeace929e42f17f01362700392a90c6750b2ec1f84f24bbba1c4ff0236
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **590.0 MB (589959353 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b71f03d7d3a1760e73e6f4370f49317d16a7e0cb22532f49c11c0ee73b2c6262`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["xwiki"]`

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
# Wed, 02 Nov 2022 18:44:10 GMT
RUN apt-get update     && DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends tzdata curl wget ca-certificates fontconfig locales     && echo "en_US.UTF-8 UTF-8" >> /etc/locale.gen     && locale-gen en_US.UTF-8     && rm -rf /var/lib/apt/lists/*
# Fri, 04 Nov 2022 23:21:41 GMT
ENV JAVA_VERSION=jdk-11.0.17+8
# Fri, 04 Nov 2022 23:22:31 GMT
RUN set -eux;     ARCH="$(dpkg --print-architecture)";     case "${ARCH}" in        aarch64|arm64)          ESUM='bd6efe3290c8b5a42f695a55a26f3e3c9c284288574879d4b7089f31f5114177';          BINARY_URL='https://github.com/adoptium/temurin11-binaries/releases/download/jdk-11.0.17%2B8/OpenJDK11U-jre_aarch64_linux_hotspot_11.0.17_8.tar.gz';          ;;        armhf|arm)          ESUM='8cf113d3d7fa808895c8d2e41bb890af21c47e38c2460e0588147a4bb8fc658d';          BINARY_URL='https://github.com/adoptium/temurin11-binaries/releases/download/jdk-11.0.17%2B8/OpenJDK11U-jre_arm_linux_hotspot_11.0.17_8.tar.gz';          ;;        ppc64el|powerpc:common64)          ESUM='0ca3d806131ab5834c501f9c625bb0248cd528af361c704503348e9c9605bedf';          BINARY_URL='https://github.com/adoptium/temurin11-binaries/releases/download/jdk-11.0.17%2B8/OpenJDK11U-jre_ppc64le_linux_hotspot_11.0.17_8.tar.gz';          ;;        s390x|s390:64-bit)          ESUM='dd3b159a374086e65cb07c4ccb226c90f9c02ef929cba6f0b642171d7ed97fa4';          BINARY_URL='https://github.com/adoptium/temurin11-binaries/releases/download/jdk-11.0.17%2B8/OpenJDK11U-jre_s390x_linux_hotspot_11.0.17_8.tar.gz';          ;;        amd64|i386:x86-64)          ESUM='752616097e09d7f60a3ad8bd312f90eaf50ac72577e55df229fe6e8091148f79';          BINARY_URL='https://github.com/adoptium/temurin11-binaries/releases/download/jdk-11.0.17%2B8/OpenJDK11U-jre_x64_linux_hotspot_11.0.17_8.tar.gz';          ;;        *)          echo "Unsupported arch: ${ARCH}";          exit 1;          ;;     esac; 	  wget -O /tmp/openjdk.tar.gz ${BINARY_URL}; 	  echo "${ESUM} */tmp/openjdk.tar.gz" | sha256sum -c -; 	  mkdir -p "$JAVA_HOME"; 	  tar --extract 	      --file /tmp/openjdk.tar.gz 	      --directory "$JAVA_HOME" 	      --strip-components 1 	      --no-same-owner 	  ;     rm /tmp/openjdk.tar.gz;     find "$JAVA_HOME/lib" -name '*.so' -exec dirname '{}' ';' | sort -u > /etc/ld.so.conf.d/docker-openjdk.conf;     ldconfig;     java -Xshare:dump;
# Fri, 04 Nov 2022 23:22:32 GMT
RUN echo Verifying install ...     && fileEncoding="$(echo 'System.out.println(System.getProperty("file.encoding"))' | jshell -s -)"; [ "$fileEncoding" = 'UTF-8' ]; rm -rf ~/.java     && echo java --version && java --version     && echo Complete.
# Sat, 05 Nov 2022 01:35:16 GMT
ENV CATALINA_HOME=/usr/local/tomcat
# Sat, 05 Nov 2022 01:35:16 GMT
ENV PATH=/usr/local/tomcat/bin:/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Sat, 05 Nov 2022 01:35:17 GMT
RUN mkdir -p "$CATALINA_HOME"
# Sat, 05 Nov 2022 01:35:17 GMT
WORKDIR /usr/local/tomcat
# Sat, 05 Nov 2022 01:35:17 GMT
ENV TOMCAT_NATIVE_LIBDIR=/usr/local/tomcat/native-jni-lib
# Sat, 05 Nov 2022 01:35:17 GMT
ENV LD_LIBRARY_PATH=/usr/local/tomcat/native-jni-lib
# Sat, 05 Nov 2022 01:39:54 GMT
ENV GPG_KEYS=48F8E69F6390C9F25CFEDCD268248959359E722B A9C5DF4D22E99998D9875A5110C01C5A2F6059E7 DCFD35E0BF8CA7344752DE8B6FB21E8933C60243
# Sat, 05 Nov 2022 01:39:54 GMT
ENV TOMCAT_MAJOR=9
# Tue, 15 Nov 2022 03:06:43 GMT
ENV TOMCAT_VERSION=9.0.69
# Tue, 15 Nov 2022 03:06:43 GMT
ENV TOMCAT_SHA512=8c883c54ce9ce43eba37756a6404cdf3477879883a3e6d146dc8a7aa5e0425f487466afe6b6da4a895927cb7cb59177b9379cec18000f2de12785be57408c779
# Tue, 15 Nov 2022 03:06:44 GMT
COPY dir:b1a33aa3993dbbfbebb33bd9aa546b60c2f2191abf1227f453d4e830f6deb35f in /usr/local/tomcat 
# Tue, 15 Nov 2022 03:06:48 GMT
RUN set -eux; 	apt-get update; 	xargs -rt apt-get install -y --no-install-recommends < "$TOMCAT_NATIVE_LIBDIR/.dependencies.txt"; 	rm -rf /var/lib/apt/lists/*
# Tue, 15 Nov 2022 03:06:49 GMT
RUN set -eux; 	nativeLines="$(catalina.sh configtest 2>&1)"; 	nativeLines="$(echo "$nativeLines" | grep 'Apache Tomcat Native')"; 	nativeLines="$(echo "$nativeLines" | sort -u)"; 	if ! echo "$nativeLines" | grep -E 'INFO: Loaded( APR based)? Apache Tomcat Native library' >&2; then 		echo >&2 "$nativeLines"; 		exit 1; 	fi
# Tue, 15 Nov 2022 03:06:49 GMT
EXPOSE 8080
# Tue, 15 Nov 2022 03:06:49 GMT
CMD ["catalina.sh" "run"]
# Wed, 11 Jan 2023 02:47:03 GMT
LABEL org.opencontainers.image.authors=XWiki Development Team <committers@xwiki.org>
# Wed, 11 Jan 2023 02:47:03 GMT
LABEL org.opencontainers.image.url=https://hub.docker.com/_/xwiki
# Wed, 11 Jan 2023 02:47:03 GMT
LABEL org.opencontainers.image.documentation=https://hub.docker.com/_/xwiki
# Wed, 11 Jan 2023 02:47:03 GMT
LABEL org.opencontainers.image.source=https://github.com/xwiki/xwiki-docker.git
# Wed, 11 Jan 2023 02:47:04 GMT
LABEL org.opencontainers.image.vendor=xwiki.org
# Wed, 11 Jan 2023 02:47:04 GMT
LABEL org.opencontainers.image.licenses=LGPL-2.1
# Wed, 11 Jan 2023 02:50:25 GMT
RUN apt-get update &&   apt-get --no-install-recommends -y install     curl     libreoffice     unzip     procps     libpostgresql-jdbc-java &&   rm -rf /var/lib/apt/lists/*
# Tue, 31 Jan 2023 00:21:26 GMT
ENV XWIKI_VERSION=15.0
# Tue, 31 Jan 2023 00:21:27 GMT
ENV XWIKI_URL_PREFIX=https://maven.xwiki.org/releases/org/xwiki/platform/xwiki-platform-distribution-war/15.0
# Tue, 31 Jan 2023 00:21:27 GMT
ENV XWIKI_DOWNLOAD_SHA256=79ba0f479bbc49521c113821adc9d91141075a9470d7f9bbb6994ca59c30d121
# Tue, 31 Jan 2023 00:22:39 GMT
RUN rm -rf /usr/local/tomcat/webapps/* &&   mkdir -p /usr/local/tomcat/temp &&   mkdir -p /usr/local/xwiki/data &&   curl -fSL "${XWIKI_URL_PREFIX}/xwiki-platform-distribution-war-${XWIKI_VERSION}.war" -o xwiki.war &&   echo "$XWIKI_DOWNLOAD_SHA256 xwiki.war" | sha256sum -c - &&   unzip -d /usr/local/tomcat/webapps/ROOT xwiki.war &&   rm -f xwiki.war
# Tue, 31 Jan 2023 00:22:40 GMT
RUN cp /usr/share/java/postgresql-jdbc4.jar /usr/local/tomcat/webapps/ROOT/WEB-INF/lib/
# Tue, 31 Jan 2023 00:22:41 GMT
COPY file:0a1be11e2eb610a1dbcd415404e3a592641110b93090030cb831e3a19a163017 in /usr/local/tomcat/bin/ 
# Tue, 31 Jan 2023 00:22:41 GMT
COPY file:4a923f484bb29a26630c19e1d617d3bf6aa6ae7c6c4a5561e97b037bcde0847c in /usr/local/tomcat/webapps/ROOT/WEB-INF/hibernate.cfg.xml 
# Tue, 31 Jan 2023 00:22:41 GMT
RUN sed -i 's/<id>org.xwiki.platform:xwiki-platform-distribution-war/<id>org.xwiki.platform:xwiki-platform-distribution-docker/'   /usr/local/tomcat/webapps/ROOT/META-INF/extension.xed
# Tue, 31 Jan 2023 00:22:41 GMT
COPY file:a47c4dcd87c9dad97aff38c49188357e6193bcad50757e516cfb08a60d4de611 in /usr/local/bin/docker-entrypoint.sh 
# Tue, 31 Jan 2023 00:22:41 GMT
VOLUME [/usr/local/xwiki]
# Tue, 31 Jan 2023 00:22:42 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 31 Jan 2023 00:22:42 GMT
CMD ["xwiki"]
```

-	Layers:
	-	`sha256:e96e057aae67380a4ddb16c337c5c3669d97fdff69ec537f02aa2cc30d814281`  
		Last Modified: Wed, 02 Nov 2022 03:03:36 GMT  
		Size: 30.4 MB (30425607 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4ced2591451da3a02e2b6bb44752b9e3f00d77789921be4df5082fb9f9880ad0`  
		Last Modified: Wed, 02 Nov 2022 18:48:43 GMT  
		Size: 12.4 MB (12439006 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:df8f874ae8c08a9e69e5fbe6c5a64200a45386132a3203d1a9a7f1146d94cfbc`  
		Last Modified: Fri, 04 Nov 2022 23:29:33 GMT  
		Size: 46.6 MB (46629936 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:111b6c7486426c4b6989102c2ee5be856e8a58e20ab0a350b24a905d536e8e7f`  
		Last Modified: Fri, 04 Nov 2022 23:29:26 GMT  
		Size: 161.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e6f84dce457c6d4f7b7291fce05f8e77998a3a7722a54125a1f1d52ca83043b4`  
		Last Modified: Sat, 05 Nov 2022 01:50:51 GMT  
		Size: 173.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a6c26749ee782392e38845ee2ba79b0da586ef6a45d8e7f29c7af14612278547`  
		Last Modified: Tue, 15 Nov 2022 03:19:57 GMT  
		Size: 12.2 MB (12200249 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4dddc6d9fa6024025b3fcfe729cab2dc544fb25476eca6e80b1af8e8d93bb0ee`  
		Last Modified: Tue, 15 Nov 2022 03:19:56 GMT  
		Size: 452.7 KB (452680 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:06637eebe5e72c8ad9019ad4eb4cdde1f11f7d4c24c7ed7374cf8966343aa2fb`  
		Last Modified: Tue, 15 Nov 2022 03:19:56 GMT  
		Size: 131.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b57f6f8bcfb0d93b8e21d3068d1f65d3f08dba05c5fab7d4c36e2359317b18c7`  
		Last Modified: Wed, 11 Jan 2023 02:53:53 GMT  
		Size: 179.7 MB (179745182 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:71a0aee972ff5a36a4c5d67f5bf6416b1b78d06c906ce727c5e8e11098d0dfd1`  
		Last Modified: Tue, 31 Jan 2023 00:25:01 GMT  
		Size: 307.1 MB (307117070 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ccc745f1273896cef68a5af6cd5713c4a2d8704628920a53e318a008f8096426`  
		Last Modified: Tue, 31 Jan 2023 00:24:44 GMT  
		Size: 936.8 KB (936848 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1593979548bc568ed36dc9f5adb8f00d8b7d3eb1fa850fc06426c2c9345b8472`  
		Last Modified: Tue, 31 Jan 2023 00:24:43 GMT  
		Size: 1.3 KB (1345 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e1e58b32c2c2a52907f7e4ad05462d3b2afd11404a9678bc656fb96029b12d8d`  
		Last Modified: Tue, 31 Jan 2023 00:24:43 GMT  
		Size: 2.5 KB (2454 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c43ce01c7b867ce6cda62f86175ba6a53f44000797d61fe604aded86980c4d41`  
		Last Modified: Tue, 31 Jan 2023 00:24:43 GMT  
		Size: 6.0 KB (6006 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6fe6f306aa61d9839a01e62f4c308a9a7d3bd4cd5ce9a58407b6585f6950f054`  
		Last Modified: Tue, 31 Jan 2023 00:24:43 GMT  
		Size: 2.5 KB (2505 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `xwiki:stable-postgres` - linux; arm64 variant v8

```console
$ docker pull xwiki@sha256:ae51c629c7a76aa7c15ebb33fcfdae3e529ef6456ada6d0dbcf9ed8fc5ecf00d
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **581.2 MB (581212250 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:70277ae3ffdca68401bb57e24e6302cc64a403bf36869f0959e54d03216b0005`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["xwiki"]`

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
# Wed, 02 Nov 2022 19:44:32 GMT
RUN apt-get update     && DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends tzdata curl wget ca-certificates fontconfig locales     && echo "en_US.UTF-8 UTF-8" >> /etc/locale.gen     && locale-gen en_US.UTF-8     && rm -rf /var/lib/apt/lists/*
# Fri, 04 Nov 2022 22:40:54 GMT
ENV JAVA_VERSION=jdk-11.0.17+8
# Fri, 04 Nov 2022 22:41:33 GMT
RUN set -eux;     ARCH="$(dpkg --print-architecture)";     case "${ARCH}" in        aarch64|arm64)          ESUM='bd6efe3290c8b5a42f695a55a26f3e3c9c284288574879d4b7089f31f5114177';          BINARY_URL='https://github.com/adoptium/temurin11-binaries/releases/download/jdk-11.0.17%2B8/OpenJDK11U-jre_aarch64_linux_hotspot_11.0.17_8.tar.gz';          ;;        armhf|arm)          ESUM='8cf113d3d7fa808895c8d2e41bb890af21c47e38c2460e0588147a4bb8fc658d';          BINARY_URL='https://github.com/adoptium/temurin11-binaries/releases/download/jdk-11.0.17%2B8/OpenJDK11U-jre_arm_linux_hotspot_11.0.17_8.tar.gz';          ;;        ppc64el|powerpc:common64)          ESUM='0ca3d806131ab5834c501f9c625bb0248cd528af361c704503348e9c9605bedf';          BINARY_URL='https://github.com/adoptium/temurin11-binaries/releases/download/jdk-11.0.17%2B8/OpenJDK11U-jre_ppc64le_linux_hotspot_11.0.17_8.tar.gz';          ;;        s390x|s390:64-bit)          ESUM='dd3b159a374086e65cb07c4ccb226c90f9c02ef929cba6f0b642171d7ed97fa4';          BINARY_URL='https://github.com/adoptium/temurin11-binaries/releases/download/jdk-11.0.17%2B8/OpenJDK11U-jre_s390x_linux_hotspot_11.0.17_8.tar.gz';          ;;        amd64|i386:x86-64)          ESUM='752616097e09d7f60a3ad8bd312f90eaf50ac72577e55df229fe6e8091148f79';          BINARY_URL='https://github.com/adoptium/temurin11-binaries/releases/download/jdk-11.0.17%2B8/OpenJDK11U-jre_x64_linux_hotspot_11.0.17_8.tar.gz';          ;;        *)          echo "Unsupported arch: ${ARCH}";          exit 1;          ;;     esac; 	  wget -O /tmp/openjdk.tar.gz ${BINARY_URL}; 	  echo "${ESUM} */tmp/openjdk.tar.gz" | sha256sum -c -; 	  mkdir -p "$JAVA_HOME"; 	  tar --extract 	      --file /tmp/openjdk.tar.gz 	      --directory "$JAVA_HOME" 	      --strip-components 1 	      --no-same-owner 	  ;     rm /tmp/openjdk.tar.gz;     find "$JAVA_HOME/lib" -name '*.so' -exec dirname '{}' ';' | sort -u > /etc/ld.so.conf.d/docker-openjdk.conf;     ldconfig;     java -Xshare:dump;
# Fri, 04 Nov 2022 22:41:34 GMT
RUN echo Verifying install ...     && fileEncoding="$(echo 'System.out.println(System.getProperty("file.encoding"))' | jshell -s -)"; [ "$fileEncoding" = 'UTF-8' ]; rm -rf ~/.java     && echo java --version && java --version     && echo Complete.
# Fri, 04 Nov 2022 23:48:38 GMT
ENV CATALINA_HOME=/usr/local/tomcat
# Fri, 04 Nov 2022 23:48:38 GMT
ENV PATH=/usr/local/tomcat/bin:/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Fri, 04 Nov 2022 23:48:38 GMT
RUN mkdir -p "$CATALINA_HOME"
# Fri, 04 Nov 2022 23:48:39 GMT
WORKDIR /usr/local/tomcat
# Fri, 04 Nov 2022 23:48:39 GMT
ENV TOMCAT_NATIVE_LIBDIR=/usr/local/tomcat/native-jni-lib
# Fri, 04 Nov 2022 23:48:39 GMT
ENV LD_LIBRARY_PATH=/usr/local/tomcat/native-jni-lib
# Fri, 04 Nov 2022 23:53:12 GMT
ENV GPG_KEYS=48F8E69F6390C9F25CFEDCD268248959359E722B A9C5DF4D22E99998D9875A5110C01C5A2F6059E7 DCFD35E0BF8CA7344752DE8B6FB21E8933C60243
# Fri, 04 Nov 2022 23:53:12 GMT
ENV TOMCAT_MAJOR=9
# Tue, 15 Nov 2022 04:57:22 GMT
ENV TOMCAT_VERSION=9.0.69
# Tue, 15 Nov 2022 04:57:22 GMT
ENV TOMCAT_SHA512=8c883c54ce9ce43eba37756a6404cdf3477879883a3e6d146dc8a7aa5e0425f487466afe6b6da4a895927cb7cb59177b9379cec18000f2de12785be57408c779
# Tue, 15 Nov 2022 04:57:22 GMT
COPY dir:096b403a5f78b17e6b4bff63128a9c93941b97f22470991610dd641633d977f1 in /usr/local/tomcat 
# Tue, 15 Nov 2022 04:57:25 GMT
RUN set -eux; 	apt-get update; 	xargs -rt apt-get install -y --no-install-recommends < "$TOMCAT_NATIVE_LIBDIR/.dependencies.txt"; 	rm -rf /var/lib/apt/lists/*
# Tue, 15 Nov 2022 04:57:26 GMT
RUN set -eux; 	nativeLines="$(catalina.sh configtest 2>&1)"; 	nativeLines="$(echo "$nativeLines" | grep 'Apache Tomcat Native')"; 	nativeLines="$(echo "$nativeLines" | sort -u)"; 	if ! echo "$nativeLines" | grep -E 'INFO: Loaded( APR based)? Apache Tomcat Native library' >&2; then 		echo >&2 "$nativeLines"; 		exit 1; 	fi
# Tue, 15 Nov 2022 04:57:26 GMT
EXPOSE 8080
# Tue, 15 Nov 2022 04:57:27 GMT
CMD ["catalina.sh" "run"]
# Wed, 11 Jan 2023 03:05:10 GMT
LABEL org.opencontainers.image.authors=XWiki Development Team <committers@xwiki.org>
# Wed, 11 Jan 2023 03:05:10 GMT
LABEL org.opencontainers.image.url=https://hub.docker.com/_/xwiki
# Wed, 11 Jan 2023 03:05:10 GMT
LABEL org.opencontainers.image.documentation=https://hub.docker.com/_/xwiki
# Wed, 11 Jan 2023 03:05:10 GMT
LABEL org.opencontainers.image.source=https://github.com/xwiki/xwiki-docker.git
# Wed, 11 Jan 2023 03:05:11 GMT
LABEL org.opencontainers.image.vendor=xwiki.org
# Wed, 11 Jan 2023 03:05:11 GMT
LABEL org.opencontainers.image.licenses=LGPL-2.1
# Wed, 11 Jan 2023 03:08:55 GMT
RUN apt-get update &&   apt-get --no-install-recommends -y install     curl     libreoffice     unzip     procps     libpostgresql-jdbc-java &&   rm -rf /var/lib/apt/lists/*
# Tue, 31 Jan 2023 00:48:10 GMT
ENV XWIKI_VERSION=15.0
# Tue, 31 Jan 2023 00:48:10 GMT
ENV XWIKI_URL_PREFIX=https://maven.xwiki.org/releases/org/xwiki/platform/xwiki-platform-distribution-war/15.0
# Tue, 31 Jan 2023 00:48:10 GMT
ENV XWIKI_DOWNLOAD_SHA256=79ba0f479bbc49521c113821adc9d91141075a9470d7f9bbb6994ca59c30d121
# Tue, 31 Jan 2023 00:54:38 GMT
RUN rm -rf /usr/local/tomcat/webapps/* &&   mkdir -p /usr/local/tomcat/temp &&   mkdir -p /usr/local/xwiki/data &&   curl -fSL "${XWIKI_URL_PREFIX}/xwiki-platform-distribution-war-${XWIKI_VERSION}.war" -o xwiki.war &&   echo "$XWIKI_DOWNLOAD_SHA256 xwiki.war" | sha256sum -c - &&   unzip -d /usr/local/tomcat/webapps/ROOT xwiki.war &&   rm -f xwiki.war
# Tue, 31 Jan 2023 00:54:41 GMT
RUN cp /usr/share/java/postgresql-jdbc4.jar /usr/local/tomcat/webapps/ROOT/WEB-INF/lib/
# Tue, 31 Jan 2023 00:54:41 GMT
COPY file:0a1be11e2eb610a1dbcd415404e3a592641110b93090030cb831e3a19a163017 in /usr/local/tomcat/bin/ 
# Tue, 31 Jan 2023 00:54:41 GMT
COPY file:4a923f484bb29a26630c19e1d617d3bf6aa6ae7c6c4a5561e97b037bcde0847c in /usr/local/tomcat/webapps/ROOT/WEB-INF/hibernate.cfg.xml 
# Tue, 31 Jan 2023 00:54:42 GMT
RUN sed -i 's/<id>org.xwiki.platform:xwiki-platform-distribution-war/<id>org.xwiki.platform:xwiki-platform-distribution-docker/'   /usr/local/tomcat/webapps/ROOT/META-INF/extension.xed
# Tue, 31 Jan 2023 00:54:42 GMT
COPY file:a47c4dcd87c9dad97aff38c49188357e6193bcad50757e516cfb08a60d4de611 in /usr/local/bin/docker-entrypoint.sh 
# Tue, 31 Jan 2023 00:54:42 GMT
VOLUME [/usr/local/xwiki]
# Tue, 31 Jan 2023 00:54:42 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 31 Jan 2023 00:54:42 GMT
CMD ["xwiki"]
```

-	Layers:
	-	`sha256:0509fae36eb0656f8bdb23f8ae64100d893bcea2563e97468d337e04d2d0410b`  
		Last Modified: Wed, 02 Nov 2022 18:50:21 GMT  
		Size: 28.4 MB (28382154 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e502a1af2bcd98f5f0d2f5e4da1a0e7bbe07a2c548e2662f7d37dce5ae1df46c`  
		Last Modified: Wed, 02 Nov 2022 19:48:28 GMT  
		Size: 12.4 MB (12396330 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bc4598c07dd818f03a0378b0341a4a8e80f0152fbb3e7d5246ca4f466f42e611`  
		Last Modified: Fri, 04 Nov 2022 22:46:46 GMT  
		Size: 45.0 MB (44958470 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:715a937a1066f998b331fcd62256ad01a5571bdf46804e97825afc64f9ebb427`  
		Last Modified: Fri, 04 Nov 2022 22:46:41 GMT  
		Size: 160.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5fb623f082f74b2fa9fc2c4e3f3a4802875cb9753cfa26ed940201ce72bb56cb`  
		Last Modified: Sat, 05 Nov 2022 00:03:40 GMT  
		Size: 172.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:33260b83200262bbd546be371ad3c1f50f5ae7228afb87982d6fa9d6b11bf26f`  
		Last Modified: Tue, 15 Nov 2022 05:10:19 GMT  
		Size: 12.2 MB (12207235 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0955fb697ea9b30a1b4f95385464f646aa1525cb6efba648e22df84ebef6b2ee`  
		Last Modified: Tue, 15 Nov 2022 05:10:18 GMT  
		Size: 452.0 KB (452021 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6eddcf66f2083b1487296a0308e0b058917c97f614f12428d82d89662038dc2e`  
		Last Modified: Tue, 15 Nov 2022 05:10:18 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1ae6a8fce0f2cd131007393c1a4eba9ce9d0501da8406af5c5ce9deb5dc187b8`  
		Last Modified: Wed, 11 Jan 2023 03:12:13 GMT  
		Size: 174.7 MB (174749274 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5351c17af011e98fdd3db4781945e719f390748d66dc50d28bef46bb2d6b6418`  
		Last Modified: Tue, 31 Jan 2023 00:56:53 GMT  
		Size: 307.1 MB (307117134 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6b632a2f6afda42ce5dc291920d8f03e04b69034e314687eb551be8eafedd92d`  
		Last Modified: Tue, 31 Jan 2023 00:56:38 GMT  
		Size: 936.9 KB (936854 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cbd6cbb6ae05692db55d5e4f46142d2e20e051631dc2fc44e5b20d3316143305`  
		Last Modified: Tue, 31 Jan 2023 00:56:38 GMT  
		Size: 1.3 KB (1348 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ceb1d88f8fd44412961c0db372cd86a999c6b2619ce80a916a4fe8ca0e63acc9`  
		Last Modified: Tue, 31 Jan 2023 00:56:38 GMT  
		Size: 2.5 KB (2458 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8d0ee5cad12d41a6d530031aabd4a92619995eb0ee20dcd24d2bb9aec6a694db`  
		Last Modified: Tue, 31 Jan 2023 00:56:38 GMT  
		Size: 6.0 KB (6006 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3c980b95519f007aea60be042d36cd33de21e6265aed0e443c5ecf9bb1f40980`  
		Last Modified: Tue, 31 Jan 2023 00:56:38 GMT  
		Size: 2.5 KB (2505 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `xwiki:stable-postgres-tomcat`

```console
$ docker pull xwiki@sha256:f6739c1133cbbece87973ddea5fbc57222abb9d7d3f8064eee9d2c2c0d46ecfa
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `xwiki:stable-postgres-tomcat` - linux; amd64

```console
$ docker pull xwiki@sha256:72928baeace929e42f17f01362700392a90c6750b2ec1f84f24bbba1c4ff0236
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **590.0 MB (589959353 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b71f03d7d3a1760e73e6f4370f49317d16a7e0cb22532f49c11c0ee73b2c6262`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["xwiki"]`

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
# Wed, 02 Nov 2022 18:44:10 GMT
RUN apt-get update     && DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends tzdata curl wget ca-certificates fontconfig locales     && echo "en_US.UTF-8 UTF-8" >> /etc/locale.gen     && locale-gen en_US.UTF-8     && rm -rf /var/lib/apt/lists/*
# Fri, 04 Nov 2022 23:21:41 GMT
ENV JAVA_VERSION=jdk-11.0.17+8
# Fri, 04 Nov 2022 23:22:31 GMT
RUN set -eux;     ARCH="$(dpkg --print-architecture)";     case "${ARCH}" in        aarch64|arm64)          ESUM='bd6efe3290c8b5a42f695a55a26f3e3c9c284288574879d4b7089f31f5114177';          BINARY_URL='https://github.com/adoptium/temurin11-binaries/releases/download/jdk-11.0.17%2B8/OpenJDK11U-jre_aarch64_linux_hotspot_11.0.17_8.tar.gz';          ;;        armhf|arm)          ESUM='8cf113d3d7fa808895c8d2e41bb890af21c47e38c2460e0588147a4bb8fc658d';          BINARY_URL='https://github.com/adoptium/temurin11-binaries/releases/download/jdk-11.0.17%2B8/OpenJDK11U-jre_arm_linux_hotspot_11.0.17_8.tar.gz';          ;;        ppc64el|powerpc:common64)          ESUM='0ca3d806131ab5834c501f9c625bb0248cd528af361c704503348e9c9605bedf';          BINARY_URL='https://github.com/adoptium/temurin11-binaries/releases/download/jdk-11.0.17%2B8/OpenJDK11U-jre_ppc64le_linux_hotspot_11.0.17_8.tar.gz';          ;;        s390x|s390:64-bit)          ESUM='dd3b159a374086e65cb07c4ccb226c90f9c02ef929cba6f0b642171d7ed97fa4';          BINARY_URL='https://github.com/adoptium/temurin11-binaries/releases/download/jdk-11.0.17%2B8/OpenJDK11U-jre_s390x_linux_hotspot_11.0.17_8.tar.gz';          ;;        amd64|i386:x86-64)          ESUM='752616097e09d7f60a3ad8bd312f90eaf50ac72577e55df229fe6e8091148f79';          BINARY_URL='https://github.com/adoptium/temurin11-binaries/releases/download/jdk-11.0.17%2B8/OpenJDK11U-jre_x64_linux_hotspot_11.0.17_8.tar.gz';          ;;        *)          echo "Unsupported arch: ${ARCH}";          exit 1;          ;;     esac; 	  wget -O /tmp/openjdk.tar.gz ${BINARY_URL}; 	  echo "${ESUM} */tmp/openjdk.tar.gz" | sha256sum -c -; 	  mkdir -p "$JAVA_HOME"; 	  tar --extract 	      --file /tmp/openjdk.tar.gz 	      --directory "$JAVA_HOME" 	      --strip-components 1 	      --no-same-owner 	  ;     rm /tmp/openjdk.tar.gz;     find "$JAVA_HOME/lib" -name '*.so' -exec dirname '{}' ';' | sort -u > /etc/ld.so.conf.d/docker-openjdk.conf;     ldconfig;     java -Xshare:dump;
# Fri, 04 Nov 2022 23:22:32 GMT
RUN echo Verifying install ...     && fileEncoding="$(echo 'System.out.println(System.getProperty("file.encoding"))' | jshell -s -)"; [ "$fileEncoding" = 'UTF-8' ]; rm -rf ~/.java     && echo java --version && java --version     && echo Complete.
# Sat, 05 Nov 2022 01:35:16 GMT
ENV CATALINA_HOME=/usr/local/tomcat
# Sat, 05 Nov 2022 01:35:16 GMT
ENV PATH=/usr/local/tomcat/bin:/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Sat, 05 Nov 2022 01:35:17 GMT
RUN mkdir -p "$CATALINA_HOME"
# Sat, 05 Nov 2022 01:35:17 GMT
WORKDIR /usr/local/tomcat
# Sat, 05 Nov 2022 01:35:17 GMT
ENV TOMCAT_NATIVE_LIBDIR=/usr/local/tomcat/native-jni-lib
# Sat, 05 Nov 2022 01:35:17 GMT
ENV LD_LIBRARY_PATH=/usr/local/tomcat/native-jni-lib
# Sat, 05 Nov 2022 01:39:54 GMT
ENV GPG_KEYS=48F8E69F6390C9F25CFEDCD268248959359E722B A9C5DF4D22E99998D9875A5110C01C5A2F6059E7 DCFD35E0BF8CA7344752DE8B6FB21E8933C60243
# Sat, 05 Nov 2022 01:39:54 GMT
ENV TOMCAT_MAJOR=9
# Tue, 15 Nov 2022 03:06:43 GMT
ENV TOMCAT_VERSION=9.0.69
# Tue, 15 Nov 2022 03:06:43 GMT
ENV TOMCAT_SHA512=8c883c54ce9ce43eba37756a6404cdf3477879883a3e6d146dc8a7aa5e0425f487466afe6b6da4a895927cb7cb59177b9379cec18000f2de12785be57408c779
# Tue, 15 Nov 2022 03:06:44 GMT
COPY dir:b1a33aa3993dbbfbebb33bd9aa546b60c2f2191abf1227f453d4e830f6deb35f in /usr/local/tomcat 
# Tue, 15 Nov 2022 03:06:48 GMT
RUN set -eux; 	apt-get update; 	xargs -rt apt-get install -y --no-install-recommends < "$TOMCAT_NATIVE_LIBDIR/.dependencies.txt"; 	rm -rf /var/lib/apt/lists/*
# Tue, 15 Nov 2022 03:06:49 GMT
RUN set -eux; 	nativeLines="$(catalina.sh configtest 2>&1)"; 	nativeLines="$(echo "$nativeLines" | grep 'Apache Tomcat Native')"; 	nativeLines="$(echo "$nativeLines" | sort -u)"; 	if ! echo "$nativeLines" | grep -E 'INFO: Loaded( APR based)? Apache Tomcat Native library' >&2; then 		echo >&2 "$nativeLines"; 		exit 1; 	fi
# Tue, 15 Nov 2022 03:06:49 GMT
EXPOSE 8080
# Tue, 15 Nov 2022 03:06:49 GMT
CMD ["catalina.sh" "run"]
# Wed, 11 Jan 2023 02:47:03 GMT
LABEL org.opencontainers.image.authors=XWiki Development Team <committers@xwiki.org>
# Wed, 11 Jan 2023 02:47:03 GMT
LABEL org.opencontainers.image.url=https://hub.docker.com/_/xwiki
# Wed, 11 Jan 2023 02:47:03 GMT
LABEL org.opencontainers.image.documentation=https://hub.docker.com/_/xwiki
# Wed, 11 Jan 2023 02:47:03 GMT
LABEL org.opencontainers.image.source=https://github.com/xwiki/xwiki-docker.git
# Wed, 11 Jan 2023 02:47:04 GMT
LABEL org.opencontainers.image.vendor=xwiki.org
# Wed, 11 Jan 2023 02:47:04 GMT
LABEL org.opencontainers.image.licenses=LGPL-2.1
# Wed, 11 Jan 2023 02:50:25 GMT
RUN apt-get update &&   apt-get --no-install-recommends -y install     curl     libreoffice     unzip     procps     libpostgresql-jdbc-java &&   rm -rf /var/lib/apt/lists/*
# Tue, 31 Jan 2023 00:21:26 GMT
ENV XWIKI_VERSION=15.0
# Tue, 31 Jan 2023 00:21:27 GMT
ENV XWIKI_URL_PREFIX=https://maven.xwiki.org/releases/org/xwiki/platform/xwiki-platform-distribution-war/15.0
# Tue, 31 Jan 2023 00:21:27 GMT
ENV XWIKI_DOWNLOAD_SHA256=79ba0f479bbc49521c113821adc9d91141075a9470d7f9bbb6994ca59c30d121
# Tue, 31 Jan 2023 00:22:39 GMT
RUN rm -rf /usr/local/tomcat/webapps/* &&   mkdir -p /usr/local/tomcat/temp &&   mkdir -p /usr/local/xwiki/data &&   curl -fSL "${XWIKI_URL_PREFIX}/xwiki-platform-distribution-war-${XWIKI_VERSION}.war" -o xwiki.war &&   echo "$XWIKI_DOWNLOAD_SHA256 xwiki.war" | sha256sum -c - &&   unzip -d /usr/local/tomcat/webapps/ROOT xwiki.war &&   rm -f xwiki.war
# Tue, 31 Jan 2023 00:22:40 GMT
RUN cp /usr/share/java/postgresql-jdbc4.jar /usr/local/tomcat/webapps/ROOT/WEB-INF/lib/
# Tue, 31 Jan 2023 00:22:41 GMT
COPY file:0a1be11e2eb610a1dbcd415404e3a592641110b93090030cb831e3a19a163017 in /usr/local/tomcat/bin/ 
# Tue, 31 Jan 2023 00:22:41 GMT
COPY file:4a923f484bb29a26630c19e1d617d3bf6aa6ae7c6c4a5561e97b037bcde0847c in /usr/local/tomcat/webapps/ROOT/WEB-INF/hibernate.cfg.xml 
# Tue, 31 Jan 2023 00:22:41 GMT
RUN sed -i 's/<id>org.xwiki.platform:xwiki-platform-distribution-war/<id>org.xwiki.platform:xwiki-platform-distribution-docker/'   /usr/local/tomcat/webapps/ROOT/META-INF/extension.xed
# Tue, 31 Jan 2023 00:22:41 GMT
COPY file:a47c4dcd87c9dad97aff38c49188357e6193bcad50757e516cfb08a60d4de611 in /usr/local/bin/docker-entrypoint.sh 
# Tue, 31 Jan 2023 00:22:41 GMT
VOLUME [/usr/local/xwiki]
# Tue, 31 Jan 2023 00:22:42 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 31 Jan 2023 00:22:42 GMT
CMD ["xwiki"]
```

-	Layers:
	-	`sha256:e96e057aae67380a4ddb16c337c5c3669d97fdff69ec537f02aa2cc30d814281`  
		Last Modified: Wed, 02 Nov 2022 03:03:36 GMT  
		Size: 30.4 MB (30425607 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4ced2591451da3a02e2b6bb44752b9e3f00d77789921be4df5082fb9f9880ad0`  
		Last Modified: Wed, 02 Nov 2022 18:48:43 GMT  
		Size: 12.4 MB (12439006 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:df8f874ae8c08a9e69e5fbe6c5a64200a45386132a3203d1a9a7f1146d94cfbc`  
		Last Modified: Fri, 04 Nov 2022 23:29:33 GMT  
		Size: 46.6 MB (46629936 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:111b6c7486426c4b6989102c2ee5be856e8a58e20ab0a350b24a905d536e8e7f`  
		Last Modified: Fri, 04 Nov 2022 23:29:26 GMT  
		Size: 161.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e6f84dce457c6d4f7b7291fce05f8e77998a3a7722a54125a1f1d52ca83043b4`  
		Last Modified: Sat, 05 Nov 2022 01:50:51 GMT  
		Size: 173.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a6c26749ee782392e38845ee2ba79b0da586ef6a45d8e7f29c7af14612278547`  
		Last Modified: Tue, 15 Nov 2022 03:19:57 GMT  
		Size: 12.2 MB (12200249 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4dddc6d9fa6024025b3fcfe729cab2dc544fb25476eca6e80b1af8e8d93bb0ee`  
		Last Modified: Tue, 15 Nov 2022 03:19:56 GMT  
		Size: 452.7 KB (452680 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:06637eebe5e72c8ad9019ad4eb4cdde1f11f7d4c24c7ed7374cf8966343aa2fb`  
		Last Modified: Tue, 15 Nov 2022 03:19:56 GMT  
		Size: 131.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b57f6f8bcfb0d93b8e21d3068d1f65d3f08dba05c5fab7d4c36e2359317b18c7`  
		Last Modified: Wed, 11 Jan 2023 02:53:53 GMT  
		Size: 179.7 MB (179745182 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:71a0aee972ff5a36a4c5d67f5bf6416b1b78d06c906ce727c5e8e11098d0dfd1`  
		Last Modified: Tue, 31 Jan 2023 00:25:01 GMT  
		Size: 307.1 MB (307117070 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ccc745f1273896cef68a5af6cd5713c4a2d8704628920a53e318a008f8096426`  
		Last Modified: Tue, 31 Jan 2023 00:24:44 GMT  
		Size: 936.8 KB (936848 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1593979548bc568ed36dc9f5adb8f00d8b7d3eb1fa850fc06426c2c9345b8472`  
		Last Modified: Tue, 31 Jan 2023 00:24:43 GMT  
		Size: 1.3 KB (1345 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e1e58b32c2c2a52907f7e4ad05462d3b2afd11404a9678bc656fb96029b12d8d`  
		Last Modified: Tue, 31 Jan 2023 00:24:43 GMT  
		Size: 2.5 KB (2454 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c43ce01c7b867ce6cda62f86175ba6a53f44000797d61fe604aded86980c4d41`  
		Last Modified: Tue, 31 Jan 2023 00:24:43 GMT  
		Size: 6.0 KB (6006 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6fe6f306aa61d9839a01e62f4c308a9a7d3bd4cd5ce9a58407b6585f6950f054`  
		Last Modified: Tue, 31 Jan 2023 00:24:43 GMT  
		Size: 2.5 KB (2505 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `xwiki:stable-postgres-tomcat` - linux; arm64 variant v8

```console
$ docker pull xwiki@sha256:ae51c629c7a76aa7c15ebb33fcfdae3e529ef6456ada6d0dbcf9ed8fc5ecf00d
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **581.2 MB (581212250 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:70277ae3ffdca68401bb57e24e6302cc64a403bf36869f0959e54d03216b0005`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["xwiki"]`

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
# Wed, 02 Nov 2022 19:44:32 GMT
RUN apt-get update     && DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends tzdata curl wget ca-certificates fontconfig locales     && echo "en_US.UTF-8 UTF-8" >> /etc/locale.gen     && locale-gen en_US.UTF-8     && rm -rf /var/lib/apt/lists/*
# Fri, 04 Nov 2022 22:40:54 GMT
ENV JAVA_VERSION=jdk-11.0.17+8
# Fri, 04 Nov 2022 22:41:33 GMT
RUN set -eux;     ARCH="$(dpkg --print-architecture)";     case "${ARCH}" in        aarch64|arm64)          ESUM='bd6efe3290c8b5a42f695a55a26f3e3c9c284288574879d4b7089f31f5114177';          BINARY_URL='https://github.com/adoptium/temurin11-binaries/releases/download/jdk-11.0.17%2B8/OpenJDK11U-jre_aarch64_linux_hotspot_11.0.17_8.tar.gz';          ;;        armhf|arm)          ESUM='8cf113d3d7fa808895c8d2e41bb890af21c47e38c2460e0588147a4bb8fc658d';          BINARY_URL='https://github.com/adoptium/temurin11-binaries/releases/download/jdk-11.0.17%2B8/OpenJDK11U-jre_arm_linux_hotspot_11.0.17_8.tar.gz';          ;;        ppc64el|powerpc:common64)          ESUM='0ca3d806131ab5834c501f9c625bb0248cd528af361c704503348e9c9605bedf';          BINARY_URL='https://github.com/adoptium/temurin11-binaries/releases/download/jdk-11.0.17%2B8/OpenJDK11U-jre_ppc64le_linux_hotspot_11.0.17_8.tar.gz';          ;;        s390x|s390:64-bit)          ESUM='dd3b159a374086e65cb07c4ccb226c90f9c02ef929cba6f0b642171d7ed97fa4';          BINARY_URL='https://github.com/adoptium/temurin11-binaries/releases/download/jdk-11.0.17%2B8/OpenJDK11U-jre_s390x_linux_hotspot_11.0.17_8.tar.gz';          ;;        amd64|i386:x86-64)          ESUM='752616097e09d7f60a3ad8bd312f90eaf50ac72577e55df229fe6e8091148f79';          BINARY_URL='https://github.com/adoptium/temurin11-binaries/releases/download/jdk-11.0.17%2B8/OpenJDK11U-jre_x64_linux_hotspot_11.0.17_8.tar.gz';          ;;        *)          echo "Unsupported arch: ${ARCH}";          exit 1;          ;;     esac; 	  wget -O /tmp/openjdk.tar.gz ${BINARY_URL}; 	  echo "${ESUM} */tmp/openjdk.tar.gz" | sha256sum -c -; 	  mkdir -p "$JAVA_HOME"; 	  tar --extract 	      --file /tmp/openjdk.tar.gz 	      --directory "$JAVA_HOME" 	      --strip-components 1 	      --no-same-owner 	  ;     rm /tmp/openjdk.tar.gz;     find "$JAVA_HOME/lib" -name '*.so' -exec dirname '{}' ';' | sort -u > /etc/ld.so.conf.d/docker-openjdk.conf;     ldconfig;     java -Xshare:dump;
# Fri, 04 Nov 2022 22:41:34 GMT
RUN echo Verifying install ...     && fileEncoding="$(echo 'System.out.println(System.getProperty("file.encoding"))' | jshell -s -)"; [ "$fileEncoding" = 'UTF-8' ]; rm -rf ~/.java     && echo java --version && java --version     && echo Complete.
# Fri, 04 Nov 2022 23:48:38 GMT
ENV CATALINA_HOME=/usr/local/tomcat
# Fri, 04 Nov 2022 23:48:38 GMT
ENV PATH=/usr/local/tomcat/bin:/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Fri, 04 Nov 2022 23:48:38 GMT
RUN mkdir -p "$CATALINA_HOME"
# Fri, 04 Nov 2022 23:48:39 GMT
WORKDIR /usr/local/tomcat
# Fri, 04 Nov 2022 23:48:39 GMT
ENV TOMCAT_NATIVE_LIBDIR=/usr/local/tomcat/native-jni-lib
# Fri, 04 Nov 2022 23:48:39 GMT
ENV LD_LIBRARY_PATH=/usr/local/tomcat/native-jni-lib
# Fri, 04 Nov 2022 23:53:12 GMT
ENV GPG_KEYS=48F8E69F6390C9F25CFEDCD268248959359E722B A9C5DF4D22E99998D9875A5110C01C5A2F6059E7 DCFD35E0BF8CA7344752DE8B6FB21E8933C60243
# Fri, 04 Nov 2022 23:53:12 GMT
ENV TOMCAT_MAJOR=9
# Tue, 15 Nov 2022 04:57:22 GMT
ENV TOMCAT_VERSION=9.0.69
# Tue, 15 Nov 2022 04:57:22 GMT
ENV TOMCAT_SHA512=8c883c54ce9ce43eba37756a6404cdf3477879883a3e6d146dc8a7aa5e0425f487466afe6b6da4a895927cb7cb59177b9379cec18000f2de12785be57408c779
# Tue, 15 Nov 2022 04:57:22 GMT
COPY dir:096b403a5f78b17e6b4bff63128a9c93941b97f22470991610dd641633d977f1 in /usr/local/tomcat 
# Tue, 15 Nov 2022 04:57:25 GMT
RUN set -eux; 	apt-get update; 	xargs -rt apt-get install -y --no-install-recommends < "$TOMCAT_NATIVE_LIBDIR/.dependencies.txt"; 	rm -rf /var/lib/apt/lists/*
# Tue, 15 Nov 2022 04:57:26 GMT
RUN set -eux; 	nativeLines="$(catalina.sh configtest 2>&1)"; 	nativeLines="$(echo "$nativeLines" | grep 'Apache Tomcat Native')"; 	nativeLines="$(echo "$nativeLines" | sort -u)"; 	if ! echo "$nativeLines" | grep -E 'INFO: Loaded( APR based)? Apache Tomcat Native library' >&2; then 		echo >&2 "$nativeLines"; 		exit 1; 	fi
# Tue, 15 Nov 2022 04:57:26 GMT
EXPOSE 8080
# Tue, 15 Nov 2022 04:57:27 GMT
CMD ["catalina.sh" "run"]
# Wed, 11 Jan 2023 03:05:10 GMT
LABEL org.opencontainers.image.authors=XWiki Development Team <committers@xwiki.org>
# Wed, 11 Jan 2023 03:05:10 GMT
LABEL org.opencontainers.image.url=https://hub.docker.com/_/xwiki
# Wed, 11 Jan 2023 03:05:10 GMT
LABEL org.opencontainers.image.documentation=https://hub.docker.com/_/xwiki
# Wed, 11 Jan 2023 03:05:10 GMT
LABEL org.opencontainers.image.source=https://github.com/xwiki/xwiki-docker.git
# Wed, 11 Jan 2023 03:05:11 GMT
LABEL org.opencontainers.image.vendor=xwiki.org
# Wed, 11 Jan 2023 03:05:11 GMT
LABEL org.opencontainers.image.licenses=LGPL-2.1
# Wed, 11 Jan 2023 03:08:55 GMT
RUN apt-get update &&   apt-get --no-install-recommends -y install     curl     libreoffice     unzip     procps     libpostgresql-jdbc-java &&   rm -rf /var/lib/apt/lists/*
# Tue, 31 Jan 2023 00:48:10 GMT
ENV XWIKI_VERSION=15.0
# Tue, 31 Jan 2023 00:48:10 GMT
ENV XWIKI_URL_PREFIX=https://maven.xwiki.org/releases/org/xwiki/platform/xwiki-platform-distribution-war/15.0
# Tue, 31 Jan 2023 00:48:10 GMT
ENV XWIKI_DOWNLOAD_SHA256=79ba0f479bbc49521c113821adc9d91141075a9470d7f9bbb6994ca59c30d121
# Tue, 31 Jan 2023 00:54:38 GMT
RUN rm -rf /usr/local/tomcat/webapps/* &&   mkdir -p /usr/local/tomcat/temp &&   mkdir -p /usr/local/xwiki/data &&   curl -fSL "${XWIKI_URL_PREFIX}/xwiki-platform-distribution-war-${XWIKI_VERSION}.war" -o xwiki.war &&   echo "$XWIKI_DOWNLOAD_SHA256 xwiki.war" | sha256sum -c - &&   unzip -d /usr/local/tomcat/webapps/ROOT xwiki.war &&   rm -f xwiki.war
# Tue, 31 Jan 2023 00:54:41 GMT
RUN cp /usr/share/java/postgresql-jdbc4.jar /usr/local/tomcat/webapps/ROOT/WEB-INF/lib/
# Tue, 31 Jan 2023 00:54:41 GMT
COPY file:0a1be11e2eb610a1dbcd415404e3a592641110b93090030cb831e3a19a163017 in /usr/local/tomcat/bin/ 
# Tue, 31 Jan 2023 00:54:41 GMT
COPY file:4a923f484bb29a26630c19e1d617d3bf6aa6ae7c6c4a5561e97b037bcde0847c in /usr/local/tomcat/webapps/ROOT/WEB-INF/hibernate.cfg.xml 
# Tue, 31 Jan 2023 00:54:42 GMT
RUN sed -i 's/<id>org.xwiki.platform:xwiki-platform-distribution-war/<id>org.xwiki.platform:xwiki-platform-distribution-docker/'   /usr/local/tomcat/webapps/ROOT/META-INF/extension.xed
# Tue, 31 Jan 2023 00:54:42 GMT
COPY file:a47c4dcd87c9dad97aff38c49188357e6193bcad50757e516cfb08a60d4de611 in /usr/local/bin/docker-entrypoint.sh 
# Tue, 31 Jan 2023 00:54:42 GMT
VOLUME [/usr/local/xwiki]
# Tue, 31 Jan 2023 00:54:42 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 31 Jan 2023 00:54:42 GMT
CMD ["xwiki"]
```

-	Layers:
	-	`sha256:0509fae36eb0656f8bdb23f8ae64100d893bcea2563e97468d337e04d2d0410b`  
		Last Modified: Wed, 02 Nov 2022 18:50:21 GMT  
		Size: 28.4 MB (28382154 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e502a1af2bcd98f5f0d2f5e4da1a0e7bbe07a2c548e2662f7d37dce5ae1df46c`  
		Last Modified: Wed, 02 Nov 2022 19:48:28 GMT  
		Size: 12.4 MB (12396330 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bc4598c07dd818f03a0378b0341a4a8e80f0152fbb3e7d5246ca4f466f42e611`  
		Last Modified: Fri, 04 Nov 2022 22:46:46 GMT  
		Size: 45.0 MB (44958470 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:715a937a1066f998b331fcd62256ad01a5571bdf46804e97825afc64f9ebb427`  
		Last Modified: Fri, 04 Nov 2022 22:46:41 GMT  
		Size: 160.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5fb623f082f74b2fa9fc2c4e3f3a4802875cb9753cfa26ed940201ce72bb56cb`  
		Last Modified: Sat, 05 Nov 2022 00:03:40 GMT  
		Size: 172.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:33260b83200262bbd546be371ad3c1f50f5ae7228afb87982d6fa9d6b11bf26f`  
		Last Modified: Tue, 15 Nov 2022 05:10:19 GMT  
		Size: 12.2 MB (12207235 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0955fb697ea9b30a1b4f95385464f646aa1525cb6efba648e22df84ebef6b2ee`  
		Last Modified: Tue, 15 Nov 2022 05:10:18 GMT  
		Size: 452.0 KB (452021 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6eddcf66f2083b1487296a0308e0b058917c97f614f12428d82d89662038dc2e`  
		Last Modified: Tue, 15 Nov 2022 05:10:18 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1ae6a8fce0f2cd131007393c1a4eba9ce9d0501da8406af5c5ce9deb5dc187b8`  
		Last Modified: Wed, 11 Jan 2023 03:12:13 GMT  
		Size: 174.7 MB (174749274 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5351c17af011e98fdd3db4781945e719f390748d66dc50d28bef46bb2d6b6418`  
		Last Modified: Tue, 31 Jan 2023 00:56:53 GMT  
		Size: 307.1 MB (307117134 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6b632a2f6afda42ce5dc291920d8f03e04b69034e314687eb551be8eafedd92d`  
		Last Modified: Tue, 31 Jan 2023 00:56:38 GMT  
		Size: 936.9 KB (936854 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cbd6cbb6ae05692db55d5e4f46142d2e20e051631dc2fc44e5b20d3316143305`  
		Last Modified: Tue, 31 Jan 2023 00:56:38 GMT  
		Size: 1.3 KB (1348 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ceb1d88f8fd44412961c0db372cd86a999c6b2619ce80a916a4fe8ca0e63acc9`  
		Last Modified: Tue, 31 Jan 2023 00:56:38 GMT  
		Size: 2.5 KB (2458 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8d0ee5cad12d41a6d530031aabd4a92619995eb0ee20dcd24d2bb9aec6a694db`  
		Last Modified: Tue, 31 Jan 2023 00:56:38 GMT  
		Size: 6.0 KB (6006 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3c980b95519f007aea60be042d36cd33de21e6265aed0e443c5ecf9bb1f40980`  
		Last Modified: Tue, 31 Jan 2023 00:56:38 GMT  
		Size: 2.5 KB (2505 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
