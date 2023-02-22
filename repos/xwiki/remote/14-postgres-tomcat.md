## `xwiki:14-postgres-tomcat`

```console
$ docker pull xwiki@sha256:48a8c82a2dcfa36f6d55a5f3e75d3e2b3aca3f80de56276b35838dc7bcb6a4a6
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `xwiki:14-postgres-tomcat` - linux; amd64

```console
$ docker pull xwiki@sha256:5cd23e4200b4eed664a61d05e3d436d0e372a3e4e985e29cb866dd9dbb573713
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **590.0 MB (589983532 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ab0dc70572c5101e5837a6281e7cb29a2b4dbf26ad0b9c91860a748aeb3360e1`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["xwiki"]`

```dockerfile
# Wed, 02 Nov 2022 18:25:55 GMT
ADD file:29c72d5be8c977acaeb6391aeb23ec27559b594e25a0bb3a6dd280bac2847b7f in / 
# Wed, 02 Nov 2022 18:25:55 GMT
CMD ["bash"]
# Wed, 02 Nov 2022 18:43:42 GMT
ENV JAVA_HOME=/opt/java/openjdk
# Wed, 02 Nov 2022 18:43:42 GMT
ENV PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 02 Nov 2022 18:43:42 GMT
ENV LANG=en_US.UTF-8 LANGUAGE=en_US:en LC_ALL=en_US.UTF-8
# Wed, 02 Nov 2022 18:44:10 GMT
RUN apt-get update     && DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends tzdata curl wget ca-certificates fontconfig locales     && echo "en_US.UTF-8 UTF-8" >> /etc/locale.gen     && locale-gen en_US.UTF-8     && rm -rf /var/lib/apt/lists/*
# Fri, 04 Nov 2022 23:21:41 GMT
ENV JAVA_VERSION=jdk-11.0.17+8
# Fri, 04 Nov 2022 23:22:31 GMT
RUN set -eux;     ARCH="$(dpkg --print-architecture)";     case "${ARCH}" in        aarch64|arm64)          ESUM='bd6efe3290c8b5a42f695a55a26f3e3c9c284288574879d4b7089f31f5114177';          BINARY_URL='https://github.com/adoptium/temurin11-binaries/releases/download/jdk-11.0.17%2B8/OpenJDK11U-jre_aarch64_linux_hotspot_11.0.17_8.tar.gz';          ;;        armhf|arm)          ESUM='8cf113d3d7fa808895c8d2e41bb890af21c47e38c2460e0588147a4bb8fc658d';          BINARY_URL='https://github.com/adoptium/temurin11-binaries/releases/download/jdk-11.0.17%2B8/OpenJDK11U-jre_arm_linux_hotspot_11.0.17_8.tar.gz';          ;;        ppc64el|powerpc:common64)          ESUM='0ca3d806131ab5834c501f9c625bb0248cd528af361c704503348e9c9605bedf';          BINARY_URL='https://github.com/adoptium/temurin11-binaries/releases/download/jdk-11.0.17%2B8/OpenJDK11U-jre_ppc64le_linux_hotspot_11.0.17_8.tar.gz';          ;;        s390x|s390:64-bit)          ESUM='dd3b159a374086e65cb07c4ccb226c90f9c02ef929cba6f0b642171d7ed97fa4';          BINARY_URL='https://github.com/adoptium/temurin11-binaries/releases/download/jdk-11.0.17%2B8/OpenJDK11U-jre_s390x_linux_hotspot_11.0.17_8.tar.gz';          ;;        amd64|i386:x86-64)          ESUM='752616097e09d7f60a3ad8bd312f90eaf50ac72577e55df229fe6e8091148f79';          BINARY_URL='https://github.com/adoptium/temurin11-binaries/releases/download/jdk-11.0.17%2B8/OpenJDK11U-jre_x64_linux_hotspot_11.0.17_8.tar.gz';          ;;        *)          echo "Unsupported arch: ${ARCH}";          exit 1;          ;;     esac; 	  wget -O /tmp/openjdk.tar.gz ${BINARY_URL}; 	  echo "${ESUM} */tmp/openjdk.tar.gz" | sha256sum -c -; 	  mkdir -p "$JAVA_HOME"; 	  tar --extract 	      --file /tmp/openjdk.tar.gz 	      --directory "$JAVA_HOME" 	      --strip-components 1 	      --no-same-owner 	  ;     rm /tmp/openjdk.tar.gz;     find "$JAVA_HOME/lib" -name '*.so' -exec dirname '{}' ';' | sort -u > /etc/ld.so.conf.d/docker-openjdk.conf;     ldconfig;     java -Xshare:dump;
# Fri, 04 Nov 2022 23:22:32 GMT
RUN echo Verifying install ...     && fileEncoding="$(echo 'System.out.println(System.getProperty("file.encoding"))' | jshell -s -)"; [ "$fileEncoding" = 'UTF-8' ]; rm -rf ~/.java     && echo java --version && java --version     && echo Complete.
# Sat, 05 Nov 2022 01:35:16 GMT
ENV CATALINA_HOME=/usr/local/tomcat
# Sat, 05 Nov 2022 01:35:16 GMT
ENV PATH=/usr/local/tomcat/bin:/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Sat, 05 Nov 2022 01:35:17 GMT
RUN mkdir -p "$CATALINA_HOME"
# Sat, 05 Nov 2022 01:35:17 GMT
WORKDIR /usr/local/tomcat
# Sat, 05 Nov 2022 01:35:17 GMT
ENV TOMCAT_NATIVE_LIBDIR=/usr/local/tomcat/native-jni-lib
# Sat, 05 Nov 2022 01:35:17 GMT
ENV LD_LIBRARY_PATH=/usr/local/tomcat/native-jni-lib
# Sat, 05 Nov 2022 01:39:54 GMT
ENV GPG_KEYS=48F8E69F6390C9F25CFEDCD268248959359E722B A9C5DF4D22E99998D9875A5110C01C5A2F6059E7 DCFD35E0BF8CA7344752DE8B6FB21E8933C60243
# Sat, 05 Nov 2022 01:39:54 GMT
ENV TOMCAT_MAJOR=9
# Tue, 15 Nov 2022 03:06:43 GMT
ENV TOMCAT_VERSION=9.0.69
# Tue, 15 Nov 2022 03:06:43 GMT
ENV TOMCAT_SHA512=8c883c54ce9ce43eba37756a6404cdf3477879883a3e6d146dc8a7aa5e0425f487466afe6b6da4a895927cb7cb59177b9379cec18000f2de12785be57408c779
# Tue, 15 Nov 2022 03:06:44 GMT
COPY dir:b1a33aa3993dbbfbebb33bd9aa546b60c2f2191abf1227f453d4e830f6deb35f in /usr/local/tomcat 
# Tue, 15 Nov 2022 03:06:48 GMT
RUN set -eux; 	apt-get update; 	xargs -rt apt-get install -y --no-install-recommends < "$TOMCAT_NATIVE_LIBDIR/.dependencies.txt"; 	rm -rf /var/lib/apt/lists/*
# Tue, 15 Nov 2022 03:06:49 GMT
RUN set -eux; 	nativeLines="$(catalina.sh configtest 2>&1)"; 	nativeLines="$(echo "$nativeLines" | grep 'Apache Tomcat Native')"; 	nativeLines="$(echo "$nativeLines" | sort -u)"; 	if ! echo "$nativeLines" | grep -E 'INFO: Loaded( APR based)? Apache Tomcat Native library' >&2; then 		echo >&2 "$nativeLines"; 		exit 1; 	fi
# Tue, 15 Nov 2022 03:06:49 GMT
EXPOSE 8080
# Tue, 15 Nov 2022 03:06:49 GMT
CMD ["catalina.sh" "run"]
# Wed, 11 Jan 2023 02:47:03 GMT
LABEL org.opencontainers.image.authors=XWiki Development Team <committers@xwiki.org>
# Wed, 11 Jan 2023 02:47:03 GMT
LABEL org.opencontainers.image.url=https://hub.docker.com/_/xwiki
# Wed, 11 Jan 2023 02:47:03 GMT
LABEL org.opencontainers.image.documentation=https://hub.docker.com/_/xwiki
# Wed, 11 Jan 2023 02:47:03 GMT
LABEL org.opencontainers.image.source=https://github.com/xwiki/xwiki-docker.git
# Wed, 11 Jan 2023 02:47:04 GMT
LABEL org.opencontainers.image.vendor=xwiki.org
# Wed, 11 Jan 2023 02:47:04 GMT
LABEL org.opencontainers.image.licenses=LGPL-2.1
# Wed, 11 Jan 2023 02:50:25 GMT
RUN apt-get update &&   apt-get --no-install-recommends -y install     curl     libreoffice     unzip     procps     libpostgresql-jdbc-java &&   rm -rf /var/lib/apt/lists/*
# Wed, 22 Feb 2023 18:40:25 GMT
ENV XWIKI_VERSION=14.10.5
# Wed, 22 Feb 2023 18:40:25 GMT
ENV XWIKI_URL_PREFIX=https://maven.xwiki.org/releases/org/xwiki/platform/xwiki-platform-distribution-war/14.10.5
# Wed, 22 Feb 2023 18:40:25 GMT
ENV XWIKI_DOWNLOAD_SHA256=f58465d0869e4c5605ae8375a09c79399d1149c7131fed3cf9959918267eb6a8
# Wed, 22 Feb 2023 18:41:04 GMT
RUN rm -rf /usr/local/tomcat/webapps/* &&   mkdir -p /usr/local/tomcat/temp &&   mkdir -p /usr/local/xwiki/data &&   curl -fSL "${XWIKI_URL_PREFIX}/xwiki-platform-distribution-war-${XWIKI_VERSION}.war" -o xwiki.war &&   echo "$XWIKI_DOWNLOAD_SHA256 xwiki.war" | sha256sum -c - &&   unzip -d /usr/local/tomcat/webapps/ROOT xwiki.war &&   rm -f xwiki.war
# Wed, 22 Feb 2023 18:41:05 GMT
RUN cp /usr/share/java/postgresql-jdbc4.jar /usr/local/tomcat/webapps/ROOT/WEB-INF/lib/
# Wed, 22 Feb 2023 18:41:05 GMT
COPY file:0a1be11e2eb610a1dbcd415404e3a592641110b93090030cb831e3a19a163017 in /usr/local/tomcat/bin/ 
# Wed, 22 Feb 2023 18:41:05 GMT
COPY file:4a923f484bb29a26630c19e1d617d3bf6aa6ae7c6c4a5561e97b037bcde0847c in /usr/local/tomcat/webapps/ROOT/WEB-INF/hibernate.cfg.xml 
# Wed, 22 Feb 2023 18:41:06 GMT
RUN sed -i 's/<id>org.xwiki.platform:xwiki-platform-distribution-war/<id>org.xwiki.platform:xwiki-platform-distribution-docker/'   /usr/local/tomcat/webapps/ROOT/META-INF/extension.xed
# Wed, 22 Feb 2023 18:41:06 GMT
COPY file:a47c4dcd87c9dad97aff38c49188357e6193bcad50757e516cfb08a60d4de611 in /usr/local/bin/docker-entrypoint.sh 
# Wed, 22 Feb 2023 18:41:06 GMT
VOLUME [/usr/local/xwiki]
# Wed, 22 Feb 2023 18:41:06 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 22 Feb 2023 18:41:06 GMT
CMD ["xwiki"]
```

-	Layers:
	-	`sha256:e96e057aae67380a4ddb16c337c5c3669d97fdff69ec537f02aa2cc30d814281`  
		Last Modified: Wed, 02 Nov 2022 03:03:36 GMT  
		Size: 30.4 MB (30425607 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4ced2591451da3a02e2b6bb44752b9e3f00d77789921be4df5082fb9f9880ad0`  
		Last Modified: Wed, 02 Nov 2022 18:48:43 GMT  
		Size: 12.4 MB (12439006 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:df8f874ae8c08a9e69e5fbe6c5a64200a45386132a3203d1a9a7f1146d94cfbc`  
		Last Modified: Fri, 04 Nov 2022 23:29:33 GMT  
		Size: 46.6 MB (46629936 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:111b6c7486426c4b6989102c2ee5be856e8a58e20ab0a350b24a905d536e8e7f`  
		Last Modified: Fri, 04 Nov 2022 23:29:26 GMT  
		Size: 161.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e6f84dce457c6d4f7b7291fce05f8e77998a3a7722a54125a1f1d52ca83043b4`  
		Last Modified: Sat, 05 Nov 2022 01:50:51 GMT  
		Size: 173.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a6c26749ee782392e38845ee2ba79b0da586ef6a45d8e7f29c7af14612278547`  
		Last Modified: Tue, 15 Nov 2022 03:19:57 GMT  
		Size: 12.2 MB (12200249 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4dddc6d9fa6024025b3fcfe729cab2dc544fb25476eca6e80b1af8e8d93bb0ee`  
		Last Modified: Tue, 15 Nov 2022 03:19:56 GMT  
		Size: 452.7 KB (452680 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:06637eebe5e72c8ad9019ad4eb4cdde1f11f7d4c24c7ed7374cf8966343aa2fb`  
		Last Modified: Tue, 15 Nov 2022 03:19:56 GMT  
		Size: 131.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b57f6f8bcfb0d93b8e21d3068d1f65d3f08dba05c5fab7d4c36e2359317b18c7`  
		Last Modified: Wed, 11 Jan 2023 02:53:53 GMT  
		Size: 179.7 MB (179745182 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b26b00a2f6717a934b9a1b08bac612aaaf57a4cfb4d82db521e7d36755621933`  
		Last Modified: Wed, 22 Feb 2023 18:43:06 GMT  
		Size: 307.1 MB (307141251 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:11801aa48fd913e3278b4d0a512df366a8ef26c1cc3e95a8439a1be90aadfd5a`  
		Last Modified: Wed, 22 Feb 2023 18:42:50 GMT  
		Size: 936.9 KB (936850 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fb4e8755162307a316ff405759f2417dc77e746651f89c83a0477ab19dc7da5d`  
		Last Modified: Wed, 22 Feb 2023 18:42:50 GMT  
		Size: 1.3 KB (1342 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2ba124a3d49367a8e2f46fc2043189f91e2dd282d40a301d9c1f79a705d35e66`  
		Last Modified: Wed, 22 Feb 2023 18:42:50 GMT  
		Size: 2.5 KB (2450 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8f421201132c3966dbb37a473df5922718780304fa03993ef75bb78522d5cafd`  
		Last Modified: Wed, 22 Feb 2023 18:42:50 GMT  
		Size: 6.0 KB (6012 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1b5dc6b32b3d1d9a80058f5ffc684363a0cfadf60ade5875fa37854ec7b46fff`  
		Last Modified: Wed, 22 Feb 2023 18:42:50 GMT  
		Size: 2.5 KB (2502 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `xwiki:14-postgres-tomcat` - linux; arm64 variant v8

```console
$ docker pull xwiki@sha256:e04b6d052b479b648834e5d960deff2f28274834a9dc812b628ccb9a624c53ef
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **581.2 MB (581199952 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:4693188024e4d84ad63e783e3377e2d600a040c344f7f36ab1bff14f5630ffe7`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["xwiki"]`

```dockerfile
# Wed, 02 Nov 2022 18:49:40 GMT
ADD file:a934fb007525d0b56966a52a22ab22560bf48b6e09917f05324042129d4d894a in / 
# Wed, 02 Nov 2022 18:49:40 GMT
CMD ["bash"]
# Wed, 02 Nov 2022 19:44:20 GMT
ENV JAVA_HOME=/opt/java/openjdk
# Wed, 02 Nov 2022 19:44:20 GMT
ENV PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 02 Nov 2022 19:44:20 GMT
ENV LANG=en_US.UTF-8 LANGUAGE=en_US:en LC_ALL=en_US.UTF-8
# Wed, 02 Nov 2022 19:44:32 GMT
RUN apt-get update     && DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends tzdata curl wget ca-certificates fontconfig locales     && echo "en_US.UTF-8 UTF-8" >> /etc/locale.gen     && locale-gen en_US.UTF-8     && rm -rf /var/lib/apt/lists/*
# Fri, 04 Nov 2022 22:40:54 GMT
ENV JAVA_VERSION=jdk-11.0.17+8
# Fri, 04 Nov 2022 22:41:33 GMT
RUN set -eux;     ARCH="$(dpkg --print-architecture)";     case "${ARCH}" in        aarch64|arm64)          ESUM='bd6efe3290c8b5a42f695a55a26f3e3c9c284288574879d4b7089f31f5114177';          BINARY_URL='https://github.com/adoptium/temurin11-binaries/releases/download/jdk-11.0.17%2B8/OpenJDK11U-jre_aarch64_linux_hotspot_11.0.17_8.tar.gz';          ;;        armhf|arm)          ESUM='8cf113d3d7fa808895c8d2e41bb890af21c47e38c2460e0588147a4bb8fc658d';          BINARY_URL='https://github.com/adoptium/temurin11-binaries/releases/download/jdk-11.0.17%2B8/OpenJDK11U-jre_arm_linux_hotspot_11.0.17_8.tar.gz';          ;;        ppc64el|powerpc:common64)          ESUM='0ca3d806131ab5834c501f9c625bb0248cd528af361c704503348e9c9605bedf';          BINARY_URL='https://github.com/adoptium/temurin11-binaries/releases/download/jdk-11.0.17%2B8/OpenJDK11U-jre_ppc64le_linux_hotspot_11.0.17_8.tar.gz';          ;;        s390x|s390:64-bit)          ESUM='dd3b159a374086e65cb07c4ccb226c90f9c02ef929cba6f0b642171d7ed97fa4';          BINARY_URL='https://github.com/adoptium/temurin11-binaries/releases/download/jdk-11.0.17%2B8/OpenJDK11U-jre_s390x_linux_hotspot_11.0.17_8.tar.gz';          ;;        amd64|i386:x86-64)          ESUM='752616097e09d7f60a3ad8bd312f90eaf50ac72577e55df229fe6e8091148f79';          BINARY_URL='https://github.com/adoptium/temurin11-binaries/releases/download/jdk-11.0.17%2B8/OpenJDK11U-jre_x64_linux_hotspot_11.0.17_8.tar.gz';          ;;        *)          echo "Unsupported arch: ${ARCH}";          exit 1;          ;;     esac; 	  wget -O /tmp/openjdk.tar.gz ${BINARY_URL}; 	  echo "${ESUM} */tmp/openjdk.tar.gz" | sha256sum -c -; 	  mkdir -p "$JAVA_HOME"; 	  tar --extract 	      --file /tmp/openjdk.tar.gz 	      --directory "$JAVA_HOME" 	      --strip-components 1 	      --no-same-owner 	  ;     rm /tmp/openjdk.tar.gz;     find "$JAVA_HOME/lib" -name '*.so' -exec dirname '{}' ';' | sort -u > /etc/ld.so.conf.d/docker-openjdk.conf;     ldconfig;     java -Xshare:dump;
# Fri, 04 Nov 2022 22:41:34 GMT
RUN echo Verifying install ...     && fileEncoding="$(echo 'System.out.println(System.getProperty("file.encoding"))' | jshell -s -)"; [ "$fileEncoding" = 'UTF-8' ]; rm -rf ~/.java     && echo java --version && java --version     && echo Complete.
# Fri, 04 Nov 2022 23:48:38 GMT
ENV CATALINA_HOME=/usr/local/tomcat
# Fri, 04 Nov 2022 23:48:38 GMT
ENV PATH=/usr/local/tomcat/bin:/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Fri, 04 Nov 2022 23:48:38 GMT
RUN mkdir -p "$CATALINA_HOME"
# Fri, 04 Nov 2022 23:48:39 GMT
WORKDIR /usr/local/tomcat
# Fri, 04 Nov 2022 23:48:39 GMT
ENV TOMCAT_NATIVE_LIBDIR=/usr/local/tomcat/native-jni-lib
# Fri, 04 Nov 2022 23:48:39 GMT
ENV LD_LIBRARY_PATH=/usr/local/tomcat/native-jni-lib
# Fri, 04 Nov 2022 23:53:12 GMT
ENV GPG_KEYS=48F8E69F6390C9F25CFEDCD268248959359E722B A9C5DF4D22E99998D9875A5110C01C5A2F6059E7 DCFD35E0BF8CA7344752DE8B6FB21E8933C60243
# Fri, 04 Nov 2022 23:53:12 GMT
ENV TOMCAT_MAJOR=9
# Tue, 15 Nov 2022 04:57:22 GMT
ENV TOMCAT_VERSION=9.0.69
# Tue, 15 Nov 2022 04:57:22 GMT
ENV TOMCAT_SHA512=8c883c54ce9ce43eba37756a6404cdf3477879883a3e6d146dc8a7aa5e0425f487466afe6b6da4a895927cb7cb59177b9379cec18000f2de12785be57408c779
# Tue, 15 Nov 2022 04:57:22 GMT
COPY dir:096b403a5f78b17e6b4bff63128a9c93941b97f22470991610dd641633d977f1 in /usr/local/tomcat 
# Tue, 15 Nov 2022 04:57:25 GMT
RUN set -eux; 	apt-get update; 	xargs -rt apt-get install -y --no-install-recommends < "$TOMCAT_NATIVE_LIBDIR/.dependencies.txt"; 	rm -rf /var/lib/apt/lists/*
# Tue, 15 Nov 2022 04:57:26 GMT
RUN set -eux; 	nativeLines="$(catalina.sh configtest 2>&1)"; 	nativeLines="$(echo "$nativeLines" | grep 'Apache Tomcat Native')"; 	nativeLines="$(echo "$nativeLines" | sort -u)"; 	if ! echo "$nativeLines" | grep -E 'INFO: Loaded( APR based)? Apache Tomcat Native library' >&2; then 		echo >&2 "$nativeLines"; 		exit 1; 	fi
# Tue, 15 Nov 2022 04:57:26 GMT
EXPOSE 8080
# Tue, 15 Nov 2022 04:57:27 GMT
CMD ["catalina.sh" "run"]
# Wed, 11 Jan 2023 03:05:10 GMT
LABEL org.opencontainers.image.authors=XWiki Development Team <committers@xwiki.org>
# Wed, 11 Jan 2023 03:05:10 GMT
LABEL org.opencontainers.image.url=https://hub.docker.com/_/xwiki
# Wed, 11 Jan 2023 03:05:10 GMT
LABEL org.opencontainers.image.documentation=https://hub.docker.com/_/xwiki
# Wed, 11 Jan 2023 03:05:10 GMT
LABEL org.opencontainers.image.source=https://github.com/xwiki/xwiki-docker.git
# Wed, 11 Jan 2023 03:05:11 GMT
LABEL org.opencontainers.image.vendor=xwiki.org
# Wed, 11 Jan 2023 03:05:11 GMT
LABEL org.opencontainers.image.licenses=LGPL-2.1
# Wed, 11 Jan 2023 03:08:55 GMT
RUN apt-get update &&   apt-get --no-install-recommends -y install     curl     libreoffice     unzip     procps     libpostgresql-jdbc-java &&   rm -rf /var/lib/apt/lists/*
# Wed, 01 Feb 2023 22:27:07 GMT
ENV XWIKI_VERSION=14.10.4
# Wed, 01 Feb 2023 22:27:07 GMT
ENV XWIKI_URL_PREFIX=https://maven.xwiki.org/releases/org/xwiki/platform/xwiki-platform-distribution-war/14.10.4
# Wed, 01 Feb 2023 22:27:07 GMT
ENV XWIKI_DOWNLOAD_SHA256=2fcfb622319172c2e424b9c11848ebfabe27cf8ef69cba39ceb5d124b7ebe713
# Wed, 01 Feb 2023 22:27:47 GMT
RUN rm -rf /usr/local/tomcat/webapps/* &&   mkdir -p /usr/local/tomcat/temp &&   mkdir -p /usr/local/xwiki/data &&   curl -fSL "${XWIKI_URL_PREFIX}/xwiki-platform-distribution-war-${XWIKI_VERSION}.war" -o xwiki.war &&   echo "$XWIKI_DOWNLOAD_SHA256 xwiki.war" | sha256sum -c - &&   unzip -d /usr/local/tomcat/webapps/ROOT xwiki.war &&   rm -f xwiki.war
# Wed, 01 Feb 2023 22:27:50 GMT
RUN cp /usr/share/java/postgresql-jdbc4.jar /usr/local/tomcat/webapps/ROOT/WEB-INF/lib/
# Wed, 01 Feb 2023 22:27:50 GMT
COPY file:0a1be11e2eb610a1dbcd415404e3a592641110b93090030cb831e3a19a163017 in /usr/local/tomcat/bin/ 
# Wed, 01 Feb 2023 22:27:50 GMT
COPY file:4a923f484bb29a26630c19e1d617d3bf6aa6ae7c6c4a5561e97b037bcde0847c in /usr/local/tomcat/webapps/ROOT/WEB-INF/hibernate.cfg.xml 
# Wed, 01 Feb 2023 22:27:50 GMT
RUN sed -i 's/<id>org.xwiki.platform:xwiki-platform-distribution-war/<id>org.xwiki.platform:xwiki-platform-distribution-docker/'   /usr/local/tomcat/webapps/ROOT/META-INF/extension.xed
# Wed, 01 Feb 2023 22:27:50 GMT
COPY file:a47c4dcd87c9dad97aff38c49188357e6193bcad50757e516cfb08a60d4de611 in /usr/local/bin/docker-entrypoint.sh 
# Wed, 01 Feb 2023 22:27:50 GMT
VOLUME [/usr/local/xwiki]
# Wed, 01 Feb 2023 22:27:51 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 01 Feb 2023 22:27:51 GMT
CMD ["xwiki"]
```

-	Layers:
	-	`sha256:0509fae36eb0656f8bdb23f8ae64100d893bcea2563e97468d337e04d2d0410b`  
		Last Modified: Wed, 02 Nov 2022 18:50:21 GMT  
		Size: 28.4 MB (28382154 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e502a1af2bcd98f5f0d2f5e4da1a0e7bbe07a2c548e2662f7d37dce5ae1df46c`  
		Last Modified: Wed, 02 Nov 2022 19:48:28 GMT  
		Size: 12.4 MB (12396330 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bc4598c07dd818f03a0378b0341a4a8e80f0152fbb3e7d5246ca4f466f42e611`  
		Last Modified: Fri, 04 Nov 2022 22:46:46 GMT  
		Size: 45.0 MB (44958470 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:715a937a1066f998b331fcd62256ad01a5571bdf46804e97825afc64f9ebb427`  
		Last Modified: Fri, 04 Nov 2022 22:46:41 GMT  
		Size: 160.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5fb623f082f74b2fa9fc2c4e3f3a4802875cb9753cfa26ed940201ce72bb56cb`  
		Last Modified: Sat, 05 Nov 2022 00:03:40 GMT  
		Size: 172.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:33260b83200262bbd546be371ad3c1f50f5ae7228afb87982d6fa9d6b11bf26f`  
		Last Modified: Tue, 15 Nov 2022 05:10:19 GMT  
		Size: 12.2 MB (12207235 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0955fb697ea9b30a1b4f95385464f646aa1525cb6efba648e22df84ebef6b2ee`  
		Last Modified: Tue, 15 Nov 2022 05:10:18 GMT  
		Size: 452.0 KB (452021 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6eddcf66f2083b1487296a0308e0b058917c97f614f12428d82d89662038dc2e`  
		Last Modified: Tue, 15 Nov 2022 05:10:18 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1ae6a8fce0f2cd131007393c1a4eba9ce9d0501da8406af5c5ce9deb5dc187b8`  
		Last Modified: Wed, 11 Jan 2023 03:12:13 GMT  
		Size: 174.7 MB (174749274 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:64fdf9e1ef0289a65afb558897bc408557b353c604c9e3bd5dfe845ddc54ab93`  
		Last Modified: Wed, 01 Feb 2023 22:30:00 GMT  
		Size: 307.1 MB (307104835 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0eee07814c2c9ef72478213f8e0091378d617e777e157e5f5550dbf992e4a8bb`  
		Last Modified: Wed, 01 Feb 2023 22:29:45 GMT  
		Size: 936.9 KB (936853 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:889aa9ab03d69382e94096e25991f58b06afde5b4238b94ac1136db5337d1028`  
		Last Modified: Wed, 01 Feb 2023 22:29:45 GMT  
		Size: 1.3 KB (1347 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d0d21fec462339352953dc0188b312a1e80154e3e38402e546f0e4200627f5dc`  
		Last Modified: Wed, 01 Feb 2023 22:29:45 GMT  
		Size: 2.5 KB (2455 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9c6493af5a9b0ca2b189b7be35d0f796b0243ab70d7f92a34a7eae40d269c8f3`  
		Last Modified: Wed, 01 Feb 2023 22:29:45 GMT  
		Size: 6.0 KB (6011 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3a5f6da30b6a4dcd443e582890b4a323952b0320b4c3474d31c01236b8f4cf5e`  
		Last Modified: Wed, 01 Feb 2023 22:29:45 GMT  
		Size: 2.5 KB (2506 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
