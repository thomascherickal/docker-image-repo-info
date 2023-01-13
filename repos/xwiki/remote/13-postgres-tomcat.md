## `xwiki:13-postgres-tomcat`

```console
$ docker pull xwiki@sha256:7d7be9ed195aa32b26473c49840ae5f61f4f88fe8f80ce8b65e8b95720650087
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `xwiki:13-postgres-tomcat` - linux; amd64

```console
$ docker pull xwiki@sha256:7a026d457d97cf1e2a4a4a0bbe8a964581c22abc14b87bf4869ea4d57bcb66de
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **575.5 MB (575490686 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:dd3593c8c4005afa1a1a76281b5f03ede254a129a575ef8071acf5e77f07d61d`
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
# Fri, 13 Jan 2023 21:26:29 GMT
ENV TOMCAT_VERSION=9.0.71
# Fri, 13 Jan 2023 21:26:29 GMT
ENV TOMCAT_SHA512=6a747e68eff4b68a8defba111103ef6b1606030c180143de0419d015052a5567fca1a86e3d3e058a10246c02b98e89431e9344f80475189573fa0d5c70bfb4cb
# Fri, 13 Jan 2023 21:26:30 GMT
COPY dir:c553b88d1b69fc83948574afcba443e11fded7dcf945801e8dcaeaccf354f922 in /usr/local/tomcat 
# Fri, 13 Jan 2023 21:26:34 GMT
RUN set -eux; 	apt-get update; 	xargs -rt apt-get install -y --no-install-recommends < "$TOMCAT_NATIVE_LIBDIR/.dependencies.txt"; 	rm -rf /var/lib/apt/lists/*
# Fri, 13 Jan 2023 21:26:35 GMT
RUN set -eux; 	nativeLines="$(catalina.sh configtest 2>&1)"; 	nativeLines="$(echo "$nativeLines" | grep 'Apache Tomcat Native')"; 	nativeLines="$(echo "$nativeLines" | sort -u)"; 	if ! echo "$nativeLines" | grep -E 'INFO: Loaded( APR based)? Apache Tomcat Native library' >&2; then 		echo >&2 "$nativeLines"; 		exit 1; 	fi
# Fri, 13 Jan 2023 21:26:35 GMT
EXPOSE 8080
# Fri, 13 Jan 2023 21:26:35 GMT
CMD ["catalina.sh" "run"]
# Fri, 13 Jan 2023 21:58:15 GMT
LABEL org.opencontainers.image.authors=XWiki Development Team <committers@xwiki.org>
# Fri, 13 Jan 2023 21:58:15 GMT
LABEL org.opencontainers.image.url=https://hub.docker.com/_/xwiki
# Fri, 13 Jan 2023 21:58:15 GMT
LABEL org.opencontainers.image.documentation=https://hub.docker.com/_/xwiki
# Fri, 13 Jan 2023 21:58:15 GMT
LABEL org.opencontainers.image.source=https://github.com/xwiki/xwiki-docker.git
# Fri, 13 Jan 2023 21:58:16 GMT
LABEL org.opencontainers.image.vendor=xwiki.org
# Fri, 13 Jan 2023 21:58:16 GMT
LABEL org.opencontainers.image.licenses=LGPL-2.1
# Fri, 13 Jan 2023 22:01:21 GMT
RUN apt-get update &&   apt-get --no-install-recommends -y install     curl     libreoffice     unzip     procps     libpostgresql-jdbc-java &&   rm -rf /var/lib/apt/lists/*
# Fri, 13 Jan 2023 22:03:10 GMT
ENV XWIKI_VERSION=13.10.11
# Fri, 13 Jan 2023 22:03:10 GMT
ENV XWIKI_URL_PREFIX=https://maven.xwiki.org/releases/org/xwiki/platform/xwiki-platform-distribution-war/13.10.11
# Fri, 13 Jan 2023 22:03:10 GMT
ENV XWIKI_DOWNLOAD_SHA256=fd4f65fdef717f64008ab54845f8bd2973916fe8621c0c9298b45a50901c84ca
# Fri, 13 Jan 2023 22:03:48 GMT
RUN rm -rf /usr/local/tomcat/webapps/* &&   mkdir -p /usr/local/tomcat/temp &&   mkdir -p /usr/local/xwiki/data &&   curl -fSL "${XWIKI_URL_PREFIX}/xwiki-platform-distribution-war-${XWIKI_VERSION}.war" -o xwiki.war &&   echo "$XWIKI_DOWNLOAD_SHA256 xwiki.war" | sha256sum -c - &&   unzip -d /usr/local/tomcat/webapps/ROOT xwiki.war &&   rm -f xwiki.war
# Fri, 13 Jan 2023 22:03:49 GMT
RUN cp /usr/share/java/postgresql-jdbc4.jar /usr/local/tomcat/webapps/ROOT/WEB-INF/lib/
# Fri, 13 Jan 2023 22:03:49 GMT
COPY file:0a1be11e2eb610a1dbcd415404e3a592641110b93090030cb831e3a19a163017 in /usr/local/tomcat/bin/ 
# Fri, 13 Jan 2023 22:03:49 GMT
COPY file:4a923f484bb29a26630c19e1d617d3bf6aa6ae7c6c4a5561e97b037bcde0847c in /usr/local/tomcat/webapps/ROOT/WEB-INF/hibernate.cfg.xml 
# Fri, 13 Jan 2023 22:03:50 GMT
RUN sed -i 's/<id>org.xwiki.platform:xwiki-platform-distribution-war/<id>org.xwiki.platform:xwiki-platform-distribution-docker/'   /usr/local/tomcat/webapps/ROOT/META-INF/extension.xed
# Fri, 13 Jan 2023 22:03:50 GMT
COPY file:a47c4dcd87c9dad97aff38c49188357e6193bcad50757e516cfb08a60d4de611 in /usr/local/bin/docker-entrypoint.sh 
# Fri, 13 Jan 2023 22:03:50 GMT
VOLUME [/usr/local/xwiki]
# Fri, 13 Jan 2023 22:03:50 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 13 Jan 2023 22:03:50 GMT
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
	-	`sha256:370064d0ba3592e825553149e7d84bae1725d220243e08d9eb32449e1e75833e`  
		Last Modified: Fri, 13 Jan 2023 21:39:09 GMT  
		Size: 12.2 MB (12205321 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3da93c4bf3ff8802031fca644b8c81cc8ba4154a4360d3cf272df5016597ac7d`  
		Last Modified: Fri, 13 Jan 2023 21:39:08 GMT  
		Size: 452.8 KB (452800 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:09b58a7bb781d7c12fbb179b7a0653cf9f11087543f250c99b5d3aa673f22e52`  
		Last Modified: Fri, 13 Jan 2023 21:39:08 GMT  
		Size: 130.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:97326679d5b571adcad7dcbd0c9f79e7983db6cf2d35e896ede2bc9c37a5891a`  
		Last Modified: Fri, 13 Jan 2023 22:06:06 GMT  
		Size: 179.7 MB (179745818 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1c306594b9ce4f1a0d99670e247141ca2480296dfe3d7166453bbfc410145d99`  
		Last Modified: Fri, 13 Jan 2023 22:07:23 GMT  
		Size: 292.6 MB (292644629 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7c74eec29f4a5508e1e9634a46ef25f41d5d5f1103302a1d5ddd188925ebf3ca`  
		Last Modified: Fri, 13 Jan 2023 22:07:07 GMT  
		Size: 936.9 KB (936850 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:015ce88ca700d1974a82707b3b3b08b9525c60ca63adc94a56c30f7a15b4f421`  
		Last Modified: Fri, 13 Jan 2023 22:07:06 GMT  
		Size: 1.3 KB (1343 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:12b2462ca836091941b04908b1ff491e8a4656d9bf7c42e5201075728a9c2a80`  
		Last Modified: Fri, 13 Jan 2023 22:07:06 GMT  
		Size: 2.5 KB (2452 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:64013c4e85e2e2ec0ed0ed982317b0a42a898317f2ce27f9bbb92661c9377b69`  
		Last Modified: Fri, 13 Jan 2023 22:07:06 GMT  
		Size: 5.4 KB (5358 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:918671da7af802d24c2daa78cb5869a9b565720a5ce6df53073f2edf1d89b20a`  
		Last Modified: Fri, 13 Jan 2023 22:07:06 GMT  
		Size: 2.5 KB (2504 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `xwiki:13-postgres-tomcat` - linux; arm64 variant v8

```console
$ docker pull xwiki@sha256:db7bc3996929154c8975214a3ef976300d829da754d3a6a2927155b0f7c9b762
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **566.3 MB (566285251 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e43edc8a1ca7c8143deed92aa08ce6bfd21d5fbd9236bde8f86f6d343af7b20d`
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
# Fri, 09 Dec 2022 08:41:35 GMT
RUN apt-get update &&   apt-get --no-install-recommends -y install     curl     libreoffice     unzip     procps     libpostgresql-jdbc-java &&   rm -rf /var/lib/apt/lists/*
# Thu, 05 Jan 2023 18:04:29 GMT
ENV XWIKI_VERSION=13.10.11
# Thu, 05 Jan 2023 18:04:29 GMT
ENV XWIKI_URL_PREFIX=https://maven.xwiki.org/releases/org/xwiki/platform/xwiki-platform-distribution-war/13.10.11
# Thu, 05 Jan 2023 18:04:29 GMT
ENV XWIKI_DOWNLOAD_SHA256=fd4f65fdef717f64008ab54845f8bd2973916fe8621c0c9298b45a50901c84ca
# Thu, 05 Jan 2023 18:05:06 GMT
RUN rm -rf /usr/local/tomcat/webapps/* &&   mkdir -p /usr/local/tomcat/temp &&   mkdir -p /usr/local/xwiki/data &&   curl -fSL "${XWIKI_URL_PREFIX}/xwiki-platform-distribution-war-${XWIKI_VERSION}.war" -o xwiki.war &&   echo "$XWIKI_DOWNLOAD_SHA256 xwiki.war" | sha256sum -c - &&   unzip -d /usr/local/tomcat/webapps/ROOT xwiki.war &&   rm -f xwiki.war
# Thu, 05 Jan 2023 18:05:09 GMT
RUN cp /usr/share/java/postgresql-jdbc4.jar /usr/local/tomcat/webapps/ROOT/WEB-INF/lib/
# Thu, 05 Jan 2023 18:05:09 GMT
COPY file:0a1be11e2eb610a1dbcd415404e3a592641110b93090030cb831e3a19a163017 in /usr/local/tomcat/bin/ 
# Thu, 05 Jan 2023 18:05:09 GMT
COPY file:4a923f484bb29a26630c19e1d617d3bf6aa6ae7c6c4a5561e97b037bcde0847c in /usr/local/tomcat/webapps/ROOT/WEB-INF/hibernate.cfg.xml 
# Thu, 05 Jan 2023 18:05:09 GMT
RUN sed -i 's/<id>org.xwiki.platform:xwiki-platform-distribution-war/<id>org.xwiki.platform:xwiki-platform-distribution-docker/'   /usr/local/tomcat/webapps/ROOT/META-INF/extension.xed
# Thu, 05 Jan 2023 18:05:09 GMT
COPY file:a47c4dcd87c9dad97aff38c49188357e6193bcad50757e516cfb08a60d4de611 in /usr/local/bin/docker-entrypoint.sh 
# Thu, 05 Jan 2023 18:05:10 GMT
VOLUME [/usr/local/xwiki]
# Thu, 05 Jan 2023 18:05:10 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 05 Jan 2023 18:05:10 GMT
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
	-	`sha256:10e6f8e7753d9fc0cd173f7c5ac1d61410ccbebbdfc1b0149f3856b021664faa`  
		Last Modified: Fri, 09 Dec 2022 08:47:49 GMT  
		Size: 174.3 MB (174289933 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6135141ca5d9d30cbd487f39b241114f89608a56d5556d9fd0b2709e4c9a4210`  
		Last Modified: Thu, 05 Jan 2023 18:07:21 GMT  
		Size: 292.6 MB (292644621 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e56f31839a1929bc53746b398dbb1242ea936cd6cf672f466225abc11cbf145b`  
		Last Modified: Thu, 05 Jan 2023 18:07:07 GMT  
		Size: 936.8 KB (936844 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4ec8e3229efd5db779784b170c6daabe4764a2f058d2e7f857fda52e531f1080`  
		Last Modified: Thu, 05 Jan 2023 18:07:06 GMT  
		Size: 1.3 KB (1340 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:59a22027312bf73fbf2d66df4c816e45752e03e3484010a7a7a204c7229ecf5b`  
		Last Modified: Thu, 05 Jan 2023 18:07:06 GMT  
		Size: 2.4 KB (2447 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9bd13e9d7593e2679a3757c50dd1950f7cb4231ecd49ce900e2cdfae93c7f51e`  
		Last Modified: Thu, 05 Jan 2023 18:07:06 GMT  
		Size: 5.4 KB (5358 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:da38558e21d13fa19b74530629fde6c40a6375426c84676c4d2d7246f7a9b452`  
		Last Modified: Thu, 05 Jan 2023 18:07:06 GMT  
		Size: 2.5 KB (2498 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
