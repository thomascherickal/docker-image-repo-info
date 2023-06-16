## `xwiki:stable-mysql-tomcat`

```console
$ docker pull xwiki@sha256:1251f5dd36e7fbec9070b5514f77155d212f96087ed6c280411d02166cde2a53
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `xwiki:stable-mysql-tomcat` - linux; amd64

```console
$ docker pull xwiki@sha256:c02a3833f4b92aedd0539c436b66440bf807b5c99fc00475e98d345a08968741
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **592.3 MB (592295239 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:37faea8b192270e1893b7fe0e612998bae03e3052279c3d9e79ed09e7b65e9c6`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["xwiki"]`

```dockerfile
# Mon, 22 May 2023 17:45:50 GMT
ARG RELEASE
# Mon, 22 May 2023 17:45:50 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Mon, 22 May 2023 17:45:50 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Mon, 22 May 2023 17:45:50 GMT
LABEL org.opencontainers.image.version=22.04
# Mon, 22 May 2023 17:45:52 GMT
ADD file:2fd2684e989d275c95e18b6f6e9ccf57ca1382ecd8faf4a66961ede28102dedf in / 
# Mon, 22 May 2023 17:45:52 GMT
CMD ["/bin/bash"]
# Fri, 02 Jun 2023 01:42:51 GMT
ENV JAVA_HOME=/opt/java/openjdk
# Fri, 02 Jun 2023 01:42:51 GMT
ENV PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Fri, 02 Jun 2023 01:42:51 GMT
ENV LANG=en_US.UTF-8 LANGUAGE=en_US:en LC_ALL=en_US.UTF-8
# Fri, 02 Jun 2023 01:43:03 GMT
RUN apt-get update     && DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends tzdata curl wget ca-certificates fontconfig locales     && echo "en_US.UTF-8 UTF-8" >> /etc/locale.gen     && locale-gen en_US.UTF-8     && rm -rf /var/lib/apt/lists/*
# Fri, 02 Jun 2023 01:43:39 GMT
ENV JAVA_VERSION=jdk-11.0.19+7
# Fri, 02 Jun 2023 01:44:06 GMT
RUN set -eux;     ARCH="$(dpkg --print-architecture)";     case "${ARCH}" in        aarch64|arm64)          ESUM='1fe4b20d808f393422610818711c728331992a4455eeeb061d3d05b45412771d';          BINARY_URL='https://github.com/adoptium/temurin11-binaries/releases/download/jdk-11.0.19%2B7/OpenJDK11U-jre_aarch64_linux_hotspot_11.0.19_7.tar.gz';          ;;        armhf|arm)          ESUM='cb754b055177381f9f6852b7e5469904a15edddd7f8e136043c28b1e33aee47c';          BINARY_URL='https://github.com/adoptium/temurin11-binaries/releases/download/jdk-11.0.19%2B7/OpenJDK11U-jre_arm_linux_hotspot_11.0.19_7.tar.gz';          ;;        ppc64el|powerpc:common64)          ESUM='8019d938e5525938ec8e68e2989c4413263b0d9b7b3f20fe0c45f6d967919cfb';          BINARY_URL='https://github.com/adoptium/temurin11-binaries/releases/download/jdk-11.0.19%2B7/OpenJDK11U-jre_ppc64le_linux_hotspot_11.0.19_7.tar.gz';          ;;        s390x|s390:64-bit)          ESUM='058419435fe6212d1bc305a14f578c314f9ff9a2d96d523c178120e84231c733';          BINARY_URL='https://github.com/adoptium/temurin11-binaries/releases/download/jdk-11.0.19%2B7/OpenJDK11U-jre_s390x_linux_hotspot_11.0.19_7.tar.gz';          ;;        amd64|i386:x86-64)          ESUM='32dcf760664f93531594b72ce9226e9216567de5705a23c9ff5a77c797948054';          BINARY_URL='https://github.com/adoptium/temurin11-binaries/releases/download/jdk-11.0.19%2B7/OpenJDK11U-jre_x64_linux_hotspot_11.0.19_7.tar.gz';          ;;        *)          echo "Unsupported arch: ${ARCH}";          exit 1;          ;;     esac; 	  wget -O /tmp/openjdk.tar.gz ${BINARY_URL}; 	  echo "${ESUM} */tmp/openjdk.tar.gz" | sha256sum -c -; 	  mkdir -p "$JAVA_HOME"; 	  tar --extract 	      --file /tmp/openjdk.tar.gz 	      --directory "$JAVA_HOME" 	      --strip-components 1 	      --no-same-owner 	  ;     rm -f /tmp/openjdk.tar.gz ${JAVA_HOME}/src.zip;     find "$JAVA_HOME/lib" -name '*.so' -exec dirname '{}' ';' | sort -u > /etc/ld.so.conf.d/docker-openjdk.conf;     ldconfig;     java -Xshare:dump;
# Fri, 02 Jun 2023 01:44:07 GMT
RUN echo Verifying install ...     && fileEncoding="$(echo 'System.out.println(System.getProperty("file.encoding"))' | jshell -s -)"; [ "$fileEncoding" = 'UTF-8' ]; rm -rf ~/.java     && echo java --version && java --version     && echo Complete.
# Sun, 04 Jun 2023 16:55:35 GMT
ENV CATALINA_HOME=/usr/local/tomcat
# Sun, 04 Jun 2023 16:55:35 GMT
ENV PATH=/usr/local/tomcat/bin:/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Sun, 04 Jun 2023 16:55:35 GMT
RUN mkdir -p "$CATALINA_HOME"
# Sun, 04 Jun 2023 16:55:35 GMT
WORKDIR /usr/local/tomcat
# Sun, 04 Jun 2023 16:55:35 GMT
ENV TOMCAT_NATIVE_LIBDIR=/usr/local/tomcat/native-jni-lib
# Sun, 04 Jun 2023 16:55:36 GMT
ENV LD_LIBRARY_PATH=/usr/local/tomcat/native-jni-lib
# Sun, 04 Jun 2023 16:57:10 GMT
ENV GPG_KEYS=48F8E69F6390C9F25CFEDCD268248959359E722B A9C5DF4D22E99998D9875A5110C01C5A2F6059E7 DCFD35E0BF8CA7344752DE8B6FB21E8933C60243
# Sun, 04 Jun 2023 16:57:10 GMT
ENV TOMCAT_MAJOR=9
# Sat, 10 Jun 2023 00:37:37 GMT
ENV TOMCAT_VERSION=9.0.76
# Sat, 10 Jun 2023 00:37:38 GMT
ENV TOMCAT_SHA512=028163cbe15367f0ab60e086b0ebc8d774e62d126d82ae9152f863d4680e280b11c9503e3b51ee7089ca9bea1bfa5b535b244a727a3021e5fa72dd7e9569af9a
# Sat, 10 Jun 2023 00:37:38 GMT
COPY dir:f5743ecd98d7370b36812d144a58b18db659a92f2246413d17bb7f46eed37cf7 in /usr/local/tomcat 
# Sat, 10 Jun 2023 00:37:42 GMT
RUN set -eux; 	apt-get update; 	xargs -rt apt-get install -y --no-install-recommends < "$TOMCAT_NATIVE_LIBDIR/.dependencies.txt"; 	rm -rf /var/lib/apt/lists/*
# Sat, 10 Jun 2023 00:37:44 GMT
RUN set -eux; 	nativeLines="$(catalina.sh configtest 2>&1)"; 	nativeLines="$(echo "$nativeLines" | grep 'Apache Tomcat Native')"; 	nativeLines="$(echo "$nativeLines" | sort -u)"; 	if ! echo "$nativeLines" | grep -E 'INFO: Loaded( APR based)? Apache Tomcat Native library' >&2; then 		echo >&2 "$nativeLines"; 		exit 1; 	fi
# Sat, 10 Jun 2023 00:37:44 GMT
EXPOSE 8080
# Sat, 10 Jun 2023 00:37:44 GMT
CMD ["catalina.sh" "run"]
# Sat, 10 Jun 2023 01:05:13 GMT
LABEL org.opencontainers.image.authors=XWiki Development Team <committers@xwiki.org>
# Sat, 10 Jun 2023 01:05:13 GMT
LABEL org.opencontainers.image.url=https://hub.docker.com/_/xwiki
# Sat, 10 Jun 2023 01:05:13 GMT
LABEL org.opencontainers.image.documentation=https://hub.docker.com/_/xwiki
# Sat, 10 Jun 2023 01:05:13 GMT
LABEL org.opencontainers.image.source=https://github.com/xwiki/xwiki-docker.git
# Sat, 10 Jun 2023 01:05:13 GMT
LABEL org.opencontainers.image.vendor=xwiki.org
# Sat, 10 Jun 2023 01:05:13 GMT
LABEL org.opencontainers.image.licenses=LGPL-2.1
# Sat, 10 Jun 2023 01:06:56 GMT
RUN apt-get update &&   apt-get --no-install-recommends -y install     curl     libreoffice     unzip     procps &&   rm -rf /var/lib/apt/lists/*
# Sat, 10 Jun 2023 01:06:57 GMT
ENV XWIKI_VERSION=15.4
# Sat, 10 Jun 2023 01:06:57 GMT
ENV XWIKI_URL_PREFIX=https://maven.xwiki.org/releases/org/xwiki/platform/xwiki-platform-distribution-war/15.4
# Sat, 10 Jun 2023 01:06:57 GMT
ENV XWIKI_DOWNLOAD_SHA256=f24def5b4e3f97c56ed03d5983766028676d6ce205bd60d3798352be5a050505
# Sat, 10 Jun 2023 01:07:35 GMT
RUN rm -rf /usr/local/tomcat/webapps/* &&   mkdir -p /usr/local/tomcat/temp &&   mkdir -p /usr/local/xwiki/data &&   curl -fSL "${XWIKI_URL_PREFIX}/xwiki-platform-distribution-war-${XWIKI_VERSION}.war" -o xwiki.war &&   echo "$XWIKI_DOWNLOAD_SHA256 xwiki.war" | sha256sum -c - &&   unzip -d /usr/local/tomcat/webapps/ROOT xwiki.war &&   rm -f xwiki.war
# Sat, 10 Jun 2023 01:07:36 GMT
ENV MYSQL_JDBC_VERSION=8.0.33
# Sat, 10 Jun 2023 01:07:36 GMT
ENV MYSQL_JDBC_SHA256=e2a3b2fc726a1ac64e998585db86b30fa8bf3f706195b78bb77c5f99bf877bd9
# Sat, 10 Jun 2023 01:07:36 GMT
ENV MYSQL_JDBC_PREFIX=https://repo1.maven.org/maven2/com/mysql/mysql-connector-j/8.0.33
# Sat, 10 Jun 2023 01:07:36 GMT
ENV MYSQL_JDBC_ARTIFACT=mysql-connector-j-8.0.33.jar
# Sat, 10 Jun 2023 01:07:36 GMT
ENV MYSQL_JDBC_TARGET=/usr/local/tomcat/webapps/ROOT/WEB-INF/lib/mysql-connector-j-8.0.33.jar
# Sat, 10 Jun 2023 01:07:37 GMT
RUN curl -fSL "${MYSQL_JDBC_PREFIX}/${MYSQL_JDBC_ARTIFACT}" -o $MYSQL_JDBC_TARGET &&   echo "$MYSQL_JDBC_SHA256 $MYSQL_JDBC_TARGET" | sha256sum -c -
# Sat, 10 Jun 2023 01:07:37 GMT
COPY file:0a1be11e2eb610a1dbcd415404e3a592641110b93090030cb831e3a19a163017 in /usr/local/tomcat/bin/ 
# Sat, 10 Jun 2023 01:07:37 GMT
COPY file:1b8409986f3e4eb79a7a0b18472cb2692a61d504fb5ef34292bc997b79fd760d in /usr/local/tomcat/webapps/ROOT/WEB-INF/hibernate.cfg.xml 
# Sat, 10 Jun 2023 01:07:38 GMT
RUN sed -i 's/<id>org.xwiki.platform:xwiki-platform-distribution-war/<id>org.xwiki.platform:xwiki-platform-distribution-docker/'   /usr/local/tomcat/webapps/ROOT/META-INF/extension.xed
# Sat, 10 Jun 2023 01:07:38 GMT
COPY file:a47c4dcd87c9dad97aff38c49188357e6193bcad50757e516cfb08a60d4de611 in /usr/local/bin/docker-entrypoint.sh 
# Sat, 10 Jun 2023 01:07:38 GMT
VOLUME [/usr/local/xwiki]
# Sat, 10 Jun 2023 01:07:38 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Sat, 10 Jun 2023 01:07:38 GMT
CMD ["xwiki"]
```

-	Layers:
	-	`sha256:d1669123f28121211977ed38e663dca1a397c0c001e5386598b96c89b1b1cd51`  
		Last Modified: Mon, 22 May 2023 20:49:59 GMT  
		Size: 30.4 MB (30430275 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7723b4ddeaefdff460e5e80fa453e1cc3a321b38d941490f9670da9ac646375b`  
		Last Modified: Fri, 02 Jun 2023 01:46:39 GMT  
		Size: 12.5 MB (12493726 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:42e8f29e341c2149d867915e16854b80377147f6a9051f61d5d926ccb70dbe17`  
		Last Modified: Fri, 02 Jun 2023 01:47:46 GMT  
		Size: 46.7 MB (46666187 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2b4e47f3a63c4e338b2efb84d399d9807797b5705ffb8ca8ce9c8214cff3e137`  
		Last Modified: Fri, 02 Jun 2023 01:47:40 GMT  
		Size: 161.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5be4cbf958f0b2c2d0a7a700e3e5fc426dc018b5921f4dce4c3c2e05eb63c3d2`  
		Last Modified: Sun, 04 Jun 2023 17:04:49 GMT  
		Size: 173.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6b91cbe0927f4b2ceb2b992bbdf934995afaa25ee50112bf7fae16106f4e8497`  
		Last Modified: Sat, 10 Jun 2023 00:45:50 GMT  
		Size: 12.3 MB (12269587 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f620e68e7ae8dd7fa78c72bd2ac1ead80035fb84612fb65d520412aa49f51f5d`  
		Last Modified: Sat, 10 Jun 2023 00:45:50 GMT  
		Size: 3.0 MB (2966238 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b376fe98716bdf23a75dc54def95710cce46769b72f2f884575b6ce41b36f5d4`  
		Last Modified: Sat, 10 Jun 2023 00:45:49 GMT  
		Size: 130.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7fa37bcb786538d937cc96b88ac0bcf25b6fec71e052c5ab8f1006039ff2fac2`  
		Last Modified: Sat, 10 Jun 2023 01:11:46 GMT  
		Size: 178.3 MB (178333271 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:20025eeb11226cd5f150afde796870f5d5bdbb8574e91340f0f9cb388868648f`  
		Last Modified: Sat, 10 Jun 2023 01:11:38 GMT  
		Size: 306.8 MB (306779664 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a858077148f25c3a4c59a20f664718c92be71a19cd6c4c5fdfedd3c1606403bb`  
		Last Modified: Sat, 10 Jun 2023 01:11:21 GMT  
		Size: 2.3 MB (2343671 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:06d8a2edd1481c0b8e63fb4ffbb08baf5c7e91091fec14473212dfce7d7f2e69`  
		Last Modified: Sat, 10 Jun 2023 01:11:21 GMT  
		Size: 1.3 KB (1346 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c7c3e2b9a1ae5911fd7f69944c4ffe363fb5291d09cf52c983e93a35acdabb2c`  
		Last Modified: Sat, 10 Jun 2023 01:11:21 GMT  
		Size: 2.3 KB (2309 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:89b8d279b11309ad960421fb110694ca253a0a46253a8d188c0c1a24f2b1bcaf`  
		Last Modified: Sat, 10 Jun 2023 01:11:21 GMT  
		Size: 6.0 KB (5997 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:389263bfe7a239395c34a74dc121510f28d944f3b103f95e2ad5df1eeadb4804`  
		Last Modified: Sat, 10 Jun 2023 01:11:22 GMT  
		Size: 2.5 KB (2504 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `xwiki:stable-mysql-tomcat` - linux; arm64 variant v8

```console
$ docker pull xwiki@sha256:c50f2a98c9156137c1cc406c585b607147b4dd9eb086cdfd2b170a76aedc98b9
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **581.1 MB (581091728 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:806c3e9df9b2e5396d792d4b7c5818d11604ad7e6aec7cd5282a96d59418ecaa`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["xwiki"]`

```dockerfile
# Mon, 05 Jun 2023 17:11:17 GMT
ARG RELEASE
# Mon, 05 Jun 2023 17:11:17 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Mon, 05 Jun 2023 17:11:17 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Mon, 05 Jun 2023 17:11:17 GMT
LABEL org.opencontainers.image.version=22.04
# Mon, 05 Jun 2023 17:11:19 GMT
ADD file:1043594b482384e967c94378b65ec4bc7a38190649a94f0325b7fb00be0a623e in / 
# Mon, 05 Jun 2023 17:11:19 GMT
CMD ["/bin/bash"]
# Fri, 16 Jun 2023 02:45:39 GMT
ENV JAVA_HOME=/opt/java/openjdk
# Fri, 16 Jun 2023 02:45:39 GMT
ENV PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Fri, 16 Jun 2023 02:45:39 GMT
ENV LANG=en_US.UTF-8 LANGUAGE=en_US:en LC_ALL=en_US.UTF-8
# Fri, 16 Jun 2023 02:46:02 GMT
RUN apt-get update     && DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends tzdata curl wget ca-certificates fontconfig locales     && echo "en_US.UTF-8 UTF-8" >> /etc/locale.gen     && locale-gen en_US.UTF-8     && rm -rf /var/lib/apt/lists/*
# Fri, 16 Jun 2023 02:46:41 GMT
ENV JAVA_VERSION=jdk-11.0.19+7
# Fri, 16 Jun 2023 02:47:10 GMT
RUN set -eux;     ARCH="$(dpkg --print-architecture)";     case "${ARCH}" in        aarch64|arm64)          ESUM='1fe4b20d808f393422610818711c728331992a4455eeeb061d3d05b45412771d';          BINARY_URL='https://github.com/adoptium/temurin11-binaries/releases/download/jdk-11.0.19%2B7/OpenJDK11U-jre_aarch64_linux_hotspot_11.0.19_7.tar.gz';          ;;        armhf|arm)          ESUM='cb754b055177381f9f6852b7e5469904a15edddd7f8e136043c28b1e33aee47c';          BINARY_URL='https://github.com/adoptium/temurin11-binaries/releases/download/jdk-11.0.19%2B7/OpenJDK11U-jre_arm_linux_hotspot_11.0.19_7.tar.gz';          ;;        ppc64el|powerpc:common64)          ESUM='8019d938e5525938ec8e68e2989c4413263b0d9b7b3f20fe0c45f6d967919cfb';          BINARY_URL='https://github.com/adoptium/temurin11-binaries/releases/download/jdk-11.0.19%2B7/OpenJDK11U-jre_ppc64le_linux_hotspot_11.0.19_7.tar.gz';          ;;        s390x|s390:64-bit)          ESUM='058419435fe6212d1bc305a14f578c314f9ff9a2d96d523c178120e84231c733';          BINARY_URL='https://github.com/adoptium/temurin11-binaries/releases/download/jdk-11.0.19%2B7/OpenJDK11U-jre_s390x_linux_hotspot_11.0.19_7.tar.gz';          ;;        amd64|i386:x86-64)          ESUM='32dcf760664f93531594b72ce9226e9216567de5705a23c9ff5a77c797948054';          BINARY_URL='https://github.com/adoptium/temurin11-binaries/releases/download/jdk-11.0.19%2B7/OpenJDK11U-jre_x64_linux_hotspot_11.0.19_7.tar.gz';          ;;        *)          echo "Unsupported arch: ${ARCH}";          exit 1;          ;;     esac; 	  wget -O /tmp/openjdk.tar.gz ${BINARY_URL}; 	  echo "${ESUM} */tmp/openjdk.tar.gz" | sha256sum -c -; 	  mkdir -p "$JAVA_HOME"; 	  tar --extract 	      --file /tmp/openjdk.tar.gz 	      --directory "$JAVA_HOME" 	      --strip-components 1 	      --no-same-owner 	  ;     rm -f /tmp/openjdk.tar.gz ${JAVA_HOME}/src.zip;     find "$JAVA_HOME/lib" -name '*.so' -exec dirname '{}' ';' | sort -u > /etc/ld.so.conf.d/docker-openjdk.conf;     ldconfig;     java -Xshare:dump;
# Fri, 16 Jun 2023 02:47:11 GMT
RUN echo Verifying install ...     && fileEncoding="$(echo 'System.out.println(System.getProperty("file.encoding"))' | jshell -s -)"; [ "$fileEncoding" = 'UTF-8' ]; rm -rf ~/.java     && echo java --version && java --version     && echo Complete.
# Fri, 16 Jun 2023 06:03:56 GMT
ENV CATALINA_HOME=/usr/local/tomcat
# Fri, 16 Jun 2023 06:03:56 GMT
ENV PATH=/usr/local/tomcat/bin:/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Fri, 16 Jun 2023 06:03:57 GMT
RUN mkdir -p "$CATALINA_HOME"
# Fri, 16 Jun 2023 06:03:57 GMT
WORKDIR /usr/local/tomcat
# Fri, 16 Jun 2023 06:03:57 GMT
ENV TOMCAT_NATIVE_LIBDIR=/usr/local/tomcat/native-jni-lib
# Fri, 16 Jun 2023 06:03:57 GMT
ENV LD_LIBRARY_PATH=/usr/local/tomcat/native-jni-lib
# Fri, 16 Jun 2023 06:06:03 GMT
ENV GPG_KEYS=48F8E69F6390C9F25CFEDCD268248959359E722B A9C5DF4D22E99998D9875A5110C01C5A2F6059E7 DCFD35E0BF8CA7344752DE8B6FB21E8933C60243
# Fri, 16 Jun 2023 06:06:03 GMT
ENV TOMCAT_MAJOR=9
# Fri, 16 Jun 2023 06:06:03 GMT
ENV TOMCAT_VERSION=9.0.76
# Fri, 16 Jun 2023 06:06:03 GMT
ENV TOMCAT_SHA512=028163cbe15367f0ab60e086b0ebc8d774e62d126d82ae9152f863d4680e280b11c9503e3b51ee7089ca9bea1bfa5b535b244a727a3021e5fa72dd7e9569af9a
# Fri, 16 Jun 2023 06:06:03 GMT
COPY dir:ade7cc9ad5c9e30d6dd85f01942565a28f1c051dbaec50c5d97968ad63e754ee in /usr/local/tomcat 
# Fri, 16 Jun 2023 06:06:07 GMT
RUN set -eux; 	apt-get update; 	xargs -rt apt-get install -y --no-install-recommends < "$TOMCAT_NATIVE_LIBDIR/.dependencies.txt"; 	rm -rf /var/lib/apt/lists/*
# Fri, 16 Jun 2023 06:06:08 GMT
RUN set -eux; 	nativeLines="$(catalina.sh configtest 2>&1)"; 	nativeLines="$(echo "$nativeLines" | grep 'Apache Tomcat Native')"; 	nativeLines="$(echo "$nativeLines" | sort -u)"; 	if ! echo "$nativeLines" | grep -E 'INFO: Loaded( APR based)? Apache Tomcat Native library' >&2; then 		echo >&2 "$nativeLines"; 		exit 1; 	fi
# Fri, 16 Jun 2023 06:06:08 GMT
EXPOSE 8080
# Fri, 16 Jun 2023 06:06:08 GMT
CMD ["catalina.sh" "run"]
# Fri, 16 Jun 2023 08:35:02 GMT
LABEL org.opencontainers.image.authors=XWiki Development Team <committers@xwiki.org>
# Fri, 16 Jun 2023 08:35:02 GMT
LABEL org.opencontainers.image.url=https://hub.docker.com/_/xwiki
# Fri, 16 Jun 2023 08:35:02 GMT
LABEL org.opencontainers.image.documentation=https://hub.docker.com/_/xwiki
# Fri, 16 Jun 2023 08:35:02 GMT
LABEL org.opencontainers.image.source=https://github.com/xwiki/xwiki-docker.git
# Fri, 16 Jun 2023 08:35:02 GMT
LABEL org.opencontainers.image.vendor=xwiki.org
# Fri, 16 Jun 2023 08:35:03 GMT
LABEL org.opencontainers.image.licenses=LGPL-2.1
# Fri, 16 Jun 2023 08:37:02 GMT
RUN apt-get update &&   apt-get --no-install-recommends -y install     curl     libreoffice     unzip     procps &&   rm -rf /var/lib/apt/lists/*
# Fri, 16 Jun 2023 08:37:05 GMT
ENV XWIKI_VERSION=15.4
# Fri, 16 Jun 2023 08:37:05 GMT
ENV XWIKI_URL_PREFIX=https://maven.xwiki.org/releases/org/xwiki/platform/xwiki-platform-distribution-war/15.4
# Fri, 16 Jun 2023 08:37:05 GMT
ENV XWIKI_DOWNLOAD_SHA256=f24def5b4e3f97c56ed03d5983766028676d6ce205bd60d3798352be5a050505
# Fri, 16 Jun 2023 08:37:45 GMT
RUN rm -rf /usr/local/tomcat/webapps/* &&   mkdir -p /usr/local/tomcat/temp &&   mkdir -p /usr/local/xwiki/data &&   curl -fSL "${XWIKI_URL_PREFIX}/xwiki-platform-distribution-war-${XWIKI_VERSION}.war" -o xwiki.war &&   echo "$XWIKI_DOWNLOAD_SHA256 xwiki.war" | sha256sum -c - &&   unzip -d /usr/local/tomcat/webapps/ROOT xwiki.war &&   rm -f xwiki.war
# Fri, 16 Jun 2023 08:37:48 GMT
ENV MYSQL_JDBC_VERSION=8.0.33
# Fri, 16 Jun 2023 08:37:48 GMT
ENV MYSQL_JDBC_SHA256=e2a3b2fc726a1ac64e998585db86b30fa8bf3f706195b78bb77c5f99bf877bd9
# Fri, 16 Jun 2023 08:37:48 GMT
ENV MYSQL_JDBC_PREFIX=https://repo1.maven.org/maven2/com/mysql/mysql-connector-j/8.0.33
# Fri, 16 Jun 2023 08:37:48 GMT
ENV MYSQL_JDBC_ARTIFACT=mysql-connector-j-8.0.33.jar
# Fri, 16 Jun 2023 08:37:48 GMT
ENV MYSQL_JDBC_TARGET=/usr/local/tomcat/webapps/ROOT/WEB-INF/lib/mysql-connector-j-8.0.33.jar
# Fri, 16 Jun 2023 08:37:49 GMT
RUN curl -fSL "${MYSQL_JDBC_PREFIX}/${MYSQL_JDBC_ARTIFACT}" -o $MYSQL_JDBC_TARGET &&   echo "$MYSQL_JDBC_SHA256 $MYSQL_JDBC_TARGET" | sha256sum -c -
# Fri, 16 Jun 2023 08:37:49 GMT
COPY file:0a1be11e2eb610a1dbcd415404e3a592641110b93090030cb831e3a19a163017 in /usr/local/tomcat/bin/ 
# Fri, 16 Jun 2023 08:37:49 GMT
COPY file:1b8409986f3e4eb79a7a0b18472cb2692a61d504fb5ef34292bc997b79fd760d in /usr/local/tomcat/webapps/ROOT/WEB-INF/hibernate.cfg.xml 
# Fri, 16 Jun 2023 08:37:49 GMT
RUN sed -i 's/<id>org.xwiki.platform:xwiki-platform-distribution-war/<id>org.xwiki.platform:xwiki-platform-distribution-docker/'   /usr/local/tomcat/webapps/ROOT/META-INF/extension.xed
# Fri, 16 Jun 2023 08:37:50 GMT
COPY file:a47c4dcd87c9dad97aff38c49188357e6193bcad50757e516cfb08a60d4de611 in /usr/local/bin/docker-entrypoint.sh 
# Fri, 16 Jun 2023 08:37:50 GMT
VOLUME [/usr/local/xwiki]
# Fri, 16 Jun 2023 08:37:50 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 16 Jun 2023 08:37:50 GMT
CMD ["xwiki"]
```

-	Layers:
	-	`sha256:a1df1d4a17c6a461a5967be8a40f1158e55e0ae4dc3b3b7ae64f57cae69eb7e7`  
		Last Modified: Wed, 07 Jun 2023 02:07:18 GMT  
		Size: 28.4 MB (28389201 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f1a707fe2fc3c87da15576bd7b678fe8f2591ad481cc638b8cfe52664b47d2cf`  
		Last Modified: Fri, 16 Jun 2023 02:49:56 GMT  
		Size: 12.5 MB (12454449 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:86e5488ab47450fbd12fc724963811b99580bfe1e5f44267a03736f0adea506b`  
		Last Modified: Fri, 16 Jun 2023 02:51:36 GMT  
		Size: 45.0 MB (45009402 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bf2dbf45ca92463ef69ad1ef7fb34bb5123ea7a7fdfe4f745d3728e89f260617`  
		Last Modified: Fri, 16 Jun 2023 02:51:31 GMT  
		Size: 160.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fd63c7176205cf09ac548a367dddd2f6f019a7d200c8afd95f8806dd6e47cf49`  
		Last Modified: Fri, 16 Jun 2023 06:15:57 GMT  
		Size: 173.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ec810a75a4132859409a64079a8a3388cb47f6cf638cec13415a9bdca18179bd`  
		Last Modified: Fri, 16 Jun 2023 06:18:10 GMT  
		Size: 12.3 MB (12275748 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5f82a4b0d8f6c942299bcc19dacf123e877cb30d4a358faca910fd1e9917a14c`  
		Last Modified: Fri, 16 Jun 2023 06:18:09 GMT  
		Size: 454.1 KB (454065 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:aa40c7c4be196f78a1f23cd4b958024a8c3d48953124bb018f4631fb06e1696c`  
		Last Modified: Fri, 16 Jun 2023 06:18:09 GMT  
		Size: 131.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b18d0affa9f4dbdfae82ef0d4e03f23989200b105e1d2da696dff48a97732af0`  
		Last Modified: Fri, 16 Jun 2023 08:41:40 GMT  
		Size: 173.4 MB (173372940 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f03776b4882b6f6d330e510053310c11bf6f4dd035683bdb06458c992b9641c0`  
		Last Modified: Fri, 16 Jun 2023 08:41:35 GMT  
		Size: 306.8 MB (306779625 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2d0f62e0f8ff87885d71e62f1d3075651c0cfed2d0e7caa20c27feef442c99f3`  
		Last Modified: Fri, 16 Jun 2023 08:41:22 GMT  
		Size: 2.3 MB (2343672 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4f84d4985682d267f22185c1b4d2dd723c4b31b8589cf7636fa4ccec262f4036`  
		Last Modified: Fri, 16 Jun 2023 08:41:21 GMT  
		Size: 1.3 KB (1345 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ccbcf89c37d3ab64d123f5e2e0bfe0d0c87e59ead46b083a89e77403a6fde708`  
		Last Modified: Fri, 16 Jun 2023 08:41:22 GMT  
		Size: 2.3 KB (2313 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:50699bbfbf450579b87b16c0bda85979e35e246199c33d6e15f1cfd540227046`  
		Last Modified: Fri, 16 Jun 2023 08:41:21 GMT  
		Size: 6.0 KB (5998 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:63714c0eb9ed1f6486ac518822e236452aaefb1496b483d60a87ef50a2a9c84a`  
		Last Modified: Fri, 16 Jun 2023 08:41:21 GMT  
		Size: 2.5 KB (2506 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
