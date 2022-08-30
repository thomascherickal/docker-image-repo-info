## `xwiki:lts-mysql-tomcat`

```console
$ docker pull xwiki@sha256:20564e1ca04544f4847b291273d51221e0e071b0e815f933b3d041aa99551774
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `xwiki:lts-mysql-tomcat` - linux; amd64

```console
$ docker pull xwiki@sha256:23c72e780605ce08fa0d0a713631e43b5c7f3ff3882c9c734bf075269a3fa563
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **575.4 MB (575416702 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:3de0f8900bfbb70bfcb75412a91e40cbc31d9119957a5d7edfbe8ce8cad57fdc`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["xwiki"]`

```dockerfile
# Tue, 02 Aug 2022 01:30:55 GMT
ADD file:396eeb65c8d737180cc1219713cf59efb214027b79d8ea0b7e58a08e7c8d7a21 in / 
# Tue, 02 Aug 2022 01:30:56 GMT
CMD ["bash"]
# Thu, 11 Aug 2022 19:20:28 GMT
ENV JAVA_HOME=/opt/java/openjdk
# Thu, 11 Aug 2022 19:20:28 GMT
ENV PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 11 Aug 2022 19:20:28 GMT
ENV LANG=en_US.UTF-8 LANGUAGE=en_US:en LC_ALL=en_US.UTF-8
# Fri, 12 Aug 2022 17:20:49 GMT
RUN apt-get update     && DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends tzdata curl wget ca-certificates fontconfig locales     && echo "en_US.UTF-8 UTF-8" >> /etc/locale.gen     && locale-gen en_US.UTF-8     && rm -rf /var/lib/apt/lists/*
# Wed, 24 Aug 2022 19:20:36 GMT
ENV JAVA_VERSION=jdk-11.0.16.1+1
# Wed, 24 Aug 2022 19:21:24 GMT
RUN set -eux;     ARCH="$(dpkg --print-architecture)";     case "${ARCH}" in        aarch64|arm64)          ESUM='b6607f28fa2906d612d517f0babe4f0f895aa1c3f901edcddb493e33c1e27364';          BINARY_URL='https://github.com/adoptium/temurin11-binaries/releases/download/jdk-11.0.16.1%2B1/OpenJDK11U-jre_aarch64_linux_hotspot_11.0.16.1_1.tar.gz';          ;;        armhf|arm)          ESUM='2ee7fe636a6a57e4718dfe597e8097b93ef8d976e4b05384433777c9f0526f5a';          BINARY_URL='https://github.com/adoptium/temurin11-binaries/releases/download/jdk-11.0.16.1%2B1/OpenJDK11U-jre_arm_linux_hotspot_11.0.16.1_1.tar.gz';          ;;        ppc64el|powerpc:common64)          ESUM='f76b64b201b64ff37f77f73ead546ebcf2af9862b7cd1a1f4e0e5628e3f6a7fc';          BINARY_URL='https://github.com/adoptium/temurin11-binaries/releases/download/jdk-11.0.16.1%2B1/OpenJDK11U-jre_ppc64le_linux_hotspot_11.0.16.1_1.tar.gz';          ;;        s390x|s390:64-bit)          ESUM='bf01489459135ab0ce1ad346a56f0dfeb2d6fe4e59854ef76a6bb989ac403f91';          BINARY_URL='https://github.com/adoptium/temurin11-binaries/releases/download/jdk-11.0.16.1%2B1/OpenJDK11U-jre_s390x_linux_hotspot_11.0.16.1_1.tar.gz';          ;;        amd64|i386:x86-64)          ESUM='1ffe1a682e8179e35238bf3f93aba0cb185850e202c676f41d38cb0561883eda';          BINARY_URL='https://github.com/adoptium/temurin11-binaries/releases/download/jdk-11.0.16.1%2B1/OpenJDK11U-jre_x64_linux_hotspot_11.0.16.1_1.tar.gz';          ;;        *)          echo "Unsupported arch: ${ARCH}";          exit 1;          ;;     esac; 	  wget -O /tmp/openjdk.tar.gz ${BINARY_URL}; 	  echo "${ESUM} */tmp/openjdk.tar.gz" | sha256sum -c -; 	  mkdir -p "$JAVA_HOME"; 	  tar --extract 	      --file /tmp/openjdk.tar.gz 	      --directory "$JAVA_HOME" 	      --strip-components 1 	      --no-same-owner 	  ;     rm /tmp/openjdk.tar.gz;     find "$JAVA_HOME/lib" -name '*.so' -exec dirname '{}' ';' | sort -u > /etc/ld.so.conf.d/docker-openjdk.conf;     ldconfig;     java -Xshare:dump;
# Wed, 24 Aug 2022 19:21:25 GMT
RUN echo Verifying install ...     && fileEncoding="$(echo 'System.out.println(System.getProperty("file.encoding"))' | jshell -s -)"; [ "$fileEncoding" = 'UTF-8' ]; rm -rf ~/.java     && echo java --version && java --version     && echo Complete.
# Wed, 24 Aug 2022 22:06:27 GMT
ENV CATALINA_HOME=/usr/local/tomcat
# Wed, 24 Aug 2022 22:06:28 GMT
ENV PATH=/usr/local/tomcat/bin:/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 24 Aug 2022 22:06:28 GMT
RUN mkdir -p "$CATALINA_HOME"
# Wed, 24 Aug 2022 22:06:28 GMT
WORKDIR /usr/local/tomcat
# Wed, 24 Aug 2022 22:06:28 GMT
ENV TOMCAT_NATIVE_LIBDIR=/usr/local/tomcat/native-jni-lib
# Wed, 24 Aug 2022 22:06:28 GMT
ENV LD_LIBRARY_PATH=/usr/local/tomcat/native-jni-lib
# Wed, 24 Aug 2022 22:12:22 GMT
ENV GPG_KEYS=48F8E69F6390C9F25CFEDCD268248959359E722B A9C5DF4D22E99998D9875A5110C01C5A2F6059E7 DCFD35E0BF8CA7344752DE8B6FB21E8933C60243
# Wed, 24 Aug 2022 22:12:22 GMT
ENV TOMCAT_MAJOR=9
# Wed, 24 Aug 2022 22:12:22 GMT
ENV TOMCAT_VERSION=9.0.65
# Wed, 24 Aug 2022 22:12:23 GMT
ENV TOMCAT_SHA512=2ae846848b8436856be11cfa18d9c62caa06ca7d3134012b2e10cbf6078753c4af20cc5d37f7dc75f1779f5c59d7c033850b8626534c3ce7e389641a67963cf6
# Wed, 24 Aug 2022 22:12:23 GMT
COPY dir:7d76aaf3de314456bb6b7fbfe122174d615def62684413c93908edc0ffa3c4d1 in /usr/local/tomcat 
# Wed, 24 Aug 2022 22:12:27 GMT
RUN set -eux; 	apt-get update; 	xargs -rt apt-get install -y --no-install-recommends < "$TOMCAT_NATIVE_LIBDIR/.dependencies.txt"; 	rm -rf /var/lib/apt/lists/*
# Wed, 24 Aug 2022 22:12:28 GMT
RUN set -eux; 	nativeLines="$(catalina.sh configtest 2>&1)"; 	nativeLines="$(echo "$nativeLines" | grep 'Apache Tomcat Native')"; 	nativeLines="$(echo "$nativeLines" | sort -u)"; 	if ! echo "$nativeLines" | grep -E 'INFO: Loaded( APR based)? Apache Tomcat Native library' >&2; then 		echo >&2 "$nativeLines"; 		exit 1; 	fi
# Wed, 24 Aug 2022 22:12:28 GMT
EXPOSE 8080
# Wed, 24 Aug 2022 22:12:28 GMT
CMD ["catalina.sh" "run"]
# Mon, 29 Aug 2022 20:04:02 GMT
LABEL org.opencontainers.image.authors=XWiki Development Team <committers@xwiki.org>
# Mon, 29 Aug 2022 20:04:03 GMT
LABEL org.opencontainers.image.url=https://hub.docker.com/_/xwiki
# Mon, 29 Aug 2022 20:04:03 GMT
LABEL org.opencontainers.image.documentation=https://hub.docker.com/_/xwiki
# Mon, 29 Aug 2022 20:04:03 GMT
LABEL org.opencontainers.image.source=https://github.com/xwiki/xwiki-docker.git
# Mon, 29 Aug 2022 20:04:03 GMT
LABEL org.opencontainers.image.vendor=xwiki.org
# Mon, 29 Aug 2022 20:04:03 GMT
LABEL org.opencontainers.image.licenses=LGPL-2.1
# Mon, 29 Aug 2022 20:05:50 GMT
RUN apt-get update &&   apt-get --no-install-recommends -y install     curl     libreoffice     unzip     procps &&   rm -rf /var/lib/apt/lists/*
# Tue, 30 Aug 2022 18:21:31 GMT
ENV XWIKI_VERSION=13.10.9
# Tue, 30 Aug 2022 18:21:31 GMT
ENV XWIKI_URL_PREFIX=https://maven.xwiki.org/releases/org/xwiki/platform/xwiki-platform-distribution-war/13.10.9
# Tue, 30 Aug 2022 18:21:31 GMT
ENV XWIKI_DOWNLOAD_SHA256=ad57639016b1bfd1cdf84de764b310a65416832645c6bbfd933ec26fd977bb6a
# Tue, 30 Aug 2022 18:22:08 GMT
RUN rm -rf /usr/local/tomcat/webapps/* &&   mkdir -p /usr/local/tomcat/temp &&   mkdir -p /usr/local/xwiki/data &&   curl -fSL "${XWIKI_URL_PREFIX}/xwiki-platform-distribution-war-${XWIKI_VERSION}.war" -o xwiki.war &&   echo "$XWIKI_DOWNLOAD_SHA256 xwiki.war" | sha256sum -c - &&   unzip -d /usr/local/tomcat/webapps/ROOT xwiki.war &&   rm -f xwiki.war
# Tue, 30 Aug 2022 18:22:09 GMT
ENV MYSQL_JDBC_VERSION=8.0.30
# Tue, 30 Aug 2022 18:22:09 GMT
ENV MYSQL_JDBC_SHA256=b5bf2f0987197c30adf74a9e419b89cda4c257da2d1142871f508416d5f2227a
# Tue, 30 Aug 2022 18:22:09 GMT
ENV MYSQL_JDBC_PREFIX=https://repo1.maven.org/maven2/mysql/mysql-connector-java/8.0.30
# Tue, 30 Aug 2022 18:22:09 GMT
ENV MYSQL_JDBC_ARTIFACT=mysql-connector-java-8.0.30.jar
# Tue, 30 Aug 2022 18:22:09 GMT
ENV MYSQL_JDBC_TARGET=/usr/local/tomcat/webapps/ROOT/WEB-INF/lib/mysql-connector-java-8.0.30.jar
# Tue, 30 Aug 2022 18:22:10 GMT
RUN curl -fSL "${MYSQL_JDBC_PREFIX}/${MYSQL_JDBC_ARTIFACT}" -o $MYSQL_JDBC_TARGET &&   echo "$MYSQL_JDBC_SHA256 $MYSQL_JDBC_TARGET" | sha256sum -c -
# Tue, 30 Aug 2022 18:22:11 GMT
COPY file:0a1be11e2eb610a1dbcd415404e3a592641110b93090030cb831e3a19a163017 in /usr/local/tomcat/bin/ 
# Tue, 30 Aug 2022 18:22:11 GMT
COPY file:1b8409986f3e4eb79a7a0b18472cb2692a61d504fb5ef34292bc997b79fd760d in /usr/local/tomcat/webapps/ROOT/WEB-INF/hibernate.cfg.xml 
# Tue, 30 Aug 2022 18:22:11 GMT
RUN sed -i 's/<id>org.xwiki.platform:xwiki-platform-distribution-war/<id>org.xwiki.platform:xwiki-platform-distribution-docker/'   /usr/local/tomcat/webapps/ROOT/META-INF/extension.xed
# Tue, 30 Aug 2022 18:22:11 GMT
COPY file:a47c4dcd87c9dad97aff38c49188357e6193bcad50757e516cfb08a60d4de611 in /usr/local/bin/docker-entrypoint.sh 
# Tue, 30 Aug 2022 18:22:11 GMT
VOLUME [/usr/local/xwiki]
# Tue, 30 Aug 2022 18:22:12 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 30 Aug 2022 18:22:12 GMT
CMD ["xwiki"]
```

-	Layers:
	-	`sha256:d19f32bd9e4106d487f1a703fc2f09c8edadd92db4405d477978e8e466ab290d`  
		Last Modified: Tue, 02 Aug 2022 01:32:15 GMT  
		Size: 30.4 MB (30426136 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d65811de5a1ce73e051835187b84371fd526024c2be009224c3a1f5adaa87c90`  
		Last Modified: Fri, 12 Aug 2022 17:28:31 GMT  
		Size: 12.5 MB (12456003 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:038f6850cd14793dfe8f7ad5b44ffe6450a213068e067d07d0cf596142a6e79b`  
		Last Modified: Wed, 24 Aug 2022 19:28:04 GMT  
		Size: 46.5 MB (46498569 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:904c98e207563182da3e2d2dc0807b12c9456b51c902b8a29e3e59acc925e909`  
		Last Modified: Wed, 24 Aug 2022 19:27:57 GMT  
		Size: 159.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7bd424e54764dba0923d1efd0cd69b9e3cbcc8aed682152775e2ecb8bc0958a9`  
		Last Modified: Wed, 24 Aug 2022 22:23:24 GMT  
		Size: 174.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:38104d2f7babb2b547ce73e8f65003bb60f12fa34c49ed7f390afbb30d889dec`  
		Last Modified: Wed, 24 Aug 2022 22:30:07 GMT  
		Size: 12.2 MB (12185036 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d394d1adc9c06f95fa14c8e4c203e1bf9afe76daa2d0b106a04adc618fca56b8`  
		Last Modified: Wed, 24 Aug 2022 22:30:06 GMT  
		Size: 452.2 KB (452155 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:14e9ee9ce292eeaa67e04d26098327c27932a9e6eada30d749417b5b4236206a`  
		Last Modified: Wed, 24 Aug 2022 22:30:06 GMT  
		Size: 130.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bcb2ca2129c38687a12dac8b147009b46603364fa6e7073d16dceee1bf4a5b6e`  
		Last Modified: Mon, 29 Aug 2022 20:12:49 GMT  
		Size: 178.3 MB (178335886 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4cf2f801ef13fbf2aef5664874a1c8213c0242f9bb052a043671f9c570f9b2bc`  
		Last Modified: Tue, 30 Aug 2022 18:24:35 GMT  
		Size: 292.7 MB (292675739 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:357406d1edee6da496f9ad07149003d85b75a245b512158192a67bbdee318c3d`  
		Last Modified: Tue, 30 Aug 2022 18:24:16 GMT  
		Size: 2.4 MB (2375231 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:415b3f4d81c6027a43e6709facedce7d54f5d7951e331a827c83145a20501f23`  
		Last Modified: Tue, 30 Aug 2022 18:24:15 GMT  
		Size: 1.3 KB (1345 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:585fce8f38c668e7e3b3211ceaf99e0821f92a76cb89c9438c05c2f917956a93`  
		Last Modified: Tue, 30 Aug 2022 18:24:15 GMT  
		Size: 2.3 KB (2305 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:18effd8ff1056bf335e0448c683288882113697edcd630518173af26d31c3ad6`  
		Last Modified: Tue, 30 Aug 2022 18:24:15 GMT  
		Size: 5.3 KB (5335 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7e72ccf0e9a9b727a0d9b0ba604df332b58846f6de38f28e4cc3622304db157d`  
		Last Modified: Tue, 30 Aug 2022 18:24:15 GMT  
		Size: 2.5 KB (2499 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `xwiki:lts-mysql-tomcat` - linux; arm64 variant v8

```console
$ docker pull xwiki@sha256:1c164b8cf7344828100b6983387f94bf7ddc4333a936efdea64459760ccffb14
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **566.4 MB (566438009 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f62476a42ed6d7bf231b4d4b5663f343071b07a0fcbb275fa6adeaa38e88a08f`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["xwiki"]`

```dockerfile
# Tue, 02 Aug 2022 01:18:59 GMT
ADD file:3db67543ea64bf6723921d19cc5d0483db5c6658fc95834d8b2b5ed48a4cbacd in / 
# Tue, 02 Aug 2022 01:18:59 GMT
CMD ["bash"]
# Thu, 11 Aug 2022 18:40:31 GMT
ENV JAVA_HOME=/opt/java/openjdk
# Thu, 11 Aug 2022 18:40:32 GMT
ENV PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 11 Aug 2022 18:40:33 GMT
ENV LANG=en_US.UTF-8 LANGUAGE=en_US:en LC_ALL=en_US.UTF-8
# Fri, 12 Aug 2022 17:40:47 GMT
RUN apt-get update     && DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends tzdata curl wget ca-certificates fontconfig locales     && echo "en_US.UTF-8 UTF-8" >> /etc/locale.gen     && locale-gen en_US.UTF-8     && rm -rf /var/lib/apt/lists/*
# Wed, 24 Aug 2022 19:41:05 GMT
ENV JAVA_VERSION=jdk-11.0.16.1+1
# Wed, 24 Aug 2022 19:41:57 GMT
RUN set -eux;     ARCH="$(dpkg --print-architecture)";     case "${ARCH}" in        aarch64|arm64)          ESUM='b6607f28fa2906d612d517f0babe4f0f895aa1c3f901edcddb493e33c1e27364';          BINARY_URL='https://github.com/adoptium/temurin11-binaries/releases/download/jdk-11.0.16.1%2B1/OpenJDK11U-jre_aarch64_linux_hotspot_11.0.16.1_1.tar.gz';          ;;        armhf|arm)          ESUM='2ee7fe636a6a57e4718dfe597e8097b93ef8d976e4b05384433777c9f0526f5a';          BINARY_URL='https://github.com/adoptium/temurin11-binaries/releases/download/jdk-11.0.16.1%2B1/OpenJDK11U-jre_arm_linux_hotspot_11.0.16.1_1.tar.gz';          ;;        ppc64el|powerpc:common64)          ESUM='f76b64b201b64ff37f77f73ead546ebcf2af9862b7cd1a1f4e0e5628e3f6a7fc';          BINARY_URL='https://github.com/adoptium/temurin11-binaries/releases/download/jdk-11.0.16.1%2B1/OpenJDK11U-jre_ppc64le_linux_hotspot_11.0.16.1_1.tar.gz';          ;;        s390x|s390:64-bit)          ESUM='bf01489459135ab0ce1ad346a56f0dfeb2d6fe4e59854ef76a6bb989ac403f91';          BINARY_URL='https://github.com/adoptium/temurin11-binaries/releases/download/jdk-11.0.16.1%2B1/OpenJDK11U-jre_s390x_linux_hotspot_11.0.16.1_1.tar.gz';          ;;        amd64|i386:x86-64)          ESUM='1ffe1a682e8179e35238bf3f93aba0cb185850e202c676f41d38cb0561883eda';          BINARY_URL='https://github.com/adoptium/temurin11-binaries/releases/download/jdk-11.0.16.1%2B1/OpenJDK11U-jre_x64_linux_hotspot_11.0.16.1_1.tar.gz';          ;;        *)          echo "Unsupported arch: ${ARCH}";          exit 1;          ;;     esac; 	  wget -O /tmp/openjdk.tar.gz ${BINARY_URL}; 	  echo "${ESUM} */tmp/openjdk.tar.gz" | sha256sum -c -; 	  mkdir -p "$JAVA_HOME"; 	  tar --extract 	      --file /tmp/openjdk.tar.gz 	      --directory "$JAVA_HOME" 	      --strip-components 1 	      --no-same-owner 	  ;     rm /tmp/openjdk.tar.gz;     find "$JAVA_HOME/lib" -name '*.so' -exec dirname '{}' ';' | sort -u > /etc/ld.so.conf.d/docker-openjdk.conf;     ldconfig;     java -Xshare:dump;
# Wed, 24 Aug 2022 19:41:58 GMT
RUN echo Verifying install ...     && fileEncoding="$(echo 'System.out.println(System.getProperty("file.encoding"))' | jshell -s -)"; [ "$fileEncoding" = 'UTF-8' ]; rm -rf ~/.java     && echo java --version && java --version     && echo Complete.
# Wed, 24 Aug 2022 21:20:21 GMT
ENV CATALINA_HOME=/usr/local/tomcat
# Wed, 24 Aug 2022 21:20:21 GMT
ENV PATH=/usr/local/tomcat/bin:/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 24 Aug 2022 21:20:22 GMT
RUN mkdir -p "$CATALINA_HOME"
# Wed, 24 Aug 2022 21:20:23 GMT
WORKDIR /usr/local/tomcat
# Wed, 24 Aug 2022 21:20:24 GMT
ENV TOMCAT_NATIVE_LIBDIR=/usr/local/tomcat/native-jni-lib
# Wed, 24 Aug 2022 21:20:25 GMT
ENV LD_LIBRARY_PATH=/usr/local/tomcat/native-jni-lib
# Wed, 24 Aug 2022 21:30:16 GMT
ENV GPG_KEYS=48F8E69F6390C9F25CFEDCD268248959359E722B A9C5DF4D22E99998D9875A5110C01C5A2F6059E7 DCFD35E0BF8CA7344752DE8B6FB21E8933C60243
# Wed, 24 Aug 2022 21:30:17 GMT
ENV TOMCAT_MAJOR=9
# Wed, 24 Aug 2022 21:30:18 GMT
ENV TOMCAT_VERSION=9.0.65
# Wed, 24 Aug 2022 21:30:19 GMT
ENV TOMCAT_SHA512=2ae846848b8436856be11cfa18d9c62caa06ca7d3134012b2e10cbf6078753c4af20cc5d37f7dc75f1779f5c59d7c033850b8626534c3ce7e389641a67963cf6
# Wed, 24 Aug 2022 21:30:21 GMT
COPY dir:61f3b0b84c95fbd33c379e9173b35a8724f3ac23ab9c8da0525ca9cedeef1145 in /usr/local/tomcat 
# Wed, 24 Aug 2022 21:30:27 GMT
RUN set -eux; 	apt-get update; 	xargs -rt apt-get install -y --no-install-recommends < "$TOMCAT_NATIVE_LIBDIR/.dependencies.txt"; 	rm -rf /var/lib/apt/lists/*
# Wed, 24 Aug 2022 21:30:29 GMT
RUN set -eux; 	nativeLines="$(catalina.sh configtest 2>&1)"; 	nativeLines="$(echo "$nativeLines" | grep 'Apache Tomcat Native')"; 	nativeLines="$(echo "$nativeLines" | sort -u)"; 	if ! echo "$nativeLines" | grep -E 'INFO: Loaded( APR based)? Apache Tomcat Native library' >&2; then 		echo >&2 "$nativeLines"; 		exit 1; 	fi
# Wed, 24 Aug 2022 21:30:30 GMT
EXPOSE 8080
# Wed, 24 Aug 2022 21:30:31 GMT
CMD ["catalina.sh" "run"]
# Mon, 29 Aug 2022 19:03:06 GMT
LABEL org.opencontainers.image.authors=XWiki Development Team <committers@xwiki.org>
# Mon, 29 Aug 2022 19:03:06 GMT
LABEL org.opencontainers.image.url=https://hub.docker.com/_/xwiki
# Mon, 29 Aug 2022 19:03:07 GMT
LABEL org.opencontainers.image.documentation=https://hub.docker.com/_/xwiki
# Mon, 29 Aug 2022 19:03:08 GMT
LABEL org.opencontainers.image.source=https://github.com/xwiki/xwiki-docker.git
# Mon, 29 Aug 2022 19:03:09 GMT
LABEL org.opencontainers.image.vendor=xwiki.org
# Mon, 29 Aug 2022 19:03:10 GMT
LABEL org.opencontainers.image.licenses=LGPL-2.1
# Mon, 29 Aug 2022 19:03:49 GMT
RUN apt-get update &&   apt-get --no-install-recommends -y install     curl     libreoffice     unzip     procps &&   rm -rf /var/lib/apt/lists/*
# Tue, 30 Aug 2022 18:48:48 GMT
ENV XWIKI_VERSION=13.10.9
# Tue, 30 Aug 2022 18:48:48 GMT
ENV XWIKI_URL_PREFIX=https://maven.xwiki.org/releases/org/xwiki/platform/xwiki-platform-distribution-war/13.10.9
# Tue, 30 Aug 2022 18:48:49 GMT
ENV XWIKI_DOWNLOAD_SHA256=ad57639016b1bfd1cdf84de764b310a65416832645c6bbfd933ec26fd977bb6a
# Tue, 30 Aug 2022 18:49:18 GMT
RUN rm -rf /usr/local/tomcat/webapps/* &&   mkdir -p /usr/local/tomcat/temp &&   mkdir -p /usr/local/xwiki/data &&   curl -fSL "${XWIKI_URL_PREFIX}/xwiki-platform-distribution-war-${XWIKI_VERSION}.war" -o xwiki.war &&   echo "$XWIKI_DOWNLOAD_SHA256 xwiki.war" | sha256sum -c - &&   unzip -d /usr/local/tomcat/webapps/ROOT xwiki.war &&   rm -f xwiki.war
# Tue, 30 Aug 2022 18:49:19 GMT
ENV MYSQL_JDBC_VERSION=8.0.30
# Tue, 30 Aug 2022 18:49:19 GMT
ENV MYSQL_JDBC_SHA256=b5bf2f0987197c30adf74a9e419b89cda4c257da2d1142871f508416d5f2227a
# Tue, 30 Aug 2022 18:49:20 GMT
ENV MYSQL_JDBC_PREFIX=https://repo1.maven.org/maven2/mysql/mysql-connector-java/8.0.30
# Tue, 30 Aug 2022 18:49:21 GMT
ENV MYSQL_JDBC_ARTIFACT=mysql-connector-java-8.0.30.jar
# Tue, 30 Aug 2022 18:49:22 GMT
ENV MYSQL_JDBC_TARGET=/usr/local/tomcat/webapps/ROOT/WEB-INF/lib/mysql-connector-java-8.0.30.jar
# Tue, 30 Aug 2022 18:49:24 GMT
RUN curl -fSL "${MYSQL_JDBC_PREFIX}/${MYSQL_JDBC_ARTIFACT}" -o $MYSQL_JDBC_TARGET &&   echo "$MYSQL_JDBC_SHA256 $MYSQL_JDBC_TARGET" | sha256sum -c -
# Tue, 30 Aug 2022 18:49:25 GMT
COPY file:0a1be11e2eb610a1dbcd415404e3a592641110b93090030cb831e3a19a163017 in /usr/local/tomcat/bin/ 
# Tue, 30 Aug 2022 18:49:26 GMT
COPY file:1b8409986f3e4eb79a7a0b18472cb2692a61d504fb5ef34292bc997b79fd760d in /usr/local/tomcat/webapps/ROOT/WEB-INF/hibernate.cfg.xml 
# Tue, 30 Aug 2022 18:49:27 GMT
RUN sed -i 's/<id>org.xwiki.platform:xwiki-platform-distribution-war/<id>org.xwiki.platform:xwiki-platform-distribution-docker/'   /usr/local/tomcat/webapps/ROOT/META-INF/extension.xed
# Tue, 30 Aug 2022 18:49:28 GMT
COPY file:a47c4dcd87c9dad97aff38c49188357e6193bcad50757e516cfb08a60d4de611 in /usr/local/bin/docker-entrypoint.sh 
# Tue, 30 Aug 2022 18:49:28 GMT
VOLUME [/usr/local/xwiki]
# Tue, 30 Aug 2022 18:49:29 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 30 Aug 2022 18:49:30 GMT
CMD ["xwiki"]
```

-	Layers:
	-	`sha256:4a3049d340b7d3651a954fd25a32c42feb1086889d6287e2f15468aef865c5c4`  
		Last Modified: Tue, 02 Aug 2022 01:20:49 GMT  
		Size: 28.4 MB (28381155 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a9a729bc90f861d8ccd964a45b6f12093afcb2172c43390409a73e938d36aa1a`  
		Last Modified: Fri, 12 Aug 2022 17:51:29 GMT  
		Size: 12.4 MB (12414351 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:042d81bb6b9272594d41df4317c8cf379d5be12ec7996d43c3ff4895df8f7481`  
		Last Modified: Wed, 24 Aug 2022 19:48:46 GMT  
		Size: 44.8 MB (44826689 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e43604d6aa5b7375e91eff36fad8ec1318a6778b92030981be3df7a05dd83427`  
		Last Modified: Wed, 24 Aug 2022 19:48:39 GMT  
		Size: 158.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:95f4ffb2ea5560a3bd73f2a4330ac7bb7ac6fa090a621775164836bad8d7b6b7`  
		Last Modified: Wed, 24 Aug 2022 21:49:52 GMT  
		Size: 140.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a769d4756b889f1731b5a45381c4c8201ef34c9f17d41190afc013b549bf4dc4`  
		Last Modified: Wed, 24 Aug 2022 21:58:03 GMT  
		Size: 12.2 MB (12191517 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bcf5121ba4d99957a68a6f13ebfc857a9d43d83e93ec97e7d5468195af81e6d8`  
		Last Modified: Wed, 24 Aug 2022 21:58:01 GMT  
		Size: 214.4 KB (214396 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:49b0de79d874a72e9cc6f0da5d66326955c607dac2cbfb69f31074dc9e5936a5`  
		Last Modified: Mon, 29 Aug 2022 19:13:40 GMT  
		Size: 173.3 MB (173346883 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:27f6d371be3a7467abf4d4f417bec237eecd1d102c9cc6de9153c5f0a88649ff`  
		Last Modified: Tue, 30 Aug 2022 18:53:21 GMT  
		Size: 292.7 MB (292675990 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4d892b4e14a25443c7e2bcd0315af9ff2397e66b8f07c2ccd6c030d7932aec81`  
		Last Modified: Tue, 30 Aug 2022 18:52:59 GMT  
		Size: 2.4 MB (2375232 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8f9a7b5db79a8b12a83f8914dcf10af180bbce5cd29a498889c235a319b837c5`  
		Last Modified: Tue, 30 Aug 2022 18:52:59 GMT  
		Size: 1.3 KB (1346 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4f0296ea3ce1711c78af87482268591f991dd089265d18e52e747bb6312a9c87`  
		Last Modified: Tue, 30 Aug 2022 18:52:59 GMT  
		Size: 2.3 KB (2310 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:96b7a4a3b435e39083178243672b6795a135f21155c536dd7dfa8af5d78bb6a7`  
		Last Modified: Tue, 30 Aug 2022 18:52:59 GMT  
		Size: 5.3 KB (5337 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:27128ae8958d791ef374bf1fc593ed86f7b9a10cc3eec8552fae6bbf54e67cfc`  
		Last Modified: Tue, 30 Aug 2022 18:52:59 GMT  
		Size: 2.5 KB (2505 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
