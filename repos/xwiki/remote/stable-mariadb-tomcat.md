## `xwiki:stable-mariadb-tomcat`

```console
$ docker pull xwiki@sha256:f17feaac020715e423425fb71720aeeadfaf00043b188f0262497aab3d42bad9
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `xwiki:stable-mariadb-tomcat` - linux; amd64

```console
$ docker pull xwiki@sha256:2f75757cf401de6514218d5a9f0be117e4f724b2021ede2b85b99d7c3ec0fe84
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **587.4 MB (587440624 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:4b866ffc3bba6e12461ea117ede5cadeca5127f28afdb7906a1ded64f69ee904`
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
# Thu, 04 May 2023 18:03:02 GMT
ENV XWIKI_VERSION=15.3
# Thu, 04 May 2023 18:03:02 GMT
ENV XWIKI_URL_PREFIX=https://maven.xwiki.org/releases/org/xwiki/platform/xwiki-platform-distribution-war/15.3
# Thu, 04 May 2023 18:03:02 GMT
ENV XWIKI_DOWNLOAD_SHA256=fbe35bcc5c6cc5764f2a1da4aca7878531f93bae069d94f399fea7d9656da3b8
# Thu, 04 May 2023 18:03:41 GMT
RUN rm -rf /usr/local/tomcat/webapps/* &&   mkdir -p /usr/local/tomcat/temp &&   mkdir -p /usr/local/xwiki/data &&   curl -fSL "${XWIKI_URL_PREFIX}/xwiki-platform-distribution-war-${XWIKI_VERSION}.war" -o xwiki.war &&   echo "$XWIKI_DOWNLOAD_SHA256 xwiki.war" | sha256sum -c - &&   unzip -d /usr/local/tomcat/webapps/ROOT xwiki.war &&   rm -f xwiki.war
# Thu, 04 May 2023 18:05:22 GMT
ENV MARIADB_JDBC_VERSION=3.1.3
# Thu, 04 May 2023 18:05:22 GMT
ENV MARIADB_JDBC_SHA256=11297ee6562426c49c81387c860153cbc131c4c3d042492d4f6d2d97ab3a1ca5
# Thu, 04 May 2023 18:05:22 GMT
ENV MARIADB_JDBC_PREFIX=https://repo1.maven.org/maven2/org/mariadb/jdbc/mariadb-java-client/3.1.3
# Thu, 04 May 2023 18:05:22 GMT
ENV MARIADB_JDBC_ARTIFACT=mariadb-java-client-3.1.3.jar
# Thu, 04 May 2023 18:05:22 GMT
ENV MARIADB_JDBC_TARGET=/usr/local/tomcat/webapps/ROOT/WEB-INF/lib/mariadb-java-client-3.1.3.jar
# Thu, 04 May 2023 18:05:23 GMT
RUN curl -fSL "${MARIADB_JDBC_PREFIX}/${MARIADB_JDBC_ARTIFACT}" -o $MARIADB_JDBC_TARGET &&   echo "$MARIADB_JDBC_SHA256 $MARIADB_JDBC_TARGET" | sha256sum -c -
# Thu, 04 May 2023 18:05:23 GMT
COPY file:0a1be11e2eb610a1dbcd415404e3a592641110b93090030cb831e3a19a163017 in /usr/local/tomcat/bin/ 
# Thu, 04 May 2023 18:05:23 GMT
COPY file:0e237c3876eeb3b5f3473a064d3e507da2df6c228ca714687930b34e3b687601 in /usr/local/tomcat/webapps/ROOT/WEB-INF/hibernate.cfg.xml 
# Thu, 04 May 2023 18:05:24 GMT
RUN sed -i 's/<id>org.xwiki.platform:xwiki-platform-distribution-war/<id>org.xwiki.platform:xwiki-platform-distribution-docker/'   /usr/local/tomcat/webapps/ROOT/META-INF/extension.xed
# Thu, 04 May 2023 18:05:24 GMT
COPY file:a47c4dcd87c9dad97aff38c49188357e6193bcad50757e516cfb08a60d4de611 in /usr/local/bin/docker-entrypoint.sh 
# Thu, 04 May 2023 18:05:24 GMT
VOLUME [/usr/local/xwiki]
# Thu, 04 May 2023 18:05:24 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 04 May 2023 18:05:24 GMT
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
	-	`sha256:eb3a9e60a1eb57809cf0769ac11bf588897c9779e42b0b61d5f676a175e48df0`  
		Last Modified: Thu, 04 May 2023 18:08:02 GMT  
		Size: 306.2 MB (306214280 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:50def37e3f4eff479ae0cf2929eaf7cdf11fdfdcc609bb3f20c25646c6b74b02`  
		Last Modified: Thu, 04 May 2023 18:09:16 GMT  
		Size: 591.4 KB (591380 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d9013f32d80fb93a21e84dbe9ed75a8f5068ab5276efa6592a2c8e200f20a5b4`  
		Last Modified: Thu, 04 May 2023 18:09:16 GMT  
		Size: 1.3 KB (1342 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1c9800dc7d508492f35cb67a8176ad0df360e4bd0929ba29bedfda1e847c7194`  
		Last Modified: Thu, 04 May 2023 18:09:16 GMT  
		Size: 2.3 KB (2313 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e1062aa99a39a557eff2e8c8f65cf9e5105a3e7ee30f21e6133a39a1074c298f`  
		Last Modified: Thu, 04 May 2023 18:09:16 GMT  
		Size: 6.0 KB (6004 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4bdf45d627dc37a0cdd1dba6ad59ad7ba4dfa24e55fafaeab5b726a0154c0240`  
		Last Modified: Thu, 04 May 2023 18:09:16 GMT  
		Size: 2.5 KB (2504 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `xwiki:stable-mariadb-tomcat` - linux; arm64 variant v8

```console
$ docker pull xwiki@sha256:0b317694619cab90bb645fdadce29ee86f870ae8dd8c9b705a4b7a4a5ecec9bb
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **578.7 MB (578724889 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:2d2e1572e20616745e9b7b4f89c5522874340d479347c72b37dd41cdab28414a`
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
# Thu, 04 May 2023 12:44:56 GMT
ENV XWIKI_VERSION=15.3
# Thu, 04 May 2023 12:44:57 GMT
ENV XWIKI_URL_PREFIX=https://maven.xwiki.org/releases/org/xwiki/platform/xwiki-platform-distribution-war/15.3
# Thu, 04 May 2023 12:44:57 GMT
ENV XWIKI_DOWNLOAD_SHA256=fbe35bcc5c6cc5764f2a1da4aca7878531f93bae069d94f399fea7d9656da3b8
# Thu, 04 May 2023 12:45:37 GMT
RUN rm -rf /usr/local/tomcat/webapps/* &&   mkdir -p /usr/local/tomcat/temp &&   mkdir -p /usr/local/xwiki/data &&   curl -fSL "${XWIKI_URL_PREFIX}/xwiki-platform-distribution-war-${XWIKI_VERSION}.war" -o xwiki.war &&   echo "$XWIKI_DOWNLOAD_SHA256 xwiki.war" | sha256sum -c - &&   unzip -d /usr/local/tomcat/webapps/ROOT xwiki.war &&   rm -f xwiki.war
# Thu, 04 May 2023 12:47:17 GMT
ENV MARIADB_JDBC_VERSION=3.1.3
# Thu, 04 May 2023 12:47:17 GMT
ENV MARIADB_JDBC_SHA256=11297ee6562426c49c81387c860153cbc131c4c3d042492d4f6d2d97ab3a1ca5
# Thu, 04 May 2023 12:47:18 GMT
ENV MARIADB_JDBC_PREFIX=https://repo1.maven.org/maven2/org/mariadb/jdbc/mariadb-java-client/3.1.3
# Thu, 04 May 2023 12:47:18 GMT
ENV MARIADB_JDBC_ARTIFACT=mariadb-java-client-3.1.3.jar
# Thu, 04 May 2023 12:47:18 GMT
ENV MARIADB_JDBC_TARGET=/usr/local/tomcat/webapps/ROOT/WEB-INF/lib/mariadb-java-client-3.1.3.jar
# Thu, 04 May 2023 12:47:18 GMT
RUN curl -fSL "${MARIADB_JDBC_PREFIX}/${MARIADB_JDBC_ARTIFACT}" -o $MARIADB_JDBC_TARGET &&   echo "$MARIADB_JDBC_SHA256 $MARIADB_JDBC_TARGET" | sha256sum -c -
# Thu, 04 May 2023 12:47:18 GMT
COPY file:0a1be11e2eb610a1dbcd415404e3a592641110b93090030cb831e3a19a163017 in /usr/local/tomcat/bin/ 
# Thu, 04 May 2023 12:47:19 GMT
COPY file:0e237c3876eeb3b5f3473a064d3e507da2df6c228ca714687930b34e3b687601 in /usr/local/tomcat/webapps/ROOT/WEB-INF/hibernate.cfg.xml 
# Thu, 04 May 2023 12:47:19 GMT
RUN sed -i 's/<id>org.xwiki.platform:xwiki-platform-distribution-war/<id>org.xwiki.platform:xwiki-platform-distribution-docker/'   /usr/local/tomcat/webapps/ROOT/META-INF/extension.xed
# Thu, 04 May 2023 12:47:19 GMT
COPY file:a47c4dcd87c9dad97aff38c49188357e6193bcad50757e516cfb08a60d4de611 in /usr/local/bin/docker-entrypoint.sh 
# Thu, 04 May 2023 12:47:19 GMT
VOLUME [/usr/local/xwiki]
# Thu, 04 May 2023 12:47:19 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 04 May 2023 12:47:19 GMT
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
	-	`sha256:562cf3757c6983c31f0982e56ad17009001f4d6504ba59fbc057bf20aafb9293`  
		Last Modified: Thu, 04 May 2023 12:49:35 GMT  
		Size: 306.2 MB (306214317 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fd2261b6155324b170f5d67b366a4428d547e581cb6ebd9513b9eacf47890f9a`  
		Last Modified: Thu, 04 May 2023 12:50:43 GMT  
		Size: 591.4 KB (591366 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3b36702f16b9400237c652001c76219ed0f0f1f85c91c21d7f447c79788e22b4`  
		Last Modified: Thu, 04 May 2023 12:50:43 GMT  
		Size: 1.3 KB (1340 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a23a60f0f87e16aa8d37acf2f0d0a51a00c2e06bc171f3f0600db991dda6e19b`  
		Last Modified: Thu, 04 May 2023 12:50:43 GMT  
		Size: 2.3 KB (2310 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fbc0c4e78c3a41cf17795f36434313dda8a60e303b196b187d71dec55da49e83`  
		Last Modified: Thu, 04 May 2023 12:50:43 GMT  
		Size: 6.0 KB (6001 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e0fca56e7a03eee9e66554a1a11859b19805cb0d8a8d18dc8580e09c7a0534b3`  
		Last Modified: Thu, 04 May 2023 12:50:43 GMT  
		Size: 2.5 KB (2503 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
