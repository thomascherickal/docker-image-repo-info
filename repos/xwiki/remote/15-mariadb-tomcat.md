## `xwiki:15-mariadb-tomcat`

```console
$ docker pull xwiki@sha256:fa0133ed372c58319f68af3dce4460ea2f8db63f5b9354cd6a6a27a9e83b6fb6
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `xwiki:15-mariadb-tomcat` - linux; amd64

```console
$ docker pull xwiki@sha256:87a7037d74e1d21a27faa38e9c67435ba322c56f2d3ca88a482e1cd508b7ad96
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **591.1 MB (591114334 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:5befb92c0fc8952a72ab1a17905e3b59b86c758f0ffba14ed260758d3ea8a325`
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
# Wed, 16 Aug 2023 15:39:50 GMT
ENV JAVA_VERSION=jdk-11.0.20+8
# Wed, 16 Aug 2023 15:40:18 GMT
RUN set -eux;     ARCH="$(dpkg --print-architecture)";     case "${ARCH}" in        aarch64|arm64)          ESUM='45e190920fb3ec61ee5213a7bd98553abf2ae7692eb9daa504fcdc9d59a7cfc4';          BINARY_URL='https://github.com/adoptium/temurin11-binaries/releases/download/jdk-11.0.20%2B8/OpenJDK11U-jre_aarch64_linux_hotspot_11.0.20_8.tar.gz';          ;;        armhf|arm)          ESUM='1e2a02364084b2d054e88a871f3efaa4450ae4f087b8f806fd95c15d5affcc7b';          BINARY_URL='https://github.com/adoptium/temurin11-binaries/releases/download/jdk-11.0.20%2B8/OpenJDK11U-jre_arm_linux_hotspot_11.0.20_8.tar.gz';          ;;        ppc64el|powerpc:common64)          ESUM='61034834b61bf080392218b25dcac2d9e3505b5e4f53539704d496be4181aadf';          BINARY_URL='https://github.com/adoptium/temurin11-binaries/releases/download/jdk-11.0.20%2B8/OpenJDK11U-jre_ppc64le_linux_hotspot_11.0.20_8.tar.gz';          ;;        s390x|s390:64-bit)          ESUM='0c7050976914e0613179446de62bb20d2845ae809f6d31bc0ed8d136f8fd3d9b';          BINARY_URL='https://github.com/adoptium/temurin11-binaries/releases/download/jdk-11.0.20%2B8/OpenJDK11U-jre_s390x_linux_hotspot_11.0.20_8.tar.gz';          ;;        amd64|i386:x86-64)          ESUM='ffb070c26ea22771f78769c569c9db3412e6486434dc6df1fd3c3438285766e7';          BINARY_URL='https://github.com/adoptium/temurin11-binaries/releases/download/jdk-11.0.20%2B8/OpenJDK11U-jre_x64_linux_hotspot_11.0.20_8.tar.gz';          ;;        *)          echo "Unsupported arch: ${ARCH}";          exit 1;          ;;     esac; 	  wget -O /tmp/openjdk.tar.gz ${BINARY_URL}; 	  echo "${ESUM} */tmp/openjdk.tar.gz" | sha256sum -c -; 	  mkdir -p "$JAVA_HOME"; 	  tar --extract 	      --file /tmp/openjdk.tar.gz 	      --directory "$JAVA_HOME" 	      --strip-components 1 	      --no-same-owner 	  ;     rm -f /tmp/openjdk.tar.gz ${JAVA_HOME}/lib/src.zip;     find "$JAVA_HOME/lib" -name '*.so' -exec dirname '{}' ';' | sort -u > /etc/ld.so.conf.d/docker-openjdk.conf;     ldconfig;     java -Xshare:dump;
# Wed, 16 Aug 2023 15:40:19 GMT
RUN echo Verifying install ...     && fileEncoding="$(echo 'System.out.println(System.getProperty("file.encoding"))' | jshell -s -)"; [ "$fileEncoding" = 'UTF-8' ]; rm -rf ~/.java     && echo java --version && java --version     && echo Complete.
# Wed, 16 Aug 2023 15:40:19 GMT
COPY file:8b8864b3e02a33a579dc216fd51b28a6047bc8eeaa03045b258980fe0cf7fcb3 in /__cacert_entrypoint.sh 
# Wed, 16 Aug 2023 15:40:19 GMT
ENTRYPOINT ["/__cacert_entrypoint.sh"]
# Wed, 16 Aug 2023 18:25:22 GMT
ENV CATALINA_HOME=/usr/local/tomcat
# Wed, 16 Aug 2023 18:25:22 GMT
ENV PATH=/usr/local/tomcat/bin:/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 16 Aug 2023 18:25:22 GMT
RUN mkdir -p "$CATALINA_HOME"
# Wed, 16 Aug 2023 18:25:22 GMT
WORKDIR /usr/local/tomcat
# Wed, 16 Aug 2023 18:25:22 GMT
ENV TOMCAT_NATIVE_LIBDIR=/usr/local/tomcat/native-jni-lib
# Wed, 16 Aug 2023 18:25:22 GMT
ENV LD_LIBRARY_PATH=/usr/local/tomcat/native-jni-lib
# Wed, 16 Aug 2023 18:28:59 GMT
ENV GPG_KEYS=48F8E69F6390C9F25CFEDCD268248959359E722B A9C5DF4D22E99998D9875A5110C01C5A2F6059E7 DCFD35E0BF8CA7344752DE8B6FB21E8933C60243
# Wed, 16 Aug 2023 18:28:59 GMT
ENV TOMCAT_MAJOR=9
# Sat, 26 Aug 2023 04:22:38 GMT
ENV TOMCAT_VERSION=9.0.80
# Sat, 26 Aug 2023 04:22:38 GMT
ENV TOMCAT_SHA512=24014441b0ccdd2dda238efa56e1a039476488943e6cf04f8a372a340a49dd21ce174ed68e2f5fcc43401e85fae6d00c5eac3d357653e91601737b6fa94476de
# Sat, 26 Aug 2023 04:22:39 GMT
COPY dir:c8a5e7fd2978cf1536b5c3ed0b313302e914d05bd8f5538b7efce8481bc019d1 in /usr/local/tomcat 
# Sat, 26 Aug 2023 04:22:43 GMT
RUN set -eux; 	apt-get update; 	xargs -rt apt-get install -y --no-install-recommends < "$TOMCAT_NATIVE_LIBDIR/.dependencies.txt"; 	rm -rf /var/lib/apt/lists/*
# Sat, 26 Aug 2023 04:22:44 GMT
RUN set -eux; 	nativeLines="$(catalina.sh configtest 2>&1)"; 	nativeLines="$(echo "$nativeLines" | grep 'Apache Tomcat Native')"; 	nativeLines="$(echo "$nativeLines" | sort -u)"; 	if ! echo "$nativeLines" | grep -E 'INFO: Loaded( APR based)? Apache Tomcat Native library' >&2; then 		echo >&2 "$nativeLines"; 		exit 1; 	fi
# Sat, 26 Aug 2023 04:22:44 GMT
EXPOSE 8080
# Sat, 26 Aug 2023 04:22:44 GMT
ENTRYPOINT []
# Sat, 26 Aug 2023 04:22:44 GMT
CMD ["catalina.sh" "run"]
# Sat, 26 Aug 2023 05:19:34 GMT
LABEL org.opencontainers.image.authors=XWiki Development Team <committers@xwiki.org>
# Sat, 26 Aug 2023 05:19:34 GMT
LABEL org.opencontainers.image.url=https://hub.docker.com/_/xwiki
# Sat, 26 Aug 2023 05:19:34 GMT
LABEL org.opencontainers.image.documentation=https://hub.docker.com/_/xwiki
# Sat, 26 Aug 2023 05:19:34 GMT
LABEL org.opencontainers.image.source=https://github.com/xwiki/xwiki-docker.git
# Sat, 26 Aug 2023 05:19:34 GMT
LABEL org.opencontainers.image.vendor=xwiki.org
# Sat, 26 Aug 2023 05:19:35 GMT
LABEL org.opencontainers.image.licenses=LGPL-2.1
# Sat, 26 Aug 2023 05:21:13 GMT
RUN apt-get update &&   apt-get --no-install-recommends -y install     curl     libreoffice     unzip     procps &&   rm -rf /var/lib/apt/lists/*
# Tue, 29 Aug 2023 19:02:24 GMT
ENV XWIKI_VERSION=15.7
# Tue, 29 Aug 2023 19:02:24 GMT
ENV XWIKI_URL_PREFIX=https://maven.xwiki.org/releases/org/xwiki/platform/xwiki-platform-distribution-war/15.7
# Tue, 29 Aug 2023 19:02:24 GMT
ENV XWIKI_DOWNLOAD_SHA256=f4c725d1b5b184693cec0477910d0a238747265820aade23961d6578f7000b64
# Tue, 29 Aug 2023 19:03:04 GMT
RUN rm -rf /usr/local/tomcat/webapps/* &&   mkdir -p /usr/local/tomcat/temp &&   mkdir -p /usr/local/xwiki/data &&   curl -fSL "${XWIKI_URL_PREFIX}/xwiki-platform-distribution-war-${XWIKI_VERSION}.war" -o xwiki.war &&   echo "$XWIKI_DOWNLOAD_SHA256 xwiki.war" | sha256sum -c - &&   unzip -d /usr/local/tomcat/webapps/ROOT xwiki.war &&   rm -f xwiki.war
# Tue, 29 Aug 2023 19:04:02 GMT
ENV MARIADB_JDBC_VERSION=3.2.0
# Tue, 29 Aug 2023 19:04:02 GMT
ENV MARIADB_JDBC_SHA256=adf9df10bc9b2a137def36d6a495812258f430d4a8f7946727c61558e6c73941
# Tue, 29 Aug 2023 19:04:02 GMT
ENV MARIADB_JDBC_PREFIX=https://repo1.maven.org/maven2/org/mariadb/jdbc/mariadb-java-client/3.2.0
# Tue, 29 Aug 2023 19:04:02 GMT
ENV MARIADB_JDBC_ARTIFACT=mariadb-java-client-3.2.0.jar
# Tue, 29 Aug 2023 19:04:02 GMT
ENV MARIADB_JDBC_TARGET=/usr/local/tomcat/webapps/ROOT/WEB-INF/lib/mariadb-java-client-3.2.0.jar
# Tue, 29 Aug 2023 19:04:03 GMT
RUN curl -fSL "${MARIADB_JDBC_PREFIX}/${MARIADB_JDBC_ARTIFACT}" -o $MARIADB_JDBC_TARGET &&   echo "$MARIADB_JDBC_SHA256 $MARIADB_JDBC_TARGET" | sha256sum -c -
# Tue, 29 Aug 2023 19:04:03 GMT
COPY file:0a1be11e2eb610a1dbcd415404e3a592641110b93090030cb831e3a19a163017 in /usr/local/tomcat/bin/ 
# Tue, 29 Aug 2023 19:04:03 GMT
COPY file:0e237c3876eeb3b5f3473a064d3e507da2df6c228ca714687930b34e3b687601 in /usr/local/tomcat/webapps/ROOT/WEB-INF/hibernate.cfg.xml 
# Tue, 29 Aug 2023 19:04:04 GMT
RUN sed -i 's/<id>org.xwiki.platform:xwiki-platform-distribution-war/<id>org.xwiki.platform:xwiki-platform-distribution-docker/'   /usr/local/tomcat/webapps/ROOT/META-INF/extension.xed
# Tue, 29 Aug 2023 19:04:04 GMT
COPY file:a47c4dcd87c9dad97aff38c49188357e6193bcad50757e516cfb08a60d4de611 in /usr/local/bin/docker-entrypoint.sh 
# Tue, 29 Aug 2023 19:04:04 GMT
VOLUME [/usr/local/xwiki]
# Tue, 29 Aug 2023 19:04:04 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 29 Aug 2023 19:04:04 GMT
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
	-	`sha256:76db90e0ce9d25cc002f8d092e2292c1c473b4d0a637a47964fecd6562d1496c`  
		Last Modified: Wed, 16 Aug 2023 15:44:24 GMT  
		Size: 46.9 MB (46864877 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ec22c511cb5328c056fa06b66a2d37107a40f7de586e81de5d0d342e4914f3fb`  
		Last Modified: Wed, 16 Aug 2023 15:44:18 GMT  
		Size: 159.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d0bf00dc5a1f2a9ebf45c843cd4f488cb34ff027a15353ca144c36014a519c4c`  
		Last Modified: Wed, 16 Aug 2023 15:44:18 GMT  
		Size: 734.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0ae06f310b6e495aa536693202667384704ed7e2ec54713b274609eff806255a`  
		Last Modified: Wed, 16 Aug 2023 18:40:28 GMT  
		Size: 173.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7728269a61fdd2bb66736640c093eed001e15c363b7d5b92e4bec548d75dcd4a`  
		Last Modified: Sat, 26 Aug 2023 04:45:20 GMT  
		Size: 12.3 MB (12285246 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ca7390f4d19e5c99b09b51e6fec4f5e3883d85023a797de829defb7fd1c36c0a`  
		Last Modified: Sat, 26 Aug 2023 04:45:19 GMT  
		Size: 455.6 KB (455606 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:610a6c4c9e5e766cb9f849757df4622c20d3600bcf87b5d2bb8a01df1beff707`  
		Last Modified: Sat, 26 Aug 2023 04:45:19 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9eb589a8467db48f5344ea2b1cff4a73d01987ecd76e2601bf834234bae1ad6b`  
		Last Modified: Sat, 26 Aug 2023 05:27:52 GMT  
		Size: 178.4 MB (178356736 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6d4749d3833df61c5c0be35cc894b136b84ca9f2ff83dd57f3c0c2223413f91a`  
		Last Modified: Tue, 29 Aug 2023 19:05:01 GMT  
		Size: 309.2 MB (309194071 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2ef23fa92ee64b4e3e651d02abe06b895fb39bb35d6cebd8bfe332fa0d973b89`  
		Last Modified: Tue, 29 Aug 2023 19:06:20 GMT  
		Size: 603.4 KB (603392 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:725394594f8346c4f995c59e3f50fb3058fd5e6c20aa01b8f03f3b3ed1700728`  
		Last Modified: Tue, 29 Aug 2023 19:06:19 GMT  
		Size: 1.3 KB (1346 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8d88e8dfd200f75860af08ae4a3018bcc3ba066c9cb67e9a0bb451e82bb4baf6`  
		Last Modified: Tue, 29 Aug 2023 19:06:19 GMT  
		Size: 2.3 KB (2311 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:feed25e23c36f65b19cda028288fa0e786777bed8666e4b2d6241cf74b5d2da2`  
		Last Modified: Tue, 29 Aug 2023 19:06:19 GMT  
		Size: 6.3 KB (6308 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:754d129398c5dc53e706483247350720f69d5b42c301cdc4ff4f888254474d74`  
		Last Modified: Tue, 29 Aug 2023 19:06:19 GMT  
		Size: 2.5 KB (2506 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `xwiki:15-mariadb-tomcat` - linux; arm64 variant v8

```console
$ docker pull xwiki@sha256:976359fe275d040ca2010cfe5fdc13c3da8fb2a67f15e97f5ab8dc6284cd193f
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **582.4 MB (582379970 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:71882e23c365a6ace3d2a157a355932b9a8c99a6155a947d14c544a6acd94481`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["xwiki"]`

```dockerfile
# Fri, 04 Aug 2023 04:51:14 GMT
ARG RELEASE
# Fri, 04 Aug 2023 04:51:14 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Fri, 04 Aug 2023 04:51:14 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Fri, 04 Aug 2023 04:51:14 GMT
LABEL org.opencontainers.image.version=22.04
# Fri, 04 Aug 2023 04:51:18 GMT
ADD file:5cf7797cf86362218d2bd85debeff136ee897af7eef95a0b8baab9f9457c3e89 in / 
# Fri, 04 Aug 2023 04:51:18 GMT
CMD ["/bin/bash"]
# Wed, 16 Aug 2023 14:23:25 GMT
ENV JAVA_HOME=/opt/java/openjdk
# Wed, 16 Aug 2023 14:23:25 GMT
ENV PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 16 Aug 2023 14:23:25 GMT
ENV LANG=en_US.UTF-8 LANGUAGE=en_US:en LC_ALL=en_US.UTF-8
# Wed, 16 Aug 2023 14:23:38 GMT
RUN apt-get update     && DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends tzdata curl wget ca-certificates fontconfig locales p11-kit     && echo "en_US.UTF-8 UTF-8" >> /etc/locale.gen     && locale-gen en_US.UTF-8     && rm -rf /var/lib/apt/lists/*
# Wed, 16 Aug 2023 14:24:03 GMT
ENV JAVA_VERSION=jdk-11.0.20+8
# Wed, 16 Aug 2023 14:24:28 GMT
RUN set -eux;     ARCH="$(dpkg --print-architecture)";     case "${ARCH}" in        aarch64|arm64)          ESUM='45e190920fb3ec61ee5213a7bd98553abf2ae7692eb9daa504fcdc9d59a7cfc4';          BINARY_URL='https://github.com/adoptium/temurin11-binaries/releases/download/jdk-11.0.20%2B8/OpenJDK11U-jre_aarch64_linux_hotspot_11.0.20_8.tar.gz';          ;;        armhf|arm)          ESUM='1e2a02364084b2d054e88a871f3efaa4450ae4f087b8f806fd95c15d5affcc7b';          BINARY_URL='https://github.com/adoptium/temurin11-binaries/releases/download/jdk-11.0.20%2B8/OpenJDK11U-jre_arm_linux_hotspot_11.0.20_8.tar.gz';          ;;        ppc64el|powerpc:common64)          ESUM='61034834b61bf080392218b25dcac2d9e3505b5e4f53539704d496be4181aadf';          BINARY_URL='https://github.com/adoptium/temurin11-binaries/releases/download/jdk-11.0.20%2B8/OpenJDK11U-jre_ppc64le_linux_hotspot_11.0.20_8.tar.gz';          ;;        s390x|s390:64-bit)          ESUM='0c7050976914e0613179446de62bb20d2845ae809f6d31bc0ed8d136f8fd3d9b';          BINARY_URL='https://github.com/adoptium/temurin11-binaries/releases/download/jdk-11.0.20%2B8/OpenJDK11U-jre_s390x_linux_hotspot_11.0.20_8.tar.gz';          ;;        amd64|i386:x86-64)          ESUM='ffb070c26ea22771f78769c569c9db3412e6486434dc6df1fd3c3438285766e7';          BINARY_URL='https://github.com/adoptium/temurin11-binaries/releases/download/jdk-11.0.20%2B8/OpenJDK11U-jre_x64_linux_hotspot_11.0.20_8.tar.gz';          ;;        *)          echo "Unsupported arch: ${ARCH}";          exit 1;          ;;     esac; 	  wget -O /tmp/openjdk.tar.gz ${BINARY_URL}; 	  echo "${ESUM} */tmp/openjdk.tar.gz" | sha256sum -c -; 	  mkdir -p "$JAVA_HOME"; 	  tar --extract 	      --file /tmp/openjdk.tar.gz 	      --directory "$JAVA_HOME" 	      --strip-components 1 	      --no-same-owner 	  ;     rm -f /tmp/openjdk.tar.gz ${JAVA_HOME}/lib/src.zip;     find "$JAVA_HOME/lib" -name '*.so' -exec dirname '{}' ';' | sort -u > /etc/ld.so.conf.d/docker-openjdk.conf;     ldconfig;     java -Xshare:dump;
# Wed, 16 Aug 2023 14:24:28 GMT
RUN echo Verifying install ...     && fileEncoding="$(echo 'System.out.println(System.getProperty("file.encoding"))' | jshell -s -)"; [ "$fileEncoding" = 'UTF-8' ]; rm -rf ~/.java     && echo java --version && java --version     && echo Complete.
# Wed, 16 Aug 2023 14:24:29 GMT
COPY file:8b8864b3e02a33a579dc216fd51b28a6047bc8eeaa03045b258980fe0cf7fcb3 in /__cacert_entrypoint.sh 
# Wed, 16 Aug 2023 14:24:29 GMT
ENTRYPOINT ["/__cacert_entrypoint.sh"]
# Wed, 16 Aug 2023 21:57:50 GMT
ENV CATALINA_HOME=/usr/local/tomcat
# Wed, 16 Aug 2023 21:57:50 GMT
ENV PATH=/usr/local/tomcat/bin:/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 16 Aug 2023 21:57:50 GMT
RUN mkdir -p "$CATALINA_HOME"
# Wed, 16 Aug 2023 21:57:50 GMT
WORKDIR /usr/local/tomcat
# Wed, 16 Aug 2023 21:57:50 GMT
ENV TOMCAT_NATIVE_LIBDIR=/usr/local/tomcat/native-jni-lib
# Wed, 16 Aug 2023 21:57:50 GMT
ENV LD_LIBRARY_PATH=/usr/local/tomcat/native-jni-lib
# Wed, 16 Aug 2023 22:00:58 GMT
ENV GPG_KEYS=48F8E69F6390C9F25CFEDCD268248959359E722B A9C5DF4D22E99998D9875A5110C01C5A2F6059E7 DCFD35E0BF8CA7344752DE8B6FB21E8933C60243
# Wed, 16 Aug 2023 22:00:58 GMT
ENV TOMCAT_MAJOR=9
# Sat, 26 Aug 2023 03:26:04 GMT
ENV TOMCAT_VERSION=9.0.80
# Sat, 26 Aug 2023 03:26:04 GMT
ENV TOMCAT_SHA512=24014441b0ccdd2dda238efa56e1a039476488943e6cf04f8a372a340a49dd21ce174ed68e2f5fcc43401e85fae6d00c5eac3d357653e91601737b6fa94476de
# Sat, 26 Aug 2023 03:26:04 GMT
COPY dir:acacd7d4dad3b8b0f101dd73367b940127d88197b14c7b70758c83b6ce530d36 in /usr/local/tomcat 
# Sat, 26 Aug 2023 03:26:08 GMT
RUN set -eux; 	apt-get update; 	xargs -rt apt-get install -y --no-install-recommends < "$TOMCAT_NATIVE_LIBDIR/.dependencies.txt"; 	rm -rf /var/lib/apt/lists/*
# Sat, 26 Aug 2023 03:26:09 GMT
RUN set -eux; 	nativeLines="$(catalina.sh configtest 2>&1)"; 	nativeLines="$(echo "$nativeLines" | grep 'Apache Tomcat Native')"; 	nativeLines="$(echo "$nativeLines" | sort -u)"; 	if ! echo "$nativeLines" | grep -E 'INFO: Loaded( APR based)? Apache Tomcat Native library' >&2; then 		echo >&2 "$nativeLines"; 		exit 1; 	fi
# Sat, 26 Aug 2023 03:26:09 GMT
EXPOSE 8080
# Sat, 26 Aug 2023 03:26:09 GMT
ENTRYPOINT []
# Sat, 26 Aug 2023 03:26:09 GMT
CMD ["catalina.sh" "run"]
# Sat, 26 Aug 2023 07:26:20 GMT
LABEL org.opencontainers.image.authors=XWiki Development Team <committers@xwiki.org>
# Sat, 26 Aug 2023 07:26:20 GMT
LABEL org.opencontainers.image.url=https://hub.docker.com/_/xwiki
# Sat, 26 Aug 2023 07:26:21 GMT
LABEL org.opencontainers.image.documentation=https://hub.docker.com/_/xwiki
# Sat, 26 Aug 2023 07:26:21 GMT
LABEL org.opencontainers.image.source=https://github.com/xwiki/xwiki-docker.git
# Sat, 26 Aug 2023 07:26:21 GMT
LABEL org.opencontainers.image.vendor=xwiki.org
# Sat, 26 Aug 2023 07:26:21 GMT
LABEL org.opencontainers.image.licenses=LGPL-2.1
# Sat, 26 Aug 2023 07:28:23 GMT
RUN apt-get update &&   apt-get --no-install-recommends -y install     curl     libreoffice     unzip     procps &&   rm -rf /var/lib/apt/lists/*
# Tue, 29 Aug 2023 18:03:16 GMT
ENV XWIKI_VERSION=15.7
# Tue, 29 Aug 2023 18:03:16 GMT
ENV XWIKI_URL_PREFIX=https://maven.xwiki.org/releases/org/xwiki/platform/xwiki-platform-distribution-war/15.7
# Tue, 29 Aug 2023 18:03:16 GMT
ENV XWIKI_DOWNLOAD_SHA256=f4c725d1b5b184693cec0477910d0a238747265820aade23961d6578f7000b64
# Tue, 29 Aug 2023 18:03:58 GMT
RUN rm -rf /usr/local/tomcat/webapps/* &&   mkdir -p /usr/local/tomcat/temp &&   mkdir -p /usr/local/xwiki/data &&   curl -fSL "${XWIKI_URL_PREFIX}/xwiki-platform-distribution-war-${XWIKI_VERSION}.war" -o xwiki.war &&   echo "$XWIKI_DOWNLOAD_SHA256 xwiki.war" | sha256sum -c - &&   unzip -d /usr/local/tomcat/webapps/ROOT xwiki.war &&   rm -f xwiki.war
# Tue, 29 Aug 2023 18:05:02 GMT
ENV MARIADB_JDBC_VERSION=3.2.0
# Tue, 29 Aug 2023 18:05:02 GMT
ENV MARIADB_JDBC_SHA256=adf9df10bc9b2a137def36d6a495812258f430d4a8f7946727c61558e6c73941
# Tue, 29 Aug 2023 18:05:02 GMT
ENV MARIADB_JDBC_PREFIX=https://repo1.maven.org/maven2/org/mariadb/jdbc/mariadb-java-client/3.2.0
# Tue, 29 Aug 2023 18:05:02 GMT
ENV MARIADB_JDBC_ARTIFACT=mariadb-java-client-3.2.0.jar
# Tue, 29 Aug 2023 18:05:02 GMT
ENV MARIADB_JDBC_TARGET=/usr/local/tomcat/webapps/ROOT/WEB-INF/lib/mariadb-java-client-3.2.0.jar
# Tue, 29 Aug 2023 18:05:03 GMT
RUN curl -fSL "${MARIADB_JDBC_PREFIX}/${MARIADB_JDBC_ARTIFACT}" -o $MARIADB_JDBC_TARGET &&   echo "$MARIADB_JDBC_SHA256 $MARIADB_JDBC_TARGET" | sha256sum -c -
# Tue, 29 Aug 2023 18:05:03 GMT
COPY file:0a1be11e2eb610a1dbcd415404e3a592641110b93090030cb831e3a19a163017 in /usr/local/tomcat/bin/ 
# Tue, 29 Aug 2023 18:05:03 GMT
COPY file:0e237c3876eeb3b5f3473a064d3e507da2df6c228ca714687930b34e3b687601 in /usr/local/tomcat/webapps/ROOT/WEB-INF/hibernate.cfg.xml 
# Tue, 29 Aug 2023 18:05:03 GMT
RUN sed -i 's/<id>org.xwiki.platform:xwiki-platform-distribution-war/<id>org.xwiki.platform:xwiki-platform-distribution-docker/'   /usr/local/tomcat/webapps/ROOT/META-INF/extension.xed
# Tue, 29 Aug 2023 18:05:03 GMT
COPY file:a47c4dcd87c9dad97aff38c49188357e6193bcad50757e516cfb08a60d4de611 in /usr/local/bin/docker-entrypoint.sh 
# Tue, 29 Aug 2023 18:05:04 GMT
VOLUME [/usr/local/xwiki]
# Tue, 29 Aug 2023 18:05:04 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 29 Aug 2023 18:05:04 GMT
CMD ["xwiki"]
```

-	Layers:
	-	`sha256:9ea365e1e52efb9567c56f02f2200f0e95ddffd579225cc5b20a6333119d2811`  
		Last Modified: Fri, 04 Aug 2023 13:35:19 GMT  
		Size: 28.4 MB (28391903 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c9820f088487afe4c2ad735189bd2cca7b6b80af8efbaf6103e1ba1ae78d9f50`  
		Last Modified: Wed, 16 Aug 2023 14:26:46 GMT  
		Size: 12.8 MB (12843960 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:18df4cee3db70d57a1589c12f83bfde09e4c3bf6160a0b3eb356eab3370967b6`  
		Last Modified: Wed, 16 Aug 2023 14:27:59 GMT  
		Size: 45.2 MB (45190335 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5f6f231b62e05bb5ce59ff0bc82a58433378ea661f20f035ce309d5677a3e178`  
		Last Modified: Wed, 16 Aug 2023 14:27:53 GMT  
		Size: 159.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:abe1025511637076ab47fbec8048619da0b06cf39894a91cb74ac033917ed42f`  
		Last Modified: Wed, 16 Aug 2023 14:27:53 GMT  
		Size: 733.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:14494679fa666a95707b60c629251656cd7932e1d2e32dc4a87b20bf9a0c87ba`  
		Last Modified: Wed, 16 Aug 2023 22:12:02 GMT  
		Size: 172.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:89e927f61da99669ccf5c76222921e5e0d770869e1f8fbfb8b8c939f0193aff6`  
		Last Modified: Sat, 26 Aug 2023 03:45:55 GMT  
		Size: 12.3 MB (12291646 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7703321057ec3a58d2f1055097663e4db52e175ce11ee98838b7c748fb99b2a1`  
		Last Modified: Sat, 26 Aug 2023 03:45:54 GMT  
		Size: 455.9 KB (455910 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d4cb118c3edf2e9cd4e7eba152bce1fb566343e12e0ce1b1a6dd3b4d0e1dba05`  
		Last Modified: Sat, 26 Aug 2023 03:45:53 GMT  
		Size: 130.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:98e1661a3fe681ab596814fb59edfa8e64f9b4d24f5fb539fac6bb3d8387c015`  
		Last Modified: Sat, 26 Aug 2023 07:34:38 GMT  
		Size: 173.4 MB (173395163 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e46ba93ea6ac4253b091b4604173078e703621b40e574d8215c1b5a803168d10`  
		Last Modified: Tue, 29 Aug 2023 18:05:57 GMT  
		Size: 309.2 MB (309193990 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f51e505956f76842afeaff85674cf43060361349a924ee7da132a3b73fb54fd3`  
		Last Modified: Tue, 29 Aug 2023 18:07:09 GMT  
		Size: 603.4 KB (603393 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4edbdc22ecbb36a06f546dccd1143aa04cf457d5d2083bc983b80733d44e5979`  
		Last Modified: Tue, 29 Aug 2023 18:07:09 GMT  
		Size: 1.3 KB (1346 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4e7228a4527ec2cca4168f4c934607ed702174b0a8d28df9c424ff3efdb74810`  
		Last Modified: Tue, 29 Aug 2023 18:07:08 GMT  
		Size: 2.3 KB (2312 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:359ce7f5126744217833ec22a810e799f509edb130daf22e6feeef7186c7e0fc`  
		Last Modified: Tue, 29 Aug 2023 18:07:08 GMT  
		Size: 6.3 KB (6312 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fa7c28d942f09e25cf282674f3356e86535520ed801da7ee442316f61fe20bc7`  
		Last Modified: Tue, 29 Aug 2023 18:07:09 GMT  
		Size: 2.5 KB (2506 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
