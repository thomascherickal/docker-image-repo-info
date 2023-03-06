## `xwiki:14-mysql-tomcat`

```console
$ docker pull xwiki@sha256:eb7e265585ba416e46e5e8497d4bbd0bb4629869b0dd13e7bcf476ff0571a73a
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `xwiki:14-mysql-tomcat` - linux; amd64

```console
$ docker pull xwiki@sha256:48bfe1a1d06f3d17973c828eb0c8e8c53d83b3e46741ac16f0a72f84b22559f4
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **590.0 MB (590039216 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d998eb704a40a8a22c7935fce3d22c160ee29ef28426391183c72be691da2d54`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["xwiki"]`

```dockerfile
# Wed, 01 Mar 2023 04:38:47 GMT
ARG RELEASE
# Wed, 01 Mar 2023 04:38:47 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Wed, 01 Mar 2023 04:38:47 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Wed, 01 Mar 2023 04:38:47 GMT
LABEL org.opencontainers.image.version=22.04
# Wed, 01 Mar 2023 04:38:48 GMT
ADD file:fb4c8244f4468cdd3f666932f05805a3882d34010d3a0c14b7c20589bf619a9c in / 
# Wed, 01 Mar 2023 04:38:49 GMT
CMD ["/bin/bash"]
# Thu, 02 Mar 2023 04:01:37 GMT
ENV JAVA_HOME=/opt/java/openjdk
# Thu, 02 Mar 2023 04:01:37 GMT
ENV PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 02 Mar 2023 04:01:37 GMT
ENV LANG=en_US.UTF-8 LANGUAGE=en_US:en LC_ALL=en_US.UTF-8
# Thu, 02 Mar 2023 04:01:51 GMT
RUN apt-get update     && DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends tzdata curl wget ca-certificates fontconfig locales     && echo "en_US.UTF-8 UTF-8" >> /etc/locale.gen     && locale-gen en_US.UTF-8     && rm -rf /var/lib/apt/lists/*
# Thu, 02 Mar 2023 04:02:42 GMT
ENV JAVA_VERSION=jdk-11.0.18+10
# Thu, 02 Mar 2023 04:03:16 GMT
RUN set -eux;     ARCH="$(dpkg --print-architecture)";     case "${ARCH}" in        aarch64|arm64)          ESUM='89bc6e93d48a37a5eff7ec5afa515c60eb3369d106d1736f5e845b3dcf8fb72c';          BINARY_URL='https://github.com/adoptium/temurin11-binaries/releases/download/jdk-11.0.18%2B10/OpenJDK11U-jre_aarch64_linux_hotspot_11.0.18_10.tar.gz';          ;;        armhf|arm)          ESUM='949482ac232e756f342de6a8592d56b58803e10d3956abff14c4958e711a0b7c';          BINARY_URL='https://github.com/adoptium/temurin11-binaries/releases/download/jdk-11.0.18%2B10/OpenJDK11U-jre_arm_linux_hotspot_11.0.18_10.tar.gz';          ;;        ppc64el|powerpc:common64)          ESUM='df32e80d5b6db60a1ed9ed04eaf267eaf17835ed2ae2c1708d8d94328c03a0a5';          BINARY_URL='https://github.com/adoptium/temurin11-binaries/releases/download/jdk-11.0.18%2B10/OpenJDK11U-jre_ppc64le_linux_hotspot_11.0.18_10.tar.gz';          ;;        s390x|s390:64-bit)          ESUM='c07df5081f78021bed0d169622e470ebd4a4525a45f84192a52580ddb912959b';          BINARY_URL='https://github.com/adoptium/temurin11-binaries/releases/download/jdk-11.0.18%2B10/OpenJDK11U-jre_s390x_linux_hotspot_11.0.18_10.tar.gz';          ;;        amd64|i386:x86-64)          ESUM='0e7b196ef8603ac3d38caaf7768b7b0a3c613d60e15a6511bcfb2c894b609e99';          BINARY_URL='https://github.com/adoptium/temurin11-binaries/releases/download/jdk-11.0.18%2B10/OpenJDK11U-jre_x64_linux_hotspot_11.0.18_10.tar.gz';          ;;        *)          echo "Unsupported arch: ${ARCH}";          exit 1;          ;;     esac; 	  wget -O /tmp/openjdk.tar.gz ${BINARY_URL}; 	  echo "${ESUM} */tmp/openjdk.tar.gz" | sha256sum -c -; 	  mkdir -p "$JAVA_HOME"; 	  tar --extract 	      --file /tmp/openjdk.tar.gz 	      --directory "$JAVA_HOME" 	      --strip-components 1 	      --no-same-owner 	  ;     rm -f /tmp/openjdk.tar.gz ${JAVA_HOME}/src.zip;     find "$JAVA_HOME/lib" -name '*.so' -exec dirname '{}' ';' | sort -u > /etc/ld.so.conf.d/docker-openjdk.conf;     ldconfig;     java -Xshare:dump;
# Thu, 02 Mar 2023 04:03:17 GMT
RUN echo Verifying install ...     && fileEncoding="$(echo 'System.out.println(System.getProperty("file.encoding"))' | jshell -s -)"; [ "$fileEncoding" = 'UTF-8' ]; rm -rf ~/.java     && echo java --version && java --version     && echo Complete.
# Thu, 02 Mar 2023 10:46:59 GMT
ENV CATALINA_HOME=/usr/local/tomcat
# Thu, 02 Mar 2023 10:46:59 GMT
ENV PATH=/usr/local/tomcat/bin:/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 02 Mar 2023 10:47:00 GMT
RUN mkdir -p "$CATALINA_HOME"
# Thu, 02 Mar 2023 10:47:00 GMT
WORKDIR /usr/local/tomcat
# Thu, 02 Mar 2023 10:47:00 GMT
ENV TOMCAT_NATIVE_LIBDIR=/usr/local/tomcat/native-jni-lib
# Thu, 02 Mar 2023 10:47:00 GMT
ENV LD_LIBRARY_PATH=/usr/local/tomcat/native-jni-lib
# Thu, 02 Mar 2023 10:49:42 GMT
ENV GPG_KEYS=48F8E69F6390C9F25CFEDCD268248959359E722B A9C5DF4D22E99998D9875A5110C01C5A2F6059E7 DCFD35E0BF8CA7344752DE8B6FB21E8933C60243
# Thu, 02 Mar 2023 10:49:42 GMT
ENV TOMCAT_MAJOR=9
# Sat, 04 Mar 2023 02:36:40 GMT
ENV TOMCAT_VERSION=9.0.73
# Sat, 04 Mar 2023 02:36:40 GMT
ENV TOMCAT_SHA512=d43fbd6c5ae00bc0ffc2559743f91abd3547c827426cb0acdc8428e060e8659b6bb41b3877deb061ab6202980de39b9558525a4256725b647d5bff93e47a5664
# Sat, 04 Mar 2023 02:36:40 GMT
COPY dir:f26a4899909bdb16ffc918a8d63373c6ccb4656abacf4343dca21a7b842082ed in /usr/local/tomcat 
# Sat, 04 Mar 2023 02:36:44 GMT
RUN set -eux; 	apt-get update; 	xargs -rt apt-get install -y --no-install-recommends < "$TOMCAT_NATIVE_LIBDIR/.dependencies.txt"; 	rm -rf /var/lib/apt/lists/*
# Sat, 04 Mar 2023 02:36:46 GMT
RUN set -eux; 	nativeLines="$(catalina.sh configtest 2>&1)"; 	nativeLines="$(echo "$nativeLines" | grep 'Apache Tomcat Native')"; 	nativeLines="$(echo "$nativeLines" | sort -u)"; 	if ! echo "$nativeLines" | grep -E 'INFO: Loaded( APR based)? Apache Tomcat Native library' >&2; then 		echo >&2 "$nativeLines"; 		exit 1; 	fi
# Sat, 04 Mar 2023 02:36:46 GMT
EXPOSE 8080
# Sat, 04 Mar 2023 02:36:46 GMT
CMD ["catalina.sh" "run"]
# Mon, 06 Mar 2023 20:25:02 GMT
LABEL org.opencontainers.image.authors=XWiki Development Team <committers@xwiki.org>
# Mon, 06 Mar 2023 20:25:02 GMT
LABEL org.opencontainers.image.url=https://hub.docker.com/_/xwiki
# Mon, 06 Mar 2023 20:25:03 GMT
LABEL org.opencontainers.image.documentation=https://hub.docker.com/_/xwiki
# Mon, 06 Mar 2023 20:25:03 GMT
LABEL org.opencontainers.image.source=https://github.com/xwiki/xwiki-docker.git
# Mon, 06 Mar 2023 20:25:03 GMT
LABEL org.opencontainers.image.vendor=xwiki.org
# Mon, 06 Mar 2023 20:25:03 GMT
LABEL org.opencontainers.image.licenses=LGPL-2.1
# Mon, 06 Mar 2023 20:26:51 GMT
RUN apt-get update &&   apt-get --no-install-recommends -y install     curl     libreoffice     unzip     procps &&   rm -rf /var/lib/apt/lists/*
# Mon, 06 Mar 2023 20:29:10 GMT
ENV XWIKI_VERSION=14.10.6
# Mon, 06 Mar 2023 20:29:10 GMT
ENV XWIKI_URL_PREFIX=https://maven.xwiki.org/releases/org/xwiki/platform/xwiki-platform-distribution-war/14.10.6
# Mon, 06 Mar 2023 20:29:10 GMT
ENV XWIKI_DOWNLOAD_SHA256=258285234a7c41f9ddc1434457e10640b7c5a7ed2c2f1782c8320a8ebc04c9a4
# Mon, 06 Mar 2023 20:29:50 GMT
RUN rm -rf /usr/local/tomcat/webapps/* &&   mkdir -p /usr/local/tomcat/temp &&   mkdir -p /usr/local/xwiki/data &&   curl -fSL "${XWIKI_URL_PREFIX}/xwiki-platform-distribution-war-${XWIKI_VERSION}.war" -o xwiki.war &&   echo "$XWIKI_DOWNLOAD_SHA256 xwiki.war" | sha256sum -c - &&   unzip -d /usr/local/tomcat/webapps/ROOT xwiki.war &&   rm -f xwiki.war
# Mon, 06 Mar 2023 20:29:51 GMT
ENV MYSQL_JDBC_VERSION=8.0.32
# Mon, 06 Mar 2023 20:29:51 GMT
ENV MYSQL_JDBC_SHA256=522329fe925980f02e5eb89b59d227245d345415ff0c08932a68c9765c13acc5
# Mon, 06 Mar 2023 20:29:51 GMT
ENV MYSQL_JDBC_PREFIX=https://repo1.maven.org/maven2/com/mysql/mysql-connector-j/8.0.32
# Mon, 06 Mar 2023 20:29:51 GMT
ENV MYSQL_JDBC_ARTIFACT=mysql-connector-j-8.0.32.jar
# Mon, 06 Mar 2023 20:29:51 GMT
ENV MYSQL_JDBC_TARGET=/usr/local/tomcat/webapps/ROOT/WEB-INF/lib/mysql-connector-j-8.0.32.jar
# Mon, 06 Mar 2023 20:29:52 GMT
RUN curl -fSL "${MYSQL_JDBC_PREFIX}/${MYSQL_JDBC_ARTIFACT}" -o $MYSQL_JDBC_TARGET &&   echo "$MYSQL_JDBC_SHA256 $MYSQL_JDBC_TARGET" | sha256sum -c -
# Mon, 06 Mar 2023 20:29:52 GMT
COPY file:0a1be11e2eb610a1dbcd415404e3a592641110b93090030cb831e3a19a163017 in /usr/local/tomcat/bin/ 
# Mon, 06 Mar 2023 20:29:52 GMT
COPY file:1b8409986f3e4eb79a7a0b18472cb2692a61d504fb5ef34292bc997b79fd760d in /usr/local/tomcat/webapps/ROOT/WEB-INF/hibernate.cfg.xml 
# Mon, 06 Mar 2023 20:29:53 GMT
RUN sed -i 's/<id>org.xwiki.platform:xwiki-platform-distribution-war/<id>org.xwiki.platform:xwiki-platform-distribution-docker/'   /usr/local/tomcat/webapps/ROOT/META-INF/extension.xed
# Mon, 06 Mar 2023 20:29:53 GMT
COPY file:a47c4dcd87c9dad97aff38c49188357e6193bcad50757e516cfb08a60d4de611 in /usr/local/bin/docker-entrypoint.sh 
# Mon, 06 Mar 2023 20:29:53 GMT
VOLUME [/usr/local/xwiki]
# Mon, 06 Mar 2023 20:29:53 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Mon, 06 Mar 2023 20:29:53 GMT
CMD ["xwiki"]
```

-	Layers:
	-	`sha256:b65bcf19d1445822c0d6f15ea82c9ed82ac1d903cfd6c1284ba7b2409a092845`  
		Last Modified: Wed, 01 Mar 2023 09:07:16 GMT  
		Size: 30.4 MB (30430002 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9e3e3d5d30a242b64d6ee4089176f1459cdfe9d3aeb58e2114cc14b420ad71e5`  
		Last Modified: Thu, 02 Mar 2023 04:07:58 GMT  
		Size: 12.4 MB (12432173 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b1afd9b3f07bf59f1db11ac95908fa4840bb36ea5ca2e38380ceb99feadec711`  
		Last Modified: Thu, 02 Mar 2023 04:10:00 GMT  
		Size: 46.6 MB (46635570 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:24c021f0294c1a9786718db8f4082e50bb41ec03fdc866e6fdb1e624b899367f`  
		Last Modified: Thu, 02 Mar 2023 04:09:54 GMT  
		Size: 158.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:56c0466cd5772f2dc1cc3012e581ad983c38a42dc0b4150a2aaf64f22cc586ce`  
		Last Modified: Thu, 02 Mar 2023 11:03:42 GMT  
		Size: 172.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f2dc1f97d115f4570e3422053df92e9f6d69adefcd79ee9d5eea99c728704030`  
		Last Modified: Sat, 04 Mar 2023 02:47:18 GMT  
		Size: 12.2 MB (12218296 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:aa8c8a0dbaef03ab5e577c7a23921c2e9c223be0de8cd3b020cec865ced7fb2e`  
		Last Modified: Sat, 04 Mar 2023 02:47:17 GMT  
		Size: 454.2 KB (454175 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ccfb026ee7e4a995c0444ea227403bed07bdde623ab5aefdd13a6aa85baa81e5`  
		Last Modified: Sat, 04 Mar 2023 02:47:17 GMT  
		Size: 130.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:155e6901c9e0207a240df31ffb93a32b09408a99307d6b4a9f426f8c5cdce879`  
		Last Modified: Mon, 06 Mar 2023 20:32:08 GMT  
		Size: 178.3 MB (178327447 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:823f4c98af118641aefa1657fd3c2f2ed00de0a776d65f63de066c105e749599`  
		Last Modified: Mon, 06 Mar 2023 20:34:14 GMT  
		Size: 307.2 MB (307186348 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1ea19d5071cc58bef2531f5d535474fdef007bca2c8c47f4f1a5b6c1198cedb1`  
		Last Modified: Mon, 06 Mar 2023 20:33:57 GMT  
		Size: 2.3 MB (2342572 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b6ecd53b84e4ff9eee4756ff9027a6c2ab7d0dc91eed3a75ee5ba4502d21655a`  
		Last Modified: Mon, 06 Mar 2023 20:33:57 GMT  
		Size: 1.3 KB (1343 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:efa72a0541a155b954d477e1afc5229ee1638be8005a6c7e0829dd7a3299fd2f`  
		Last Modified: Mon, 06 Mar 2023 20:33:57 GMT  
		Size: 2.3 KB (2309 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a22a6537805b9da8869dc9539ad377aa9f63cbedcf316fd54dcef99aaa565cf2`  
		Last Modified: Mon, 06 Mar 2023 20:33:57 GMT  
		Size: 6.0 KB (6015 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4c74e5fffe17e684d80baf710e6f802aac1dcfc6a3312ab1c4f0a9678a9dd81e`  
		Last Modified: Mon, 06 Mar 2023 20:33:57 GMT  
		Size: 2.5 KB (2506 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `xwiki:14-mysql-tomcat` - linux; arm64 variant v8

```console
$ docker pull xwiki@sha256:02e25854ef7f909f7e0b08ba36399fc2171184372f440e9397ba4326ca921ac7
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **581.3 MB (581325130 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:78f5a91ede1dc6da715e5e7e0ceb3c9ee94e9ab3dddec658a74509bf5069b759`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["xwiki"]`

```dockerfile
# Wed, 01 Mar 2023 04:47:53 GMT
ARG RELEASE
# Wed, 01 Mar 2023 04:47:53 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Wed, 01 Mar 2023 04:47:54 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Wed, 01 Mar 2023 04:47:54 GMT
LABEL org.opencontainers.image.version=22.04
# Wed, 01 Mar 2023 04:48:01 GMT
ADD file:cf91de9ab30abab112d58c0a7f3bbb35853a02b2e406c65c89430ff049573c47 in / 
# Wed, 01 Mar 2023 04:48:01 GMT
CMD ["/bin/bash"]
# Thu, 02 Mar 2023 04:27:42 GMT
ENV JAVA_HOME=/opt/java/openjdk
# Thu, 02 Mar 2023 04:27:42 GMT
ENV PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 02 Mar 2023 04:27:42 GMT
ENV LANG=en_US.UTF-8 LANGUAGE=en_US:en LC_ALL=en_US.UTF-8
# Thu, 02 Mar 2023 04:27:55 GMT
RUN apt-get update     && DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends tzdata curl wget ca-certificates fontconfig locales     && echo "en_US.UTF-8 UTF-8" >> /etc/locale.gen     && locale-gen en_US.UTF-8     && rm -rf /var/lib/apt/lists/*
# Thu, 02 Mar 2023 04:28:47 GMT
ENV JAVA_VERSION=jdk-11.0.18+10
# Thu, 02 Mar 2023 04:29:16 GMT
RUN set -eux;     ARCH="$(dpkg --print-architecture)";     case "${ARCH}" in        aarch64|arm64)          ESUM='89bc6e93d48a37a5eff7ec5afa515c60eb3369d106d1736f5e845b3dcf8fb72c';          BINARY_URL='https://github.com/adoptium/temurin11-binaries/releases/download/jdk-11.0.18%2B10/OpenJDK11U-jre_aarch64_linux_hotspot_11.0.18_10.tar.gz';          ;;        armhf|arm)          ESUM='949482ac232e756f342de6a8592d56b58803e10d3956abff14c4958e711a0b7c';          BINARY_URL='https://github.com/adoptium/temurin11-binaries/releases/download/jdk-11.0.18%2B10/OpenJDK11U-jre_arm_linux_hotspot_11.0.18_10.tar.gz';          ;;        ppc64el|powerpc:common64)          ESUM='df32e80d5b6db60a1ed9ed04eaf267eaf17835ed2ae2c1708d8d94328c03a0a5';          BINARY_URL='https://github.com/adoptium/temurin11-binaries/releases/download/jdk-11.0.18%2B10/OpenJDK11U-jre_ppc64le_linux_hotspot_11.0.18_10.tar.gz';          ;;        s390x|s390:64-bit)          ESUM='c07df5081f78021bed0d169622e470ebd4a4525a45f84192a52580ddb912959b';          BINARY_URL='https://github.com/adoptium/temurin11-binaries/releases/download/jdk-11.0.18%2B10/OpenJDK11U-jre_s390x_linux_hotspot_11.0.18_10.tar.gz';          ;;        amd64|i386:x86-64)          ESUM='0e7b196ef8603ac3d38caaf7768b7b0a3c613d60e15a6511bcfb2c894b609e99';          BINARY_URL='https://github.com/adoptium/temurin11-binaries/releases/download/jdk-11.0.18%2B10/OpenJDK11U-jre_x64_linux_hotspot_11.0.18_10.tar.gz';          ;;        *)          echo "Unsupported arch: ${ARCH}";          exit 1;          ;;     esac; 	  wget -O /tmp/openjdk.tar.gz ${BINARY_URL}; 	  echo "${ESUM} */tmp/openjdk.tar.gz" | sha256sum -c -; 	  mkdir -p "$JAVA_HOME"; 	  tar --extract 	      --file /tmp/openjdk.tar.gz 	      --directory "$JAVA_HOME" 	      --strip-components 1 	      --no-same-owner 	  ;     rm -f /tmp/openjdk.tar.gz ${JAVA_HOME}/src.zip;     find "$JAVA_HOME/lib" -name '*.so' -exec dirname '{}' ';' | sort -u > /etc/ld.so.conf.d/docker-openjdk.conf;     ldconfig;     java -Xshare:dump;
# Thu, 02 Mar 2023 04:29:17 GMT
RUN echo Verifying install ...     && fileEncoding="$(echo 'System.out.println(System.getProperty("file.encoding"))' | jshell -s -)"; [ "$fileEncoding" = 'UTF-8' ]; rm -rf ~/.java     && echo java --version && java --version     && echo Complete.
# Thu, 02 Mar 2023 07:44:26 GMT
ENV CATALINA_HOME=/usr/local/tomcat
# Thu, 02 Mar 2023 07:44:26 GMT
ENV PATH=/usr/local/tomcat/bin:/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 02 Mar 2023 07:44:27 GMT
RUN mkdir -p "$CATALINA_HOME"
# Thu, 02 Mar 2023 07:44:27 GMT
WORKDIR /usr/local/tomcat
# Thu, 02 Mar 2023 07:44:27 GMT
ENV TOMCAT_NATIVE_LIBDIR=/usr/local/tomcat/native-jni-lib
# Thu, 02 Mar 2023 07:44:27 GMT
ENV LD_LIBRARY_PATH=/usr/local/tomcat/native-jni-lib
# Thu, 02 Mar 2023 07:46:39 GMT
ENV GPG_KEYS=48F8E69F6390C9F25CFEDCD268248959359E722B A9C5DF4D22E99998D9875A5110C01C5A2F6059E7 DCFD35E0BF8CA7344752DE8B6FB21E8933C60243
# Thu, 02 Mar 2023 07:46:39 GMT
ENV TOMCAT_MAJOR=9
# Sat, 04 Mar 2023 02:25:13 GMT
ENV TOMCAT_VERSION=9.0.73
# Sat, 04 Mar 2023 02:25:13 GMT
ENV TOMCAT_SHA512=d43fbd6c5ae00bc0ffc2559743f91abd3547c827426cb0acdc8428e060e8659b6bb41b3877deb061ab6202980de39b9558525a4256725b647d5bff93e47a5664
# Sat, 04 Mar 2023 02:25:14 GMT
COPY dir:1165545ec5e5b08c9a9d8966c16fe23890ef899a1009c6349b5d66e988d7c045 in /usr/local/tomcat 
# Sat, 04 Mar 2023 02:25:17 GMT
RUN set -eux; 	apt-get update; 	xargs -rt apt-get install -y --no-install-recommends < "$TOMCAT_NATIVE_LIBDIR/.dependencies.txt"; 	rm -rf /var/lib/apt/lists/*
# Sat, 04 Mar 2023 02:25:18 GMT
RUN set -eux; 	nativeLines="$(catalina.sh configtest 2>&1)"; 	nativeLines="$(echo "$nativeLines" | grep 'Apache Tomcat Native')"; 	nativeLines="$(echo "$nativeLines" | sort -u)"; 	if ! echo "$nativeLines" | grep -E 'INFO: Loaded( APR based)? Apache Tomcat Native library' >&2; then 		echo >&2 "$nativeLines"; 		exit 1; 	fi
# Sat, 04 Mar 2023 02:25:19 GMT
EXPOSE 8080
# Sat, 04 Mar 2023 02:25:19 GMT
CMD ["catalina.sh" "run"]
# Mon, 06 Mar 2023 20:52:57 GMT
LABEL org.opencontainers.image.authors=XWiki Development Team <committers@xwiki.org>
# Mon, 06 Mar 2023 20:52:57 GMT
LABEL org.opencontainers.image.url=https://hub.docker.com/_/xwiki
# Mon, 06 Mar 2023 20:52:57 GMT
LABEL org.opencontainers.image.documentation=https://hub.docker.com/_/xwiki
# Mon, 06 Mar 2023 20:52:58 GMT
LABEL org.opencontainers.image.source=https://github.com/xwiki/xwiki-docker.git
# Mon, 06 Mar 2023 20:52:58 GMT
LABEL org.opencontainers.image.vendor=xwiki.org
# Mon, 06 Mar 2023 20:52:58 GMT
LABEL org.opencontainers.image.licenses=LGPL-2.1
# Mon, 06 Mar 2023 20:55:07 GMT
RUN apt-get update &&   apt-get --no-install-recommends -y install     curl     libreoffice     unzip     procps &&   rm -rf /var/lib/apt/lists/*
# Mon, 06 Mar 2023 20:57:33 GMT
ENV XWIKI_VERSION=14.10.6
# Mon, 06 Mar 2023 20:57:33 GMT
ENV XWIKI_URL_PREFIX=https://maven.xwiki.org/releases/org/xwiki/platform/xwiki-platform-distribution-war/14.10.6
# Mon, 06 Mar 2023 20:57:33 GMT
ENV XWIKI_DOWNLOAD_SHA256=258285234a7c41f9ddc1434457e10640b7c5a7ed2c2f1782c8320a8ebc04c9a4
# Mon, 06 Mar 2023 20:58:13 GMT
RUN rm -rf /usr/local/tomcat/webapps/* &&   mkdir -p /usr/local/tomcat/temp &&   mkdir -p /usr/local/xwiki/data &&   curl -fSL "${XWIKI_URL_PREFIX}/xwiki-platform-distribution-war-${XWIKI_VERSION}.war" -o xwiki.war &&   echo "$XWIKI_DOWNLOAD_SHA256 xwiki.war" | sha256sum -c - &&   unzip -d /usr/local/tomcat/webapps/ROOT xwiki.war &&   rm -f xwiki.war
# Mon, 06 Mar 2023 20:58:15 GMT
ENV MYSQL_JDBC_VERSION=8.0.32
# Mon, 06 Mar 2023 20:58:15 GMT
ENV MYSQL_JDBC_SHA256=522329fe925980f02e5eb89b59d227245d345415ff0c08932a68c9765c13acc5
# Mon, 06 Mar 2023 20:58:16 GMT
ENV MYSQL_JDBC_PREFIX=https://repo1.maven.org/maven2/com/mysql/mysql-connector-j/8.0.32
# Mon, 06 Mar 2023 20:58:16 GMT
ENV MYSQL_JDBC_ARTIFACT=mysql-connector-j-8.0.32.jar
# Mon, 06 Mar 2023 20:58:16 GMT
ENV MYSQL_JDBC_TARGET=/usr/local/tomcat/webapps/ROOT/WEB-INF/lib/mysql-connector-j-8.0.32.jar
# Mon, 06 Mar 2023 20:58:17 GMT
RUN curl -fSL "${MYSQL_JDBC_PREFIX}/${MYSQL_JDBC_ARTIFACT}" -o $MYSQL_JDBC_TARGET &&   echo "$MYSQL_JDBC_SHA256 $MYSQL_JDBC_TARGET" | sha256sum -c -
# Mon, 06 Mar 2023 20:58:17 GMT
COPY file:0a1be11e2eb610a1dbcd415404e3a592641110b93090030cb831e3a19a163017 in /usr/local/tomcat/bin/ 
# Mon, 06 Mar 2023 20:58:17 GMT
COPY file:1b8409986f3e4eb79a7a0b18472cb2692a61d504fb5ef34292bc997b79fd760d in /usr/local/tomcat/webapps/ROOT/WEB-INF/hibernate.cfg.xml 
# Mon, 06 Mar 2023 20:58:17 GMT
RUN sed -i 's/<id>org.xwiki.platform:xwiki-platform-distribution-war/<id>org.xwiki.platform:xwiki-platform-distribution-docker/'   /usr/local/tomcat/webapps/ROOT/META-INF/extension.xed
# Mon, 06 Mar 2023 20:58:17 GMT
COPY file:a47c4dcd87c9dad97aff38c49188357e6193bcad50757e516cfb08a60d4de611 in /usr/local/bin/docker-entrypoint.sh 
# Mon, 06 Mar 2023 20:58:17 GMT
VOLUME [/usr/local/xwiki]
# Mon, 06 Mar 2023 20:58:17 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Mon, 06 Mar 2023 20:58:17 GMT
CMD ["xwiki"]
```

-	Layers:
	-	`sha256:986c4f6be3072d9528a459c780295bd053806536d2295a6de6aad327eaf19fad`  
		Last Modified: Wed, 01 Mar 2023 09:02:52 GMT  
		Size: 28.4 MB (28387922 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:219ba20309dcd99cff3a43c2f3c01df9170ee1fe02df71ead98cfcef30b9c450`  
		Last Modified: Thu, 02 Mar 2023 04:33:24 GMT  
		Size: 12.4 MB (12390219 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:82d5722bd69e931b1cf3e955e992893a8ea2e124b586c19b553fbe8a2d94f988`  
		Last Modified: Thu, 02 Mar 2023 04:35:11 GMT  
		Size: 45.0 MB (44977970 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9a2d1016d6ffd5bed4cc6724687b1659787f8e3d1c112f02173b5efcb5425180`  
		Last Modified: Thu, 02 Mar 2023 04:35:06 GMT  
		Size: 159.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e56f31cf77054a813fd2027944ece84d43497ed9c07608a3226933ae3158c327`  
		Last Modified: Thu, 02 Mar 2023 07:59:18 GMT  
		Size: 171.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ce6bc7fda76a5c0ff2cdea89cbedf391e508bb545773fe84f8a14c62fff7593f`  
		Last Modified: Sat, 04 Mar 2023 02:35:15 GMT  
		Size: 12.2 MB (12225283 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0d65e68fd56125d52872fa82de169a3d0fcc6a86422da6b53cfff161d021c443`  
		Last Modified: Sat, 04 Mar 2023 02:35:13 GMT  
		Size: 453.7 KB (453702 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5f0e981a1141d04e05adeaaea4db0da160634a45e6948448d57ed0d4be56376d`  
		Last Modified: Sat, 04 Mar 2023 02:35:13 GMT  
		Size: 130.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:425b19227a1d89be6360979159fd2779eda10bc49ebf77323dbbddd0cb5fa247`  
		Last Modified: Mon, 06 Mar 2023 21:00:13 GMT  
		Size: 173.3 MB (173348489 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:33ce3c6242ab6bc5457caca9dc30a524d84813d7b13ae9210767da857dcc0907`  
		Last Modified: Mon, 06 Mar 2023 21:01:58 GMT  
		Size: 307.2 MB (307186335 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4ce4845dc50cfef88144c2dd1759a31967795305c2306b39f08ecb6875e7bd33`  
		Last Modified: Mon, 06 Mar 2023 21:01:44 GMT  
		Size: 2.3 MB (2342571 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1b26bd595929ceb82823f0dcb8e065fa3eb1329ddd785fda76bd070fafeb9e18`  
		Last Modified: Mon, 06 Mar 2023 21:01:43 GMT  
		Size: 1.3 KB (1345 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6c6211995a3cabf764e978b1007f3ea024e507938223dacdec39be597bf5981a`  
		Last Modified: Mon, 06 Mar 2023 21:01:43 GMT  
		Size: 2.3 KB (2311 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:839d18258510074d5e2fcf7c7ac8fa76df8f66dfd403148e3c5dafa77411a5c4`  
		Last Modified: Mon, 06 Mar 2023 21:01:43 GMT  
		Size: 6.0 KB (6017 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fd04ddf9970bdb7d4318a080fe952f532e94d44a02720420bbefd92ffe593a5a`  
		Last Modified: Mon, 06 Mar 2023 21:01:43 GMT  
		Size: 2.5 KB (2506 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
