## `xwiki:mariadb-tomcat`

```console
$ docker pull xwiki@sha256:a79116132172740391a1a5ee34fb74f2bee360a492226e7aa3d0340e1f024016
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `xwiki:mariadb-tomcat` - linux; amd64

```console
$ docker pull xwiki@sha256:6814d28ace3d45dd9d013566783229a5cb3fc5be6b54e635764cbea2105bd09a
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **588.0 MB (588012357 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:1370226000340ae932ba13ebc8425cee8e97db05ab6862d6be11afbcac8ccb8c`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["xwiki"]`

```dockerfile
# Tue, 25 Apr 2023 17:30:47 GMT
ARG RELEASE
# Tue, 25 Apr 2023 17:30:47 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Tue, 25 Apr 2023 17:30:47 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Tue, 25 Apr 2023 17:30:47 GMT
LABEL org.opencontainers.image.version=22.04
# Tue, 25 Apr 2023 17:30:49 GMT
ADD file:2fc6364d149eccc7f94ead482a0dcf24b0e44cc0d00ac6a2c1797776153e9608 in / 
# Tue, 25 Apr 2023 17:30:49 GMT
CMD ["/bin/bash"]
# Thu, 04 May 2023 07:26:20 GMT
ENV JAVA_HOME=/opt/java/openjdk
# Thu, 04 May 2023 07:26:20 GMT
ENV PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 04 May 2023 07:26:20 GMT
ENV LANG=en_US.UTF-8 LANGUAGE=en_US:en LC_ALL=en_US.UTF-8
# Thu, 04 May 2023 07:26:43 GMT
RUN apt-get update     && DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends tzdata curl wget ca-certificates fontconfig locales     && echo "en_US.UTF-8 UTF-8" >> /etc/locale.gen     && locale-gen en_US.UTF-8     && rm -rf /var/lib/apt/lists/*
# Thu, 04 May 2023 07:27:16 GMT
ENV JAVA_VERSION=jdk-11.0.19+7
# Thu, 04 May 2023 07:27:39 GMT
RUN set -eux;     ARCH="$(dpkg --print-architecture)";     case "${ARCH}" in        aarch64|arm64)          ESUM='1fe4b20d808f393422610818711c728331992a4455eeeb061d3d05b45412771d';          BINARY_URL='https://github.com/adoptium/temurin11-binaries/releases/download/jdk-11.0.19%2B7/OpenJDK11U-jre_aarch64_linux_hotspot_11.0.19_7.tar.gz';          ;;        armhf|arm)          ESUM='cb754b055177381f9f6852b7e5469904a15edddd7f8e136043c28b1e33aee47c';          BINARY_URL='https://github.com/adoptium/temurin11-binaries/releases/download/jdk-11.0.19%2B7/OpenJDK11U-jre_arm_linux_hotspot_11.0.19_7.tar.gz';          ;;        ppc64el|powerpc:common64)          ESUM='8019d938e5525938ec8e68e2989c4413263b0d9b7b3f20fe0c45f6d967919cfb';          BINARY_URL='https://github.com/adoptium/temurin11-binaries/releases/download/jdk-11.0.19%2B7/OpenJDK11U-jre_ppc64le_linux_hotspot_11.0.19_7.tar.gz';          ;;        s390x|s390:64-bit)          ESUM='058419435fe6212d1bc305a14f578c314f9ff9a2d96d523c178120e84231c733';          BINARY_URL='https://github.com/adoptium/temurin11-binaries/releases/download/jdk-11.0.19%2B7/OpenJDK11U-jre_s390x_linux_hotspot_11.0.19_7.tar.gz';          ;;        amd64|i386:x86-64)          ESUM='32dcf760664f93531594b72ce9226e9216567de5705a23c9ff5a77c797948054';          BINARY_URL='https://github.com/adoptium/temurin11-binaries/releases/download/jdk-11.0.19%2B7/OpenJDK11U-jre_x64_linux_hotspot_11.0.19_7.tar.gz';          ;;        *)          echo "Unsupported arch: ${ARCH}";          exit 1;          ;;     esac; 	  wget -O /tmp/openjdk.tar.gz ${BINARY_URL}; 	  echo "${ESUM} */tmp/openjdk.tar.gz" | sha256sum -c -; 	  mkdir -p "$JAVA_HOME"; 	  tar --extract 	      --file /tmp/openjdk.tar.gz 	      --directory "$JAVA_HOME" 	      --strip-components 1 	      --no-same-owner 	  ;     rm -f /tmp/openjdk.tar.gz ${JAVA_HOME}/src.zip;     find "$JAVA_HOME/lib" -name '*.so' -exec dirname '{}' ';' | sort -u > /etc/ld.so.conf.d/docker-openjdk.conf;     ldconfig;     java -Xshare:dump;
# Thu, 04 May 2023 07:27:40 GMT
RUN echo Verifying install ...     && fileEncoding="$(echo 'System.out.println(System.getProperty("file.encoding"))' | jshell -s -)"; [ "$fileEncoding" = 'UTF-8' ]; rm -rf ~/.java     && echo java --version && java --version     && echo Complete.
# Thu, 04 May 2023 16:13:14 GMT
ENV CATALINA_HOME=/usr/local/tomcat
# Thu, 04 May 2023 16:13:14 GMT
ENV PATH=/usr/local/tomcat/bin:/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 04 May 2023 16:13:14 GMT
RUN mkdir -p "$CATALINA_HOME"
# Thu, 04 May 2023 16:13:14 GMT
WORKDIR /usr/local/tomcat
# Thu, 04 May 2023 16:13:14 GMT
ENV TOMCAT_NATIVE_LIBDIR=/usr/local/tomcat/native-jni-lib
# Thu, 04 May 2023 16:13:15 GMT
ENV LD_LIBRARY_PATH=/usr/local/tomcat/native-jni-lib
# Thu, 04 May 2023 16:14:45 GMT
ENV GPG_KEYS=48F8E69F6390C9F25CFEDCD268248959359E722B A9C5DF4D22E99998D9875A5110C01C5A2F6059E7 DCFD35E0BF8CA7344752DE8B6FB21E8933C60243
# Thu, 04 May 2023 16:14:45 GMT
ENV TOMCAT_MAJOR=9
# Wed, 10 May 2023 18:01:17 GMT
ENV TOMCAT_VERSION=9.0.75
# Wed, 10 May 2023 18:01:17 GMT
ENV TOMCAT_SHA512=e29905e693598b64d958dd22b8d866590163917bdc6e1cfd363a8a06f97ecc89284b863b3ab2448f43903623564c3fd952c7a9bd33df8476d57f6873c2d463c7
# Wed, 10 May 2023 18:01:17 GMT
COPY dir:606cc669e6833afa7967597ca36d4a4497efbb54719c008108649021142d7549 in /usr/local/tomcat 
# Wed, 10 May 2023 18:01:21 GMT
RUN set -eux; 	apt-get update; 	xargs -rt apt-get install -y --no-install-recommends < "$TOMCAT_NATIVE_LIBDIR/.dependencies.txt"; 	rm -rf /var/lib/apt/lists/*
# Wed, 10 May 2023 18:01:23 GMT
RUN set -eux; 	nativeLines="$(catalina.sh configtest 2>&1)"; 	nativeLines="$(echo "$nativeLines" | grep 'Apache Tomcat Native')"; 	nativeLines="$(echo "$nativeLines" | sort -u)"; 	if ! echo "$nativeLines" | grep -E 'INFO: Loaded( APR based)? Apache Tomcat Native library' >&2; then 		echo >&2 "$nativeLines"; 		exit 1; 	fi
# Wed, 10 May 2023 18:01:23 GMT
EXPOSE 8080
# Wed, 10 May 2023 18:01:23 GMT
CMD ["catalina.sh" "run"]
# Wed, 10 May 2023 18:27:13 GMT
LABEL org.opencontainers.image.authors=XWiki Development Team <committers@xwiki.org>
# Wed, 10 May 2023 18:27:13 GMT
LABEL org.opencontainers.image.url=https://hub.docker.com/_/xwiki
# Wed, 10 May 2023 18:27:13 GMT
LABEL org.opencontainers.image.documentation=https://hub.docker.com/_/xwiki
# Wed, 10 May 2023 18:27:13 GMT
LABEL org.opencontainers.image.source=https://github.com/xwiki/xwiki-docker.git
# Wed, 10 May 2023 18:27:13 GMT
LABEL org.opencontainers.image.vendor=xwiki.org
# Wed, 10 May 2023 18:27:13 GMT
LABEL org.opencontainers.image.licenses=LGPL-2.1
# Wed, 10 May 2023 18:28:05 GMT
RUN apt-get update &&   apt-get --no-install-recommends -y install     curl     libreoffice     unzip     procps &&   rm -rf /var/lib/apt/lists/*
# Tue, 30 May 2023 22:28:52 GMT
ENV XWIKI_VERSION=15.4
# Tue, 30 May 2023 22:28:52 GMT
ENV XWIKI_URL_PREFIX=https://maven.xwiki.org/releases/org/xwiki/platform/xwiki-platform-distribution-war/15.4
# Tue, 30 May 2023 22:28:52 GMT
ENV XWIKI_DOWNLOAD_SHA256=f24def5b4e3f97c56ed03d5983766028676d6ce205bd60d3798352be5a050505
# Tue, 30 May 2023 22:29:31 GMT
RUN rm -rf /usr/local/tomcat/webapps/* &&   mkdir -p /usr/local/tomcat/temp &&   mkdir -p /usr/local/xwiki/data &&   curl -fSL "${XWIKI_URL_PREFIX}/xwiki-platform-distribution-war-${XWIKI_VERSION}.war" -o xwiki.war &&   echo "$XWIKI_DOWNLOAD_SHA256 xwiki.war" | sha256sum -c - &&   unzip -d /usr/local/tomcat/webapps/ROOT xwiki.war &&   rm -f xwiki.war
# Tue, 30 May 2023 22:30:30 GMT
ENV MARIADB_JDBC_VERSION=3.1.4
# Tue, 30 May 2023 22:30:30 GMT
ENV MARIADB_JDBC_SHA256=eb88b5d727d82e25117e2b6fabcec1daf734633b0a576456c73215884c189ad4
# Tue, 30 May 2023 22:30:30 GMT
ENV MARIADB_JDBC_PREFIX=https://repo1.maven.org/maven2/org/mariadb/jdbc/mariadb-java-client/3.1.4
# Tue, 30 May 2023 22:30:30 GMT
ENV MARIADB_JDBC_ARTIFACT=mariadb-java-client-3.1.4.jar
# Tue, 30 May 2023 22:30:30 GMT
ENV MARIADB_JDBC_TARGET=/usr/local/tomcat/webapps/ROOT/WEB-INF/lib/mariadb-java-client-3.1.4.jar
# Tue, 30 May 2023 22:30:31 GMT
RUN curl -fSL "${MARIADB_JDBC_PREFIX}/${MARIADB_JDBC_ARTIFACT}" -o $MARIADB_JDBC_TARGET &&   echo "$MARIADB_JDBC_SHA256 $MARIADB_JDBC_TARGET" | sha256sum -c -
# Tue, 30 May 2023 22:30:31 GMT
COPY file:0a1be11e2eb610a1dbcd415404e3a592641110b93090030cb831e3a19a163017 in /usr/local/tomcat/bin/ 
# Tue, 30 May 2023 22:30:31 GMT
COPY file:0e237c3876eeb3b5f3473a064d3e507da2df6c228ca714687930b34e3b687601 in /usr/local/tomcat/webapps/ROOT/WEB-INF/hibernate.cfg.xml 
# Tue, 30 May 2023 22:30:32 GMT
RUN sed -i 's/<id>org.xwiki.platform:xwiki-platform-distribution-war/<id>org.xwiki.platform:xwiki-platform-distribution-docker/'   /usr/local/tomcat/webapps/ROOT/META-INF/extension.xed
# Tue, 30 May 2023 22:30:32 GMT
COPY file:a47c4dcd87c9dad97aff38c49188357e6193bcad50757e516cfb08a60d4de611 in /usr/local/bin/docker-entrypoint.sh 
# Tue, 30 May 2023 22:30:32 GMT
VOLUME [/usr/local/xwiki]
# Tue, 30 May 2023 22:30:32 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 30 May 2023 22:30:32 GMT
CMD ["xwiki"]
```

-	Layers:
	-	`sha256:1bc677758ad7fa4503417ae5be18809c5a8679b5b36fcd1464d5a8e41cb13305`  
		Last Modified: Tue, 25 Apr 2023 22:54:44 GMT  
		Size: 30.4 MB (30430220 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:458b02b5411a07f3b354cde2b461caffc1bb184a3413b5736a9e67ee87cb28b2`  
		Last Modified: Thu, 04 May 2023 07:30:02 GMT  
		Size: 12.5 MB (12504170 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b04a165ead1d5eabe89dc88e53286af89caab22a5d20c53007b9e6e508affb4b`  
		Last Modified: Thu, 04 May 2023 07:31:19 GMT  
		Size: 46.7 MB (46666270 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1187c73b18505bd4495bc03ccbdb723388dfe4d633fd12be845dfe8e253e48e2`  
		Last Modified: Thu, 04 May 2023 07:31:12 GMT  
		Size: 159.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8c833cbb14374cde014505e77f6a6122773984a691844e4138fc15cae99ba625`  
		Last Modified: Thu, 04 May 2023 16:24:19 GMT  
		Size: 173.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:439ac04571c77c4330db518bc8f35b70f8723246ed34c98787f7ac8d7dc30b42`  
		Last Modified: Wed, 10 May 2023 18:09:06 GMT  
		Size: 12.2 MB (12236613 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3d8e775ba0b76c6692c0b9211e4b94653ba2aa16fdc7a5e3347aba962b684508`  
		Last Modified: Wed, 10 May 2023 18:09:06 GMT  
		Size: 454.2 KB (454222 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bee5c1ba4848e97d4e3c43d9d4bca0eeeccf2d5d7f6d805d748da4a7d24ad14e`  
		Last Modified: Wed, 10 May 2023 18:09:05 GMT  
		Size: 130.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ffadd10be916fc5729676141f5d0ba6aa30968b75555790e449d4988dc81332a`  
		Last Modified: Wed, 10 May 2023 18:32:42 GMT  
		Size: 178.3 MB (178334017 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:87bd4429f182b939dfdfa03ae6b1d84db110abe119031beb45663084f8f4f9ee`  
		Last Modified: Tue, 30 May 2023 22:31:16 GMT  
		Size: 306.8 MB (306779668 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4f09b1ab80268a02eb6d643aba1231b2838f9c9848f2d2a1192eff5c9be69744`  
		Last Modified: Tue, 30 May 2023 22:32:26 GMT  
		Size: 594.6 KB (594555 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:13909e71c5e5d0926295d8b6cf2a3e939f1bdb77d43c22a124d87e89d52b1f66`  
		Last Modified: Tue, 30 May 2023 22:32:25 GMT  
		Size: 1.3 KB (1346 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ca9c8cf0fa1191b24df10bbe75d17cefc589b8d2335770b9ee306233b59b4ed1`  
		Last Modified: Tue, 30 May 2023 22:32:25 GMT  
		Size: 2.3 KB (2313 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5ee984b856198cbbda51a8dce64fae4211238e71e84c18e87ed78c584e2c4322`  
		Last Modified: Tue, 30 May 2023 22:32:25 GMT  
		Size: 6.0 KB (5995 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:07fd204f3a55320372afffe3014cb13aa1a85efccf0a99f5380ee3d8dc2e4bb0`  
		Last Modified: Tue, 30 May 2023 22:32:25 GMT  
		Size: 2.5 KB (2506 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `xwiki:mariadb-tomcat` - linux; arm64 variant v8

```console
$ docker pull xwiki@sha256:a17b11be41664c36af3006b6ebc90eb02a4aee5b6a3ec168111f6abc9d858ebc
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **581.6 MB (581636482 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:dd19fb449f0391683e2d2c962de1172f473f40993517da4af8ef344dbb80ab52`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["xwiki"]`

```dockerfile
# Mon, 22 May 2023 17:53:00 GMT
ARG RELEASE
# Mon, 22 May 2023 17:53:01 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Mon, 22 May 2023 17:53:01 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Mon, 22 May 2023 17:53:01 GMT
LABEL org.opencontainers.image.version=22.04
# Mon, 22 May 2023 17:53:07 GMT
ADD file:f0435ed8dcf91cc69ec63b6b16d9efac56e5a6a7ec518e1fcc3df7457d3113ed in / 
# Mon, 22 May 2023 17:53:08 GMT
CMD ["/bin/bash"]
# Thu, 01 Jun 2023 23:18:29 GMT
ENV JAVA_HOME=/opt/java/openjdk
# Thu, 01 Jun 2023 23:18:30 GMT
ENV PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 01 Jun 2023 23:18:30 GMT
ENV LANG=en_US.UTF-8 LANGUAGE=en_US:en LC_ALL=en_US.UTF-8
# Thu, 01 Jun 2023 23:18:44 GMT
RUN apt-get update     && DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends tzdata curl wget ca-certificates fontconfig locales     && echo "en_US.UTF-8 UTF-8" >> /etc/locale.gen     && locale-gen en_US.UTF-8     && rm -rf /var/lib/apt/lists/*
# Thu, 01 Jun 2023 23:19:07 GMT
ENV JAVA_VERSION=jdk-11.0.19+7
# Thu, 01 Jun 2023 23:19:30 GMT
RUN set -eux;     ARCH="$(dpkg --print-architecture)";     case "${ARCH}" in        aarch64|arm64)          ESUM='1fe4b20d808f393422610818711c728331992a4455eeeb061d3d05b45412771d';          BINARY_URL='https://github.com/adoptium/temurin11-binaries/releases/download/jdk-11.0.19%2B7/OpenJDK11U-jre_aarch64_linux_hotspot_11.0.19_7.tar.gz';          ;;        armhf|arm)          ESUM='cb754b055177381f9f6852b7e5469904a15edddd7f8e136043c28b1e33aee47c';          BINARY_URL='https://github.com/adoptium/temurin11-binaries/releases/download/jdk-11.0.19%2B7/OpenJDK11U-jre_arm_linux_hotspot_11.0.19_7.tar.gz';          ;;        ppc64el|powerpc:common64)          ESUM='8019d938e5525938ec8e68e2989c4413263b0d9b7b3f20fe0c45f6d967919cfb';          BINARY_URL='https://github.com/adoptium/temurin11-binaries/releases/download/jdk-11.0.19%2B7/OpenJDK11U-jre_ppc64le_linux_hotspot_11.0.19_7.tar.gz';          ;;        s390x|s390:64-bit)          ESUM='058419435fe6212d1bc305a14f578c314f9ff9a2d96d523c178120e84231c733';          BINARY_URL='https://github.com/adoptium/temurin11-binaries/releases/download/jdk-11.0.19%2B7/OpenJDK11U-jre_s390x_linux_hotspot_11.0.19_7.tar.gz';          ;;        amd64|i386:x86-64)          ESUM='32dcf760664f93531594b72ce9226e9216567de5705a23c9ff5a77c797948054';          BINARY_URL='https://github.com/adoptium/temurin11-binaries/releases/download/jdk-11.0.19%2B7/OpenJDK11U-jre_x64_linux_hotspot_11.0.19_7.tar.gz';          ;;        *)          echo "Unsupported arch: ${ARCH}";          exit 1;          ;;     esac; 	  wget -O /tmp/openjdk.tar.gz ${BINARY_URL}; 	  echo "${ESUM} */tmp/openjdk.tar.gz" | sha256sum -c -; 	  mkdir -p "$JAVA_HOME"; 	  tar --extract 	      --file /tmp/openjdk.tar.gz 	      --directory "$JAVA_HOME" 	      --strip-components 1 	      --no-same-owner 	  ;     rm -f /tmp/openjdk.tar.gz ${JAVA_HOME}/src.zip;     find "$JAVA_HOME/lib" -name '*.so' -exec dirname '{}' ';' | sort -u > /etc/ld.so.conf.d/docker-openjdk.conf;     ldconfig;     java -Xshare:dump;
# Thu, 01 Jun 2023 23:19:31 GMT
RUN echo Verifying install ...     && fileEncoding="$(echo 'System.out.println(System.getProperty("file.encoding"))' | jshell -s -)"; [ "$fileEncoding" = 'UTF-8' ]; rm -rf ~/.java     && echo java --version && java --version     && echo Complete.
# Fri, 02 Jun 2023 01:57:47 GMT
ENV CATALINA_HOME=/usr/local/tomcat
# Fri, 02 Jun 2023 01:57:47 GMT
ENV PATH=/usr/local/tomcat/bin:/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Fri, 02 Jun 2023 01:57:48 GMT
RUN mkdir -p "$CATALINA_HOME"
# Fri, 02 Jun 2023 01:57:48 GMT
WORKDIR /usr/local/tomcat
# Fri, 02 Jun 2023 01:57:48 GMT
ENV TOMCAT_NATIVE_LIBDIR=/usr/local/tomcat/native-jni-lib
# Fri, 02 Jun 2023 01:57:48 GMT
ENV LD_LIBRARY_PATH=/usr/local/tomcat/native-jni-lib
# Fri, 02 Jun 2023 01:59:05 GMT
ENV GPG_KEYS=48F8E69F6390C9F25CFEDCD268248959359E722B A9C5DF4D22E99998D9875A5110C01C5A2F6059E7 DCFD35E0BF8CA7344752DE8B6FB21E8933C60243
# Fri, 02 Jun 2023 01:59:05 GMT
ENV TOMCAT_MAJOR=9
# Fri, 02 Jun 2023 01:59:05 GMT
ENV TOMCAT_VERSION=9.0.75
# Fri, 02 Jun 2023 01:59:05 GMT
ENV TOMCAT_SHA512=e29905e693598b64d958dd22b8d866590163917bdc6e1cfd363a8a06f97ecc89284b863b3ab2448f43903623564c3fd952c7a9bd33df8476d57f6873c2d463c7
# Fri, 02 Jun 2023 01:59:05 GMT
COPY dir:6772160db6f147cd31589cbb67d4cc64fba9465bcc14e4e3f07be9451759501e in /usr/local/tomcat 
# Fri, 02 Jun 2023 01:59:09 GMT
RUN set -eux; 	apt-get update; 	xargs -rt apt-get install -y --no-install-recommends < "$TOMCAT_NATIVE_LIBDIR/.dependencies.txt"; 	rm -rf /var/lib/apt/lists/*
# Fri, 02 Jun 2023 01:59:10 GMT
RUN set -eux; 	nativeLines="$(catalina.sh configtest 2>&1)"; 	nativeLines="$(echo "$nativeLines" | grep 'Apache Tomcat Native')"; 	nativeLines="$(echo "$nativeLines" | sort -u)"; 	if ! echo "$nativeLines" | grep -E 'INFO: Loaded( APR based)? Apache Tomcat Native library' >&2; then 		echo >&2 "$nativeLines"; 		exit 1; 	fi
# Fri, 02 Jun 2023 01:59:10 GMT
EXPOSE 8080
# Fri, 02 Jun 2023 01:59:10 GMT
CMD ["catalina.sh" "run"]
# Fri, 02 Jun 2023 03:24:00 GMT
LABEL org.opencontainers.image.authors=XWiki Development Team <committers@xwiki.org>
# Fri, 02 Jun 2023 03:24:00 GMT
LABEL org.opencontainers.image.url=https://hub.docker.com/_/xwiki
# Fri, 02 Jun 2023 03:24:00 GMT
LABEL org.opencontainers.image.documentation=https://hub.docker.com/_/xwiki
# Fri, 02 Jun 2023 03:24:00 GMT
LABEL org.opencontainers.image.source=https://github.com/xwiki/xwiki-docker.git
# Fri, 02 Jun 2023 03:24:00 GMT
LABEL org.opencontainers.image.vendor=xwiki.org
# Fri, 02 Jun 2023 03:24:00 GMT
LABEL org.opencontainers.image.licenses=LGPL-2.1
# Fri, 02 Jun 2023 03:25:42 GMT
RUN apt-get update &&   apt-get --no-install-recommends -y install     curl     libreoffice     unzip     procps &&   rm -rf /var/lib/apt/lists/*
# Fri, 02 Jun 2023 03:25:45 GMT
ENV XWIKI_VERSION=15.4
# Fri, 02 Jun 2023 03:25:45 GMT
ENV XWIKI_URL_PREFIX=https://maven.xwiki.org/releases/org/xwiki/platform/xwiki-platform-distribution-war/15.4
# Fri, 02 Jun 2023 03:25:45 GMT
ENV XWIKI_DOWNLOAD_SHA256=f24def5b4e3f97c56ed03d5983766028676d6ce205bd60d3798352be5a050505
# Fri, 02 Jun 2023 03:26:26 GMT
RUN rm -rf /usr/local/tomcat/webapps/* &&   mkdir -p /usr/local/tomcat/temp &&   mkdir -p /usr/local/xwiki/data &&   curl -fSL "${XWIKI_URL_PREFIX}/xwiki-platform-distribution-war-${XWIKI_VERSION}.war" -o xwiki.war &&   echo "$XWIKI_DOWNLOAD_SHA256 xwiki.war" | sha256sum -c - &&   unzip -d /usr/local/tomcat/webapps/ROOT xwiki.war &&   rm -f xwiki.war
# Fri, 02 Jun 2023 03:28:00 GMT
ENV MARIADB_JDBC_VERSION=3.1.4
# Fri, 02 Jun 2023 03:28:00 GMT
ENV MARIADB_JDBC_SHA256=eb88b5d727d82e25117e2b6fabcec1daf734633b0a576456c73215884c189ad4
# Fri, 02 Jun 2023 03:28:00 GMT
ENV MARIADB_JDBC_PREFIX=https://repo1.maven.org/maven2/org/mariadb/jdbc/mariadb-java-client/3.1.4
# Fri, 02 Jun 2023 03:28:01 GMT
ENV MARIADB_JDBC_ARTIFACT=mariadb-java-client-3.1.4.jar
# Fri, 02 Jun 2023 03:28:01 GMT
ENV MARIADB_JDBC_TARGET=/usr/local/tomcat/webapps/ROOT/WEB-INF/lib/mariadb-java-client-3.1.4.jar
# Fri, 02 Jun 2023 03:28:01 GMT
RUN curl -fSL "${MARIADB_JDBC_PREFIX}/${MARIADB_JDBC_ARTIFACT}" -o $MARIADB_JDBC_TARGET &&   echo "$MARIADB_JDBC_SHA256 $MARIADB_JDBC_TARGET" | sha256sum -c -
# Fri, 02 Jun 2023 03:28:01 GMT
COPY file:0a1be11e2eb610a1dbcd415404e3a592641110b93090030cb831e3a19a163017 in /usr/local/tomcat/bin/ 
# Fri, 02 Jun 2023 03:28:01 GMT
COPY file:0e237c3876eeb3b5f3473a064d3e507da2df6c228ca714687930b34e3b687601 in /usr/local/tomcat/webapps/ROOT/WEB-INF/hibernate.cfg.xml 
# Fri, 02 Jun 2023 03:28:02 GMT
RUN sed -i 's/<id>org.xwiki.platform:xwiki-platform-distribution-war/<id>org.xwiki.platform:xwiki-platform-distribution-docker/'   /usr/local/tomcat/webapps/ROOT/META-INF/extension.xed
# Fri, 02 Jun 2023 03:28:02 GMT
COPY file:a47c4dcd87c9dad97aff38c49188357e6193bcad50757e516cfb08a60d4de611 in /usr/local/bin/docker-entrypoint.sh 
# Fri, 02 Jun 2023 03:28:02 GMT
VOLUME [/usr/local/xwiki]
# Fri, 02 Jun 2023 03:28:02 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 02 Jun 2023 03:28:02 GMT
CMD ["xwiki"]
```

-	Layers:
	-	`sha256:6c7698a779f6d8c45a39a6721fb5cce267d66ff8ab5181c55aa6d02c8ddacd01`  
		Last Modified: Tue, 23 May 2023 02:05:13 GMT  
		Size: 28.4 MB (28389044 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f90f9c81eab3c275d75f3cf9f4840e195cfa7c5372d500bfeb5a040f3fc88262`  
		Last Modified: Thu, 01 Jun 2023 23:21:25 GMT  
		Size: 12.5 MB (12452855 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f6fcc328ac0affca0471a6a1d24001fbf5d6927268b63108576c160df5647af7`  
		Last Modified: Thu, 01 Jun 2023 23:22:22 GMT  
		Size: 45.0 MB (45009479 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8cf5c29166d38f94500a3660aa3baef35070a8822a01cc0d45dd1ca1e9ace769`  
		Last Modified: Thu, 01 Jun 2023 23:22:18 GMT  
		Size: 160.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c37df8cc9a991ed50f676003a7c9f6ebeeaa4b5b28a42b6126522c569938d544`  
		Last Modified: Fri, 02 Jun 2023 02:06:06 GMT  
		Size: 174.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:73e19b4e105eebc0ba47bb90c9ef63b8c9b604e0cee4eab1fb482a68b3664586`  
		Last Modified: Fri, 02 Jun 2023 02:07:50 GMT  
		Size: 12.2 MB (12242189 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4850a1ed957a95b8a94a2957ccd1b4ed1227f7c8997a70eed6f9ff693b648e8e`  
		Last Modified: Fri, 02 Jun 2023 02:07:50 GMT  
		Size: 2.8 MB (2806582 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:35c42a0a43520047ad78ac489284036db953e98cca2d1d4bd31b523bd0c6ba28`  
		Last Modified: Fri, 02 Jun 2023 02:07:49 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:616eeb0d98e442348091228bd6eca84c2670b963a7ea7bd083875cb0d3a97862`  
		Last Modified: Fri, 02 Jun 2023 03:30:20 GMT  
		Size: 173.3 MB (173349470 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3294b0658c293f95f1b4c42dace3400a7c838d608ba7e56b604f1e0e221d011a`  
		Last Modified: Fri, 02 Jun 2023 03:30:15 GMT  
		Size: 306.8 MB (306779696 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d580c6e44a09e409a0c5bb90f9e33ff08ac6c1de90af839bdd10571e0169a82c`  
		Last Modified: Fri, 02 Jun 2023 03:31:26 GMT  
		Size: 594.5 KB (594550 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4ada7e821f0c78168e36f3ecdf6f07f1b641e857f85f523027cbdc528f0b09ba`  
		Last Modified: Fri, 02 Jun 2023 03:31:25 GMT  
		Size: 1.3 KB (1344 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ac19601c1e414dac1e5cd3e076bb66bc415cebc02823084973abbe1e89bfad18`  
		Last Modified: Fri, 02 Jun 2023 03:31:26 GMT  
		Size: 2.3 KB (2311 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d5d8da5361f17c7f4f79bae566554f6bb49c06a1206dcbc4ad3d16eb4c7af680`  
		Last Modified: Fri, 02 Jun 2023 03:31:26 GMT  
		Size: 6.0 KB (5997 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:79e8c5165664cce102bfb81051577b12b08989e10133772c7ee07ac174a9716a`  
		Last Modified: Fri, 02 Jun 2023 03:31:26 GMT  
		Size: 2.5 KB (2502 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
