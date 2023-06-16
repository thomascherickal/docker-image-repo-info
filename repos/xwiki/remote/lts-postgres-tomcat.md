## `xwiki:lts-postgres-tomcat`

```console
$ docker pull xwiki@sha256:e5b4ec5a77459dacc496c22e2680b803be8048693e532f2a92a0187c9083f663
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `xwiki:lts-postgres-tomcat` - linux; amd64

```console
$ docker pull xwiki@sha256:9a4b7e4a8ffaa281e3dedfe35b9ac700bf24f7e384e1787fd5b6c4770138d94f
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **592.3 MB (592301986 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:3ce4b4174ac14f1ee8e5b536aadf712c30c52f1b19c7e24784e0305115f1e952`
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
# Sat, 10 Jun 2023 01:08:17 GMT
RUN apt-get update &&   apt-get --no-install-recommends -y install     curl     libreoffice     unzip     procps     libpostgresql-jdbc-java &&   rm -rf /var/lib/apt/lists/*
# Sat, 10 Jun 2023 01:10:08 GMT
ENV XWIKI_VERSION=14.10.12
# Sat, 10 Jun 2023 01:10:08 GMT
ENV XWIKI_URL_PREFIX=https://maven.xwiki.org/releases/org/xwiki/platform/xwiki-platform-distribution-war/14.10.12
# Sat, 10 Jun 2023 01:10:08 GMT
ENV XWIKI_DOWNLOAD_SHA256=45a7eb79eaf7c29094c7cb3fe97cb221f02509b6a8bdb8c382f34cc0d77eeb9c
# Sat, 10 Jun 2023 01:10:47 GMT
RUN rm -rf /usr/local/tomcat/webapps/* &&   mkdir -p /usr/local/tomcat/temp &&   mkdir -p /usr/local/xwiki/data &&   curl -fSL "${XWIKI_URL_PREFIX}/xwiki-platform-distribution-war-${XWIKI_VERSION}.war" -o xwiki.war &&   echo "$XWIKI_DOWNLOAD_SHA256 xwiki.war" | sha256sum -c - &&   unzip -d /usr/local/tomcat/webapps/ROOT xwiki.war &&   rm -f xwiki.war
# Sat, 10 Jun 2023 01:10:48 GMT
RUN cp /usr/share/java/postgresql-jdbc4.jar /usr/local/tomcat/webapps/ROOT/WEB-INF/lib/
# Sat, 10 Jun 2023 01:10:48 GMT
COPY file:0a1be11e2eb610a1dbcd415404e3a592641110b93090030cb831e3a19a163017 in /usr/local/tomcat/bin/ 
# Sat, 10 Jun 2023 01:10:48 GMT
COPY file:4a923f484bb29a26630c19e1d617d3bf6aa6ae7c6c4a5561e97b037bcde0847c in /usr/local/tomcat/webapps/ROOT/WEB-INF/hibernate.cfg.xml 
# Sat, 10 Jun 2023 01:10:49 GMT
RUN sed -i 's/<id>org.xwiki.platform:xwiki-platform-distribution-war/<id>org.xwiki.platform:xwiki-platform-distribution-docker/'   /usr/local/tomcat/webapps/ROOT/META-INF/extension.xed
# Sat, 10 Jun 2023 01:10:49 GMT
COPY file:a47c4dcd87c9dad97aff38c49188357e6193bcad50757e516cfb08a60d4de611 in /usr/local/bin/docker-entrypoint.sh 
# Sat, 10 Jun 2023 01:10:49 GMT
VOLUME [/usr/local/xwiki]
# Sat, 10 Jun 2023 01:10:49 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Sat, 10 Jun 2023 01:10:49 GMT
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
	-	`sha256:97fa1394faf71fc54b7885f80cd1ff593ac763945623360571b9e14a75c35983`  
		Last Modified: Sat, 10 Jun 2023 01:12:40 GMT  
		Size: 179.3 MB (179274428 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:be232844ac58c7f5576204267451fa8e8673ac60842626deb025eda0f250a012`  
		Last Modified: Sat, 10 Jun 2023 01:14:16 GMT  
		Size: 307.3 MB (307251913 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5c2c1f25014edad33be80a0d44c08e8f461261d52f721caa9d53bd8b9be47c63`  
		Last Modified: Sat, 10 Jun 2023 01:14:00 GMT  
		Size: 936.8 KB (936846 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6cb94d52b533ba0a988f3f8d84499052a59d66b8226f406caaf3a6d10e97da52`  
		Last Modified: Sat, 10 Jun 2023 01:13:59 GMT  
		Size: 1.3 KB (1346 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:239b687833187403a3932f23cbe4f597715847278a643678697ee7ed97cd706b`  
		Last Modified: Sat, 10 Jun 2023 01:13:59 GMT  
		Size: 2.5 KB (2457 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:49f1e2ae2accd008d515a918836f7b68e5bc666b4ae6b4574ac7ffe7fce7d28d`  
		Last Modified: Sat, 10 Jun 2023 01:13:59 GMT  
		Size: 6.0 KB (6015 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6853f982a34129b644efcd27a88c77994992b24e4dc9c13b23692237472f2450`  
		Last Modified: Sat, 10 Jun 2023 01:13:59 GMT  
		Size: 2.5 KB (2504 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `xwiki:lts-postgres-tomcat` - linux; arm64 variant v8

```console
$ docker pull xwiki@sha256:302424b6e60500ac953db0acbbfca81391ba8d67fe41604f28e0e24a53fce4b4
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **581.1 MB (581096573 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e8871279bf1b6489d2208b71ef40d6ea624a4639a949e8f9d9f2d7b789bf165e`
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
# Fri, 16 Jun 2023 08:38:18 GMT
RUN apt-get update &&   apt-get --no-install-recommends -y install     curl     libreoffice     unzip     procps     libpostgresql-jdbc-java &&   rm -rf /var/lib/apt/lists/*
# Fri, 16 Jun 2023 08:40:09 GMT
ENV XWIKI_VERSION=14.10.12
# Fri, 16 Jun 2023 08:40:10 GMT
ENV XWIKI_URL_PREFIX=https://maven.xwiki.org/releases/org/xwiki/platform/xwiki-platform-distribution-war/14.10.12
# Fri, 16 Jun 2023 08:40:10 GMT
ENV XWIKI_DOWNLOAD_SHA256=45a7eb79eaf7c29094c7cb3fe97cb221f02509b6a8bdb8c382f34cc0d77eeb9c
# Fri, 16 Jun 2023 08:40:50 GMT
RUN rm -rf /usr/local/tomcat/webapps/* &&   mkdir -p /usr/local/tomcat/temp &&   mkdir -p /usr/local/xwiki/data &&   curl -fSL "${XWIKI_URL_PREFIX}/xwiki-platform-distribution-war-${XWIKI_VERSION}.war" -o xwiki.war &&   echo "$XWIKI_DOWNLOAD_SHA256 xwiki.war" | sha256sum -c - &&   unzip -d /usr/local/tomcat/webapps/ROOT xwiki.war &&   rm -f xwiki.war
# Fri, 16 Jun 2023 08:40:52 GMT
RUN cp /usr/share/java/postgresql-jdbc4.jar /usr/local/tomcat/webapps/ROOT/WEB-INF/lib/
# Fri, 16 Jun 2023 08:40:52 GMT
COPY file:0a1be11e2eb610a1dbcd415404e3a592641110b93090030cb831e3a19a163017 in /usr/local/tomcat/bin/ 
# Fri, 16 Jun 2023 08:40:53 GMT
COPY file:4a923f484bb29a26630c19e1d617d3bf6aa6ae7c6c4a5561e97b037bcde0847c in /usr/local/tomcat/webapps/ROOT/WEB-INF/hibernate.cfg.xml 
# Fri, 16 Jun 2023 08:40:53 GMT
RUN sed -i 's/<id>org.xwiki.platform:xwiki-platform-distribution-war/<id>org.xwiki.platform:xwiki-platform-distribution-docker/'   /usr/local/tomcat/webapps/ROOT/META-INF/extension.xed
# Fri, 16 Jun 2023 08:40:53 GMT
COPY file:a47c4dcd87c9dad97aff38c49188357e6193bcad50757e516cfb08a60d4de611 in /usr/local/bin/docker-entrypoint.sh 
# Fri, 16 Jun 2023 08:40:53 GMT
VOLUME [/usr/local/xwiki]
# Fri, 16 Jun 2023 08:40:53 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 16 Jun 2023 08:40:53 GMT
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
	-	`sha256:c39ac1621db1ef9aa8b14326a6dc2e420abb620210dcb258091c7dc92347f234`  
		Last Modified: Fri, 16 Jun 2023 08:42:27 GMT  
		Size: 174.3 MB (174312132 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3792e76d9349a984593ce838c72be826684c15fe7ab634fe12f9d7dc1ca270c7`  
		Last Modified: Fri, 16 Jun 2023 08:43:57 GMT  
		Size: 307.3 MB (307251932 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5aa4f9ee990da22eadb26998fa9ded304bf03fa61b49d99d8b02c688ab1df1c9`  
		Last Modified: Fri, 16 Jun 2023 08:43:43 GMT  
		Size: 936.9 KB (936851 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bd40dda6c2bcef3017f1a8bbae4ad333a74dcf7c2a1d314059e67b5236b64d34`  
		Last Modified: Fri, 16 Jun 2023 08:43:43 GMT  
		Size: 1.3 KB (1347 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:82ca142337b3a088e4d6e935b8c344d8a798ed93a391e8a40068e96d82d98204`  
		Last Modified: Fri, 16 Jun 2023 08:43:42 GMT  
		Size: 2.5 KB (2457 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bdec165f74145e64ad5a11891060dcea2f179eccd8bd198af280ef74650bcbf3`  
		Last Modified: Fri, 16 Jun 2023 08:43:42 GMT  
		Size: 6.0 KB (6019 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:85d3d53d008c5253694f27eb0810842fbbe1a1fa56731f40c1d47d9a036ae086`  
		Last Modified: Fri, 16 Jun 2023 08:43:42 GMT  
		Size: 2.5 KB (2506 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
