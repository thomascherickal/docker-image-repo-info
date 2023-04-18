## `xwiki:lts-postgres`

```console
$ docker pull xwiki@sha256:811d5834cf334a885a154d9da98890057b050d2d790c64e118cad5748d733d90
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `xwiki:lts-postgres` - linux; amd64

```console
$ docker pull xwiki@sha256:ca9d6d2738fda2e533a24196adfe0f5a63dff1533a29db581206626ce256ef88
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **590.1 MB (590091729 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:8f43ee3e713d0c0d7be3a73bf347736bea89c0932f4d1b2c355382ee5247cd2e`
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
# Thu, 16 Mar 2023 02:45:18 GMT
ENV JAVA_VERSION=jdk-11.0.18+10
# Thu, 16 Mar 2023 02:45:50 GMT
RUN set -eux;     ARCH="$(dpkg --print-architecture)";     case "${ARCH}" in        aarch64|arm64)          ESUM='89bc6e93d48a37a5eff7ec5afa515c60eb3369d106d1736f5e845b3dcf8fb72c';          BINARY_URL='https://github.com/adoptium/temurin11-binaries/releases/download/jdk-11.0.18%2B10/OpenJDK11U-jre_aarch64_linux_hotspot_11.0.18_10.tar.gz';          ;;        armhf|arm)          ESUM='949482ac232e756f342de6a8592d56b58803e10d3956abff14c4958e711a0b7c';          BINARY_URL='https://github.com/adoptium/temurin11-binaries/releases/download/jdk-11.0.18%2B10/OpenJDK11U-jre_arm_linux_hotspot_11.0.18_10.tar.gz';          ;;        ppc64el|powerpc:common64)          ESUM='df32e80d5b6db60a1ed9ed04eaf267eaf17835ed2ae2c1708d8d94328c03a0a5';          BINARY_URL='https://github.com/adoptium/temurin11-binaries/releases/download/jdk-11.0.18%2B10/OpenJDK11U-jre_ppc64le_linux_hotspot_11.0.18_10.tar.gz';          ;;        s390x|s390:64-bit)          ESUM='c07df5081f78021bed0d169622e470ebd4a4525a45f84192a52580ddb912959b';          BINARY_URL='https://github.com/adoptium/temurin11-binaries/releases/download/jdk-11.0.18%2B10/OpenJDK11U-jre_s390x_linux_hotspot_11.0.18_10.tar.gz';          ;;        amd64|i386:x86-64)          ESUM='0e7b196ef8603ac3d38caaf7768b7b0a3c613d60e15a6511bcfb2c894b609e99';          BINARY_URL='https://github.com/adoptium/temurin11-binaries/releases/download/jdk-11.0.18%2B10/OpenJDK11U-jre_x64_linux_hotspot_11.0.18_10.tar.gz';          ;;        *)          echo "Unsupported arch: ${ARCH}";          exit 1;          ;;     esac; 	  wget -O /tmp/openjdk.tar.gz ${BINARY_URL}; 	  echo "${ESUM} */tmp/openjdk.tar.gz" | sha256sum -c -; 	  mkdir -p "$JAVA_HOME"; 	  tar --extract 	      --file /tmp/openjdk.tar.gz 	      --directory "$JAVA_HOME" 	      --strip-components 1 	      --no-same-owner 	  ;     rm -f /tmp/openjdk.tar.gz ${JAVA_HOME}/src.zip;     find "$JAVA_HOME/lib" -name '*.so' -exec dirname '{}' ';' | sort -u > /etc/ld.so.conf.d/docker-openjdk.conf;     ldconfig;     java -Xshare:dump;
# Thu, 16 Mar 2023 02:45:50 GMT
RUN echo Verifying install ...     && fileEncoding="$(echo 'System.out.println(System.getProperty("file.encoding"))' | jshell -s -)"; [ "$fileEncoding" = 'UTF-8' ]; rm -rf ~/.java     && echo java --version && java --version     && echo Complete.
# Thu, 16 Mar 2023 08:06:48 GMT
ENV CATALINA_HOME=/usr/local/tomcat
# Thu, 16 Mar 2023 08:06:48 GMT
ENV PATH=/usr/local/tomcat/bin:/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 16 Mar 2023 08:06:48 GMT
RUN mkdir -p "$CATALINA_HOME"
# Thu, 16 Mar 2023 08:06:48 GMT
WORKDIR /usr/local/tomcat
# Thu, 16 Mar 2023 08:06:48 GMT
ENV TOMCAT_NATIVE_LIBDIR=/usr/local/tomcat/native-jni-lib
# Thu, 16 Mar 2023 08:06:49 GMT
ENV LD_LIBRARY_PATH=/usr/local/tomcat/native-jni-lib
# Thu, 16 Mar 2023 08:09:22 GMT
ENV GPG_KEYS=48F8E69F6390C9F25CFEDCD268248959359E722B A9C5DF4D22E99998D9875A5110C01C5A2F6059E7 DCFD35E0BF8CA7344752DE8B6FB21E8933C60243
# Thu, 16 Mar 2023 08:09:22 GMT
ENV TOMCAT_MAJOR=9
# Tue, 18 Apr 2023 18:31:35 GMT
ENV TOMCAT_VERSION=9.0.74
# Tue, 18 Apr 2023 18:31:35 GMT
ENV TOMCAT_SHA512=0e173fc2a76404c41c571c50a1956a2b867870d767200bd30f48d89bf04a4b6337f12e6577415da932cd2dfef9b4e9e9fdd52bd873afb06c6258b0e64244a44e
# Tue, 18 Apr 2023 18:31:36 GMT
COPY dir:b36786b0aedf695afc76054632233ea0fc4a7792546a7bdf7a5c4615bc597c83 in /usr/local/tomcat 
# Tue, 18 Apr 2023 18:31:40 GMT
RUN set -eux; 	apt-get update; 	xargs -rt apt-get install -y --no-install-recommends < "$TOMCAT_NATIVE_LIBDIR/.dependencies.txt"; 	rm -rf /var/lib/apt/lists/*
# Tue, 18 Apr 2023 18:31:41 GMT
RUN set -eux; 	nativeLines="$(catalina.sh configtest 2>&1)"; 	nativeLines="$(echo "$nativeLines" | grep 'Apache Tomcat Native')"; 	nativeLines="$(echo "$nativeLines" | sort -u)"; 	if ! echo "$nativeLines" | grep -E 'INFO: Loaded( APR based)? Apache Tomcat Native library' >&2; then 		echo >&2 "$nativeLines"; 		exit 1; 	fi
# Tue, 18 Apr 2023 18:31:41 GMT
EXPOSE 8080
# Tue, 18 Apr 2023 18:31:42 GMT
CMD ["catalina.sh" "run"]
# Tue, 18 Apr 2023 18:58:52 GMT
LABEL org.opencontainers.image.authors=XWiki Development Team <committers@xwiki.org>
# Tue, 18 Apr 2023 18:58:52 GMT
LABEL org.opencontainers.image.url=https://hub.docker.com/_/xwiki
# Tue, 18 Apr 2023 18:58:52 GMT
LABEL org.opencontainers.image.documentation=https://hub.docker.com/_/xwiki
# Tue, 18 Apr 2023 18:58:52 GMT
LABEL org.opencontainers.image.source=https://github.com/xwiki/xwiki-docker.git
# Tue, 18 Apr 2023 18:58:52 GMT
LABEL org.opencontainers.image.vendor=xwiki.org
# Tue, 18 Apr 2023 18:58:52 GMT
LABEL org.opencontainers.image.licenses=LGPL-2.1
# Tue, 18 Apr 2023 19:01:55 GMT
RUN apt-get update &&   apt-get --no-install-recommends -y install     curl     libreoffice     unzip     procps     libpostgresql-jdbc-java &&   rm -rf /var/lib/apt/lists/*
# Tue, 18 Apr 2023 19:03:32 GMT
ENV XWIKI_VERSION=14.10.8
# Tue, 18 Apr 2023 19:03:32 GMT
ENV XWIKI_URL_PREFIX=https://maven.xwiki.org/releases/org/xwiki/platform/xwiki-platform-distribution-war/14.10.8
# Tue, 18 Apr 2023 19:03:32 GMT
ENV XWIKI_DOWNLOAD_SHA256=dec61a1f0f5edf6c414aaa16d41821da25c6508dafcaa25d624a97ae55966b1d
# Tue, 18 Apr 2023 19:04:11 GMT
RUN rm -rf /usr/local/tomcat/webapps/* &&   mkdir -p /usr/local/tomcat/temp &&   mkdir -p /usr/local/xwiki/data &&   curl -fSL "${XWIKI_URL_PREFIX}/xwiki-platform-distribution-war-${XWIKI_VERSION}.war" -o xwiki.war &&   echo "$XWIKI_DOWNLOAD_SHA256 xwiki.war" | sha256sum -c - &&   unzip -d /usr/local/tomcat/webapps/ROOT xwiki.war &&   rm -f xwiki.war
# Tue, 18 Apr 2023 19:04:12 GMT
RUN cp /usr/share/java/postgresql-jdbc4.jar /usr/local/tomcat/webapps/ROOT/WEB-INF/lib/
# Tue, 18 Apr 2023 19:04:12 GMT
COPY file:0a1be11e2eb610a1dbcd415404e3a592641110b93090030cb831e3a19a163017 in /usr/local/tomcat/bin/ 
# Tue, 18 Apr 2023 19:04:12 GMT
COPY file:4a923f484bb29a26630c19e1d617d3bf6aa6ae7c6c4a5561e97b037bcde0847c in /usr/local/tomcat/webapps/ROOT/WEB-INF/hibernate.cfg.xml 
# Tue, 18 Apr 2023 19:04:13 GMT
RUN sed -i 's/<id>org.xwiki.platform:xwiki-platform-distribution-war/<id>org.xwiki.platform:xwiki-platform-distribution-docker/'   /usr/local/tomcat/webapps/ROOT/META-INF/extension.xed
# Tue, 18 Apr 2023 19:04:13 GMT
COPY file:a47c4dcd87c9dad97aff38c49188357e6193bcad50757e516cfb08a60d4de611 in /usr/local/bin/docker-entrypoint.sh 
# Tue, 18 Apr 2023 19:04:13 GMT
VOLUME [/usr/local/xwiki]
# Tue, 18 Apr 2023 19:04:13 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 18 Apr 2023 19:04:13 GMT
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
	-	`sha256:9f3fc5460b4b76e852651fec42e4cde1337c4bf503657efbe5521f379b19748a`  
		Last Modified: Thu, 16 Mar 2023 02:52:30 GMT  
		Size: 46.6 MB (46635547 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a7a8054900958099c4da9d407d5b7d023cf76df2b891f916546c0ddb7e26a697`  
		Last Modified: Thu, 16 Mar 2023 02:52:23 GMT  
		Size: 159.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:28433e65ef6c711796f104c155386ec51d210e29e92ed4d7859db73e3c2cb719`  
		Last Modified: Thu, 16 Mar 2023 08:23:13 GMT  
		Size: 171.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a1ab3dcf35d88cd7ff0595953d322dc1367d5f8a248acc59543c2f3d1898be5c`  
		Last Modified: Tue, 18 Apr 2023 18:39:40 GMT  
		Size: 12.2 MB (12233790 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fa21f10fb2810013104d95a91f775c7089dcc7a747821d618bad4aa53ccaf923`  
		Last Modified: Tue, 18 Apr 2023 18:39:40 GMT  
		Size: 454.2 KB (454193 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b6c624db7c0516c2f258d7f58188d1942973007af56fc342254e40b14b4d50fe`  
		Last Modified: Tue, 18 Apr 2023 18:39:39 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:67f0bdd770ef63a62eeec602b1d6348d61fa8dd8b28e57bd567e430e3da51541`  
		Last Modified: Tue, 18 Apr 2023 19:06:04 GMT  
		Size: 179.7 MB (179745203 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b173e1a008405c1a5f9d558e9b0fc0e3df0b46870e9994c646534b00ed6833f5`  
		Last Modified: Tue, 18 Apr 2023 19:07:40 GMT  
		Size: 307.2 MB (307211356 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:62f5eba282d5f840fa369aa085dafb2416851a41068ea39089ba515593f890be`  
		Last Modified: Tue, 18 Apr 2023 19:07:24 GMT  
		Size: 936.8 KB (936849 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d9b18a5686571fa0e653f87f2f0a56001592f46a28c3d5b0784108de37c64aa3`  
		Last Modified: Tue, 18 Apr 2023 19:07:24 GMT  
		Size: 1.3 KB (1342 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:203c11e7264a47ce1e61f5eaa0e6bbccce0feeea9eae8d6d0f75d6cb4b9089c4`  
		Last Modified: Tue, 18 Apr 2023 19:07:24 GMT  
		Size: 2.5 KB (2454 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b7b70ff79cfdd11c893e48943ab471bb1df32e96a69aa6de038fb2d0237dc5b1`  
		Last Modified: Tue, 18 Apr 2023 19:07:24 GMT  
		Size: 6.0 KB (6014 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:98bd6cf8f38776e72ff04831788ae468fa742597cb7dc08caa27ca5a6e3fa86e`  
		Last Modified: Tue, 18 Apr 2023 19:07:24 GMT  
		Size: 2.5 KB (2503 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `xwiki:lts-postgres` - linux; arm64 variant v8

```console
$ docker pull xwiki@sha256:0cb88acaaabb83c71ed0e497591316fe6cc981d1e2ffff230319796cbb013433
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **581.4 MB (581361661 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:97de05453de62c5569fe3ef521f782438ddbf238ffed841b89aafcbdba03da3d`
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
# Thu, 16 Mar 2023 01:53:41 GMT
ENV JAVA_VERSION=jdk-11.0.18+10
# Thu, 16 Mar 2023 01:54:08 GMT
RUN set -eux;     ARCH="$(dpkg --print-architecture)";     case "${ARCH}" in        aarch64|arm64)          ESUM='89bc6e93d48a37a5eff7ec5afa515c60eb3369d106d1736f5e845b3dcf8fb72c';          BINARY_URL='https://github.com/adoptium/temurin11-binaries/releases/download/jdk-11.0.18%2B10/OpenJDK11U-jre_aarch64_linux_hotspot_11.0.18_10.tar.gz';          ;;        armhf|arm)          ESUM='949482ac232e756f342de6a8592d56b58803e10d3956abff14c4958e711a0b7c';          BINARY_URL='https://github.com/adoptium/temurin11-binaries/releases/download/jdk-11.0.18%2B10/OpenJDK11U-jre_arm_linux_hotspot_11.0.18_10.tar.gz';          ;;        ppc64el|powerpc:common64)          ESUM='df32e80d5b6db60a1ed9ed04eaf267eaf17835ed2ae2c1708d8d94328c03a0a5';          BINARY_URL='https://github.com/adoptium/temurin11-binaries/releases/download/jdk-11.0.18%2B10/OpenJDK11U-jre_ppc64le_linux_hotspot_11.0.18_10.tar.gz';          ;;        s390x|s390:64-bit)          ESUM='c07df5081f78021bed0d169622e470ebd4a4525a45f84192a52580ddb912959b';          BINARY_URL='https://github.com/adoptium/temurin11-binaries/releases/download/jdk-11.0.18%2B10/OpenJDK11U-jre_s390x_linux_hotspot_11.0.18_10.tar.gz';          ;;        amd64|i386:x86-64)          ESUM='0e7b196ef8603ac3d38caaf7768b7b0a3c613d60e15a6511bcfb2c894b609e99';          BINARY_URL='https://github.com/adoptium/temurin11-binaries/releases/download/jdk-11.0.18%2B10/OpenJDK11U-jre_x64_linux_hotspot_11.0.18_10.tar.gz';          ;;        *)          echo "Unsupported arch: ${ARCH}";          exit 1;          ;;     esac; 	  wget -O /tmp/openjdk.tar.gz ${BINARY_URL}; 	  echo "${ESUM} */tmp/openjdk.tar.gz" | sha256sum -c -; 	  mkdir -p "$JAVA_HOME"; 	  tar --extract 	      --file /tmp/openjdk.tar.gz 	      --directory "$JAVA_HOME" 	      --strip-components 1 	      --no-same-owner 	  ;     rm -f /tmp/openjdk.tar.gz ${JAVA_HOME}/src.zip;     find "$JAVA_HOME/lib" -name '*.so' -exec dirname '{}' ';' | sort -u > /etc/ld.so.conf.d/docker-openjdk.conf;     ldconfig;     java -Xshare:dump;
# Thu, 16 Mar 2023 01:54:09 GMT
RUN echo Verifying install ...     && fileEncoding="$(echo 'System.out.println(System.getProperty("file.encoding"))' | jshell -s -)"; [ "$fileEncoding" = 'UTF-8' ]; rm -rf ~/.java     && echo java --version && java --version     && echo Complete.
# Thu, 16 Mar 2023 06:27:32 GMT
ENV CATALINA_HOME=/usr/local/tomcat
# Thu, 16 Mar 2023 06:27:32 GMT
ENV PATH=/usr/local/tomcat/bin:/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 16 Mar 2023 06:27:32 GMT
RUN mkdir -p "$CATALINA_HOME"
# Thu, 16 Mar 2023 06:27:32 GMT
WORKDIR /usr/local/tomcat
# Thu, 16 Mar 2023 06:27:32 GMT
ENV TOMCAT_NATIVE_LIBDIR=/usr/local/tomcat/native-jni-lib
# Thu, 16 Mar 2023 06:27:32 GMT
ENV LD_LIBRARY_PATH=/usr/local/tomcat/native-jni-lib
# Thu, 16 Mar 2023 06:29:35 GMT
ENV GPG_KEYS=48F8E69F6390C9F25CFEDCD268248959359E722B A9C5DF4D22E99998D9875A5110C01C5A2F6059E7 DCFD35E0BF8CA7344752DE8B6FB21E8933C60243
# Thu, 16 Mar 2023 06:29:35 GMT
ENV TOMCAT_MAJOR=9
# Thu, 16 Mar 2023 06:29:35 GMT
ENV TOMCAT_VERSION=9.0.73
# Thu, 16 Mar 2023 06:29:35 GMT
ENV TOMCAT_SHA512=d43fbd6c5ae00bc0ffc2559743f91abd3547c827426cb0acdc8428e060e8659b6bb41b3877deb061ab6202980de39b9558525a4256725b647d5bff93e47a5664
# Tue, 28 Mar 2023 01:34:36 GMT
COPY dir:792802298cee72ee36ea3bb63646b5835815276ef6d3cdae0d0497a60688489c in /usr/local/tomcat 
# Tue, 28 Mar 2023 01:34:39 GMT
RUN set -eux; 	apt-get update; 	xargs -rt apt-get install -y --no-install-recommends < "$TOMCAT_NATIVE_LIBDIR/.dependencies.txt"; 	rm -rf /var/lib/apt/lists/*
# Tue, 28 Mar 2023 01:34:40 GMT
RUN set -eux; 	nativeLines="$(catalina.sh configtest 2>&1)"; 	nativeLines="$(echo "$nativeLines" | grep 'Apache Tomcat Native')"; 	nativeLines="$(echo "$nativeLines" | sort -u)"; 	if ! echo "$nativeLines" | grep -E 'INFO: Loaded( APR based)? Apache Tomcat Native library' >&2; then 		echo >&2 "$nativeLines"; 		exit 1; 	fi
# Tue, 28 Mar 2023 01:34:40 GMT
EXPOSE 8080
# Tue, 28 Mar 2023 01:34:41 GMT
CMD ["catalina.sh" "run"]
# Tue, 28 Mar 2023 05:15:24 GMT
LABEL org.opencontainers.image.authors=XWiki Development Team <committers@xwiki.org>
# Tue, 28 Mar 2023 05:15:24 GMT
LABEL org.opencontainers.image.url=https://hub.docker.com/_/xwiki
# Tue, 28 Mar 2023 05:15:24 GMT
LABEL org.opencontainers.image.documentation=https://hub.docker.com/_/xwiki
# Tue, 28 Mar 2023 05:15:24 GMT
LABEL org.opencontainers.image.source=https://github.com/xwiki/xwiki-docker.git
# Tue, 28 Mar 2023 05:15:24 GMT
LABEL org.opencontainers.image.vendor=xwiki.org
# Tue, 28 Mar 2023 05:15:24 GMT
LABEL org.opencontainers.image.licenses=LGPL-2.1
# Tue, 28 Mar 2023 05:19:08 GMT
RUN apt-get update &&   apt-get --no-install-recommends -y install     curl     libreoffice     unzip     procps     libpostgresql-jdbc-java &&   rm -rf /var/lib/apt/lists/*
# Tue, 11 Apr 2023 19:48:16 GMT
ENV XWIKI_VERSION=14.10.8
# Tue, 11 Apr 2023 19:48:16 GMT
ENV XWIKI_URL_PREFIX=https://maven.xwiki.org/releases/org/xwiki/platform/xwiki-platform-distribution-war/14.10.8
# Tue, 11 Apr 2023 19:48:16 GMT
ENV XWIKI_DOWNLOAD_SHA256=dec61a1f0f5edf6c414aaa16d41821da25c6508dafcaa25d624a97ae55966b1d
# Tue, 11 Apr 2023 19:48:56 GMT
RUN rm -rf /usr/local/tomcat/webapps/* &&   mkdir -p /usr/local/tomcat/temp &&   mkdir -p /usr/local/xwiki/data &&   curl -fSL "${XWIKI_URL_PREFIX}/xwiki-platform-distribution-war-${XWIKI_VERSION}.war" -o xwiki.war &&   echo "$XWIKI_DOWNLOAD_SHA256 xwiki.war" | sha256sum -c - &&   unzip -d /usr/local/tomcat/webapps/ROOT xwiki.war &&   rm -f xwiki.war
# Tue, 11 Apr 2023 19:48:59 GMT
RUN cp /usr/share/java/postgresql-jdbc4.jar /usr/local/tomcat/webapps/ROOT/WEB-INF/lib/
# Tue, 11 Apr 2023 19:48:59 GMT
COPY file:0a1be11e2eb610a1dbcd415404e3a592641110b93090030cb831e3a19a163017 in /usr/local/tomcat/bin/ 
# Tue, 11 Apr 2023 19:48:59 GMT
COPY file:4a923f484bb29a26630c19e1d617d3bf6aa6ae7c6c4a5561e97b037bcde0847c in /usr/local/tomcat/webapps/ROOT/WEB-INF/hibernate.cfg.xml 
# Tue, 11 Apr 2023 19:48:59 GMT
RUN sed -i 's/<id>org.xwiki.platform:xwiki-platform-distribution-war/<id>org.xwiki.platform:xwiki-platform-distribution-docker/'   /usr/local/tomcat/webapps/ROOT/META-INF/extension.xed
# Tue, 11 Apr 2023 19:48:59 GMT
COPY file:a47c4dcd87c9dad97aff38c49188357e6193bcad50757e516cfb08a60d4de611 in /usr/local/bin/docker-entrypoint.sh 
# Tue, 11 Apr 2023 19:48:59 GMT
VOLUME [/usr/local/xwiki]
# Tue, 11 Apr 2023 19:48:59 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 11 Apr 2023 19:48:59 GMT
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
	-	`sha256:26126947450108b9349ce5c70904451e6ada86d51dde32223e9d9de1e567f89f`  
		Last Modified: Thu, 16 Mar 2023 02:00:06 GMT  
		Size: 45.0 MB (44977990 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:48a873c16c3848ad12697e893cb753bb353c55c7d09fbbcdb67983aafbbd885b`  
		Last Modified: Thu, 16 Mar 2023 02:00:02 GMT  
		Size: 160.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c171da1e14cae24bb7b0a542326df4c310966690ef3395e8a77f7387a3638df0`  
		Last Modified: Thu, 16 Mar 2023 06:42:14 GMT  
		Size: 171.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:883b43c8c381fd15755085a004c51fa9addaa5ef6854823183ee550d31895f37`  
		Last Modified: Tue, 28 Mar 2023 01:49:32 GMT  
		Size: 12.2 MB (12225311 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:383b927feee7cf1770e37ed30db05c04ad0f243a0f2df4ee74c7fd624646f3fb`  
		Last Modified: Tue, 28 Mar 2023 01:49:31 GMT  
		Size: 453.2 KB (453237 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ec5a50ba89c62496d20e83a06f2ad9faf92d551aaffa29b3a2deb3d87e57d25d`  
		Last Modified: Tue, 28 Mar 2023 01:49:30 GMT  
		Size: 130.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6ad257cb0650e1bb2291054e5039546d7c390523bd44317bed4f4cdef7b12551`  
		Last Modified: Tue, 28 Mar 2023 05:23:18 GMT  
		Size: 174.8 MB (174766914 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7c9702ebcddf5e8461b222de863c72ed9cba2f6e672e12211d703a5d40817170`  
		Last Modified: Tue, 11 Apr 2023 19:50:26 GMT  
		Size: 307.2 MB (307211273 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:db3152f4d37b7ab889b5d7c972bdbfd5c3c80aa015afa6e0b32a6bc5d792c655`  
		Last Modified: Tue, 11 Apr 2023 19:50:13 GMT  
		Size: 936.8 KB (936849 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5547706b5c21036630d85a285ca4d2d4a03c36ffa61f1b3795fae305a6aa6911`  
		Last Modified: Tue, 11 Apr 2023 19:50:12 GMT  
		Size: 1.3 KB (1342 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cf00186743dc84fd224a90a6a6cda53fd72153094f3678c67b7c193d41eccd9d`  
		Last Modified: Tue, 11 Apr 2023 19:50:12 GMT  
		Size: 2.5 KB (2451 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:df36745ae83ea0a3cdb53ee08bf3d5676e4a87e0408372db33ccd0f71ecdbc9e`  
		Last Modified: Tue, 11 Apr 2023 19:50:12 GMT  
		Size: 6.0 KB (6014 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c6b9e1ece91fa3666ff4f242f6985eba6867d1295e4011edc4678da41c1556d6`  
		Last Modified: Tue, 11 Apr 2023 19:50:12 GMT  
		Size: 2.5 KB (2498 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
