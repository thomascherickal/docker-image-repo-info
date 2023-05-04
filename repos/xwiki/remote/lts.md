## `xwiki:lts`

```console
$ docker pull xwiki@sha256:bed801ab9e6aad7cca1950c2af43905b5f2b5fe14ba11bf85a5fff075a52eb7f
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `xwiki:lts` - linux; amd64

```console
$ docker pull xwiki@sha256:517d2728b0f6dc6b5a31d6be9caefd593bd3a62c0f191b90f28bb065a336bf7e
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **593.1 MB (593107142 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:17ca8de588e04caec7bb194aae1c0538894874fdb046f3569b71db49145dbf74`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["xwiki"]`

```dockerfile
# Wed, 08 Mar 2023 04:44:25 GMT
ARG RELEASE
# Wed, 08 Mar 2023 04:44:25 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Wed, 08 Mar 2023 04:44:25 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Wed, 08 Mar 2023 04:44:25 GMT
LABEL org.opencontainers.image.version=22.04
# Wed, 08 Mar 2023 04:44:27 GMT
ADD file:c8ef6447752cab2541ffca9e3cfa27d581f3491bc8f356f6eafd951243609341 in / 
# Wed, 08 Mar 2023 04:44:27 GMT
CMD ["/bin/bash"]
# Thu, 16 Mar 2023 02:44:03 GMT
ENV JAVA_HOME=/opt/java/openjdk
# Thu, 16 Mar 2023 02:44:03 GMT
ENV PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 16 Mar 2023 02:44:04 GMT
ENV LANG=en_US.UTF-8 LANGUAGE=en_US:en LC_ALL=en_US.UTF-8
# Thu, 16 Mar 2023 02:44:26 GMT
RUN apt-get update     && DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends tzdata curl wget ca-certificates fontconfig locales     && echo "en_US.UTF-8 UTF-8" >> /etc/locale.gen     && locale-gen en_US.UTF-8     && rm -rf /var/lib/apt/lists/*
# Wed, 26 Apr 2023 19:21:22 GMT
ENV JAVA_VERSION=jdk-11.0.19+7
# Wed, 26 Apr 2023 19:22:16 GMT
RUN set -eux;     ARCH="$(dpkg --print-architecture)";     case "${ARCH}" in        aarch64|arm64)          ESUM='1fe4b20d808f393422610818711c728331992a4455eeeb061d3d05b45412771d';          BINARY_URL='https://github.com/adoptium/temurin11-binaries/releases/download/jdk-11.0.19%2B7/OpenJDK11U-jre_aarch64_linux_hotspot_11.0.19_7.tar.gz';          ;;        armhf|arm)          ESUM='cb754b055177381f9f6852b7e5469904a15edddd7f8e136043c28b1e33aee47c';          BINARY_URL='https://github.com/adoptium/temurin11-binaries/releases/download/jdk-11.0.19%2B7/OpenJDK11U-jre_arm_linux_hotspot_11.0.19_7.tar.gz';          ;;        ppc64el|powerpc:common64)          ESUM='8019d938e5525938ec8e68e2989c4413263b0d9b7b3f20fe0c45f6d967919cfb';          BINARY_URL='https://github.com/adoptium/temurin11-binaries/releases/download/jdk-11.0.19%2B7/OpenJDK11U-jre_ppc64le_linux_hotspot_11.0.19_7.tar.gz';          ;;        s390x|s390:64-bit)          ESUM='058419435fe6212d1bc305a14f578c314f9ff9a2d96d523c178120e84231c733';          BINARY_URL='https://github.com/adoptium/temurin11-binaries/releases/download/jdk-11.0.19%2B7/OpenJDK11U-jre_s390x_linux_hotspot_11.0.19_7.tar.gz';          ;;        amd64|i386:x86-64)          ESUM='32dcf760664f93531594b72ce9226e9216567de5705a23c9ff5a77c797948054';          BINARY_URL='https://github.com/adoptium/temurin11-binaries/releases/download/jdk-11.0.19%2B7/OpenJDK11U-jre_x64_linux_hotspot_11.0.19_7.tar.gz';          ;;        *)          echo "Unsupported arch: ${ARCH}";          exit 1;          ;;     esac; 	  wget -O /tmp/openjdk.tar.gz ${BINARY_URL}; 	  echo "${ESUM} */tmp/openjdk.tar.gz" | sha256sum -c -; 	  mkdir -p "$JAVA_HOME"; 	  tar --extract 	      --file /tmp/openjdk.tar.gz 	      --directory "$JAVA_HOME" 	      --strip-components 1 	      --no-same-owner 	  ;     rm -f /tmp/openjdk.tar.gz ${JAVA_HOME}/src.zip;     find "$JAVA_HOME/lib" -name '*.so' -exec dirname '{}' ';' | sort -u > /etc/ld.so.conf.d/docker-openjdk.conf;     ldconfig;     java -Xshare:dump;
# Wed, 26 Apr 2023 19:22:17 GMT
RUN echo Verifying install ...     && fileEncoding="$(echo 'System.out.println(System.getProperty("file.encoding"))' | jshell -s -)"; [ "$fileEncoding" = 'UTF-8' ]; rm -rf ~/.java     && echo java --version && java --version     && echo Complete.
# Wed, 26 Apr 2023 21:37:18 GMT
ENV CATALINA_HOME=/usr/local/tomcat
# Wed, 26 Apr 2023 21:37:18 GMT
ENV PATH=/usr/local/tomcat/bin:/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 26 Apr 2023 21:37:19 GMT
RUN mkdir -p "$CATALINA_HOME"
# Wed, 26 Apr 2023 21:37:19 GMT
WORKDIR /usr/local/tomcat
# Wed, 26 Apr 2023 21:37:19 GMT
ENV TOMCAT_NATIVE_LIBDIR=/usr/local/tomcat/native-jni-lib
# Wed, 26 Apr 2023 21:37:19 GMT
ENV LD_LIBRARY_PATH=/usr/local/tomcat/native-jni-lib
# Wed, 26 Apr 2023 21:39:48 GMT
ENV GPG_KEYS=48F8E69F6390C9F25CFEDCD268248959359E722B A9C5DF4D22E99998D9875A5110C01C5A2F6059E7 DCFD35E0BF8CA7344752DE8B6FB21E8933C60243
# Wed, 26 Apr 2023 21:39:48 GMT
ENV TOMCAT_MAJOR=9
# Wed, 26 Apr 2023 21:39:48 GMT
ENV TOMCAT_VERSION=9.0.74
# Wed, 26 Apr 2023 21:39:48 GMT
ENV TOMCAT_SHA512=0e173fc2a76404c41c571c50a1956a2b867870d767200bd30f48d89bf04a4b6337f12e6577415da932cd2dfef9b4e9e9fdd52bd873afb06c6258b0e64244a44e
# Wed, 26 Apr 2023 21:39:49 GMT
COPY dir:5320b315c314b0e9f3cc6996868871dc8ed5e2b7036f98555dcf5deb36030170 in /usr/local/tomcat 
# Wed, 26 Apr 2023 21:39:53 GMT
RUN set -eux; 	apt-get update; 	xargs -rt apt-get install -y --no-install-recommends < "$TOMCAT_NATIVE_LIBDIR/.dependencies.txt"; 	rm -rf /var/lib/apt/lists/*
# Wed, 26 Apr 2023 21:39:54 GMT
RUN set -eux; 	nativeLines="$(catalina.sh configtest 2>&1)"; 	nativeLines="$(echo "$nativeLines" | grep 'Apache Tomcat Native')"; 	nativeLines="$(echo "$nativeLines" | sort -u)"; 	if ! echo "$nativeLines" | grep -E 'INFO: Loaded( APR based)? Apache Tomcat Native library' >&2; then 		echo >&2 "$nativeLines"; 		exit 1; 	fi
# Wed, 26 Apr 2023 21:39:55 GMT
EXPOSE 8080
# Wed, 26 Apr 2023 21:39:55 GMT
CMD ["catalina.sh" "run"]
# Wed, 26 Apr 2023 23:27:30 GMT
LABEL org.opencontainers.image.authors=XWiki Development Team <committers@xwiki.org>
# Wed, 26 Apr 2023 23:27:30 GMT
LABEL org.opencontainers.image.url=https://hub.docker.com/_/xwiki
# Wed, 26 Apr 2023 23:27:30 GMT
LABEL org.opencontainers.image.documentation=https://hub.docker.com/_/xwiki
# Wed, 26 Apr 2023 23:27:30 GMT
LABEL org.opencontainers.image.source=https://github.com/xwiki/xwiki-docker.git
# Wed, 26 Apr 2023 23:27:30 GMT
LABEL org.opencontainers.image.vendor=xwiki.org
# Wed, 26 Apr 2023 23:27:30 GMT
LABEL org.opencontainers.image.licenses=LGPL-2.1
# Wed, 26 Apr 2023 23:29:06 GMT
RUN apt-get update &&   apt-get --no-install-recommends -y install     curl     libreoffice     unzip     procps &&   rm -rf /var/lib/apt/lists/*
# Wed, 26 Apr 2023 23:31:20 GMT
ENV XWIKI_VERSION=14.10.9
# Wed, 26 Apr 2023 23:31:20 GMT
ENV XWIKI_URL_PREFIX=https://maven.xwiki.org/releases/org/xwiki/platform/xwiki-platform-distribution-war/14.10.9
# Wed, 26 Apr 2023 23:31:20 GMT
ENV XWIKI_DOWNLOAD_SHA256=81594962a2101d54866bccf768ea5b1637f836c57c5b212e221d043e96f5f35d
# Wed, 26 Apr 2023 23:31:59 GMT
RUN rm -rf /usr/local/tomcat/webapps/* &&   mkdir -p /usr/local/tomcat/temp &&   mkdir -p /usr/local/xwiki/data &&   curl -fSL "${XWIKI_URL_PREFIX}/xwiki-platform-distribution-war-${XWIKI_VERSION}.war" -o xwiki.war &&   echo "$XWIKI_DOWNLOAD_SHA256 xwiki.war" | sha256sum -c - &&   unzip -d /usr/local/tomcat/webapps/ROOT xwiki.war &&   rm -f xwiki.war
# Wed, 26 Apr 2023 23:32:00 GMT
ENV MYSQL_JDBC_VERSION=8.0.33
# Wed, 26 Apr 2023 23:32:00 GMT
ENV MYSQL_JDBC_SHA256=e2a3b2fc726a1ac64e998585db86b30fa8bf3f706195b78bb77c5f99bf877bd9
# Wed, 26 Apr 2023 23:32:00 GMT
ENV MYSQL_JDBC_PREFIX=https://repo1.maven.org/maven2/com/mysql/mysql-connector-j/8.0.33
# Wed, 26 Apr 2023 23:32:00 GMT
ENV MYSQL_JDBC_ARTIFACT=mysql-connector-j-8.0.33.jar
# Wed, 26 Apr 2023 23:32:00 GMT
ENV MYSQL_JDBC_TARGET=/usr/local/tomcat/webapps/ROOT/WEB-INF/lib/mysql-connector-j-8.0.33.jar
# Wed, 26 Apr 2023 23:32:01 GMT
RUN curl -fSL "${MYSQL_JDBC_PREFIX}/${MYSQL_JDBC_ARTIFACT}" -o $MYSQL_JDBC_TARGET &&   echo "$MYSQL_JDBC_SHA256 $MYSQL_JDBC_TARGET" | sha256sum -c -
# Wed, 26 Apr 2023 23:32:01 GMT
COPY file:0a1be11e2eb610a1dbcd415404e3a592641110b93090030cb831e3a19a163017 in /usr/local/tomcat/bin/ 
# Wed, 26 Apr 2023 23:32:02 GMT
COPY file:1b8409986f3e4eb79a7a0b18472cb2692a61d504fb5ef34292bc997b79fd760d in /usr/local/tomcat/webapps/ROOT/WEB-INF/hibernate.cfg.xml 
# Wed, 26 Apr 2023 23:32:02 GMT
RUN sed -i 's/<id>org.xwiki.platform:xwiki-platform-distribution-war/<id>org.xwiki.platform:xwiki-platform-distribution-docker/'   /usr/local/tomcat/webapps/ROOT/META-INF/extension.xed
# Wed, 26 Apr 2023 23:32:02 GMT
COPY file:a47c4dcd87c9dad97aff38c49188357e6193bcad50757e516cfb08a60d4de611 in /usr/local/bin/docker-entrypoint.sh 
# Wed, 26 Apr 2023 23:32:02 GMT
VOLUME [/usr/local/xwiki]
# Wed, 26 Apr 2023 23:32:02 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 26 Apr 2023 23:32:02 GMT
CMD ["xwiki"]
```

-	Layers:
	-	`sha256:74ac377868f863e123f24c409f79709f7563fa464557c36a09cf6f85c8b92b7f`  
		Last Modified: Wed, 08 Mar 2023 09:03:15 GMT  
		Size: 30.4 MB (30429963 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b9cabe75b440d785eb2f20422368c248b28fd9c219a5d5db5aacb7de3d43f02c`  
		Last Modified: Thu, 16 Mar 2023 02:50:26 GMT  
		Size: 12.4 MB (12432056 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bfbcf8099cd9542ade150b47ea122e9893483fa7b4eeb7cb77dcd4fce39e8daf`  
		Last Modified: Wed, 26 Apr 2023 19:31:33 GMT  
		Size: 46.7 MB (46666342 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c3863dc13d82a92b998a5173cbace3570e2ae1e307b6f15c1a615218421c75f7`  
		Last Modified: Wed, 26 Apr 2023 19:31:26 GMT  
		Size: 160.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:604e9cacab100369ab7798fdac4858aa39492f22e4dc4aaa8f1be05b524bfc15`  
		Last Modified: Wed, 26 Apr 2023 21:51:09 GMT  
		Size: 172.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a016b39d8d26774e51e6a79fcb03c5f3206045b806b5f3609556773179d787ef`  
		Last Modified: Wed, 26 Apr 2023 21:53:17 GMT  
		Size: 12.2 MB (12233838 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:db258d59e12806948bf3e4af14a5d62d87e867a14562a0fba551388742906574`  
		Last Modified: Wed, 26 Apr 2023 21:53:16 GMT  
		Size: 3.0 MB (2967684 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d2dce82d22e3a93205400ba38dc99d3f09142785886bd8d1b0b0f656e936bba7`  
		Last Modified: Wed, 26 Apr 2023 21:53:16 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:de7a163738aedd6a170822731b8a82a6768963eb6bec68f44fd6672fb36eb8f7`  
		Last Modified: Wed, 26 Apr 2023 23:33:42 GMT  
		Size: 178.8 MB (178803411 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0d915df1c99877f5a0143382db8e0de3cca1ed6e05fddbae2b749f882b69c02e`  
		Last Modified: Wed, 26 Apr 2023 23:35:27 GMT  
		Size: 307.2 MB (307217562 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7da88e017a4494689d6646cf676de9ebbdd93ed05a2ad59ff7b7ae3e06d01670`  
		Last Modified: Wed, 26 Apr 2023 23:35:11 GMT  
		Size: 2.3 MB (2343672 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fada470f9b598e389a101dd4a99c9dbeae41ed61820dd65221fbd4c848cefb0b`  
		Last Modified: Wed, 26 Apr 2023 23:35:11 GMT  
		Size: 1.3 KB (1341 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a1811312ee607d76c4e010ff100523775983ed529d86a69e57aa27e1cc495403`  
		Last Modified: Wed, 26 Apr 2023 23:35:11 GMT  
		Size: 2.3 KB (2303 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:44c50a2cb9bd3ca62f01350f237d94331f8acc5dd918f837427dd65e139c3879`  
		Last Modified: Wed, 26 Apr 2023 23:35:11 GMT  
		Size: 6.0 KB (6012 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:842d6ba01d6e5c02dd731caa4cfe9080692ede7add427ccd06f70cbddf545a43`  
		Last Modified: Wed, 26 Apr 2023 23:35:11 GMT  
		Size: 2.5 KB (2497 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `xwiki:lts` - linux; arm64 variant v8

```console
$ docker pull xwiki@sha256:90f355a5633fdbd7df847afb3eb8839fec15681b76b5f9372ed3eada899e351a
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **584.2 MB (584232359 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:8b823c253678cf2cca11709d3c7653c647ce25bfc30322b6fbb2a50f37bc8854`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["xwiki"]`

```dockerfile
# Wed, 08 Mar 2023 04:32:38 GMT
ARG RELEASE
# Wed, 08 Mar 2023 04:32:38 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Wed, 08 Mar 2023 04:32:38 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Wed, 08 Mar 2023 04:32:39 GMT
LABEL org.opencontainers.image.version=22.04
# Wed, 08 Mar 2023 04:32:40 GMT
ADD file:79b36308bc382d9cae7197b4cecc21430f4e8f3e8bec3547d0f00bcff7681e60 in / 
# Wed, 08 Mar 2023 04:32:41 GMT
CMD ["/bin/bash"]
# Thu, 16 Mar 2023 01:52:25 GMT
ENV JAVA_HOME=/opt/java/openjdk
# Thu, 16 Mar 2023 01:52:25 GMT
ENV PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 16 Mar 2023 01:52:26 GMT
ENV LANG=en_US.UTF-8 LANGUAGE=en_US:en LC_ALL=en_US.UTF-8
# Thu, 16 Mar 2023 01:52:57 GMT
RUN apt-get update     && DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends tzdata curl wget ca-certificates fontconfig locales     && echo "en_US.UTF-8 UTF-8" >> /etc/locale.gen     && locale-gen en_US.UTF-8     && rm -rf /var/lib/apt/lists/*
# Wed, 26 Apr 2023 19:40:30 GMT
ENV JAVA_VERSION=jdk-11.0.19+7
# Wed, 26 Apr 2023 19:41:19 GMT
RUN set -eux;     ARCH="$(dpkg --print-architecture)";     case "${ARCH}" in        aarch64|arm64)          ESUM='1fe4b20d808f393422610818711c728331992a4455eeeb061d3d05b45412771d';          BINARY_URL='https://github.com/adoptium/temurin11-binaries/releases/download/jdk-11.0.19%2B7/OpenJDK11U-jre_aarch64_linux_hotspot_11.0.19_7.tar.gz';          ;;        armhf|arm)          ESUM='cb754b055177381f9f6852b7e5469904a15edddd7f8e136043c28b1e33aee47c';          BINARY_URL='https://github.com/adoptium/temurin11-binaries/releases/download/jdk-11.0.19%2B7/OpenJDK11U-jre_arm_linux_hotspot_11.0.19_7.tar.gz';          ;;        ppc64el|powerpc:common64)          ESUM='8019d938e5525938ec8e68e2989c4413263b0d9b7b3f20fe0c45f6d967919cfb';          BINARY_URL='https://github.com/adoptium/temurin11-binaries/releases/download/jdk-11.0.19%2B7/OpenJDK11U-jre_ppc64le_linux_hotspot_11.0.19_7.tar.gz';          ;;        s390x|s390:64-bit)          ESUM='058419435fe6212d1bc305a14f578c314f9ff9a2d96d523c178120e84231c733';          BINARY_URL='https://github.com/adoptium/temurin11-binaries/releases/download/jdk-11.0.19%2B7/OpenJDK11U-jre_s390x_linux_hotspot_11.0.19_7.tar.gz';          ;;        amd64|i386:x86-64)          ESUM='32dcf760664f93531594b72ce9226e9216567de5705a23c9ff5a77c797948054';          BINARY_URL='https://github.com/adoptium/temurin11-binaries/releases/download/jdk-11.0.19%2B7/OpenJDK11U-jre_x64_linux_hotspot_11.0.19_7.tar.gz';          ;;        *)          echo "Unsupported arch: ${ARCH}";          exit 1;          ;;     esac; 	  wget -O /tmp/openjdk.tar.gz ${BINARY_URL}; 	  echo "${ESUM} */tmp/openjdk.tar.gz" | sha256sum -c -; 	  mkdir -p "$JAVA_HOME"; 	  tar --extract 	      --file /tmp/openjdk.tar.gz 	      --directory "$JAVA_HOME" 	      --strip-components 1 	      --no-same-owner 	  ;     rm -f /tmp/openjdk.tar.gz ${JAVA_HOME}/src.zip;     find "$JAVA_HOME/lib" -name '*.so' -exec dirname '{}' ';' | sort -u > /etc/ld.so.conf.d/docker-openjdk.conf;     ldconfig;     java -Xshare:dump;
# Wed, 26 Apr 2023 19:41:20 GMT
RUN echo Verifying install ...     && fileEncoding="$(echo 'System.out.println(System.getProperty("file.encoding"))' | jshell -s -)"; [ "$fileEncoding" = 'UTF-8' ]; rm -rf ~/.java     && echo java --version && java --version     && echo Complete.
# Wed, 26 Apr 2023 21:50:02 GMT
ENV CATALINA_HOME=/usr/local/tomcat
# Wed, 26 Apr 2023 21:50:03 GMT
ENV PATH=/usr/local/tomcat/bin:/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 26 Apr 2023 21:50:03 GMT
RUN mkdir -p "$CATALINA_HOME"
# Wed, 26 Apr 2023 21:50:03 GMT
WORKDIR /usr/local/tomcat
# Wed, 26 Apr 2023 21:50:03 GMT
ENV TOMCAT_NATIVE_LIBDIR=/usr/local/tomcat/native-jni-lib
# Wed, 26 Apr 2023 21:50:03 GMT
ENV LD_LIBRARY_PATH=/usr/local/tomcat/native-jni-lib
# Wed, 26 Apr 2023 21:52:19 GMT
ENV GPG_KEYS=48F8E69F6390C9F25CFEDCD268248959359E722B A9C5DF4D22E99998D9875A5110C01C5A2F6059E7 DCFD35E0BF8CA7344752DE8B6FB21E8933C60243
# Wed, 26 Apr 2023 21:52:19 GMT
ENV TOMCAT_MAJOR=9
# Wed, 26 Apr 2023 21:52:19 GMT
ENV TOMCAT_VERSION=9.0.74
# Wed, 26 Apr 2023 21:52:19 GMT
ENV TOMCAT_SHA512=0e173fc2a76404c41c571c50a1956a2b867870d767200bd30f48d89bf04a4b6337f12e6577415da932cd2dfef9b4e9e9fdd52bd873afb06c6258b0e64244a44e
# Wed, 03 May 2023 10:34:01 GMT
COPY dir:1b3ffa94d53334456e5196a86aeeb76ed6f795144bf9a998168cb83d7ab92bb5 in /usr/local/tomcat 
# Wed, 03 May 2023 10:34:05 GMT
RUN set -eux; 	apt-get update; 	xargs -rt apt-get install -y --no-install-recommends < "$TOMCAT_NATIVE_LIBDIR/.dependencies.txt"; 	rm -rf /var/lib/apt/lists/*
# Wed, 03 May 2023 10:34:06 GMT
RUN set -eux; 	nativeLines="$(catalina.sh configtest 2>&1)"; 	nativeLines="$(echo "$nativeLines" | grep 'Apache Tomcat Native')"; 	nativeLines="$(echo "$nativeLines" | sort -u)"; 	if ! echo "$nativeLines" | grep -E 'INFO: Loaded( APR based)? Apache Tomcat Native library' >&2; then 		echo >&2 "$nativeLines"; 		exit 1; 	fi
# Wed, 03 May 2023 10:34:06 GMT
EXPOSE 8080
# Wed, 03 May 2023 10:34:06 GMT
CMD ["catalina.sh" "run"]
# Thu, 04 May 2023 03:03:54 GMT
LABEL org.opencontainers.image.authors=XWiki Development Team <committers@xwiki.org>
# Thu, 04 May 2023 03:03:54 GMT
LABEL org.opencontainers.image.url=https://hub.docker.com/_/xwiki
# Thu, 04 May 2023 03:03:54 GMT
LABEL org.opencontainers.image.documentation=https://hub.docker.com/_/xwiki
# Thu, 04 May 2023 03:03:54 GMT
LABEL org.opencontainers.image.source=https://github.com/xwiki/xwiki-docker.git
# Thu, 04 May 2023 03:03:54 GMT
LABEL org.opencontainers.image.vendor=xwiki.org
# Thu, 04 May 2023 03:03:54 GMT
LABEL org.opencontainers.image.licenses=LGPL-2.1
# Thu, 04 May 2023 03:06:11 GMT
RUN apt-get update &&   apt-get --no-install-recommends -y install     curl     libreoffice     unzip     procps &&   rm -rf /var/lib/apt/lists/*
# Thu, 04 May 2023 03:08:27 GMT
ENV XWIKI_VERSION=14.10.9
# Thu, 04 May 2023 03:08:27 GMT
ENV XWIKI_URL_PREFIX=https://maven.xwiki.org/releases/org/xwiki/platform/xwiki-platform-distribution-war/14.10.9
# Thu, 04 May 2023 03:08:27 GMT
ENV XWIKI_DOWNLOAD_SHA256=81594962a2101d54866bccf768ea5b1637f836c57c5b212e221d043e96f5f35d
# Thu, 04 May 2023 03:09:06 GMT
RUN rm -rf /usr/local/tomcat/webapps/* &&   mkdir -p /usr/local/tomcat/temp &&   mkdir -p /usr/local/xwiki/data &&   curl -fSL "${XWIKI_URL_PREFIX}/xwiki-platform-distribution-war-${XWIKI_VERSION}.war" -o xwiki.war &&   echo "$XWIKI_DOWNLOAD_SHA256 xwiki.war" | sha256sum -c - &&   unzip -d /usr/local/tomcat/webapps/ROOT xwiki.war &&   rm -f xwiki.war
# Thu, 04 May 2023 03:09:09 GMT
ENV MYSQL_JDBC_VERSION=8.0.33
# Thu, 04 May 2023 03:09:09 GMT
ENV MYSQL_JDBC_SHA256=e2a3b2fc726a1ac64e998585db86b30fa8bf3f706195b78bb77c5f99bf877bd9
# Thu, 04 May 2023 03:09:09 GMT
ENV MYSQL_JDBC_PREFIX=https://repo1.maven.org/maven2/com/mysql/mysql-connector-j/8.0.33
# Thu, 04 May 2023 03:09:09 GMT
ENV MYSQL_JDBC_ARTIFACT=mysql-connector-j-8.0.33.jar
# Thu, 04 May 2023 03:09:09 GMT
ENV MYSQL_JDBC_TARGET=/usr/local/tomcat/webapps/ROOT/WEB-INF/lib/mysql-connector-j-8.0.33.jar
# Thu, 04 May 2023 03:09:10 GMT
RUN curl -fSL "${MYSQL_JDBC_PREFIX}/${MYSQL_JDBC_ARTIFACT}" -o $MYSQL_JDBC_TARGET &&   echo "$MYSQL_JDBC_SHA256 $MYSQL_JDBC_TARGET" | sha256sum -c -
# Thu, 04 May 2023 03:09:10 GMT
COPY file:0a1be11e2eb610a1dbcd415404e3a592641110b93090030cb831e3a19a163017 in /usr/local/tomcat/bin/ 
# Thu, 04 May 2023 03:09:10 GMT
COPY file:1b8409986f3e4eb79a7a0b18472cb2692a61d504fb5ef34292bc997b79fd760d in /usr/local/tomcat/webapps/ROOT/WEB-INF/hibernate.cfg.xml 
# Thu, 04 May 2023 03:09:10 GMT
RUN sed -i 's/<id>org.xwiki.platform:xwiki-platform-distribution-war/<id>org.xwiki.platform:xwiki-platform-distribution-docker/'   /usr/local/tomcat/webapps/ROOT/META-INF/extension.xed
# Thu, 04 May 2023 03:09:10 GMT
COPY file:a47c4dcd87c9dad97aff38c49188357e6193bcad50757e516cfb08a60d4de611 in /usr/local/bin/docker-entrypoint.sh 
# Thu, 04 May 2023 03:09:10 GMT
VOLUME [/usr/local/xwiki]
# Thu, 04 May 2023 03:09:11 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 04 May 2023 03:09:11 GMT
CMD ["xwiki"]
```

-	Layers:
	-	`sha256:b2ddfd337773edbf5766dce2fdbeef139ba8c42724e29eda157c84e9f97f1bce`  
		Last Modified: Wed, 08 Mar 2023 12:37:24 GMT  
		Size: 28.4 MB (28387554 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:35794a35c4aa2299e9a7a69f4eafa7f96eb1832e2a04b3d85773522111018ca6`  
		Last Modified: Thu, 16 Mar 2023 01:58:19 GMT  
		Size: 12.4 MB (12389767 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c7672a2f0cc0331254a0757eb49533b4f8d679db185c8984d43d8d82a3188dd3`  
		Last Modified: Wed, 26 Apr 2023 19:47:57 GMT  
		Size: 45.0 MB (45009454 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:74e0edba07c031c877237b33c630b18502292fbf815970b5b9859fb781cd77ae`  
		Last Modified: Wed, 26 Apr 2023 19:47:52 GMT  
		Size: 161.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b2aafa1b8069234ff15c05df12d4c35ec32460721bbd7730e99647efe3aa6585`  
		Last Modified: Wed, 26 Apr 2023 22:02:33 GMT  
		Size: 173.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:90db2dff3a4d1cbba422034d42da2b9158b74336efe840f6fce08a10d4f376b8`  
		Last Modified: Wed, 03 May 2023 10:49:24 GMT  
		Size: 12.2 MB (12239982 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e454a1434a13880a74667b25be9077114a98b423871b898590ccbbc9c09bb8f4`  
		Last Modified: Wed, 03 May 2023 10:49:24 GMT  
		Size: 2.8 MB (2808572 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:09113a88008a74c8c91980887d7135750e44ff3ec5b960195deb093009017eb7`  
		Last Modified: Wed, 03 May 2023 10:49:23 GMT  
		Size: 131.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:00e474f24e2888d9ff4084b22818396eafc20484a2a52b597730662ef222bfd9`  
		Last Modified: Thu, 04 May 2023 03:10:41 GMT  
		Size: 173.8 MB (173823166 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:56329660fcd8fda3ec594de2e46176c3655dbf45979ed9303f96bd1ec760bf20`  
		Last Modified: Thu, 04 May 2023 03:12:17 GMT  
		Size: 307.2 MB (307217563 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f673f9427ff352c9a2c5ff550cb54fbc49a890c85448828ab5a360671ac27e48`  
		Last Modified: Thu, 04 May 2023 03:12:04 GMT  
		Size: 2.3 MB (2343672 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:177c4957fb4fbd6772f27fcd5b0c859a7a3ff06d343f0ae7b581e3d541665fc2`  
		Last Modified: Thu, 04 May 2023 03:12:03 GMT  
		Size: 1.3 KB (1343 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:90d01b8844c7964c5d2abd4ed227ffc91a9b701e730a777c44b3e09d042fb479`  
		Last Modified: Thu, 04 May 2023 03:12:03 GMT  
		Size: 2.3 KB (2306 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:aeb28f8c0565745b77c1a37032e92ac1c2e96a542799c5a1486902c7c30b9576`  
		Last Modified: Thu, 04 May 2023 03:12:03 GMT  
		Size: 6.0 KB (6013 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:681e20063ebae5828ccfa36974e789fdf2ca11c563c59c7455625b026a49c135`  
		Last Modified: Thu, 04 May 2023 03:12:03 GMT  
		Size: 2.5 KB (2502 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
