## `xwiki:lts-mysql-tomcat`

```console
$ docker pull xwiki@sha256:9096e6b74d834e57702b69a244de1751391d001622117fbeb056d9ec9ff9e4be
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `xwiki:lts-mysql-tomcat` - linux; amd64

```console
$ docker pull xwiki@sha256:39545143ec78250d4c7eca4be9af4fb3c478110059a24c19f248822b21177c2c
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **575.4 MB (575358121 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:0a2b48a62500a1ef395da3c99edc778f2d1eef3d69fa34fcf7ed6b35c8fd8153`
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
# Fri, 09 Dec 2022 12:21:21 GMT
ENV XWIKI_VERSION=13.10.10
# Fri, 09 Dec 2022 12:21:21 GMT
ENV XWIKI_URL_PREFIX=https://maven.xwiki.org/releases/org/xwiki/platform/xwiki-platform-distribution-war/13.10.10
# Fri, 09 Dec 2022 12:21:21 GMT
ENV XWIKI_DOWNLOAD_SHA256=bae87a16d291d321d0848fcba55e455bfcd4b1890597cd9b735d98013cf44bad
# Fri, 09 Dec 2022 12:21:58 GMT
RUN rm -rf /usr/local/tomcat/webapps/* &&   mkdir -p /usr/local/tomcat/temp &&   mkdir -p /usr/local/xwiki/data &&   curl -fSL "${XWIKI_URL_PREFIX}/xwiki-platform-distribution-war-${XWIKI_VERSION}.war" -o xwiki.war &&   echo "$XWIKI_DOWNLOAD_SHA256 xwiki.war" | sha256sum -c - &&   unzip -d /usr/local/tomcat/webapps/ROOT xwiki.war &&   rm -f xwiki.war
# Fri, 09 Dec 2022 12:21:59 GMT
ENV MYSQL_JDBC_VERSION=8.0.30
# Fri, 09 Dec 2022 12:22:00 GMT
ENV MYSQL_JDBC_SHA256=b5bf2f0987197c30adf74a9e419b89cda4c257da2d1142871f508416d5f2227a
# Fri, 09 Dec 2022 12:22:00 GMT
ENV MYSQL_JDBC_PREFIX=https://repo1.maven.org/maven2/mysql/mysql-connector-java/8.0.30
# Fri, 09 Dec 2022 12:22:00 GMT
ENV MYSQL_JDBC_ARTIFACT=mysql-connector-java-8.0.30.jar
# Fri, 09 Dec 2022 12:22:00 GMT
ENV MYSQL_JDBC_TARGET=/usr/local/tomcat/webapps/ROOT/WEB-INF/lib/mysql-connector-java-8.0.30.jar
# Fri, 09 Dec 2022 12:22:01 GMT
RUN curl -fSL "${MYSQL_JDBC_PREFIX}/${MYSQL_JDBC_ARTIFACT}" -o $MYSQL_JDBC_TARGET &&   echo "$MYSQL_JDBC_SHA256 $MYSQL_JDBC_TARGET" | sha256sum -c -
# Fri, 09 Dec 2022 12:22:01 GMT
COPY file:0a1be11e2eb610a1dbcd415404e3a592641110b93090030cb831e3a19a163017 in /usr/local/tomcat/bin/ 
# Fri, 09 Dec 2022 12:22:01 GMT
COPY file:1b8409986f3e4eb79a7a0b18472cb2692a61d504fb5ef34292bc997b79fd760d in /usr/local/tomcat/webapps/ROOT/WEB-INF/hibernate.cfg.xml 
# Fri, 09 Dec 2022 12:22:02 GMT
RUN sed -i 's/<id>org.xwiki.platform:xwiki-platform-distribution-war/<id>org.xwiki.platform:xwiki-platform-distribution-docker/'   /usr/local/tomcat/webapps/ROOT/META-INF/extension.xed
# Fri, 09 Dec 2022 12:22:02 GMT
COPY file:a47c4dcd87c9dad97aff38c49188357e6193bcad50757e516cfb08a60d4de611 in /usr/local/bin/docker-entrypoint.sh 
# Fri, 09 Dec 2022 12:22:02 GMT
VOLUME [/usr/local/xwiki]
# Fri, 09 Dec 2022 12:22:02 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 09 Dec 2022 12:22:02 GMT
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
	-	`sha256:8e5cbed093dd22e101c6517a31df0c6b9961f0bc788c6e3b11e844d2cfa7d622`  
		Last Modified: Fri, 09 Dec 2022 12:27:35 GMT  
		Size: 292.5 MB (292492620 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2c25a596d6e3143924fd84ec322979e1c053b186e1dcbb9282c2a3c250be0920`  
		Last Modified: Fri, 09 Dec 2022 12:27:18 GMT  
		Size: 2.4 MB (2375237 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e538a86b3cc7129d9e5eacdd4cae124b020b3d84f924fa7a48d3fce08d406822`  
		Last Modified: Fri, 09 Dec 2022 12:27:18 GMT  
		Size: 1.3 KB (1344 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2bc753a97ceaa285af1890ef47c4a82f3282d1ebd65b5ebfe32697455b756791`  
		Last Modified: Fri, 09 Dec 2022 12:27:18 GMT  
		Size: 2.3 KB (2307 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e35eeb6bfa0bb6d7c24be0ea721bfaabc6671652486c562faf9543678f5331fc`  
		Last Modified: Fri, 09 Dec 2022 12:27:18 GMT  
		Size: 5.4 KB (5362 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d9d8eacf890e610b34b28fad5d09e267c244d610966e2aca8aac52e076557c54`  
		Last Modified: Fri, 09 Dec 2022 12:27:18 GMT  
		Size: 2.5 KB (2504 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `xwiki:lts-mysql-tomcat` - linux; arm64 variant v8

```console
$ docker pull xwiki@sha256:9508a895aa9738a15042f2302337fe5600dd142ae352be620fa66fb44080a0ed
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **566.6 MB (566628471 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:5870568d394ce1df9ccc37e8f7b81c125de7131a82c6d1f205fc7b168f0b877c`
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
# Fri, 09 Dec 2022 08:44:09 GMT
ENV XWIKI_VERSION=13.10.10
# Fri, 09 Dec 2022 08:44:09 GMT
ENV XWIKI_URL_PREFIX=https://maven.xwiki.org/releases/org/xwiki/platform/xwiki-platform-distribution-war/13.10.10
# Fri, 09 Dec 2022 08:44:09 GMT
ENV XWIKI_DOWNLOAD_SHA256=bae87a16d291d321d0848fcba55e455bfcd4b1890597cd9b735d98013cf44bad
# Fri, 09 Dec 2022 08:44:47 GMT
RUN rm -rf /usr/local/tomcat/webapps/* &&   mkdir -p /usr/local/tomcat/temp &&   mkdir -p /usr/local/xwiki/data &&   curl -fSL "${XWIKI_URL_PREFIX}/xwiki-platform-distribution-war-${XWIKI_VERSION}.war" -o xwiki.war &&   echo "$XWIKI_DOWNLOAD_SHA256 xwiki.war" | sha256sum -c - &&   unzip -d /usr/local/tomcat/webapps/ROOT xwiki.war &&   rm -f xwiki.war
# Fri, 09 Dec 2022 08:44:49 GMT
ENV MYSQL_JDBC_VERSION=8.0.30
# Fri, 09 Dec 2022 08:44:49 GMT
ENV MYSQL_JDBC_SHA256=b5bf2f0987197c30adf74a9e419b89cda4c257da2d1142871f508416d5f2227a
# Fri, 09 Dec 2022 08:44:49 GMT
ENV MYSQL_JDBC_PREFIX=https://repo1.maven.org/maven2/mysql/mysql-connector-java/8.0.30
# Fri, 09 Dec 2022 08:44:49 GMT
ENV MYSQL_JDBC_ARTIFACT=mysql-connector-java-8.0.30.jar
# Fri, 09 Dec 2022 08:44:49 GMT
ENV MYSQL_JDBC_TARGET=/usr/local/tomcat/webapps/ROOT/WEB-INF/lib/mysql-connector-java-8.0.30.jar
# Fri, 09 Dec 2022 08:44:50 GMT
RUN curl -fSL "${MYSQL_JDBC_PREFIX}/${MYSQL_JDBC_ARTIFACT}" -o $MYSQL_JDBC_TARGET &&   echo "$MYSQL_JDBC_SHA256 $MYSQL_JDBC_TARGET" | sha256sum -c -
# Fri, 09 Dec 2022 08:44:50 GMT
COPY file:0a1be11e2eb610a1dbcd415404e3a592641110b93090030cb831e3a19a163017 in /usr/local/tomcat/bin/ 
# Fri, 09 Dec 2022 08:44:50 GMT
COPY file:1b8409986f3e4eb79a7a0b18472cb2692a61d504fb5ef34292bc997b79fd760d in /usr/local/tomcat/webapps/ROOT/WEB-INF/hibernate.cfg.xml 
# Fri, 09 Dec 2022 08:44:50 GMT
RUN sed -i 's/<id>org.xwiki.platform:xwiki-platform-distribution-war/<id>org.xwiki.platform:xwiki-platform-distribution-docker/'   /usr/local/tomcat/webapps/ROOT/META-INF/extension.xed
# Fri, 09 Dec 2022 08:44:50 GMT
COPY file:a47c4dcd87c9dad97aff38c49188357e6193bcad50757e516cfb08a60d4de611 in /usr/local/bin/docker-entrypoint.sh 
# Fri, 09 Dec 2022 08:44:51 GMT
VOLUME [/usr/local/xwiki]
# Fri, 09 Dec 2022 08:44:51 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 09 Dec 2022 08:44:51 GMT
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
	-	`sha256:5b5d4a4e2851629395ceb9323fc46ec08eb99dd9cde35d7fe706ff0dcee0af5d`  
		Last Modified: Fri, 09 Dec 2022 08:49:42 GMT  
		Size: 292.5 MB (292492636 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:83f9c23d37645e7c2dfe8fb79529b7ba336645a550bc0687d0f34adb0787191a`  
		Last Modified: Fri, 09 Dec 2022 08:49:28 GMT  
		Size: 2.4 MB (2375239 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:32e9daaaebd71110005da2a8984d3a44c1e1b821b05b526847f18295bdc1f3e1`  
		Last Modified: Fri, 09 Dec 2022 08:49:28 GMT  
		Size: 1.3 KB (1343 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5106031fefd698e0e17cc0b240d072f7e402b7ce4d2ecdccdd5e03f548179525`  
		Last Modified: Fri, 09 Dec 2022 08:49:27 GMT  
		Size: 2.3 KB (2310 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:05e426294aed1be22b76a3c47ac30e69eb9bbb814ca57fb0940210ae2ff85194`  
		Last Modified: Fri, 09 Dec 2022 08:49:27 GMT  
		Size: 5.4 KB (5366 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f9cbb5541145f6ab070dba9e0f7be7d6f6e4913bf44c042b3a7c001574655a15`  
		Last Modified: Fri, 09 Dec 2022 08:49:27 GMT  
		Size: 2.5 KB (2504 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
