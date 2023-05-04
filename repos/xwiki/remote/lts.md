## `xwiki:lts`

```console
$ docker pull xwiki@sha256:43327a2a71b966facd67461e795b531bf2d0651e544b0613154dc144bfee952f
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `xwiki:lts` - linux; amd64

```console
$ docker pull xwiki@sha256:d568f0c928a9e17fb27dbfd0fef106d855829244ae9cd16b2f14751012825f19
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **590.2 MB (590196167 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:13a6a5087283ef3ced9c4afe544a93642b5cefcb4a1e54315705769ce70ce081`
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
# Thu, 04 May 2023 16:14:45 GMT
ENV TOMCAT_VERSION=9.0.74
# Thu, 04 May 2023 16:14:45 GMT
ENV TOMCAT_SHA512=0e173fc2a76404c41c571c50a1956a2b867870d767200bd30f48d89bf04a4b6337f12e6577415da932cd2dfef9b4e9e9fdd52bd873afb06c6258b0e64244a44e
# Thu, 04 May 2023 16:14:45 GMT
COPY dir:b0e4a4d8b42864897ce7424e425a74770eb105a9679711ef5243f1a8a8b245e9 in /usr/local/tomcat 
# Thu, 04 May 2023 16:14:49 GMT
RUN set -eux; 	apt-get update; 	xargs -rt apt-get install -y --no-install-recommends < "$TOMCAT_NATIVE_LIBDIR/.dependencies.txt"; 	rm -rf /var/lib/apt/lists/*
# Thu, 04 May 2023 16:14:51 GMT
RUN set -eux; 	nativeLines="$(catalina.sh configtest 2>&1)"; 	nativeLines="$(echo "$nativeLines" | grep 'Apache Tomcat Native')"; 	nativeLines="$(echo "$nativeLines" | sort -u)"; 	if ! echo "$nativeLines" | grep -E 'INFO: Loaded( APR based)? Apache Tomcat Native library' >&2; then 		echo >&2 "$nativeLines"; 		exit 1; 	fi
# Thu, 04 May 2023 16:14:51 GMT
EXPOSE 8080
# Thu, 04 May 2023 16:14:51 GMT
CMD ["catalina.sh" "run"]
# Thu, 04 May 2023 18:01:21 GMT
LABEL org.opencontainers.image.authors=XWiki Development Team <committers@xwiki.org>
# Thu, 04 May 2023 18:01:21 GMT
LABEL org.opencontainers.image.url=https://hub.docker.com/_/xwiki
# Thu, 04 May 2023 18:01:21 GMT
LABEL org.opencontainers.image.documentation=https://hub.docker.com/_/xwiki
# Thu, 04 May 2023 18:01:21 GMT
LABEL org.opencontainers.image.source=https://github.com/xwiki/xwiki-docker.git
# Thu, 04 May 2023 18:01:21 GMT
LABEL org.opencontainers.image.vendor=xwiki.org
# Thu, 04 May 2023 18:01:21 GMT
LABEL org.opencontainers.image.licenses=LGPL-2.1
# Thu, 04 May 2023 18:03:00 GMT
RUN apt-get update &&   apt-get --no-install-recommends -y install     curl     libreoffice     unzip     procps &&   rm -rf /var/lib/apt/lists/*
# Thu, 04 May 2023 18:05:26 GMT
ENV XWIKI_VERSION=14.10.9
# Thu, 04 May 2023 18:05:26 GMT
ENV XWIKI_URL_PREFIX=https://maven.xwiki.org/releases/org/xwiki/platform/xwiki-platform-distribution-war/14.10.9
# Thu, 04 May 2023 18:05:26 GMT
ENV XWIKI_DOWNLOAD_SHA256=81594962a2101d54866bccf768ea5b1637f836c57c5b212e221d043e96f5f35d
# Thu, 04 May 2023 18:06:05 GMT
RUN rm -rf /usr/local/tomcat/webapps/* &&   mkdir -p /usr/local/tomcat/temp &&   mkdir -p /usr/local/xwiki/data &&   curl -fSL "${XWIKI_URL_PREFIX}/xwiki-platform-distribution-war-${XWIKI_VERSION}.war" -o xwiki.war &&   echo "$XWIKI_DOWNLOAD_SHA256 xwiki.war" | sha256sum -c - &&   unzip -d /usr/local/tomcat/webapps/ROOT xwiki.war &&   rm -f xwiki.war
# Thu, 04 May 2023 18:06:06 GMT
ENV MYSQL_JDBC_VERSION=8.0.33
# Thu, 04 May 2023 18:06:06 GMT
ENV MYSQL_JDBC_SHA256=e2a3b2fc726a1ac64e998585db86b30fa8bf3f706195b78bb77c5f99bf877bd9
# Thu, 04 May 2023 18:06:06 GMT
ENV MYSQL_JDBC_PREFIX=https://repo1.maven.org/maven2/com/mysql/mysql-connector-j/8.0.33
# Thu, 04 May 2023 18:06:06 GMT
ENV MYSQL_JDBC_ARTIFACT=mysql-connector-j-8.0.33.jar
# Thu, 04 May 2023 18:06:06 GMT
ENV MYSQL_JDBC_TARGET=/usr/local/tomcat/webapps/ROOT/WEB-INF/lib/mysql-connector-j-8.0.33.jar
# Thu, 04 May 2023 18:06:07 GMT
RUN curl -fSL "${MYSQL_JDBC_PREFIX}/${MYSQL_JDBC_ARTIFACT}" -o $MYSQL_JDBC_TARGET &&   echo "$MYSQL_JDBC_SHA256 $MYSQL_JDBC_TARGET" | sha256sum -c -
# Thu, 04 May 2023 18:06:07 GMT
COPY file:0a1be11e2eb610a1dbcd415404e3a592641110b93090030cb831e3a19a163017 in /usr/local/tomcat/bin/ 
# Thu, 04 May 2023 18:06:07 GMT
COPY file:1b8409986f3e4eb79a7a0b18472cb2692a61d504fb5ef34292bc997b79fd760d in /usr/local/tomcat/webapps/ROOT/WEB-INF/hibernate.cfg.xml 
# Thu, 04 May 2023 18:06:08 GMT
RUN sed -i 's/<id>org.xwiki.platform:xwiki-platform-distribution-war/<id>org.xwiki.platform:xwiki-platform-distribution-docker/'   /usr/local/tomcat/webapps/ROOT/META-INF/extension.xed
# Thu, 04 May 2023 18:06:08 GMT
COPY file:a47c4dcd87c9dad97aff38c49188357e6193bcad50757e516cfb08a60d4de611 in /usr/local/bin/docker-entrypoint.sh 
# Thu, 04 May 2023 18:06:08 GMT
VOLUME [/usr/local/xwiki]
# Thu, 04 May 2023 18:06:08 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 04 May 2023 18:06:08 GMT
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
	-	`sha256:4264e4760d2a7debfc08f73bf1efebaa02ead837d4f39a9a6e09f08298158c19`  
		Last Modified: Thu, 04 May 2023 16:26:06 GMT  
		Size: 12.2 MB (12233789 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1971dc9b322ead3793a56ed9ac9bde4024d47c5bf0c22263953dc3d45617684b`  
		Last Modified: Thu, 04 May 2023 16:26:05 GMT  
		Size: 454.2 KB (454201 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:643a5190b82ab103827b7ed38f38160f9dcefb22a1f374adb8d04e8a5f41cf18`  
		Last Modified: Thu, 04 May 2023 16:26:05 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0ee69ef579f708bbbe04b7e04178fbbea7fa140c5371ca432fa39f3184457dec`  
		Last Modified: Thu, 04 May 2023 18:07:49 GMT  
		Size: 178.3 MB (178333690 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8b8f6f9bc3b20c6c5177c1e43a8f18e097cc18baeebc77294ec1c4ec02391e2e`  
		Last Modified: Thu, 04 May 2023 18:09:50 GMT  
		Size: 307.2 MB (307217527 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f7e5d570cb6a30b974e4f441047fef66656f166b0ab5e582207372aa1abf917c`  
		Last Modified: Thu, 04 May 2023 18:09:35 GMT  
		Size: 2.3 MB (2343673 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fe4101351414805a6d9f6017b13a05947f363db759164dc594aafeba50e83126`  
		Last Modified: Thu, 04 May 2023 18:09:34 GMT  
		Size: 1.3 KB (1345 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a05edd15d2e5fb558d103dc1d2d13201cace4eb19e082157ae73c5ea5e00c13e`  
		Last Modified: Thu, 04 May 2023 18:09:34 GMT  
		Size: 2.3 KB (2305 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:412d06504ad24e71169dbebd32f59486e6d78d4cad7cbf7e932a8b8619bb71e9`  
		Last Modified: Thu, 04 May 2023 18:09:34 GMT  
		Size: 6.0 KB (6011 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f380e2b96d338be70b2bd97eeb09fe0c0307222781d4f7a3c7c049fc38ab453c`  
		Last Modified: Thu, 04 May 2023 18:09:34 GMT  
		Size: 2.5 KB (2505 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `xwiki:lts` - linux; arm64 variant v8

```console
$ docker pull xwiki@sha256:4c939f6d5a4b1df8985be3e9a6fa00f0f6dfe10d41bd2a45dac9bedae30fbe49
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **581.5 MB (581480414 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:340b76283cf5979380a9b8b18338ee822a3d97b8850fb38f38ccecb6d55c30cb`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["xwiki"]`

```dockerfile
# Tue, 25 Apr 2023 17:31:58 GMT
ARG RELEASE
# Tue, 25 Apr 2023 17:31:58 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Tue, 25 Apr 2023 17:31:58 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Tue, 25 Apr 2023 17:31:59 GMT
LABEL org.opencontainers.image.version=22.04
# Tue, 25 Apr 2023 17:32:02 GMT
ADD file:aee0d7770ef2f24dc9697e86d391529d001a4013b6e30a3ac90a57932814a57e in / 
# Tue, 25 Apr 2023 17:32:02 GMT
CMD ["/bin/bash"]
# Thu, 04 May 2023 03:25:09 GMT
ENV JAVA_HOME=/opt/java/openjdk
# Thu, 04 May 2023 03:25:09 GMT
ENV PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 04 May 2023 03:25:09 GMT
ENV LANG=en_US.UTF-8 LANGUAGE=en_US:en LC_ALL=en_US.UTF-8
# Thu, 04 May 2023 03:25:23 GMT
RUN apt-get update     && DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends tzdata curl wget ca-certificates fontconfig locales     && echo "en_US.UTF-8 UTF-8" >> /etc/locale.gen     && locale-gen en_US.UTF-8     && rm -rf /var/lib/apt/lists/*
# Thu, 04 May 2023 03:25:47 GMT
ENV JAVA_VERSION=jdk-11.0.19+7
# Thu, 04 May 2023 03:26:09 GMT
RUN set -eux;     ARCH="$(dpkg --print-architecture)";     case "${ARCH}" in        aarch64|arm64)          ESUM='1fe4b20d808f393422610818711c728331992a4455eeeb061d3d05b45412771d';          BINARY_URL='https://github.com/adoptium/temurin11-binaries/releases/download/jdk-11.0.19%2B7/OpenJDK11U-jre_aarch64_linux_hotspot_11.0.19_7.tar.gz';          ;;        armhf|arm)          ESUM='cb754b055177381f9f6852b7e5469904a15edddd7f8e136043c28b1e33aee47c';          BINARY_URL='https://github.com/adoptium/temurin11-binaries/releases/download/jdk-11.0.19%2B7/OpenJDK11U-jre_arm_linux_hotspot_11.0.19_7.tar.gz';          ;;        ppc64el|powerpc:common64)          ESUM='8019d938e5525938ec8e68e2989c4413263b0d9b7b3f20fe0c45f6d967919cfb';          BINARY_URL='https://github.com/adoptium/temurin11-binaries/releases/download/jdk-11.0.19%2B7/OpenJDK11U-jre_ppc64le_linux_hotspot_11.0.19_7.tar.gz';          ;;        s390x|s390:64-bit)          ESUM='058419435fe6212d1bc305a14f578c314f9ff9a2d96d523c178120e84231c733';          BINARY_URL='https://github.com/adoptium/temurin11-binaries/releases/download/jdk-11.0.19%2B7/OpenJDK11U-jre_s390x_linux_hotspot_11.0.19_7.tar.gz';          ;;        amd64|i386:x86-64)          ESUM='32dcf760664f93531594b72ce9226e9216567de5705a23c9ff5a77c797948054';          BINARY_URL='https://github.com/adoptium/temurin11-binaries/releases/download/jdk-11.0.19%2B7/OpenJDK11U-jre_x64_linux_hotspot_11.0.19_7.tar.gz';          ;;        *)          echo "Unsupported arch: ${ARCH}";          exit 1;          ;;     esac; 	  wget -O /tmp/openjdk.tar.gz ${BINARY_URL}; 	  echo "${ESUM} */tmp/openjdk.tar.gz" | sha256sum -c -; 	  mkdir -p "$JAVA_HOME"; 	  tar --extract 	      --file /tmp/openjdk.tar.gz 	      --directory "$JAVA_HOME" 	      --strip-components 1 	      --no-same-owner 	  ;     rm -f /tmp/openjdk.tar.gz ${JAVA_HOME}/src.zip;     find "$JAVA_HOME/lib" -name '*.so' -exec dirname '{}' ';' | sort -u > /etc/ld.so.conf.d/docker-openjdk.conf;     ldconfig;     java -Xshare:dump;
# Thu, 04 May 2023 03:26:10 GMT
RUN echo Verifying install ...     && fileEncoding="$(echo 'System.out.println(System.getProperty("file.encoding"))' | jshell -s -)"; [ "$fileEncoding" = 'UTF-8' ]; rm -rf ~/.java     && echo java --version && java --version     && echo Complete.
# Thu, 04 May 2023 11:14:20 GMT
ENV CATALINA_HOME=/usr/local/tomcat
# Thu, 04 May 2023 11:14:20 GMT
ENV PATH=/usr/local/tomcat/bin:/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 04 May 2023 11:14:21 GMT
RUN mkdir -p "$CATALINA_HOME"
# Thu, 04 May 2023 11:14:21 GMT
WORKDIR /usr/local/tomcat
# Thu, 04 May 2023 11:14:21 GMT
ENV TOMCAT_NATIVE_LIBDIR=/usr/local/tomcat/native-jni-lib
# Thu, 04 May 2023 11:14:21 GMT
ENV LD_LIBRARY_PATH=/usr/local/tomcat/native-jni-lib
# Thu, 04 May 2023 11:15:34 GMT
ENV GPG_KEYS=48F8E69F6390C9F25CFEDCD268248959359E722B A9C5DF4D22E99998D9875A5110C01C5A2F6059E7 DCFD35E0BF8CA7344752DE8B6FB21E8933C60243
# Thu, 04 May 2023 11:15:34 GMT
ENV TOMCAT_MAJOR=9
# Thu, 04 May 2023 11:15:34 GMT
ENV TOMCAT_VERSION=9.0.74
# Thu, 04 May 2023 11:15:34 GMT
ENV TOMCAT_SHA512=0e173fc2a76404c41c571c50a1956a2b867870d767200bd30f48d89bf04a4b6337f12e6577415da932cd2dfef9b4e9e9fdd52bd873afb06c6258b0e64244a44e
# Thu, 04 May 2023 11:15:35 GMT
COPY dir:0bcabfd400bd3bc041b1c80129dc5d15866643de006f873a085fbcc882fbdfdb in /usr/local/tomcat 
# Thu, 04 May 2023 11:15:38 GMT
RUN set -eux; 	apt-get update; 	xargs -rt apt-get install -y --no-install-recommends < "$TOMCAT_NATIVE_LIBDIR/.dependencies.txt"; 	rm -rf /var/lib/apt/lists/*
# Thu, 04 May 2023 11:15:39 GMT
RUN set -eux; 	nativeLines="$(catalina.sh configtest 2>&1)"; 	nativeLines="$(echo "$nativeLines" | grep 'Apache Tomcat Native')"; 	nativeLines="$(echo "$nativeLines" | sort -u)"; 	if ! echo "$nativeLines" | grep -E 'INFO: Loaded( APR based)? Apache Tomcat Native library' >&2; then 		echo >&2 "$nativeLines"; 		exit 1; 	fi
# Thu, 04 May 2023 11:15:40 GMT
EXPOSE 8080
# Thu, 04 May 2023 11:15:40 GMT
CMD ["catalina.sh" "run"]
# Thu, 04 May 2023 12:42:47 GMT
LABEL org.opencontainers.image.authors=XWiki Development Team <committers@xwiki.org>
# Thu, 04 May 2023 12:42:47 GMT
LABEL org.opencontainers.image.url=https://hub.docker.com/_/xwiki
# Thu, 04 May 2023 12:42:48 GMT
LABEL org.opencontainers.image.documentation=https://hub.docker.com/_/xwiki
# Thu, 04 May 2023 12:42:48 GMT
LABEL org.opencontainers.image.source=https://github.com/xwiki/xwiki-docker.git
# Thu, 04 May 2023 12:42:48 GMT
LABEL org.opencontainers.image.vendor=xwiki.org
# Thu, 04 May 2023 12:42:48 GMT
LABEL org.opencontainers.image.licenses=LGPL-2.1
# Thu, 04 May 2023 12:44:53 GMT
RUN apt-get update &&   apt-get --no-install-recommends -y install     curl     libreoffice     unzip     procps &&   rm -rf /var/lib/apt/lists/*
# Thu, 04 May 2023 12:47:21 GMT
ENV XWIKI_VERSION=14.10.9
# Thu, 04 May 2023 12:47:21 GMT
ENV XWIKI_URL_PREFIX=https://maven.xwiki.org/releases/org/xwiki/platform/xwiki-platform-distribution-war/14.10.9
# Thu, 04 May 2023 12:47:21 GMT
ENV XWIKI_DOWNLOAD_SHA256=81594962a2101d54866bccf768ea5b1637f836c57c5b212e221d043e96f5f35d
# Thu, 04 May 2023 12:48:00 GMT
RUN rm -rf /usr/local/tomcat/webapps/* &&   mkdir -p /usr/local/tomcat/temp &&   mkdir -p /usr/local/xwiki/data &&   curl -fSL "${XWIKI_URL_PREFIX}/xwiki-platform-distribution-war-${XWIKI_VERSION}.war" -o xwiki.war &&   echo "$XWIKI_DOWNLOAD_SHA256 xwiki.war" | sha256sum -c - &&   unzip -d /usr/local/tomcat/webapps/ROOT xwiki.war &&   rm -f xwiki.war
# Thu, 04 May 2023 12:48:03 GMT
ENV MYSQL_JDBC_VERSION=8.0.33
# Thu, 04 May 2023 12:48:03 GMT
ENV MYSQL_JDBC_SHA256=e2a3b2fc726a1ac64e998585db86b30fa8bf3f706195b78bb77c5f99bf877bd9
# Thu, 04 May 2023 12:48:03 GMT
ENV MYSQL_JDBC_PREFIX=https://repo1.maven.org/maven2/com/mysql/mysql-connector-j/8.0.33
# Thu, 04 May 2023 12:48:03 GMT
ENV MYSQL_JDBC_ARTIFACT=mysql-connector-j-8.0.33.jar
# Thu, 04 May 2023 12:48:03 GMT
ENV MYSQL_JDBC_TARGET=/usr/local/tomcat/webapps/ROOT/WEB-INF/lib/mysql-connector-j-8.0.33.jar
# Thu, 04 May 2023 12:48:04 GMT
RUN curl -fSL "${MYSQL_JDBC_PREFIX}/${MYSQL_JDBC_ARTIFACT}" -o $MYSQL_JDBC_TARGET &&   echo "$MYSQL_JDBC_SHA256 $MYSQL_JDBC_TARGET" | sha256sum -c -
# Thu, 04 May 2023 12:48:04 GMT
COPY file:0a1be11e2eb610a1dbcd415404e3a592641110b93090030cb831e3a19a163017 in /usr/local/tomcat/bin/ 
# Thu, 04 May 2023 12:48:04 GMT
COPY file:1b8409986f3e4eb79a7a0b18472cb2692a61d504fb5ef34292bc997b79fd760d in /usr/local/tomcat/webapps/ROOT/WEB-INF/hibernate.cfg.xml 
# Thu, 04 May 2023 12:48:04 GMT
RUN sed -i 's/<id>org.xwiki.platform:xwiki-platform-distribution-war/<id>org.xwiki.platform:xwiki-platform-distribution-docker/'   /usr/local/tomcat/webapps/ROOT/META-INF/extension.xed
# Thu, 04 May 2023 12:48:05 GMT
COPY file:a47c4dcd87c9dad97aff38c49188357e6193bcad50757e516cfb08a60d4de611 in /usr/local/bin/docker-entrypoint.sh 
# Thu, 04 May 2023 12:48:05 GMT
VOLUME [/usr/local/xwiki]
# Thu, 04 May 2023 12:48:05 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 04 May 2023 12:48:05 GMT
CMD ["xwiki"]
```

-	Layers:
	-	`sha256:f3f60f415e9a03eed88bd5dd5268c841cde08dacf16911a3ef1e4e0fcdd76568`  
		Last Modified: Wed, 26 Apr 2023 02:08:37 GMT  
		Size: 28.4 MB (28389440 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:89fb3595122d1cb6fffe722e2624c3c89b00776b393256a5444af56ceda691cf`  
		Last Modified: Thu, 04 May 2023 03:28:13 GMT  
		Size: 12.5 MB (12463858 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5542665e33e692b672a405517e6e267c4c6e210bc410b97a6a1ce732618caa87`  
		Last Modified: Thu, 04 May 2023 03:29:19 GMT  
		Size: 45.0 MB (45009401 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3e52b8550f0ced98adb0880bd041e361ffb69810e6071e6d71eb2ec0c8ecfad5`  
		Last Modified: Thu, 04 May 2023 03:29:14 GMT  
		Size: 160.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5ea5566732e0a920d0a63e4fbebf073d2c49e3f80716df462e73f895cc0c5dfa`  
		Last Modified: Thu, 04 May 2023 11:24:23 GMT  
		Size: 173.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:134f234c43263b3eada6763cc65397d96cdc17419b9d9c14c79d4b7e35e9cee5`  
		Last Modified: Thu, 04 May 2023 11:26:07 GMT  
		Size: 12.2 MB (12239971 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e3efae6aba6925ec511bd7a9fb49149380b2d71b62c10e71a0cd8acd04b559dc`  
		Last Modified: Thu, 04 May 2023 11:26:06 GMT  
		Size: 453.7 KB (453686 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:49137d740c7145f0a272da7935eebd70172db0c8ab54f2d3a8f9b4ecee02b771`  
		Last Modified: Thu, 04 May 2023 11:26:05 GMT  
		Size: 130.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:40220eff64fe6bee4cd0f6ed5d86c091d30b6671bd50ba8574969f6797656808`  
		Last Modified: Thu, 04 May 2023 12:49:38 GMT  
		Size: 173.4 MB (173350233 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9dbaeafeabd93126303105c70ddbad02cb59d462f5c35305bb561be7d0491874`  
		Last Modified: Thu, 04 May 2023 12:51:15 GMT  
		Size: 307.2 MB (307217526 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:773862037c83b913abe36e2ced95126e1ee646a9bfcf2457eb4fc30a4253548e`  
		Last Modified: Thu, 04 May 2023 12:51:01 GMT  
		Size: 2.3 MB (2343676 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e51e51b377bb6beaee5dbd0a71921194f68052e5ffaccbbcada71930a631cb2b`  
		Last Modified: Thu, 04 May 2023 12:51:01 GMT  
		Size: 1.3 KB (1342 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6774a791b55bd03290494873dda0ed43f59aa7f7fd51609b727440601b9dd461`  
		Last Modified: Thu, 04 May 2023 12:51:01 GMT  
		Size: 2.3 KB (2306 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:54106b42bccee5350ad9e29761849ff34b3c6a18697184ec16c14fa13537b58a`  
		Last Modified: Thu, 04 May 2023 12:51:01 GMT  
		Size: 6.0 KB (6012 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:544d1e7b8b61592cfff4fdeb26071db27348b16ce4472d4317c320dd0e32ec24`  
		Last Modified: Thu, 04 May 2023 12:51:01 GMT  
		Size: 2.5 KB (2500 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
