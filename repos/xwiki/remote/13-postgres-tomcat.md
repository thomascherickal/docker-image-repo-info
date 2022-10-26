## `xwiki:13-postgres-tomcat`

```console
$ docker pull xwiki@sha256:5110bb54b61b5d54aa6de6d07187eb709cff4416e3b31ffb025cf691e8f79b4d
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `xwiki:13-postgres-tomcat` - linux; amd64

```console
$ docker pull xwiki@sha256:0cb9d4c22353b95593f7654dc564a2a606f1f27df79425ef6c74b2d09ee3ffbc
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **574.9 MB (574898529 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:59e183ba46dd07d0224fa218a22a31dd39d6ff7bb24f70375620e3ab9ffb47bf`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["xwiki"]`

```dockerfile
# Tue, 04 Oct 2022 23:35:20 GMT
ADD file:6cd2e13356aa5339c1f2abd3c210a52f6ed74fae05cd61aa09f37b6a4764f65c in / 
# Tue, 04 Oct 2022 23:35:20 GMT
CMD ["bash"]
# Wed, 05 Oct 2022 16:59:56 GMT
ENV JAVA_HOME=/opt/java/openjdk
# Wed, 05 Oct 2022 16:59:56 GMT
ENV PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 05 Oct 2022 16:59:56 GMT
ENV LANG=en_US.UTF-8 LANGUAGE=en_US:en LC_ALL=en_US.UTF-8
# Wed, 05 Oct 2022 17:00:37 GMT
RUN apt-get update     && DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends tzdata curl wget ca-certificates fontconfig locales     && echo "en_US.UTF-8 UTF-8" >> /etc/locale.gen     && locale-gen en_US.UTF-8     && rm -rf /var/lib/apt/lists/*
# Wed, 05 Oct 2022 17:01:31 GMT
ENV JAVA_VERSION=jdk-11.0.16.1+1
# Wed, 05 Oct 2022 17:02:03 GMT
RUN set -eux;     ARCH="$(dpkg --print-architecture)";     case "${ARCH}" in        aarch64|arm64)          ESUM='b6607f28fa2906d612d517f0babe4f0f895aa1c3f901edcddb493e33c1e27364';          BINARY_URL='https://github.com/adoptium/temurin11-binaries/releases/download/jdk-11.0.16.1%2B1/OpenJDK11U-jre_aarch64_linux_hotspot_11.0.16.1_1.tar.gz';          ;;        armhf|arm)          ESUM='2ee7fe636a6a57e4718dfe597e8097b93ef8d976e4b05384433777c9f0526f5a';          BINARY_URL='https://github.com/adoptium/temurin11-binaries/releases/download/jdk-11.0.16.1%2B1/OpenJDK11U-jre_arm_linux_hotspot_11.0.16.1_1.tar.gz';          ;;        ppc64el|powerpc:common64)          ESUM='f76b64b201b64ff37f77f73ead546ebcf2af9862b7cd1a1f4e0e5628e3f6a7fc';          BINARY_URL='https://github.com/adoptium/temurin11-binaries/releases/download/jdk-11.0.16.1%2B1/OpenJDK11U-jre_ppc64le_linux_hotspot_11.0.16.1_1.tar.gz';          ;;        s390x|s390:64-bit)          ESUM='bf01489459135ab0ce1ad346a56f0dfeb2d6fe4e59854ef76a6bb989ac403f91';          BINARY_URL='https://github.com/adoptium/temurin11-binaries/releases/download/jdk-11.0.16.1%2B1/OpenJDK11U-jre_s390x_linux_hotspot_11.0.16.1_1.tar.gz';          ;;        amd64|i386:x86-64)          ESUM='1ffe1a682e8179e35238bf3f93aba0cb185850e202c676f41d38cb0561883eda';          BINARY_URL='https://github.com/adoptium/temurin11-binaries/releases/download/jdk-11.0.16.1%2B1/OpenJDK11U-jre_x64_linux_hotspot_11.0.16.1_1.tar.gz';          ;;        *)          echo "Unsupported arch: ${ARCH}";          exit 1;          ;;     esac; 	  wget -O /tmp/openjdk.tar.gz ${BINARY_URL}; 	  echo "${ESUM} */tmp/openjdk.tar.gz" | sha256sum -c -; 	  mkdir -p "$JAVA_HOME"; 	  tar --extract 	      --file /tmp/openjdk.tar.gz 	      --directory "$JAVA_HOME" 	      --strip-components 1 	      --no-same-owner 	  ;     rm /tmp/openjdk.tar.gz;     find "$JAVA_HOME/lib" -name '*.so' -exec dirname '{}' ';' | sort -u > /etc/ld.so.conf.d/docker-openjdk.conf;     ldconfig;     java -Xshare:dump;
# Wed, 05 Oct 2022 17:02:04 GMT
RUN echo Verifying install ...     && fileEncoding="$(echo 'System.out.println(System.getProperty("file.encoding"))' | jshell -s -)"; [ "$fileEncoding" = 'UTF-8' ]; rm -rf ~/.java     && echo java --version && java --version     && echo Complete.
# Thu, 06 Oct 2022 05:18:33 GMT
ENV CATALINA_HOME=/usr/local/tomcat
# Thu, 06 Oct 2022 05:18:33 GMT
ENV PATH=/usr/local/tomcat/bin:/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 06 Oct 2022 05:18:33 GMT
RUN mkdir -p "$CATALINA_HOME"
# Thu, 06 Oct 2022 05:18:33 GMT
WORKDIR /usr/local/tomcat
# Thu, 06 Oct 2022 05:18:34 GMT
ENV TOMCAT_NATIVE_LIBDIR=/usr/local/tomcat/native-jni-lib
# Thu, 06 Oct 2022 05:18:34 GMT
ENV LD_LIBRARY_PATH=/usr/local/tomcat/native-jni-lib
# Thu, 06 Oct 2022 05:25:51 GMT
ENV GPG_KEYS=48F8E69F6390C9F25CFEDCD268248959359E722B A9C5DF4D22E99998D9875A5110C01C5A2F6059E7 DCFD35E0BF8CA7344752DE8B6FB21E8933C60243
# Thu, 06 Oct 2022 05:25:51 GMT
ENV TOMCAT_MAJOR=9
# Sat, 08 Oct 2022 00:08:04 GMT
ENV TOMCAT_VERSION=9.0.68
# Sat, 08 Oct 2022 00:08:04 GMT
ENV TOMCAT_SHA512=840b21c5cd2bfea7bbfed99741c166608fa1515bb00475ebd4eccfd4f3ed2a1be6bfffd590b2a6600003205b62f271b6ba0937e557fc65a536df61cb4f7b7c8f
# Sat, 08 Oct 2022 00:08:04 GMT
COPY dir:e73e3631cb353a0953a6b8788956ed401a34aaa6d3cbf09074d5766c2961573c in /usr/local/tomcat 
# Sat, 08 Oct 2022 00:08:08 GMT
RUN set -eux; 	apt-get update; 	xargs -rt apt-get install -y --no-install-recommends < "$TOMCAT_NATIVE_LIBDIR/.dependencies.txt"; 	rm -rf /var/lib/apt/lists/*
# Sat, 08 Oct 2022 00:08:10 GMT
RUN set -eux; 	nativeLines="$(catalina.sh configtest 2>&1)"; 	nativeLines="$(echo "$nativeLines" | grep 'Apache Tomcat Native')"; 	nativeLines="$(echo "$nativeLines" | sort -u)"; 	if ! echo "$nativeLines" | grep -E 'INFO: Loaded( APR based)? Apache Tomcat Native library' >&2; then 		echo >&2 "$nativeLines"; 		exit 1; 	fi
# Sat, 08 Oct 2022 00:08:10 GMT
EXPOSE 8080
# Sat, 08 Oct 2022 00:08:10 GMT
CMD ["catalina.sh" "run"]
# Sat, 08 Oct 2022 00:41:45 GMT
LABEL org.opencontainers.image.authors=XWiki Development Team <committers@xwiki.org>
# Sat, 08 Oct 2022 00:41:45 GMT
LABEL org.opencontainers.image.url=https://hub.docker.com/_/xwiki
# Sat, 08 Oct 2022 00:41:45 GMT
LABEL org.opencontainers.image.documentation=https://hub.docker.com/_/xwiki
# Sat, 08 Oct 2022 00:41:45 GMT
LABEL org.opencontainers.image.source=https://github.com/xwiki/xwiki-docker.git
# Sat, 08 Oct 2022 00:41:45 GMT
LABEL org.opencontainers.image.vendor=xwiki.org
# Sat, 08 Oct 2022 00:41:46 GMT
LABEL org.opencontainers.image.licenses=LGPL-2.1
# Sat, 08 Oct 2022 00:45:35 GMT
RUN apt-get update &&   apt-get --no-install-recommends -y install     curl     libreoffice     unzip     procps     libpostgresql-jdbc-java &&   rm -rf /var/lib/apt/lists/*
# Sat, 08 Oct 2022 00:49:27 GMT
ENV XWIKI_VERSION=13.10.9
# Sat, 08 Oct 2022 00:49:28 GMT
ENV XWIKI_URL_PREFIX=https://maven.xwiki.org/releases/org/xwiki/platform/xwiki-platform-distribution-war/13.10.9
# Sat, 08 Oct 2022 00:49:28 GMT
ENV XWIKI_DOWNLOAD_SHA256=ad57639016b1bfd1cdf84de764b310a65416832645c6bbfd933ec26fd977bb6a
# Sat, 08 Oct 2022 00:50:05 GMT
RUN rm -rf /usr/local/tomcat/webapps/* &&   mkdir -p /usr/local/tomcat/temp &&   mkdir -p /usr/local/xwiki/data &&   curl -fSL "${XWIKI_URL_PREFIX}/xwiki-platform-distribution-war-${XWIKI_VERSION}.war" -o xwiki.war &&   echo "$XWIKI_DOWNLOAD_SHA256 xwiki.war" | sha256sum -c - &&   unzip -d /usr/local/tomcat/webapps/ROOT xwiki.war &&   rm -f xwiki.war
# Sat, 08 Oct 2022 00:50:06 GMT
RUN cp /usr/share/java/postgresql-jdbc4.jar /usr/local/tomcat/webapps/ROOT/WEB-INF/lib/
# Sat, 08 Oct 2022 00:50:07 GMT
COPY file:0a1be11e2eb610a1dbcd415404e3a592641110b93090030cb831e3a19a163017 in /usr/local/tomcat/bin/ 
# Sat, 08 Oct 2022 00:50:07 GMT
COPY file:4a923f484bb29a26630c19e1d617d3bf6aa6ae7c6c4a5561e97b037bcde0847c in /usr/local/tomcat/webapps/ROOT/WEB-INF/hibernate.cfg.xml 
# Sat, 08 Oct 2022 00:50:07 GMT
RUN sed -i 's/<id>org.xwiki.platform:xwiki-platform-distribution-war/<id>org.xwiki.platform:xwiki-platform-distribution-docker/'   /usr/local/tomcat/webapps/ROOT/META-INF/extension.xed
# Sat, 08 Oct 2022 00:50:07 GMT
COPY file:a47c4dcd87c9dad97aff38c49188357e6193bcad50757e516cfb08a60d4de611 in /usr/local/bin/docker-entrypoint.sh 
# Sat, 08 Oct 2022 00:50:07 GMT
VOLUME [/usr/local/xwiki]
# Sat, 08 Oct 2022 00:50:08 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Sat, 08 Oct 2022 00:50:08 GMT
CMD ["xwiki"]
```

-	Layers:
	-	`sha256:cf92e523b49ea3d1fae59f5f082437a5f96c244fda6697995920142ff31d59cf`  
		Last Modified: Tue, 04 Oct 2022 03:04:01 GMT  
		Size: 30.4 MB (30428928 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:be4c7f172af2471a1945e9feb3dab4254026b8c38f20c75ae781436a4495e6db`  
		Last Modified: Wed, 05 Oct 2022 17:07:10 GMT  
		Size: 12.4 MB (12442343 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:521599bc479fb2b0da911ac0f7237ba1dd87823d0d2b609de333aef4766022a0`  
		Last Modified: Wed, 05 Oct 2022 17:09:25 GMT  
		Size: 46.5 MB (46498622 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:08fd90861fe76e553b9447451baf69d735ce869c254ee2968b0e893c35bd7a38`  
		Last Modified: Wed, 05 Oct 2022 17:09:19 GMT  
		Size: 161.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9ba416a4250746409b3c6db8225e8a0b0e59fcac990b18d4e524f989705055f9`  
		Last Modified: Thu, 06 Oct 2022 05:39:32 GMT  
		Size: 172.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7aefc9ef78986ecc1379e087a1a553201a82680cf5f2503b61d69b96c80492ee`  
		Last Modified: Sat, 08 Oct 2022 00:19:39 GMT  
		Size: 12.2 MB (12192002 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:95b673e50fff974c40ac161c0b405fb0aee5481f6df19da4980bcf939adf2fcc`  
		Last Modified: Sat, 08 Oct 2022 00:19:38 GMT  
		Size: 452.6 KB (452644 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:026cbea7dd95773d548c970dca685fc3ad9346a738d8245cf9f123833c18bfeb`  
		Last Modified: Sat, 08 Oct 2022 00:19:38 GMT  
		Size: 131.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6c36f3773b2d9c501a1628bbba2bc169b5ccce608686f351411a190dce51f495`  
		Last Modified: Sat, 08 Oct 2022 00:52:41 GMT  
		Size: 179.3 MB (179259331 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7bf85e8dae7d6b0e77481939e710cba893cceebbaeb39d83e1a72ae851afbb4e`  
		Last Modified: Sat, 08 Oct 2022 00:55:47 GMT  
		Size: 292.7 MB (292675730 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a138f3278decb3fe7841f4a9b8c0f9b34b045dd1debe1def3a8fb29582a0f523`  
		Last Modified: Sat, 08 Oct 2022 00:55:28 GMT  
		Size: 936.8 KB (936848 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2a3b2e24d27330ea30d05856b2f14af0ee716697ab41dec75cc632baf52bb556`  
		Last Modified: Sat, 08 Oct 2022 00:55:28 GMT  
		Size: 1.3 KB (1340 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:39f26970a9a6b61c5690df158e233e755181f7a33adbcac690266b1385b5bafb`  
		Last Modified: Sat, 08 Oct 2022 00:55:28 GMT  
		Size: 2.4 KB (2448 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cd0731dd7e87d1a8b11ec36150252510c251afa0355ff7d38042d5f83f3b533d`  
		Last Modified: Sat, 08 Oct 2022 00:55:28 GMT  
		Size: 5.3 KB (5329 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5e64e177872969173939fe174a6ce9b63a442d16e869fc05db697c5306ccfb11`  
		Last Modified: Sat, 08 Oct 2022 00:55:28 GMT  
		Size: 2.5 KB (2500 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `xwiki:13-postgres-tomcat` - linux; arm64 variant v8

```console
$ docker pull xwiki@sha256:a146728451baa7c40f3d0f226f71f7c5011f9072399aee5e02354c7593779b3b
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **566.7 MB (566660640 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ec49f1b2544c16e0eec613ca0b2703f43c2771ef74ca8f62dfea7c8966497123`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["xwiki"]`

```dockerfile
# Tue, 25 Oct 2022 05:55:02 GMT
ADD file:515177312f20fb1814b89bfccfe695fa2354bbb6d43fdb6e018bf5b1acc17e9f in / 
# Tue, 25 Oct 2022 05:55:02 GMT
CMD ["bash"]
# Wed, 26 Oct 2022 01:08:29 GMT
ENV JAVA_HOME=/opt/java/openjdk
# Wed, 26 Oct 2022 01:08:29 GMT
ENV PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 26 Oct 2022 01:08:30 GMT
ENV LANG=en_US.UTF-8 LANGUAGE=en_US:en LC_ALL=en_US.UTF-8
# Wed, 26 Oct 2022 01:09:02 GMT
RUN apt-get update     && DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends tzdata curl wget ca-certificates fontconfig locales     && echo "en_US.UTF-8 UTF-8" >> /etc/locale.gen     && locale-gen en_US.UTF-8     && rm -rf /var/lib/apt/lists/*
# Wed, 26 Oct 2022 01:10:29 GMT
ENV JAVA_VERSION=jdk-11.0.16.1+1
# Wed, 26 Oct 2022 01:11:06 GMT
RUN set -eux;     ARCH="$(dpkg --print-architecture)";     case "${ARCH}" in        aarch64|arm64)          ESUM='b6607f28fa2906d612d517f0babe4f0f895aa1c3f901edcddb493e33c1e27364';          BINARY_URL='https://github.com/adoptium/temurin11-binaries/releases/download/jdk-11.0.16.1%2B1/OpenJDK11U-jre_aarch64_linux_hotspot_11.0.16.1_1.tar.gz';          ;;        armhf|arm)          ESUM='2ee7fe636a6a57e4718dfe597e8097b93ef8d976e4b05384433777c9f0526f5a';          BINARY_URL='https://github.com/adoptium/temurin11-binaries/releases/download/jdk-11.0.16.1%2B1/OpenJDK11U-jre_arm_linux_hotspot_11.0.16.1_1.tar.gz';          ;;        ppc64el|powerpc:common64)          ESUM='f76b64b201b64ff37f77f73ead546ebcf2af9862b7cd1a1f4e0e5628e3f6a7fc';          BINARY_URL='https://github.com/adoptium/temurin11-binaries/releases/download/jdk-11.0.16.1%2B1/OpenJDK11U-jre_ppc64le_linux_hotspot_11.0.16.1_1.tar.gz';          ;;        s390x|s390:64-bit)          ESUM='bf01489459135ab0ce1ad346a56f0dfeb2d6fe4e59854ef76a6bb989ac403f91';          BINARY_URL='https://github.com/adoptium/temurin11-binaries/releases/download/jdk-11.0.16.1%2B1/OpenJDK11U-jre_s390x_linux_hotspot_11.0.16.1_1.tar.gz';          ;;        amd64|i386:x86-64)          ESUM='1ffe1a682e8179e35238bf3f93aba0cb185850e202c676f41d38cb0561883eda';          BINARY_URL='https://github.com/adoptium/temurin11-binaries/releases/download/jdk-11.0.16.1%2B1/OpenJDK11U-jre_x64_linux_hotspot_11.0.16.1_1.tar.gz';          ;;        *)          echo "Unsupported arch: ${ARCH}";          exit 1;          ;;     esac; 	  wget -O /tmp/openjdk.tar.gz ${BINARY_URL}; 	  echo "${ESUM} */tmp/openjdk.tar.gz" | sha256sum -c -; 	  mkdir -p "$JAVA_HOME"; 	  tar --extract 	      --file /tmp/openjdk.tar.gz 	      --directory "$JAVA_HOME" 	      --strip-components 1 	      --no-same-owner 	  ;     rm /tmp/openjdk.tar.gz;     find "$JAVA_HOME/lib" -name '*.so' -exec dirname '{}' ';' | sort -u > /etc/ld.so.conf.d/docker-openjdk.conf;     ldconfig;     java -Xshare:dump;
# Wed, 26 Oct 2022 01:11:07 GMT
RUN echo Verifying install ...     && fileEncoding="$(echo 'System.out.println(System.getProperty("file.encoding"))' | jshell -s -)"; [ "$fileEncoding" = 'UTF-8' ]; rm -rf ~/.java     && echo java --version && java --version     && echo Complete.
# Wed, 26 Oct 2022 17:11:05 GMT
ENV CATALINA_HOME=/usr/local/tomcat
# Wed, 26 Oct 2022 17:11:05 GMT
ENV PATH=/usr/local/tomcat/bin:/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 26 Oct 2022 17:11:05 GMT
RUN mkdir -p "$CATALINA_HOME"
# Wed, 26 Oct 2022 17:11:05 GMT
WORKDIR /usr/local/tomcat
# Wed, 26 Oct 2022 17:11:06 GMT
ENV TOMCAT_NATIVE_LIBDIR=/usr/local/tomcat/native-jni-lib
# Wed, 26 Oct 2022 17:11:06 GMT
ENV LD_LIBRARY_PATH=/usr/local/tomcat/native-jni-lib
# Wed, 26 Oct 2022 17:19:37 GMT
ENV GPG_KEYS=48F8E69F6390C9F25CFEDCD268248959359E722B A9C5DF4D22E99998D9875A5110C01C5A2F6059E7 DCFD35E0BF8CA7344752DE8B6FB21E8933C60243
# Wed, 26 Oct 2022 17:19:37 GMT
ENV TOMCAT_MAJOR=9
# Wed, 26 Oct 2022 17:19:37 GMT
ENV TOMCAT_VERSION=9.0.68
# Wed, 26 Oct 2022 17:19:37 GMT
ENV TOMCAT_SHA512=840b21c5cd2bfea7bbfed99741c166608fa1515bb00475ebd4eccfd4f3ed2a1be6bfffd590b2a6600003205b62f271b6ba0937e557fc65a536df61cb4f7b7c8f
# Wed, 26 Oct 2022 17:19:38 GMT
COPY dir:19b70270aa9cf6d706cd5db112445c59eb2a1298cc73e91aab9918f3461b4435 in /usr/local/tomcat 
# Wed, 26 Oct 2022 17:19:41 GMT
RUN set -eux; 	apt-get update; 	xargs -rt apt-get install -y --no-install-recommends < "$TOMCAT_NATIVE_LIBDIR/.dependencies.txt"; 	rm -rf /var/lib/apt/lists/*
# Wed, 26 Oct 2022 17:19:42 GMT
RUN set -eux; 	nativeLines="$(catalina.sh configtest 2>&1)"; 	nativeLines="$(echo "$nativeLines" | grep 'Apache Tomcat Native')"; 	nativeLines="$(echo "$nativeLines" | sort -u)"; 	if ! echo "$nativeLines" | grep -E 'INFO: Loaded( APR based)? Apache Tomcat Native library' >&2; then 		echo >&2 "$nativeLines"; 		exit 1; 	fi
# Wed, 26 Oct 2022 17:19:42 GMT
EXPOSE 8080
# Wed, 26 Oct 2022 17:19:42 GMT
CMD ["catalina.sh" "run"]
# Wed, 26 Oct 2022 18:58:51 GMT
LABEL org.opencontainers.image.authors=XWiki Development Team <committers@xwiki.org>
# Wed, 26 Oct 2022 18:58:51 GMT
LABEL org.opencontainers.image.url=https://hub.docker.com/_/xwiki
# Wed, 26 Oct 2022 18:58:51 GMT
LABEL org.opencontainers.image.documentation=https://hub.docker.com/_/xwiki
# Wed, 26 Oct 2022 18:58:51 GMT
LABEL org.opencontainers.image.source=https://github.com/xwiki/xwiki-docker.git
# Wed, 26 Oct 2022 18:58:52 GMT
LABEL org.opencontainers.image.vendor=xwiki.org
# Wed, 26 Oct 2022 18:58:52 GMT
LABEL org.opencontainers.image.licenses=LGPL-2.1
# Wed, 26 Oct 2022 19:01:07 GMT
RUN apt-get update &&   apt-get --no-install-recommends -y install     curl     libreoffice     unzip     procps     libpostgresql-jdbc-java &&   rm -rf /var/lib/apt/lists/*
# Wed, 26 Oct 2022 19:04:40 GMT
ENV XWIKI_VERSION=13.10.9
# Wed, 26 Oct 2022 19:04:40 GMT
ENV XWIKI_URL_PREFIX=https://maven.xwiki.org/releases/org/xwiki/platform/xwiki-platform-distribution-war/13.10.9
# Wed, 26 Oct 2022 19:04:40 GMT
ENV XWIKI_DOWNLOAD_SHA256=ad57639016b1bfd1cdf84de764b310a65416832645c6bbfd933ec26fd977bb6a
# Wed, 26 Oct 2022 19:05:17 GMT
RUN rm -rf /usr/local/tomcat/webapps/* &&   mkdir -p /usr/local/tomcat/temp &&   mkdir -p /usr/local/xwiki/data &&   curl -fSL "${XWIKI_URL_PREFIX}/xwiki-platform-distribution-war-${XWIKI_VERSION}.war" -o xwiki.war &&   echo "$XWIKI_DOWNLOAD_SHA256 xwiki.war" | sha256sum -c - &&   unzip -d /usr/local/tomcat/webapps/ROOT xwiki.war &&   rm -f xwiki.war
# Wed, 26 Oct 2022 19:05:19 GMT
RUN cp /usr/share/java/postgresql-jdbc4.jar /usr/local/tomcat/webapps/ROOT/WEB-INF/lib/
# Wed, 26 Oct 2022 19:05:19 GMT
COPY file:0a1be11e2eb610a1dbcd415404e3a592641110b93090030cb831e3a19a163017 in /usr/local/tomcat/bin/ 
# Wed, 26 Oct 2022 19:05:19 GMT
COPY file:4a923f484bb29a26630c19e1d617d3bf6aa6ae7c6c4a5561e97b037bcde0847c in /usr/local/tomcat/webapps/ROOT/WEB-INF/hibernate.cfg.xml 
# Wed, 26 Oct 2022 19:05:20 GMT
RUN sed -i 's/<id>org.xwiki.platform:xwiki-platform-distribution-war/<id>org.xwiki.platform:xwiki-platform-distribution-docker/'   /usr/local/tomcat/webapps/ROOT/META-INF/extension.xed
# Wed, 26 Oct 2022 19:05:20 GMT
COPY file:a47c4dcd87c9dad97aff38c49188357e6193bcad50757e516cfb08a60d4de611 in /usr/local/bin/docker-entrypoint.sh 
# Wed, 26 Oct 2022 19:05:20 GMT
VOLUME [/usr/local/xwiki]
# Wed, 26 Oct 2022 19:05:20 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 26 Oct 2022 19:05:20 GMT
CMD ["xwiki"]
```

-	Layers:
	-	`sha256:56a2caa6b2c66e01954c1a013b37ea359b6e6af8989dbfb958124b6318771af4`  
		Last Modified: Tue, 25 Oct 2022 05:56:14 GMT  
		Size: 28.4 MB (28382489 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d8d33b973dbba18a894c3b9064cedfece84e92985bce6e3be86a5efef3afdea8`  
		Last Modified: Wed, 26 Oct 2022 01:16:34 GMT  
		Size: 12.4 MB (12400371 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:05a6960b661b00d7e89ea4da7f8c5d2b571d0fd35007d448e17a2d178931aa42`  
		Last Modified: Wed, 26 Oct 2022 01:19:26 GMT  
		Size: 44.8 MB (44824650 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d046e5da0a7155986a366554538db9c6dc0dc232da3c7371c4a7f8820c766739`  
		Last Modified: Wed, 26 Oct 2022 01:19:21 GMT  
		Size: 160.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7e2b7e8ec1dfcdbb8e5a9b2d91a66efd6e7890187e39b81ae20b3e7cdcd34fcd`  
		Last Modified: Wed, 26 Oct 2022 17:35:35 GMT  
		Size: 173.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e4faa8a44e55bcf121db0d88d2c2c46596dead61108d821af57ed2cd29027445`  
		Last Modified: Wed, 26 Oct 2022 17:42:49 GMT  
		Size: 12.2 MB (12200353 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0c86ceac19f6bc02db83ad0acfe2ab7352de33d019ba1b9c9255ae48cce51489`  
		Last Modified: Wed, 26 Oct 2022 17:42:48 GMT  
		Size: 452.0 KB (452025 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:13c1d8957962e1a8cc040e5ae2ae5ae95f438b443ba81a3cf40fa90f1795475c`  
		Last Modified: Wed, 26 Oct 2022 17:42:48 GMT  
		Size: 130.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b2bb2cfed5f381e0e2e90cbb33e5cbd7c650ba8fcc0d5df8ec3b44901bd1f9ec`  
		Last Modified: Wed, 26 Oct 2022 19:07:39 GMT  
		Size: 174.8 MB (174776071 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:925f934510555d2af4d7a5860bab5d9a15361c2111d529da0f72d4d328b1b940`  
		Last Modified: Wed, 26 Oct 2022 19:10:40 GMT  
		Size: 292.7 MB (292675744 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:64497925f4eebe4b26cea65df8841b955b01776012373ecc37330533281f155d`  
		Last Modified: Wed, 26 Oct 2022 19:10:26 GMT  
		Size: 936.8 KB (936846 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c10a0b3fa53a7361e2e9565247f3052c6fe2c1fdb22baa71c4657e01e88e2bb9`  
		Last Modified: Wed, 26 Oct 2022 19:10:25 GMT  
		Size: 1.3 KB (1341 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5d3e6c6938ccafae303d7cfac399d869253208c5a898889fbaa9c85c33989052`  
		Last Modified: Wed, 26 Oct 2022 19:10:25 GMT  
		Size: 2.5 KB (2451 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:240cda5bb6ea73f3f7ade124144eccfea62b39c0e47156018288180db347e19b`  
		Last Modified: Wed, 26 Oct 2022 19:10:25 GMT  
		Size: 5.3 KB (5332 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6d2c60901772f998c7ec5fd415d8a285e4605c0281aae820b12594b88a59aaec`  
		Last Modified: Wed, 26 Oct 2022 19:10:25 GMT  
		Size: 2.5 KB (2504 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
