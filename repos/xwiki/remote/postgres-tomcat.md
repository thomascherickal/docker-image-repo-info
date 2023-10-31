## `xwiki:postgres-tomcat`

```console
$ docker pull xwiki@sha256:c044ea93ee88fe3aed33d6d3c7462db7558193d7fc2872fa9511c53beefede62
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `xwiki:postgres-tomcat` - linux; amd64

```console
$ docker pull xwiki@sha256:cda88ef14e32fb718519a355fef9ba387358af8afb5cf07b7e37ff62c575312f
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **591.7 MB (591745576 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:2e2834c96b3e05b70e71b49888829d95a03256cdcc3f63c5e99a8eb72308c809`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["xwiki"]`

```dockerfile
# Thu, 05 Oct 2023 07:33:30 GMT
ARG RELEASE
# Thu, 05 Oct 2023 07:33:30 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Thu, 05 Oct 2023 07:33:30 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Thu, 05 Oct 2023 07:33:30 GMT
LABEL org.opencontainers.image.version=22.04
# Thu, 05 Oct 2023 07:33:32 GMT
ADD file:63d5ab3ef0aab308c0e71cb67292c5467f60deafa9b0418cbb220affcd078444 in / 
# Thu, 05 Oct 2023 07:33:32 GMT
CMD ["/bin/bash"]
# Fri, 13 Oct 2023 05:51:05 GMT
ENV JAVA_HOME=/opt/java/openjdk
# Fri, 13 Oct 2023 05:51:05 GMT
ENV PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Fri, 13 Oct 2023 05:51:05 GMT
ENV LANG=en_US.UTF-8 LANGUAGE=en_US:en LC_ALL=en_US.UTF-8
# Fri, 13 Oct 2023 05:51:27 GMT
RUN apt-get update     && DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends tzdata curl wget ca-certificates fontconfig locales p11-kit     && echo "en_US.UTF-8 UTF-8" >> /etc/locale.gen     && locale-gen en_US.UTF-8     && rm -rf /var/lib/apt/lists/*
# Fri, 13 Oct 2023 05:52:21 GMT
ENV JAVA_VERSION=jdk-11.0.20.1+1
# Fri, 13 Oct 2023 05:52:54 GMT
RUN set -eux;     ARCH="$(dpkg --print-architecture)";     case "${ARCH}" in        aarch64|arm64)          ESUM='0f69f5c05cb7fb2804be3735ed31ce92acff1a51ef29be544b89f83c90d2ea2a';          BINARY_URL='https://github.com/adoptium/temurin11-binaries/releases/download/jdk-11.0.20.1%2B1/OpenJDK11U-jre_aarch64_linux_hotspot_11.0.20.1_1.tar.gz';          ;;        armhf|arm)          ESUM='2fc1cc935897312c0bc2515b2e7ea1fa3b267e77305a1b51a8c3917d92af380f';          BINARY_URL='https://github.com/adoptium/temurin11-binaries/releases/download/jdk-11.0.20.1%2B1/OpenJDK11U-jre_arm_linux_hotspot_11.0.20.1_1.tar.gz';          ;;        ppc64el|powerpc:common64)          ESUM='7963580e5c3abe55e6b9d2297f2e2cde7b227d28204497bec5f17bb37762c7b7';          BINARY_URL='https://github.com/adoptium/temurin11-binaries/releases/download/jdk-11.0.20.1%2B1/OpenJDK11U-jre_ppc64le_linux_hotspot_11.0.20.1_1.tar.gz';          ;;        s390x|s390:64-bit)          ESUM='cf7fa0f0291687ebcb5f87f5db3a8d94525fd65832adc636c4c6e1f3174d9997';          BINARY_URL='https://github.com/adoptium/temurin11-binaries/releases/download/jdk-11.0.20.1%2B1/OpenJDK11U-jre_s390x_linux_hotspot_11.0.20.1_1.tar.gz';          ;;        amd64|i386:x86-64)          ESUM='bc6ed047e50b09611b419c878e4ea3ea36594bd79f64001a5b53decf72669d33';          BINARY_URL='https://github.com/adoptium/temurin11-binaries/releases/download/jdk-11.0.20.1%2B1/OpenJDK11U-jre_x64_linux_hotspot_11.0.20.1_1.tar.gz';          ;;        *)          echo "Unsupported arch: ${ARCH}";          exit 1;          ;;     esac; 	  wget -O /tmp/openjdk.tar.gz ${BINARY_URL}; 	  echo "${ESUM} */tmp/openjdk.tar.gz" | sha256sum -c -; 	  mkdir -p "$JAVA_HOME"; 	  tar --extract 	      --file /tmp/openjdk.tar.gz 	      --directory "$JAVA_HOME" 	      --strip-components 1 	      --no-same-owner 	  ;     rm -f /tmp/openjdk.tar.gz ${JAVA_HOME}/lib/src.zip;     find "$JAVA_HOME/lib" -name '*.so' -exec dirname '{}' ';' | sort -u > /etc/ld.so.conf.d/docker-openjdk.conf;     ldconfig;     java -Xshare:dump;
# Fri, 13 Oct 2023 05:52:55 GMT
RUN echo Verifying install ...     && fileEncoding="$(echo 'System.out.println(System.getProperty("file.encoding"))' | jshell -s -)"; [ "$fileEncoding" = 'UTF-8' ]; rm -rf ~/.java     && echo java --version && java --version     && echo Complete.
# Fri, 13 Oct 2023 05:52:55 GMT
COPY file:8b8864b3e02a33a579dc216fd51b28a6047bc8eeaa03045b258980fe0cf7fcb3 in /__cacert_entrypoint.sh 
# Fri, 13 Oct 2023 05:52:55 GMT
ENTRYPOINT ["/__cacert_entrypoint.sh"]
# Fri, 13 Oct 2023 10:28:19 GMT
ENV CATALINA_HOME=/usr/local/tomcat
# Fri, 13 Oct 2023 10:28:19 GMT
ENV PATH=/usr/local/tomcat/bin:/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Fri, 13 Oct 2023 10:28:20 GMT
RUN mkdir -p "$CATALINA_HOME"
# Fri, 13 Oct 2023 10:28:20 GMT
WORKDIR /usr/local/tomcat
# Fri, 13 Oct 2023 10:28:20 GMT
ENV TOMCAT_NATIVE_LIBDIR=/usr/local/tomcat/native-jni-lib
# Fri, 13 Oct 2023 10:28:20 GMT
ENV LD_LIBRARY_PATH=/usr/local/tomcat/native-jni-lib
# Fri, 13 Oct 2023 10:32:29 GMT
ENV GPG_KEYS=48F8E69F6390C9F25CFEDCD268248959359E722B A9C5DF4D22E99998D9875A5110C01C5A2F6059E7 DCFD35E0BF8CA7344752DE8B6FB21E8933C60243
# Fri, 13 Oct 2023 10:32:29 GMT
ENV TOMCAT_MAJOR=9
# Sat, 14 Oct 2023 02:47:32 GMT
ENV TOMCAT_VERSION=9.0.82
# Sat, 14 Oct 2023 02:47:32 GMT
ENV TOMCAT_SHA512=2b13f11f4e0d0b9aee667c256c6ea5d2853b067e8b7e8293f117da050d3833fda8aa9d9ad278bd12fb7fbf0825108c7d0384509f44c05f9bad73eb099cfaa128
# Sat, 14 Oct 2023 02:47:33 GMT
COPY dir:fb96ce348250e086bf106fe9d5484733fa12ed9333dc7b58a5cb6c24e9b2d83b in /usr/local/tomcat 
# Sat, 14 Oct 2023 02:47:38 GMT
RUN set -eux; 	apt-get update; 	xargs -rt apt-get install -y --no-install-recommends < "$TOMCAT_NATIVE_LIBDIR/.dependencies.txt"; 	rm -rf /var/lib/apt/lists/*
# Sat, 14 Oct 2023 02:47:39 GMT
RUN set -eux; 	nativeLines="$(catalina.sh configtest 2>&1)"; 	nativeLines="$(echo "$nativeLines" | grep 'Apache Tomcat Native')"; 	nativeLines="$(echo "$nativeLines" | sort -u)"; 	if ! echo "$nativeLines" | grep -E 'INFO: Loaded( APR based)? Apache Tomcat Native library' >&2; then 		echo >&2 "$nativeLines"; 		exit 1; 	fi
# Sat, 14 Oct 2023 02:47:39 GMT
EXPOSE 8080
# Sat, 14 Oct 2023 02:47:39 GMT
ENTRYPOINT []
# Sat, 14 Oct 2023 02:47:39 GMT
CMD ["catalina.sh" "run"]
# Sat, 14 Oct 2023 03:45:28 GMT
LABEL org.opencontainers.image.authors=XWiki Development Team <committers@xwiki.org>
# Sat, 14 Oct 2023 03:45:28 GMT
LABEL org.opencontainers.image.url=https://hub.docker.com/_/xwiki
# Sat, 14 Oct 2023 03:45:28 GMT
LABEL org.opencontainers.image.documentation=https://hub.docker.com/_/xwiki
# Sat, 14 Oct 2023 03:45:28 GMT
LABEL org.opencontainers.image.source=https://github.com/xwiki/xwiki-docker.git
# Sat, 14 Oct 2023 03:45:28 GMT
LABEL org.opencontainers.image.vendor=xwiki.org
# Sat, 14 Oct 2023 03:45:28 GMT
LABEL org.opencontainers.image.licenses=LGPL-2.1
# Sat, 14 Oct 2023 03:47:48 GMT
RUN apt-get update &&   apt-get --no-install-recommends -y install     curl     libreoffice     unzip     procps     libpostgresql-jdbc-java &&   rm -rf /var/lib/apt/lists/*
# Sat, 14 Oct 2023 03:47:49 GMT
ENV XWIKI_VERSION=15.8
# Sat, 14 Oct 2023 03:47:49 GMT
ENV XWIKI_URL_PREFIX=https://maven.xwiki.org/releases/org/xwiki/platform/xwiki-platform-distribution-war/15.8
# Sat, 14 Oct 2023 03:47:49 GMT
ENV XWIKI_DOWNLOAD_SHA256=359e44485615722ab533559ec3e3334197a10935e4dfa6fc872b93d1447475fc
# Sat, 14 Oct 2023 03:48:28 GMT
RUN rm -rf /usr/local/tomcat/webapps/* &&   mkdir -p /usr/local/tomcat/temp &&   mkdir -p /usr/local/xwiki/data &&   curl -fSL "${XWIKI_URL_PREFIX}/xwiki-platform-distribution-war-${XWIKI_VERSION}.war" -o xwiki.war &&   echo "$XWIKI_DOWNLOAD_SHA256 xwiki.war" | sha256sum -c - &&   unzip -d /usr/local/tomcat/webapps/ROOT xwiki.war &&   rm -f xwiki.war
# Sat, 14 Oct 2023 03:48:29 GMT
RUN cp /usr/share/java/postgresql-jdbc4.jar /usr/local/tomcat/webapps/ROOT/WEB-INF/lib/
# Sat, 14 Oct 2023 03:48:29 GMT
COPY file:0a1be11e2eb610a1dbcd415404e3a592641110b93090030cb831e3a19a163017 in /usr/local/tomcat/bin/ 
# Sat, 14 Oct 2023 03:48:29 GMT
COPY file:4a923f484bb29a26630c19e1d617d3bf6aa6ae7c6c4a5561e97b037bcde0847c in /usr/local/tomcat/webapps/ROOT/WEB-INF/hibernate.cfg.xml 
# Sat, 14 Oct 2023 03:48:30 GMT
RUN sed -i 's/<id>org.xwiki.platform:xwiki-platform-distribution-war/<id>org.xwiki.platform:xwiki-platform-distribution-docker/'   /usr/local/tomcat/webapps/ROOT/META-INF/extension.xed
# Sat, 14 Oct 2023 03:48:30 GMT
COPY file:a47c4dcd87c9dad97aff38c49188357e6193bcad50757e516cfb08a60d4de611 in /usr/local/bin/docker-entrypoint.sh 
# Sat, 14 Oct 2023 03:48:30 GMT
VOLUME [/usr/local/xwiki]
# Sat, 14 Oct 2023 03:48:30 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Sat, 14 Oct 2023 03:48:30 GMT
CMD ["xwiki"]
```

-	Layers:
	-	`sha256:43f89b94cd7df92a2f7e565b8fb1b7f502eff2cd225508cbd7ea2d36a9a3a601`  
		Last Modified: Thu, 05 Oct 2023 08:42:10 GMT  
		Size: 30.4 MB (30439111 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:39769250f2be0be25f38285d2996eb4dcbdfaddd7ad6c025b98e2fc2d955a973`  
		Last Modified: Fri, 13 Oct 2023 05:56:41 GMT  
		Size: 12.9 MB (12902386 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:82babd302d33d75c4fedb65bb3d20e34411c7f99bc5588475ff6e66e29953a58`  
		Last Modified: Fri, 13 Oct 2023 05:58:44 GMT  
		Size: 46.9 MB (46864502 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a249d4c681b877f3d4a8b17450e476f499c02a18a640cfc0b10e03a26a597ff3`  
		Last Modified: Fri, 13 Oct 2023 05:58:37 GMT  
		Size: 159.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:72d9be105ba94f2bf9de6e30a7b00993eaebc8a491e4288166ec8763be2af594`  
		Last Modified: Fri, 13 Oct 2023 05:58:37 GMT  
		Size: 734.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6d70fc3226fa72202d161a322f1806e6e2ce4bf44b14e9fd002adef27e5f13bd`  
		Last Modified: Fri, 13 Oct 2023 10:47:39 GMT  
		Size: 172.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bda06be904e3470636fa156b851a7459c8e1f8bcc10216c3599862dad9d09b83`  
		Last Modified: Sat, 14 Oct 2023 02:59:11 GMT  
		Size: 12.3 MB (12315379 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:80a3860110177dd34fbf44aa862baff927f5c4ead212f9ff169e384ed6083fa2`  
		Last Modified: Sat, 14 Oct 2023 02:59:10 GMT  
		Size: 455.5 KB (455499 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:09933162e202e3d566dcb5dea8127603893cee815abb27ce4137e3f30f7cc048`  
		Last Modified: Sat, 14 Oct 2023 02:59:10 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:355d5f1d147463386854d04ad1ed35522909606359ae0dc3626723eee47fd88c`  
		Last Modified: Sat, 14 Oct 2023 03:54:13 GMT  
		Size: 179.3 MB (179295359 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6098d26f9fc6864aa3f149f13eb096240e01130a98d33c012c05fbeac8766e8f`  
		Last Modified: Sat, 14 Oct 2023 03:54:11 GMT  
		Size: 308.5 MB (308522691 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:868944f7fdefa6dfdde623657984fb581dad32eee9638676323933ea81c997f3`  
		Last Modified: Sat, 14 Oct 2023 03:53:49 GMT  
		Size: 936.8 KB (936846 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ac6a465b4b1fa8ffc7943790cc9f0ac9b87f7eebe5fed3bd1d75559d896b9cba`  
		Last Modified: Sat, 14 Oct 2023 03:53:49 GMT  
		Size: 1.3 KB (1341 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fe7698ff2bd9cc126c61cf5fb6439869f86b5004b9a242640f763146b8c97eb1`  
		Last Modified: Sat, 14 Oct 2023 03:53:49 GMT  
		Size: 2.4 KB (2448 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c14e560a0447ab596cc3401e367c0394e9e3530a2db1fb48585bb32ed75db542`  
		Last Modified: Sat, 14 Oct 2023 03:53:49 GMT  
		Size: 6.3 KB (6315 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ca69b927d3e41d6b0297b9189fa9d30849fe50f0d034a25472ab9c55428db219`  
		Last Modified: Sat, 14 Oct 2023 03:53:49 GMT  
		Size: 2.5 KB (2505 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `xwiki:postgres-tomcat` - linux; arm64 variant v8

```console
$ docker pull xwiki@sha256:9addf4fbfc740278247f9c54b0f7ccdc83e0aca0316aa147eef8dfc85fd05cf4
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **585.6 MB (585575238 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:9d6fc318bb90a39c50164d85811f9ea796714128574544ff325d1f9e8136cd29`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["xwiki"]`

```dockerfile
# Thu, 05 Oct 2023 07:32:20 GMT
ARG RELEASE
# Thu, 05 Oct 2023 07:32:21 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Thu, 05 Oct 2023 07:32:21 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Thu, 05 Oct 2023 07:32:21 GMT
LABEL org.opencontainers.image.version=22.04
# Thu, 05 Oct 2023 07:32:22 GMT
ADD file:f8594e26831508c318e42c8dfd9942041031087b8de1bf3fec11fd75b8b30fd4 in / 
# Thu, 05 Oct 2023 07:32:22 GMT
CMD ["/bin/bash"]
# Fri, 13 Oct 2023 02:46:31 GMT
ENV JAVA_HOME=/opt/java/openjdk
# Fri, 13 Oct 2023 02:46:31 GMT
ENV PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Fri, 13 Oct 2023 02:46:31 GMT
ENV LANG=en_US.UTF-8 LANGUAGE=en_US:en LC_ALL=en_US.UTF-8
# Mon, 30 Oct 2023 23:41:33 GMT
RUN set -eux;     apt-get update;     DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends         curl         wget         fontconfig         ca-certificates p11-kit         tzdata         locales     ;     echo "en_US.UTF-8 UTF-8" >> /etc/locale.gen;     locale-gen en_US.UTF-8;     rm -rf /var/lib/apt/lists/*
# Mon, 30 Oct 2023 23:41:33 GMT
ENV JAVA_VERSION=jdk-11.0.21+9
# Mon, 30 Oct 2023 23:43:00 GMT
RUN set -eux;     ARCH="$(dpkg --print-architecture)";     case "${ARCH}" in        aarch64|arm64)          ESUM='8dc527e5c5da62f80ad3b6a2cd7b1789f745b1d90d5e83faba45f7a1d0b6cab8';          BINARY_URL='https://github.com/adoptium/temurin11-binaries/releases/download/jdk-11.0.21%2B9/OpenJDK11U-jre_aarch64_linux_hotspot_11.0.21_9.tar.gz';          ;;        amd64|i386:x86-64)          ESUM='156861bb901ef18759e05f6f008595220c7d1318a46758531b957b0c950ef2c3';          BINARY_URL='https://github.com/adoptium/temurin11-binaries/releases/download/jdk-11.0.21%2B9/OpenJDK11U-jre_x64_linux_hotspot_11.0.21_9.tar.gz';          ;;        armhf|arm)          ESUM='7c12ca8f195bf719368016a1c3e7f06f8f06e4a573dc3dce0befbe30a388ffa3';          BINARY_URL='https://github.com/adoptium/temurin11-binaries/releases/download/jdk-11.0.21%2B9/OpenJDK11U-jre_arm_linux_hotspot_11.0.21_9.tar.gz';          ;;        ppc64el|powerpc:common64)          ESUM='286e37ce06316185377eea847d2aa9f1523b9f1428684e59e772f2f6055e89b9';          BINARY_URL='https://github.com/adoptium/temurin11-binaries/releases/download/jdk-11.0.21%2B9/OpenJDK11U-jre_ppc64le_linux_hotspot_11.0.21_9.tar.gz';          ;;        s390x|s390:64-bit)          ESUM='78f18503970715c03b8e6e70191d9001c883edab23d9f51ff434e4a03c6237bd';          BINARY_URL='https://github.com/adoptium/temurin11-binaries/releases/download/jdk-11.0.21%2B9/OpenJDK11U-jre_s390x_linux_hotspot_11.0.21_9.tar.gz';          ;;        *)          echo "Unsupported arch: ${ARCH}";          exit 1;          ;;     esac;     wget --progress=dot:giga -O /tmp/openjdk.tar.gz ${BINARY_URL};     echo "${ESUM} */tmp/openjdk.tar.gz" | sha256sum -c -;     mkdir -p "$JAVA_HOME";     tar --extract         --file /tmp/openjdk.tar.gz         --directory "$JAVA_HOME"         --strip-components 1         --no-same-owner     ;     rm -f /tmp/openjdk.tar.gz ${JAVA_HOME}/lib/src.zip;     find "$JAVA_HOME/lib" -name '*.so' -exec dirname '{}' ';' | sort -u > /etc/ld.so.conf.d/docker-openjdk.conf;     ldconfig;     java -Xshare:dump;
# Mon, 30 Oct 2023 23:43:01 GMT
RUN set -eux;     echo "Verifying install ...";     echo "java --version"; java --version;     echo "Complete."
# Mon, 30 Oct 2023 23:43:01 GMT
COPY file:8b8864b3e02a33a579dc216fd51b28a6047bc8eeaa03045b258980fe0cf7fcb3 in /__cacert_entrypoint.sh 
# Mon, 30 Oct 2023 23:43:01 GMT
ENTRYPOINT ["/__cacert_entrypoint.sh"]
# Tue, 31 Oct 2023 02:56:56 GMT
ENV CATALINA_HOME=/usr/local/tomcat
# Tue, 31 Oct 2023 02:56:57 GMT
ENV PATH=/usr/local/tomcat/bin:/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 31 Oct 2023 02:56:57 GMT
RUN mkdir -p "$CATALINA_HOME"
# Tue, 31 Oct 2023 02:56:57 GMT
WORKDIR /usr/local/tomcat
# Tue, 31 Oct 2023 02:56:57 GMT
ENV TOMCAT_NATIVE_LIBDIR=/usr/local/tomcat/native-jni-lib
# Tue, 31 Oct 2023 02:56:57 GMT
ENV LD_LIBRARY_PATH=/usr/local/tomcat/native-jni-lib
# Tue, 31 Oct 2023 03:00:06 GMT
ENV GPG_KEYS=48F8E69F6390C9F25CFEDCD268248959359E722B A9C5DF4D22E99998D9875A5110C01C5A2F6059E7 DCFD35E0BF8CA7344752DE8B6FB21E8933C60243
# Tue, 31 Oct 2023 03:00:06 GMT
ENV TOMCAT_MAJOR=9
# Tue, 31 Oct 2023 03:00:06 GMT
ENV TOMCAT_VERSION=9.0.82
# Tue, 31 Oct 2023 03:00:06 GMT
ENV TOMCAT_SHA512=2b13f11f4e0d0b9aee667c256c6ea5d2853b067e8b7e8293f117da050d3833fda8aa9d9ad278bd12fb7fbf0825108c7d0384509f44c05f9bad73eb099cfaa128
# Tue, 31 Oct 2023 03:00:06 GMT
COPY dir:8754492acebcfe4fe04b0583bac4d3d93afaa6139254eaf140e87831c5de5fae in /usr/local/tomcat 
# Tue, 31 Oct 2023 03:00:10 GMT
RUN set -eux; 	apt-get update; 	xargs -rt apt-get install -y --no-install-recommends < "$TOMCAT_NATIVE_LIBDIR/.dependencies.txt"; 	rm -rf /var/lib/apt/lists/*
# Tue, 31 Oct 2023 03:00:11 GMT
RUN set -eux; 	nativeLines="$(catalina.sh configtest 2>&1)"; 	nativeLines="$(echo "$nativeLines" | grep 'Apache Tomcat Native')"; 	nativeLines="$(echo "$nativeLines" | sort -u)"; 	if ! echo "$nativeLines" | grep -E 'INFO: Loaded( APR based)? Apache Tomcat Native library' >&2; then 		echo >&2 "$nativeLines"; 		exit 1; 	fi
# Tue, 31 Oct 2023 03:00:11 GMT
EXPOSE 8080
# Tue, 31 Oct 2023 03:00:11 GMT
ENTRYPOINT []
# Tue, 31 Oct 2023 03:00:11 GMT
CMD ["catalina.sh" "run"]
# Tue, 31 Oct 2023 04:24:28 GMT
LABEL org.opencontainers.image.authors=XWiki Development Team <committers@xwiki.org>
# Tue, 31 Oct 2023 04:24:29 GMT
LABEL org.opencontainers.image.url=https://hub.docker.com/_/xwiki
# Tue, 31 Oct 2023 04:24:29 GMT
LABEL org.opencontainers.image.documentation=https://hub.docker.com/_/xwiki
# Tue, 31 Oct 2023 04:24:29 GMT
LABEL org.opencontainers.image.source=https://github.com/xwiki/xwiki-docker.git
# Tue, 31 Oct 2023 04:24:29 GMT
LABEL org.opencontainers.image.vendor=xwiki.org
# Tue, 31 Oct 2023 04:24:29 GMT
LABEL org.opencontainers.image.licenses=LGPL-2.1
# Tue, 31 Oct 2023 04:28:14 GMT
RUN apt-get update &&   apt-get --no-install-recommends -y install     curl     libreoffice     unzip     procps     libpostgresql-jdbc-java &&   rm -rf /var/lib/apt/lists/*
# Tue, 31 Oct 2023 04:28:17 GMT
ENV XWIKI_VERSION=15.8
# Tue, 31 Oct 2023 04:28:17 GMT
ENV XWIKI_URL_PREFIX=https://maven.xwiki.org/releases/org/xwiki/platform/xwiki-platform-distribution-war/15.8
# Tue, 31 Oct 2023 04:28:17 GMT
ENV XWIKI_DOWNLOAD_SHA256=359e44485615722ab533559ec3e3334197a10935e4dfa6fc872b93d1447475fc
# Tue, 31 Oct 2023 04:28:59 GMT
RUN rm -rf /usr/local/tomcat/webapps/* &&   mkdir -p /usr/local/tomcat/temp &&   mkdir -p /usr/local/xwiki/data &&   curl -fSL "${XWIKI_URL_PREFIX}/xwiki-platform-distribution-war-${XWIKI_VERSION}.war" -o xwiki.war &&   echo "$XWIKI_DOWNLOAD_SHA256 xwiki.war" | sha256sum -c - &&   unzip -d /usr/local/tomcat/webapps/ROOT xwiki.war &&   rm -f xwiki.war
# Tue, 31 Oct 2023 04:29:02 GMT
RUN cp /usr/share/java/postgresql-jdbc4.jar /usr/local/tomcat/webapps/ROOT/WEB-INF/lib/
# Tue, 31 Oct 2023 04:29:02 GMT
COPY file:0a1be11e2eb610a1dbcd415404e3a592641110b93090030cb831e3a19a163017 in /usr/local/tomcat/bin/ 
# Tue, 31 Oct 2023 04:29:02 GMT
COPY file:4a923f484bb29a26630c19e1d617d3bf6aa6ae7c6c4a5561e97b037bcde0847c in /usr/local/tomcat/webapps/ROOT/WEB-INF/hibernate.cfg.xml 
# Tue, 31 Oct 2023 04:29:02 GMT
RUN sed -i 's/<id>org.xwiki.platform:xwiki-platform-distribution-war/<id>org.xwiki.platform:xwiki-platform-distribution-docker/'   /usr/local/tomcat/webapps/ROOT/META-INF/extension.xed
# Tue, 31 Oct 2023 04:29:02 GMT
COPY file:a47c4dcd87c9dad97aff38c49188357e6193bcad50757e516cfb08a60d4de611 in /usr/local/bin/docker-entrypoint.sh 
# Tue, 31 Oct 2023 04:29:02 GMT
VOLUME [/usr/local/xwiki]
# Tue, 31 Oct 2023 04:29:03 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 31 Oct 2023 04:29:03 GMT
CMD ["xwiki"]
```

-	Layers:
	-	`sha256:895d322e8e5957c04af3ab7b3431f2a562182d34167c6e159e02044150a66967`  
		Last Modified: Thu, 05 Oct 2023 08:57:30 GMT  
		Size: 28.4 MB (28391939 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4035bfa3ea28e4a939fa769d2862227b94b4b5b961f65ac5df2ea3df7a0c51e4`  
		Last Modified: Mon, 30 Oct 2023 23:48:25 GMT  
		Size: 12.8 MB (12843579 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:44426d62154b920edc46b4f9c3d95ead5cff773239ebb0640ed78a3eabd75d3d`  
		Last Modified: Mon, 30 Oct 2023 23:49:42 GMT  
		Size: 45.4 MB (45399290 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a5b0a8b8196635efd1dce5dd763022df6a147662cd3aa1dcff312442551fce3d`  
		Last Modified: Mon, 30 Oct 2023 23:49:37 GMT  
		Size: 159.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:deeea1065ab43308ab77465a15be2c3e434488174fb1da412ee0e1f868c0ea93`  
		Last Modified: Mon, 30 Oct 2023 23:49:37 GMT  
		Size: 732.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:63f94ea910cb3af1fe712475caf27c4ff01461027655150f4c642120033d2267`  
		Last Modified: Tue, 31 Oct 2023 03:10:49 GMT  
		Size: 170.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d8a8008513efd39a0f4ccee25576aba434caaac1336e6f5de140e6e098c06e61`  
		Last Modified: Tue, 31 Oct 2023 03:14:04 GMT  
		Size: 12.3 MB (12323862 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f5d1140858fb04f2435d7c00d473576f8aa86d828d1746d2c7a1cd2db4ff68e2`  
		Last Modified: Tue, 31 Oct 2023 03:14:03 GMT  
		Size: 2.8 MB (2810137 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8a24a2f4303583c442267a0085b344ca1c142e3c1002b540c0661244a397ec58`  
		Last Modified: Tue, 31 Oct 2023 03:14:03 GMT  
		Size: 130.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1916479ef3f5430044e711b7aeaed2061664dd26c0804d18806385735439eac1`  
		Last Modified: Tue, 31 Oct 2023 04:34:29 GMT  
		Size: 174.3 MB (174333074 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:95dd16bc7e9b0c890cac616b7cca862760653e578ac5f0ea0f820a8b6d8fc9ca`  
		Last Modified: Tue, 31 Oct 2023 04:34:30 GMT  
		Size: 308.5 MB (308522697 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d558332f03cfe55951cce0f6d132d15144e514706f3fcb7c835254c68bf9825a`  
		Last Modified: Tue, 31 Oct 2023 04:34:12 GMT  
		Size: 936.8 KB (936848 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b60300b66d89f394a3bebf324ff53553a2bfa21dbb71621deafcda0730f93850`  
		Last Modified: Tue, 31 Oct 2023 04:34:11 GMT  
		Size: 1.3 KB (1343 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:68355ae4f9bbbc4f2315bc113dd3a216f21bbd3e28c5aaa6353342847abc36db`  
		Last Modified: Tue, 31 Oct 2023 04:34:11 GMT  
		Size: 2.5 KB (2456 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:521459ebaeb513a23aec400512d8cc7b8b8696a3d3c13e99d94d40dc1f68082d`  
		Last Modified: Tue, 31 Oct 2023 04:34:11 GMT  
		Size: 6.3 KB (6318 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6ba06291fe6c3367c23b286e04c8d930f5c0c658976fc25359cf4723a8429ae4`  
		Last Modified: Tue, 31 Oct 2023 04:34:11 GMT  
		Size: 2.5 KB (2504 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
