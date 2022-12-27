## `xwiki:lts-mysql-tomcat`

```console
$ docker pull xwiki@sha256:9611ce52dad0bad32969abf304ee60ff1731cd76dfe9ee6e9490292280345e33
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `xwiki:lts-mysql-tomcat` - linux; amd64

```console
$ docker pull xwiki@sha256:56577b16a4418543f9a3b77b51c1f9f693348680fa3d343a2d085a37db0825e2
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **589.9 MB (589855408 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b14ec210c955b150a310546416abadce10ee857e899412d22bc45a0b6e5cff7e`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["xwiki"]`

```dockerfile
# Fri, 09 Dec 2022 01:20:30 GMT
ADD file:481dd2da6de71525248eba186feeeafcc73cc956ade0a196a4e8b0c2424e74b9 in / 
# Fri, 09 Dec 2022 01:20:31 GMT
CMD ["bash"]
# Fri, 09 Dec 2022 01:42:58 GMT
ENV JAVA_HOME=/opt/java/openjdk
# Fri, 09 Dec 2022 01:42:58 GMT
ENV PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Fri, 09 Dec 2022 01:42:58 GMT
ENV LANG=en_US.UTF-8 LANGUAGE=en_US:en LC_ALL=en_US.UTF-8
# Fri, 09 Dec 2022 01:43:29 GMT
RUN apt-get update     && DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends tzdata curl wget ca-certificates fontconfig locales     && echo "en_US.UTF-8 UTF-8" >> /etc/locale.gen     && locale-gen en_US.UTF-8     && rm -rf /var/lib/apt/lists/*
# Fri, 09 Dec 2022 01:44:23 GMT
ENV JAVA_VERSION=jdk-11.0.17+8
# Fri, 09 Dec 2022 01:44:54 GMT
RUN set -eux;     ARCH="$(dpkg --print-architecture)";     case "${ARCH}" in        aarch64|arm64)          ESUM='bd6efe3290c8b5a42f695a55a26f3e3c9c284288574879d4b7089f31f5114177';          BINARY_URL='https://github.com/adoptium/temurin11-binaries/releases/download/jdk-11.0.17%2B8/OpenJDK11U-jre_aarch64_linux_hotspot_11.0.17_8.tar.gz';          ;;        armhf|arm)          ESUM='8cf113d3d7fa808895c8d2e41bb890af21c47e38c2460e0588147a4bb8fc658d';          BINARY_URL='https://github.com/adoptium/temurin11-binaries/releases/download/jdk-11.0.17%2B8/OpenJDK11U-jre_arm_linux_hotspot_11.0.17_8.tar.gz';          ;;        ppc64el|powerpc:common64)          ESUM='0ca3d806131ab5834c501f9c625bb0248cd528af361c704503348e9c9605bedf';          BINARY_URL='https://github.com/adoptium/temurin11-binaries/releases/download/jdk-11.0.17%2B8/OpenJDK11U-jre_ppc64le_linux_hotspot_11.0.17_8.tar.gz';          ;;        s390x|s390:64-bit)          ESUM='dd3b159a374086e65cb07c4ccb226c90f9c02ef929cba6f0b642171d7ed97fa4';          BINARY_URL='https://github.com/adoptium/temurin11-binaries/releases/download/jdk-11.0.17%2B8/OpenJDK11U-jre_s390x_linux_hotspot_11.0.17_8.tar.gz';          ;;        amd64|i386:x86-64)          ESUM='752616097e09d7f60a3ad8bd312f90eaf50ac72577e55df229fe6e8091148f79';          BINARY_URL='https://github.com/adoptium/temurin11-binaries/releases/download/jdk-11.0.17%2B8/OpenJDK11U-jre_x64_linux_hotspot_11.0.17_8.tar.gz';          ;;        *)          echo "Unsupported arch: ${ARCH}";          exit 1;          ;;     esac; 	  wget -O /tmp/openjdk.tar.gz ${BINARY_URL}; 	  echo "${ESUM} */tmp/openjdk.tar.gz" | sha256sum -c -; 	  mkdir -p "$JAVA_HOME"; 	  tar --extract 	      --file /tmp/openjdk.tar.gz 	      --directory "$JAVA_HOME" 	      --strip-components 1 	      --no-same-owner 	  ;     rm /tmp/openjdk.tar.gz;     find "$JAVA_HOME/lib" -name '*.so' -exec dirname '{}' ';' | sort -u > /etc/ld.so.conf.d/docker-openjdk.conf;     ldconfig;     java -Xshare:dump;
# Fri, 09 Dec 2022 01:44:55 GMT
RUN echo Verifying install ...     && fileEncoding="$(echo 'System.out.println(System.getProperty("file.encoding"))' | jshell -s -)"; [ "$fileEncoding" = 'UTF-8' ]; rm -rf ~/.java     && echo java --version && java --version     && echo Complete.
# Fri, 09 Dec 2022 07:42:48 GMT
ENV CATALINA_HOME=/usr/local/tomcat
# Fri, 09 Dec 2022 07:42:48 GMT
ENV PATH=/usr/local/tomcat/bin:/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Fri, 09 Dec 2022 07:42:49 GMT
RUN mkdir -p "$CATALINA_HOME"
# Fri, 09 Dec 2022 07:42:49 GMT
WORKDIR /usr/local/tomcat
# Fri, 09 Dec 2022 07:42:49 GMT
ENV TOMCAT_NATIVE_LIBDIR=/usr/local/tomcat/native-jni-lib
# Fri, 09 Dec 2022 07:42:49 GMT
ENV LD_LIBRARY_PATH=/usr/local/tomcat/native-jni-lib
# Fri, 09 Dec 2022 07:51:45 GMT
ENV GPG_KEYS=48F8E69F6390C9F25CFEDCD268248959359E722B A9C5DF4D22E99998D9875A5110C01C5A2F6059E7 DCFD35E0BF8CA7344752DE8B6FB21E8933C60243
# Fri, 09 Dec 2022 07:51:45 GMT
ENV TOMCAT_MAJOR=9
# Fri, 09 Dec 2022 07:51:45 GMT
ENV TOMCAT_VERSION=9.0.70
# Fri, 09 Dec 2022 07:51:45 GMT
ENV TOMCAT_SHA512=9b57b332f4cfb2c4b9250b95924314507ebafec44f732e755be96d35e1a50d98ca3ea11a8c62e0c6fde2541d31a981f5ca792ea9931b2551b81b495932474726
# Fri, 09 Dec 2022 07:51:46 GMT
COPY dir:ad3e3615457fca7eb47012da062f283055daf509419afb3f97fe80052570f492 in /usr/local/tomcat 
# Fri, 09 Dec 2022 07:51:50 GMT
RUN set -eux; 	apt-get update; 	xargs -rt apt-get install -y --no-install-recommends < "$TOMCAT_NATIVE_LIBDIR/.dependencies.txt"; 	rm -rf /var/lib/apt/lists/*
# Fri, 09 Dec 2022 07:51:51 GMT
RUN set -eux; 	nativeLines="$(catalina.sh configtest 2>&1)"; 	nativeLines="$(echo "$nativeLines" | grep 'Apache Tomcat Native')"; 	nativeLines="$(echo "$nativeLines" | sort -u)"; 	if ! echo "$nativeLines" | grep -E 'INFO: Loaded( APR based)? Apache Tomcat Native library' >&2; then 		echo >&2 "$nativeLines"; 		exit 1; 	fi
# Fri, 09 Dec 2022 07:51:51 GMT
EXPOSE 8080
# Fri, 09 Dec 2022 07:51:51 GMT
CMD ["catalina.sh" "run"]
# Fri, 09 Dec 2022 12:15:32 GMT
LABEL org.opencontainers.image.authors=XWiki Development Team <committers@xwiki.org>
# Fri, 09 Dec 2022 12:15:32 GMT
LABEL org.opencontainers.image.url=https://hub.docker.com/_/xwiki
# Fri, 09 Dec 2022 12:15:33 GMT
LABEL org.opencontainers.image.documentation=https://hub.docker.com/_/xwiki
# Fri, 09 Dec 2022 12:15:33 GMT
LABEL org.opencontainers.image.source=https://github.com/xwiki/xwiki-docker.git
# Fri, 09 Dec 2022 12:15:33 GMT
LABEL org.opencontainers.image.vendor=xwiki.org
# Fri, 09 Dec 2022 12:15:33 GMT
LABEL org.opencontainers.image.licenses=LGPL-2.1
# Fri, 09 Dec 2022 12:17:17 GMT
RUN apt-get update &&   apt-get --no-install-recommends -y install     curl     libreoffice     unzip     procps &&   rm -rf /var/lib/apt/lists/*
# Tue, 27 Dec 2022 18:07:05 GMT
ENV XWIKI_VERSION=14.10.2
# Tue, 27 Dec 2022 18:07:05 GMT
ENV XWIKI_URL_PREFIX=https://maven.xwiki.org/releases/org/xwiki/platform/xwiki-platform-distribution-war/14.10.2
# Tue, 27 Dec 2022 18:07:05 GMT
ENV XWIKI_DOWNLOAD_SHA256=d84eda7c2952dd4e7336abf3dbe4cec58e8f857938925b130b02296d415d3f14
# Tue, 27 Dec 2022 18:07:53 GMT
RUN rm -rf /usr/local/tomcat/webapps/* &&   mkdir -p /usr/local/tomcat/temp &&   mkdir -p /usr/local/xwiki/data &&   curl -fSL "${XWIKI_URL_PREFIX}/xwiki-platform-distribution-war-${XWIKI_VERSION}.war" -o xwiki.war &&   echo "$XWIKI_DOWNLOAD_SHA256 xwiki.war" | sha256sum -c - &&   unzip -d /usr/local/tomcat/webapps/ROOT xwiki.war &&   rm -f xwiki.war
# Tue, 27 Dec 2022 18:07:54 GMT
ENV MYSQL_JDBC_VERSION=8.0.31
# Tue, 27 Dec 2022 18:07:54 GMT
ENV MYSQL_JDBC_SHA256=5249e3dc6d6531b37790e3f61845b96db5e41e891d3d8edb0e2e3a1b53ca2f4f
# Tue, 27 Dec 2022 18:07:54 GMT
ENV MYSQL_JDBC_PREFIX=https://repo1.maven.org/maven2/com/mysql/mysql-connector-j/8.0.31
# Tue, 27 Dec 2022 18:07:54 GMT
ENV MYSQL_JDBC_ARTIFACT=mysql-connector-j-8.0.31.jar
# Tue, 27 Dec 2022 18:07:54 GMT
ENV MYSQL_JDBC_TARGET=/usr/local/tomcat/webapps/ROOT/WEB-INF/lib/mysql-connector-j-8.0.31.jar
# Tue, 27 Dec 2022 18:07:55 GMT
RUN curl -fSL "${MYSQL_JDBC_PREFIX}/${MYSQL_JDBC_ARTIFACT}" -o $MYSQL_JDBC_TARGET &&   echo "$MYSQL_JDBC_SHA256 $MYSQL_JDBC_TARGET" | sha256sum -c -
# Tue, 27 Dec 2022 18:07:55 GMT
COPY file:0a1be11e2eb610a1dbcd415404e3a592641110b93090030cb831e3a19a163017 in /usr/local/tomcat/bin/ 
# Tue, 27 Dec 2022 18:07:55 GMT
COPY file:1b8409986f3e4eb79a7a0b18472cb2692a61d504fb5ef34292bc997b79fd760d in /usr/local/tomcat/webapps/ROOT/WEB-INF/hibernate.cfg.xml 
# Tue, 27 Dec 2022 18:07:56 GMT
RUN sed -i 's/<id>org.xwiki.platform:xwiki-platform-distribution-war/<id>org.xwiki.platform:xwiki-platform-distribution-docker/'   /usr/local/tomcat/webapps/ROOT/META-INF/extension.xed
# Tue, 27 Dec 2022 18:07:56 GMT
COPY file:a47c4dcd87c9dad97aff38c49188357e6193bcad50757e516cfb08a60d4de611 in /usr/local/bin/docker-entrypoint.sh 
# Tue, 27 Dec 2022 18:07:56 GMT
VOLUME [/usr/local/xwiki]
# Tue, 27 Dec 2022 18:07:56 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 27 Dec 2022 18:07:56 GMT
CMD ["xwiki"]
```

-	Layers:
	-	`sha256:6e3729cf69e0ce2de9e779575a1fec8b7fb5efdfa822829290ab6d5d1bc3e797`  
		Last Modified: Thu, 08 Dec 2022 14:10:00 GMT  
		Size: 30.4 MB (30428708 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:96aa423488f0ed1e9bf6c6da11fa7fb53568d1ea4003892416b3adeccb47e3bf`  
		Last Modified: Fri, 09 Dec 2022 01:50:02 GMT  
		Size: 12.4 MB (12432218 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a149af9550da920d6e3c2939b43e257b858d65f5733af488a97f721d34f907ef`  
		Last Modified: Fri, 09 Dec 2022 01:52:09 GMT  
		Size: 46.6 MB (46632223 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e1a0fd4e771cad4fe553a76281b2095d46b07749710d4dbbaf1b1d07c764c43d`  
		Last Modified: Fri, 09 Dec 2022 01:52:02 GMT  
		Size: 160.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8274493ddef8dca07c72767bb58b89ea95bb83cfe512214b2e61bc33066a10a2`  
		Last Modified: Fri, 09 Dec 2022 08:05:08 GMT  
		Size: 172.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f4b854a69411509041e0f76c9110724992af4f0b41f3c9f4406c16d8d4bb2dec`  
		Last Modified: Fri, 09 Dec 2022 08:12:38 GMT  
		Size: 12.2 MB (12205387 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9ce2d88f7c975696550bbba0f29b0d9186bb50a5af9af52780a0f02c86fd51aa`  
		Last Modified: Fri, 09 Dec 2022 08:12:37 GMT  
		Size: 452.8 KB (452765 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bef1e7209c510a541f551fa27cd8bce35a5c90272f9e6cbc94ec811b0d45dd44`  
		Last Modified: Fri, 09 Dec 2022 08:12:36 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:31cb3de5dbc0c239480a9b7284657d263b942e587f5de6c3904685c329e13da5`  
		Last Modified: Fri, 09 Dec 2022 12:24:18 GMT  
		Size: 178.3 MB (178326985 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a305cac5507b4f5bec08c27ad4e7dc514695431935dff1764238a01543a3061a`  
		Last Modified: Tue, 27 Dec 2022 18:10:10 GMT  
		Size: 307.0 MB (306987314 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a9b3feed3bfbb04469ed3a9cc9e0c237881ad15c0eec9379e0da0a48e05d5521`  
		Last Modified: Tue, 27 Dec 2022 18:09:53 GMT  
		Size: 2.4 MB (2377184 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7c7cd9b3ab872764044a11a90ae81468372053d81dd697e0eb7b8e0c4f099a64`  
		Last Modified: Tue, 27 Dec 2022 18:09:53 GMT  
		Size: 1.3 KB (1344 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7cf737cceeb35c150a723b291ba891d7b3802c0953afa089b74671effe71326a`  
		Last Modified: Tue, 27 Dec 2022 18:09:53 GMT  
		Size: 2.3 KB (2308 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8206f5238d0911c84de600e49a5c133d9d17b8d877047d5a571cd5026eb084a8`  
		Last Modified: Tue, 27 Dec 2022 18:09:53 GMT  
		Size: 6.0 KB (6007 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c369a12a69873aac0ae774b8a3a3c34b987a46a95516497e46bc6da1885e1773`  
		Last Modified: Tue, 27 Dec 2022 18:09:53 GMT  
		Size: 2.5 KB (2504 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `xwiki:lts-mysql-tomcat` - linux; arm64 variant v8

```console
$ docker pull xwiki@sha256:41651370883a67fac27cfb16b57caeeae80006c8260aba02e1577b86e6953e23
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **581.1 MB (581125727 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:480bfe3c7fe53cbdea1a14d6b247f6f6000045a4fd034dafbceef9dfd6190d35`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["xwiki"]`

```dockerfile
# Fri, 09 Dec 2022 01:46:57 GMT
ADD file:429a55a11d4bcd15647d1316d9debd9ead4b4ab5c0b9146894d07c39aa814290 in / 
# Fri, 09 Dec 2022 01:46:57 GMT
CMD ["bash"]
# Fri, 09 Dec 2022 03:39:20 GMT
ENV JAVA_HOME=/opt/java/openjdk
# Fri, 09 Dec 2022 03:39:20 GMT
ENV PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Fri, 09 Dec 2022 03:39:20 GMT
ENV LANG=en_US.UTF-8 LANGUAGE=en_US:en LC_ALL=en_US.UTF-8
# Fri, 09 Dec 2022 03:39:39 GMT
RUN apt-get update     && DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends tzdata curl wget ca-certificates fontconfig locales     && echo "en_US.UTF-8 UTF-8" >> /etc/locale.gen     && locale-gen en_US.UTF-8     && rm -rf /var/lib/apt/lists/*
# Fri, 09 Dec 2022 03:40:34 GMT
ENV JAVA_VERSION=jdk-11.0.17+8
# Fri, 09 Dec 2022 03:41:02 GMT
RUN set -eux;     ARCH="$(dpkg --print-architecture)";     case "${ARCH}" in        aarch64|arm64)          ESUM='bd6efe3290c8b5a42f695a55a26f3e3c9c284288574879d4b7089f31f5114177';          BINARY_URL='https://github.com/adoptium/temurin11-binaries/releases/download/jdk-11.0.17%2B8/OpenJDK11U-jre_aarch64_linux_hotspot_11.0.17_8.tar.gz';          ;;        armhf|arm)          ESUM='8cf113d3d7fa808895c8d2e41bb890af21c47e38c2460e0588147a4bb8fc658d';          BINARY_URL='https://github.com/adoptium/temurin11-binaries/releases/download/jdk-11.0.17%2B8/OpenJDK11U-jre_arm_linux_hotspot_11.0.17_8.tar.gz';          ;;        ppc64el|powerpc:common64)          ESUM='0ca3d806131ab5834c501f9c625bb0248cd528af361c704503348e9c9605bedf';          BINARY_URL='https://github.com/adoptium/temurin11-binaries/releases/download/jdk-11.0.17%2B8/OpenJDK11U-jre_ppc64le_linux_hotspot_11.0.17_8.tar.gz';          ;;        s390x|s390:64-bit)          ESUM='dd3b159a374086e65cb07c4ccb226c90f9c02ef929cba6f0b642171d7ed97fa4';          BINARY_URL='https://github.com/adoptium/temurin11-binaries/releases/download/jdk-11.0.17%2B8/OpenJDK11U-jre_s390x_linux_hotspot_11.0.17_8.tar.gz';          ;;        amd64|i386:x86-64)          ESUM='752616097e09d7f60a3ad8bd312f90eaf50ac72577e55df229fe6e8091148f79';          BINARY_URL='https://github.com/adoptium/temurin11-binaries/releases/download/jdk-11.0.17%2B8/OpenJDK11U-jre_x64_linux_hotspot_11.0.17_8.tar.gz';          ;;        *)          echo "Unsupported arch: ${ARCH}";          exit 1;          ;;     esac; 	  wget -O /tmp/openjdk.tar.gz ${BINARY_URL}; 	  echo "${ESUM} */tmp/openjdk.tar.gz" | sha256sum -c -; 	  mkdir -p "$JAVA_HOME"; 	  tar --extract 	      --file /tmp/openjdk.tar.gz 	      --directory "$JAVA_HOME" 	      --strip-components 1 	      --no-same-owner 	  ;     rm /tmp/openjdk.tar.gz;     find "$JAVA_HOME/lib" -name '*.so' -exec dirname '{}' ';' | sort -u > /etc/ld.so.conf.d/docker-openjdk.conf;     ldconfig;     java -Xshare:dump;
# Fri, 09 Dec 2022 03:41:03 GMT
RUN echo Verifying install ...     && fileEncoding="$(echo 'System.out.println(System.getProperty("file.encoding"))' | jshell -s -)"; [ "$fileEncoding" = 'UTF-8' ]; rm -rf ~/.java     && echo java --version && java --version     && echo Complete.
# Fri, 09 Dec 2022 06:19:35 GMT
ENV CATALINA_HOME=/usr/local/tomcat
# Fri, 09 Dec 2022 06:19:35 GMT
ENV PATH=/usr/local/tomcat/bin:/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Fri, 09 Dec 2022 06:19:36 GMT
RUN mkdir -p "$CATALINA_HOME"
# Fri, 09 Dec 2022 06:19:36 GMT
WORKDIR /usr/local/tomcat
# Fri, 09 Dec 2022 06:19:36 GMT
ENV TOMCAT_NATIVE_LIBDIR=/usr/local/tomcat/native-jni-lib
# Fri, 09 Dec 2022 06:19:36 GMT
ENV LD_LIBRARY_PATH=/usr/local/tomcat/native-jni-lib
# Fri, 09 Dec 2022 06:26:36 GMT
ENV GPG_KEYS=48F8E69F6390C9F25CFEDCD268248959359E722B A9C5DF4D22E99998D9875A5110C01C5A2F6059E7 DCFD35E0BF8CA7344752DE8B6FB21E8933C60243
# Fri, 09 Dec 2022 06:26:36 GMT
ENV TOMCAT_MAJOR=9
# Fri, 09 Dec 2022 06:26:36 GMT
ENV TOMCAT_VERSION=9.0.70
# Fri, 09 Dec 2022 06:26:36 GMT
ENV TOMCAT_SHA512=9b57b332f4cfb2c4b9250b95924314507ebafec44f732e755be96d35e1a50d98ca3ea11a8c62e0c6fde2541d31a981f5ca792ea9931b2551b81b495932474726
# Fri, 09 Dec 2022 06:26:37 GMT
COPY dir:27bf917e8591b961da8271d4df44f32813c3d789939ac0dae5703638df90129f in /usr/local/tomcat 
# Fri, 09 Dec 2022 06:26:40 GMT
RUN set -eux; 	apt-get update; 	xargs -rt apt-get install -y --no-install-recommends < "$TOMCAT_NATIVE_LIBDIR/.dependencies.txt"; 	rm -rf /var/lib/apt/lists/*
# Fri, 09 Dec 2022 06:26:41 GMT
RUN set -eux; 	nativeLines="$(catalina.sh configtest 2>&1)"; 	nativeLines="$(echo "$nativeLines" | grep 'Apache Tomcat Native')"; 	nativeLines="$(echo "$nativeLines" | sort -u)"; 	if ! echo "$nativeLines" | grep -E 'INFO: Loaded( APR based)? Apache Tomcat Native library' >&2; then 		echo >&2 "$nativeLines"; 		exit 1; 	fi
# Fri, 09 Dec 2022 06:26:41 GMT
EXPOSE 8080
# Fri, 09 Dec 2022 06:26:41 GMT
CMD ["catalina.sh" "run"]
# Fri, 09 Dec 2022 08:37:06 GMT
LABEL org.opencontainers.image.authors=XWiki Development Team <committers@xwiki.org>
# Fri, 09 Dec 2022 08:37:06 GMT
LABEL org.opencontainers.image.url=https://hub.docker.com/_/xwiki
# Fri, 09 Dec 2022 08:37:06 GMT
LABEL org.opencontainers.image.documentation=https://hub.docker.com/_/xwiki
# Fri, 09 Dec 2022 08:37:06 GMT
LABEL org.opencontainers.image.source=https://github.com/xwiki/xwiki-docker.git
# Fri, 09 Dec 2022 08:37:06 GMT
LABEL org.opencontainers.image.vendor=xwiki.org
# Fri, 09 Dec 2022 08:37:06 GMT
LABEL org.opencontainers.image.licenses=LGPL-2.1
# Fri, 09 Dec 2022 08:38:55 GMT
RUN apt-get update &&   apt-get --no-install-recommends -y install     curl     libreoffice     unzip     procps &&   rm -rf /var/lib/apt/lists/*
# Tue, 27 Dec 2022 17:16:15 GMT
ENV XWIKI_VERSION=14.10.2
# Tue, 27 Dec 2022 17:16:15 GMT
ENV XWIKI_URL_PREFIX=https://maven.xwiki.org/releases/org/xwiki/platform/xwiki-platform-distribution-war/14.10.2
# Tue, 27 Dec 2022 17:16:15 GMT
ENV XWIKI_DOWNLOAD_SHA256=d84eda7c2952dd4e7336abf3dbe4cec58e8f857938925b130b02296d415d3f14
# Tue, 27 Dec 2022 17:16:55 GMT
RUN rm -rf /usr/local/tomcat/webapps/* &&   mkdir -p /usr/local/tomcat/temp &&   mkdir -p /usr/local/xwiki/data &&   curl -fSL "${XWIKI_URL_PREFIX}/xwiki-platform-distribution-war-${XWIKI_VERSION}.war" -o xwiki.war &&   echo "$XWIKI_DOWNLOAD_SHA256 xwiki.war" | sha256sum -c - &&   unzip -d /usr/local/tomcat/webapps/ROOT xwiki.war &&   rm -f xwiki.war
# Tue, 27 Dec 2022 17:16:57 GMT
ENV MYSQL_JDBC_VERSION=8.0.31
# Tue, 27 Dec 2022 17:16:57 GMT
ENV MYSQL_JDBC_SHA256=5249e3dc6d6531b37790e3f61845b96db5e41e891d3d8edb0e2e3a1b53ca2f4f
# Tue, 27 Dec 2022 17:16:57 GMT
ENV MYSQL_JDBC_PREFIX=https://repo1.maven.org/maven2/com/mysql/mysql-connector-j/8.0.31
# Tue, 27 Dec 2022 17:16:57 GMT
ENV MYSQL_JDBC_ARTIFACT=mysql-connector-j-8.0.31.jar
# Tue, 27 Dec 2022 17:16:57 GMT
ENV MYSQL_JDBC_TARGET=/usr/local/tomcat/webapps/ROOT/WEB-INF/lib/mysql-connector-j-8.0.31.jar
# Tue, 27 Dec 2022 17:16:58 GMT
RUN curl -fSL "${MYSQL_JDBC_PREFIX}/${MYSQL_JDBC_ARTIFACT}" -o $MYSQL_JDBC_TARGET &&   echo "$MYSQL_JDBC_SHA256 $MYSQL_JDBC_TARGET" | sha256sum -c -
# Tue, 27 Dec 2022 17:16:58 GMT
COPY file:0a1be11e2eb610a1dbcd415404e3a592641110b93090030cb831e3a19a163017 in /usr/local/tomcat/bin/ 
# Tue, 27 Dec 2022 17:16:58 GMT
COPY file:1b8409986f3e4eb79a7a0b18472cb2692a61d504fb5ef34292bc997b79fd760d in /usr/local/tomcat/webapps/ROOT/WEB-INF/hibernate.cfg.xml 
# Tue, 27 Dec 2022 17:16:59 GMT
RUN sed -i 's/<id>org.xwiki.platform:xwiki-platform-distribution-war/<id>org.xwiki.platform:xwiki-platform-distribution-docker/'   /usr/local/tomcat/webapps/ROOT/META-INF/extension.xed
# Tue, 27 Dec 2022 17:16:59 GMT
COPY file:a47c4dcd87c9dad97aff38c49188357e6193bcad50757e516cfb08a60d4de611 in /usr/local/bin/docker-entrypoint.sh 
# Tue, 27 Dec 2022 17:16:59 GMT
VOLUME [/usr/local/xwiki]
# Tue, 27 Dec 2022 17:16:59 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 27 Dec 2022 17:16:59 GMT
CMD ["xwiki"]
```

-	Layers:
	-	`sha256:10175de2f0c4f7d306f660ee073bce12b824c8012dd19b3c140aae053fabd1cc`  
		Last Modified: Thu, 08 Dec 2022 18:50:01 GMT  
		Size: 28.4 MB (28384475 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6940ebf96dce07e0f2d684dad9d95a74c7620e493977fa2d52970797dafd6002`  
		Last Modified: Fri, 09 Dec 2022 03:45:30 GMT  
		Size: 12.4 MB (12391491 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4d2520d28fa515fc27705b801be6fde980d49f51a3b88eabe99e12972db955a2`  
		Last Modified: Fri, 09 Dec 2022 03:47:29 GMT  
		Size: 45.0 MB (44958320 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c049d25ee0757b5605c2b49028f6889b320f687e38aeb775e846ea61d4748610`  
		Last Modified: Fri, 09 Dec 2022 03:47:25 GMT  
		Size: 160.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f38ba8d6e08bbdb0162029a97116c026e3f070efdc57e95557d46282a03a84f4`  
		Last Modified: Fri, 09 Dec 2022 06:39:07 GMT  
		Size: 172.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:22af54d54ccccf7f6b67bd9c7f03837e5e9544746ecc2db7e6db90b91a7279eb`  
		Last Modified: Fri, 09 Dec 2022 06:46:31 GMT  
		Size: 12.2 MB (12214036 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:605f90e7b26fb97847bd2a59d109f6ebe1de5489537157f4c5f4282919b4ee24`  
		Last Modified: Fri, 09 Dec 2022 06:46:30 GMT  
		Size: 453.4 KB (453426 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ec67c51d618203c6edf94a8c05f9233e928782864e78df774e92ed2f1df7d111`  
		Last Modified: Fri, 09 Dec 2022 06:46:35 GMT  
		Size: 130.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:07da5ebf9ec134d7484c5d1cc68ef8bd8efdd64185acb60bacb395f3033d019b`  
		Last Modified: Fri, 09 Dec 2022 08:46:59 GMT  
		Size: 173.3 MB (173346863 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3c4885a12e1d8c67cbf4030893d9c36195a73294899b33d04e6a3c389f15c7a3`  
		Last Modified: Tue, 27 Dec 2022 17:20:40 GMT  
		Size: 307.0 MB (306987301 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:99c869abd859ca98c1a958df0892338af471cc84b3bee688feabbc54543a5e14`  
		Last Modified: Tue, 27 Dec 2022 17:20:26 GMT  
		Size: 2.4 MB (2377184 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:101406ea2f622364e0f2cff30c02df7036b50fc5f60ed7e4dcd1f2a1d1bafd88`  
		Last Modified: Tue, 27 Dec 2022 17:20:26 GMT  
		Size: 1.3 KB (1345 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f7f254ba0b238dc3b67d9d57c8290317104d375f5ee8e5411aa4c2772b3e0197`  
		Last Modified: Tue, 27 Dec 2022 17:20:26 GMT  
		Size: 2.3 KB (2310 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:48c685fce2f8b0997a9faea6317d879cd12a7ccd978a9cdb939a5b644a123a9e`  
		Last Modified: Tue, 27 Dec 2022 17:20:26 GMT  
		Size: 6.0 KB (6008 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:37bd5e6f2da7a8e7325de700cba1330ab11e4e6cc35290aafd5359023f818615`  
		Last Modified: Tue, 27 Dec 2022 17:20:26 GMT  
		Size: 2.5 KB (2506 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
