## `tomcat:8-jre17-temurin-jammy`

```console
$ docker pull tomcat@sha256:842c8b07e2db5ec616c2fec9b52d23e4fc6afab5478837fb98c2bfeb5e66fc72
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 5
	-	linux; amd64
	-	linux; arm variant v7
	-	linux; arm64 variant v8
	-	linux; ppc64le
	-	linux; s390x

### `tomcat:8-jre17-temurin-jammy` - linux; amd64

```console
$ docker pull tomcat@sha256:4884d7ac43d649bd663b270b429cf01a9eaad4819aca5ec25c1051343914d425
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **106.9 MB (106880044 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:62114b8242fcf9d188d0058237fb65ce4e0f2599bedebf3e9ace99a71045bf12`
-	Default Command: `["catalina.sh","run"]`

```dockerfile
# Wed, 28 Jun 2023 08:37:40 GMT
ARG RELEASE
# Wed, 28 Jun 2023 08:37:40 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Wed, 28 Jun 2023 08:37:40 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Wed, 28 Jun 2023 08:37:40 GMT
LABEL org.opencontainers.image.version=22.04
# Wed, 28 Jun 2023 08:37:42 GMT
ADD file:140fb5108b4a2861b5718ad03b4a5174bba03589ea8d4c053e6a0b282f439ff3 in / 
# Wed, 28 Jun 2023 08:37:42 GMT
CMD ["/bin/bash"]
# Tue, 04 Jul 2023 20:33:49 GMT
ENV JAVA_HOME=/opt/java/openjdk
# Tue, 04 Jul 2023 20:33:49 GMT
ENV PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 04 Jul 2023 20:33:49 GMT
ENV LANG=en_US.UTF-8 LANGUAGE=en_US:en LC_ALL=en_US.UTF-8
# Thu, 03 Aug 2023 02:38:42 GMT
RUN apt-get update     && DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends tzdata curl wget ca-certificates fontconfig locales p11-kit binutils     && echo "en_US.UTF-8 UTF-8" >> /etc/locale.gen     && locale-gen en_US.UTF-8     && rm -rf /var/lib/apt/lists/*
# Tue, 08 Aug 2023 19:23:54 GMT
ENV JAVA_VERSION=jdk-17.0.8+7
# Tue, 08 Aug 2023 19:24:34 GMT
RUN set -eux;     ARCH="$(dpkg --print-architecture)";     case "${ARCH}" in        aarch64|arm64)          ESUM='42525ae2951a669803c75ba5987dc8333c664dae50c3e12174f736a506b4aa15';          BINARY_URL='https://github.com/adoptium/temurin17-binaries/releases/download/jdk-17.0.8%2B7/OpenJDK17U-jre_aarch64_linux_hotspot_17.0.8_7.tar.gz';          ;;        armhf|arm)          ESUM='20fa06a86e1647f5997c511dd19e4d1c9839d2500f835973fc9b3c86b87030a0';          BINARY_URL='https://github.com/adoptium/temurin17-binaries/releases/download/jdk-17.0.8%2B7/OpenJDK17U-jre_arm_linux_hotspot_17.0.8_7.tar.gz';          ;;        ppc64el|powerpc:common64)          ESUM='1cf2cf7dca98c74860799b162b9f2eeaaf1ad1e78f5cb7479fe7bd1ccfea3227';          BINARY_URL='https://github.com/adoptium/temurin17-binaries/releases/download/jdk-17.0.8%2B7/OpenJDK17U-jre_ppc64le_linux_hotspot_17.0.8_7.tar.gz';          ;;        s390x|s390:64-bit)          ESUM='4df17b19510864651c1d620baaf13766a448d43ee7848ea9ff69db10d26467b6';          BINARY_URL='https://github.com/adoptium/temurin17-binaries/releases/download/jdk-17.0.8%2B7/OpenJDK17U-jre_s390x_linux_hotspot_17.0.8_7.tar.gz';          ;;        amd64|i386:x86-64)          ESUM='dddbb5f817a77445711528a414678806b00b83c92701fe595c50cdb207758ae9';          BINARY_URL='https://github.com/adoptium/temurin17-binaries/releases/download/jdk-17.0.8%2B7/OpenJDK17U-jre_x64_linux_hotspot_17.0.8_7.tar.gz';          ;;        *)          echo "Unsupported arch: ${ARCH}";          exit 1;          ;;     esac; 	  wget -O /tmp/openjdk.tar.gz ${BINARY_URL}; 	  echo "${ESUM} */tmp/openjdk.tar.gz" | sha256sum -c -; 	  mkdir -p "$JAVA_HOME"; 	  tar --extract 	      --file /tmp/openjdk.tar.gz 	      --directory "$JAVA_HOME" 	      --strip-components 1 	      --no-same-owner 	  ;     rm -f /tmp/openjdk.tar.gz ${JAVA_HOME}/lib/src.zip;     find "$JAVA_HOME/lib" -name '*.so' -exec dirname '{}' ';' | sort -u > /etc/ld.so.conf.d/docker-openjdk.conf;     ldconfig;     java -Xshare:dump;
# Tue, 08 Aug 2023 19:24:35 GMT
RUN echo Verifying install ...     && fileEncoding="$(echo 'System.out.println(System.getProperty("file.encoding"))' | jshell -s -)"; [ "$fileEncoding" = 'UTF-8' ]; rm -rf ~/.java     && echo java --version && java --version     && echo Complete.
# Tue, 08 Aug 2023 19:24:35 GMT
COPY file:0673fe0a4a716089bcd96321c8de60149aea8a94ae7c4ba827ecc4a74a9789a3 in / 
# Tue, 08 Aug 2023 19:24:35 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Tue, 08 Aug 2023 21:18:50 GMT
ENV CATALINA_HOME=/usr/local/tomcat
# Tue, 08 Aug 2023 21:18:50 GMT
ENV PATH=/usr/local/tomcat/bin:/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 08 Aug 2023 21:18:51 GMT
RUN mkdir -p "$CATALINA_HOME"
# Tue, 08 Aug 2023 21:18:51 GMT
WORKDIR /usr/local/tomcat
# Tue, 08 Aug 2023 21:18:51 GMT
ENV TOMCAT_NATIVE_LIBDIR=/usr/local/tomcat/native-jni-lib
# Tue, 08 Aug 2023 21:18:51 GMT
ENV LD_LIBRARY_PATH=/usr/local/tomcat/native-jni-lib
# Tue, 08 Aug 2023 21:25:33 GMT
ENV GPG_KEYS=05AB33110949707C93A279E3D3EFE6B686867BA6 07E48665A34DCAFAE522E5E6266191C37C037D42 47309207D818FFD8DCD3F83F1931D684307A10A5 541FBE7D8F78B25E055DDEE13C370389288584E7 5C3C5F3E314C866292F359A8F3AD5C94A67F707E 765908099ACF92702C7D949BFA0C35EA8AA299F1 79F7026C690BAA50B92CD8B66A3AD3F4F22C4FED 9BA44C2621385CB966EBA586F72C284D731FABEE A27677289986DB50844682F8ACB77FC2E86E29AC A9C5DF4D22E99998D9875A5110C01C5A2F6059E7 DCFD35E0BF8CA7344752DE8B6FB21E8933C60243 F3A04C595DB5B6A5F1ECA43E3B7BBB100D811BBE F7DA48BB64BCB84ECBA7EE6935CD23C10D498E23
# Tue, 08 Aug 2023 21:25:33 GMT
ENV TOMCAT_MAJOR=8
# Tue, 08 Aug 2023 21:25:33 GMT
ENV TOMCAT_VERSION=8.5.91
# Tue, 08 Aug 2023 21:25:33 GMT
ENV TOMCAT_SHA512=9e6770e9c9c3b630011c0f0e320b31bb0ea3700d52247a12d544ea25f9ee4d93613ad6ccb7939f97fb05e1760978a7547eccb16352d73fa28886134ba58f3f8c
# Tue, 08 Aug 2023 21:25:34 GMT
COPY dir:975045cea72de9ce0815a797d605e045950eca82d3ec4f8dfe035804a38a3de1 in /usr/local/tomcat 
# Tue, 08 Aug 2023 21:25:37 GMT
RUN set -eux; 	apt-get update; 	xargs -rt apt-get install -y --no-install-recommends < "$TOMCAT_NATIVE_LIBDIR/.dependencies.txt"; 	rm -rf /var/lib/apt/lists/*
# Tue, 08 Aug 2023 21:25:38 GMT
RUN set -eux; 	nativeLines="$(catalina.sh configtest 2>&1)"; 	nativeLines="$(echo "$nativeLines" | grep 'Apache Tomcat Native')"; 	nativeLines="$(echo "$nativeLines" | sort -u)"; 	if ! echo "$nativeLines" | grep -E 'INFO: Loaded( APR based)? Apache Tomcat Native library' >&2; then 		echo >&2 "$nativeLines"; 		exit 1; 	fi
# Tue, 08 Aug 2023 21:25:39 GMT
EXPOSE 8080
# Sat, 12 Aug 2023 00:21:50 GMT
ENTRYPOINT []
# Sat, 12 Aug 2023 00:21:50 GMT
CMD ["catalina.sh" "run"]
```

-	Layers:
	-	`sha256:9d19ee268e0d7bcf6716e6658ee1b0384a71d6f2f9aa1ae2085610cf7c7b316f`  
		Last Modified: Wed, 28 Jun 2023 11:50:41 GMT  
		Size: 30.4 MB (30431229 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1ccd2d5dafe8ee2e15a3fbe193041c068fdadeda1797014f93048fa9a300e06e`  
		Last Modified: Thu, 03 Aug 2023 02:42:45 GMT  
		Size: 17.5 MB (17456332 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2e8d00d3cd21ab1461905d090b64208447c8d4ded1b3f5e97afe50eaab0948bd`  
		Last Modified: Tue, 08 Aug 2023 19:33:24 GMT  
		Size: 47.2 MB (47209358 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:08bc8ffa8e991537c3aefdccb53f3a681735303cf5f851a861dba3835456ceef`  
		Last Modified: Tue, 08 Aug 2023 19:33:17 GMT  
		Size: 161.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:77a5ebc0e652dba949dc337249e9181f2a0103841f91c7cacf3225966748ca45`  
		Last Modified: Tue, 08 Aug 2023 19:33:18 GMT  
		Size: 667.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c2823590b4a76e9365555683c26fd09ad1fe2ab92d2102d4a9a3ef9f46316795`  
		Last Modified: Tue, 08 Aug 2023 21:32:53 GMT  
		Size: 172.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4c17427a843c4b6a2f5e2fb2f7ce1c740e0ed2f33811f3182ab886fe2ba347d1`  
		Last Modified: Tue, 08 Aug 2023 21:39:00 GMT  
		Size: 11.3 MB (11323648 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b1583c70692bf42f7746eff6de742e090c7920e93a870fb19eff4f90cca02114`  
		Last Modified: Tue, 08 Aug 2023 21:38:59 GMT  
		Size: 458.3 KB (458348 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7b5245945e0cf2ed17e648f362178b10e81c62613c104cc96777e15debc92415`  
		Last Modified: Tue, 08 Aug 2023 21:38:59 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `tomcat:8-jre17-temurin-jammy` - linux; arm variant v7

```console
$ docker pull tomcat@sha256:d0715c01bd6f7bec0569ed4f74f032a4f64b7b439a11111172313b6cd844cbe0
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **101.0 MB (101019897 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b142cb44d3ab98caec2afe0a8eb2f74a07391ac37b6fa5ef76cd218d31adc0f2`
-	Default Command: `["catalina.sh","run"]`

```dockerfile
# Wed, 28 Jun 2023 08:41:15 GMT
ARG RELEASE
# Wed, 28 Jun 2023 08:41:15 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Wed, 28 Jun 2023 08:41:15 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Wed, 28 Jun 2023 08:41:15 GMT
LABEL org.opencontainers.image.version=22.04
# Wed, 28 Jun 2023 08:41:18 GMT
ADD file:c13f43a31510c7a4eaa7e4ca90e4f973b19895658b1f9993cab5f93979d4e2dc in / 
# Wed, 28 Jun 2023 08:41:18 GMT
CMD ["/bin/bash"]
# Tue, 04 Jul 2023 20:09:30 GMT
ENV JAVA_HOME=/opt/java/openjdk
# Tue, 04 Jul 2023 20:09:30 GMT
ENV PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 04 Jul 2023 20:09:30 GMT
ENV LANG=en_US.UTF-8 LANGUAGE=en_US:en LC_ALL=en_US.UTF-8
# Tue, 08 Aug 2023 19:01:27 GMT
RUN apt-get update     && DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends tzdata curl wget ca-certificates fontconfig locales p11-kit binutils     && echo "en_US.UTF-8 UTF-8" >> /etc/locale.gen     && locale-gen en_US.UTF-8     && rm -rf /var/lib/apt/lists/*
# Tue, 08 Aug 2023 19:01:27 GMT
ENV JAVA_VERSION=jdk-17.0.8+7
# Tue, 08 Aug 2023 19:01:56 GMT
RUN set -eux;     ARCH="$(dpkg --print-architecture)";     case "${ARCH}" in        aarch64|arm64)          ESUM='42525ae2951a669803c75ba5987dc8333c664dae50c3e12174f736a506b4aa15';          BINARY_URL='https://github.com/adoptium/temurin17-binaries/releases/download/jdk-17.0.8%2B7/OpenJDK17U-jre_aarch64_linux_hotspot_17.0.8_7.tar.gz';          ;;        armhf|arm)          ESUM='20fa06a86e1647f5997c511dd19e4d1c9839d2500f835973fc9b3c86b87030a0';          BINARY_URL='https://github.com/adoptium/temurin17-binaries/releases/download/jdk-17.0.8%2B7/OpenJDK17U-jre_arm_linux_hotspot_17.0.8_7.tar.gz';          ;;        ppc64el|powerpc:common64)          ESUM='1cf2cf7dca98c74860799b162b9f2eeaaf1ad1e78f5cb7479fe7bd1ccfea3227';          BINARY_URL='https://github.com/adoptium/temurin17-binaries/releases/download/jdk-17.0.8%2B7/OpenJDK17U-jre_ppc64le_linux_hotspot_17.0.8_7.tar.gz';          ;;        s390x|s390:64-bit)          ESUM='4df17b19510864651c1d620baaf13766a448d43ee7848ea9ff69db10d26467b6';          BINARY_URL='https://github.com/adoptium/temurin17-binaries/releases/download/jdk-17.0.8%2B7/OpenJDK17U-jre_s390x_linux_hotspot_17.0.8_7.tar.gz';          ;;        amd64|i386:x86-64)          ESUM='dddbb5f817a77445711528a414678806b00b83c92701fe595c50cdb207758ae9';          BINARY_URL='https://github.com/adoptium/temurin17-binaries/releases/download/jdk-17.0.8%2B7/OpenJDK17U-jre_x64_linux_hotspot_17.0.8_7.tar.gz';          ;;        *)          echo "Unsupported arch: ${ARCH}";          exit 1;          ;;     esac; 	  wget -O /tmp/openjdk.tar.gz ${BINARY_URL}; 	  echo "${ESUM} */tmp/openjdk.tar.gz" | sha256sum -c -; 	  mkdir -p "$JAVA_HOME"; 	  tar --extract 	      --file /tmp/openjdk.tar.gz 	      --directory "$JAVA_HOME" 	      --strip-components 1 	      --no-same-owner 	  ;     rm -f /tmp/openjdk.tar.gz ${JAVA_HOME}/lib/src.zip;     find "$JAVA_HOME/lib" -name '*.so' -exec dirname '{}' ';' | sort -u > /etc/ld.so.conf.d/docker-openjdk.conf;     ldconfig;     java -Xshare:dump;
# Tue, 08 Aug 2023 19:01:57 GMT
RUN echo Verifying install ...     && fileEncoding="$(echo 'System.out.println(System.getProperty("file.encoding"))' | jshell -s -)"; [ "$fileEncoding" = 'UTF-8' ]; rm -rf ~/.java     && echo java --version && java --version     && echo Complete.
# Mon, 14 Aug 2023 18:09:53 GMT
COPY file:8b8864b3e02a33a579dc216fd51b28a6047bc8eeaa03045b258980fe0cf7fcb3 in /__cacert_entrypoint.sh 
# Mon, 14 Aug 2023 18:09:53 GMT
ENTRYPOINT ["/__cacert_entrypoint.sh"]
# Mon, 14 Aug 2023 18:51:46 GMT
ENV CATALINA_HOME=/usr/local/tomcat
# Mon, 14 Aug 2023 18:51:46 GMT
ENV PATH=/usr/local/tomcat/bin:/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Mon, 14 Aug 2023 18:51:47 GMT
RUN mkdir -p "$CATALINA_HOME"
# Mon, 14 Aug 2023 18:51:47 GMT
WORKDIR /usr/local/tomcat
# Mon, 14 Aug 2023 18:51:47 GMT
ENV TOMCAT_NATIVE_LIBDIR=/usr/local/tomcat/native-jni-lib
# Mon, 14 Aug 2023 18:51:47 GMT
ENV LD_LIBRARY_PATH=/usr/local/tomcat/native-jni-lib
# Mon, 14 Aug 2023 18:58:14 GMT
ENV GPG_KEYS=05AB33110949707C93A279E3D3EFE6B686867BA6 07E48665A34DCAFAE522E5E6266191C37C037D42 47309207D818FFD8DCD3F83F1931D684307A10A5 541FBE7D8F78B25E055DDEE13C370389288584E7 5C3C5F3E314C866292F359A8F3AD5C94A67F707E 765908099ACF92702C7D949BFA0C35EA8AA299F1 79F7026C690BAA50B92CD8B66A3AD3F4F22C4FED 9BA44C2621385CB966EBA586F72C284D731FABEE A27677289986DB50844682F8ACB77FC2E86E29AC A9C5DF4D22E99998D9875A5110C01C5A2F6059E7 DCFD35E0BF8CA7344752DE8B6FB21E8933C60243 F3A04C595DB5B6A5F1ECA43E3B7BBB100D811BBE F7DA48BB64BCB84ECBA7EE6935CD23C10D498E23
# Mon, 14 Aug 2023 18:58:14 GMT
ENV TOMCAT_MAJOR=8
# Mon, 14 Aug 2023 18:58:14 GMT
ENV TOMCAT_VERSION=8.5.91
# Mon, 14 Aug 2023 18:58:14 GMT
ENV TOMCAT_SHA512=9e6770e9c9c3b630011c0f0e320b31bb0ea3700d52247a12d544ea25f9ee4d93613ad6ccb7939f97fb05e1760978a7547eccb16352d73fa28886134ba58f3f8c
# Mon, 14 Aug 2023 18:58:15 GMT
COPY dir:207aca6dac97228587c59b3f4ee3e85a829c222b50d73a3950b8f59f125f4d76 in /usr/local/tomcat 
# Mon, 14 Aug 2023 18:58:20 GMT
RUN set -eux; 	apt-get update; 	xargs -rt apt-get install -y --no-install-recommends < "$TOMCAT_NATIVE_LIBDIR/.dependencies.txt"; 	rm -rf /var/lib/apt/lists/*
# Mon, 14 Aug 2023 18:58:21 GMT
RUN set -eux; 	nativeLines="$(catalina.sh configtest 2>&1)"; 	nativeLines="$(echo "$nativeLines" | grep 'Apache Tomcat Native')"; 	nativeLines="$(echo "$nativeLines" | sort -u)"; 	if ! echo "$nativeLines" | grep -E 'INFO: Loaded( APR based)? Apache Tomcat Native library' >&2; then 		echo >&2 "$nativeLines"; 		exit 1; 	fi
# Mon, 14 Aug 2023 18:58:21 GMT
EXPOSE 8080
# Mon, 14 Aug 2023 18:58:21 GMT
ENTRYPOINT []
# Mon, 14 Aug 2023 18:58:21 GMT
CMD ["catalina.sh" "run"]
```

-	Layers:
	-	`sha256:63b96265cfe95b9cec847027033d4226b783ecd042036f5c809a7386027f56b0`  
		Last Modified: Fri, 30 Jun 2023 02:08:02 GMT  
		Size: 27.0 MB (27026961 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:03fa46b0671072c68047e10f8c7e3ffe9a06840284e9e91967baa3a634b82942`  
		Last Modified: Tue, 08 Aug 2023 19:05:31 GMT  
		Size: 17.6 MB (17587022 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1cdefdabf9b237a15bba43d46b9a45b115a62f6228347761b66dea4db3bd2933`  
		Last Modified: Tue, 08 Aug 2023 19:06:19 GMT  
		Size: 44.7 MB (44718688 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c68298a8e3e0f0bd7f4031f081ab530e4d621ac9633a8771fd4f3ed1f3d752c8`  
		Last Modified: Tue, 08 Aug 2023 19:06:12 GMT  
		Size: 160.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3687f0f77ae5f58c56db16da25cfd3deb12c13eab29631101cbe02e8f9d6b5d9`  
		Last Modified: Mon, 14 Aug 2023 18:12:00 GMT  
		Size: 733.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:715effe9447ef1e11754f7cbef2f6cfbe5e0b1f5993a05e95a87924764a2e85f`  
		Last Modified: Mon, 14 Aug 2023 19:04:37 GMT  
		Size: 173.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5952670e2b58fbb7f6d9ffd76ffe693de87c880de2d766e40f35c4a4f84fc38f`  
		Last Modified: Mon, 14 Aug 2023 19:10:30 GMT  
		Size: 11.3 MB (11254826 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8e78a1fd8929551d8a868226aa71a5ab3c392c566ec58cea55dd33accb54ac09`  
		Last Modified: Mon, 14 Aug 2023 19:10:29 GMT  
		Size: 431.2 KB (431204 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2edc3ef7f4c4a0531e7311c47ea6f221aa213f6ff0b21a403e1336442c41a0eb`  
		Last Modified: Mon, 14 Aug 2023 19:10:29 GMT  
		Size: 130.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `tomcat:8-jre17-temurin-jammy` - linux; arm64 variant v8

```console
$ docker pull tomcat@sha256:f0c29882470d6b40230e14a8501d17eeac4b9fa62e621bb87c0cae725f5cf3e9
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **105.7 MB (105701146 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f84ded7054e6aba2c2fd843bc9b8ad6d6ac81062377ff924e3b8efb3d16dfa33`
-	Default Command: `["catalina.sh","run"]`

```dockerfile
# Wed, 28 Jun 2023 08:42:48 GMT
ARG RELEASE
# Wed, 28 Jun 2023 08:42:48 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Wed, 28 Jun 2023 08:42:48 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Wed, 28 Jun 2023 08:42:48 GMT
LABEL org.opencontainers.image.version=22.04
# Wed, 28 Jun 2023 08:42:50 GMT
ADD file:262490f82459c14632f5c9a6d6a5cf6c07b4f307e8fd380fa764662cda46e88f in / 
# Wed, 28 Jun 2023 08:42:50 GMT
CMD ["/bin/bash"]
# Tue, 04 Jul 2023 15:32:45 GMT
ENV JAVA_HOME=/opt/java/openjdk
# Tue, 04 Jul 2023 15:32:45 GMT
ENV PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 04 Jul 2023 15:32:45 GMT
ENV LANG=en_US.UTF-8 LANGUAGE=en_US:en LC_ALL=en_US.UTF-8
# Thu, 03 Aug 2023 01:08:59 GMT
RUN apt-get update     && DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends tzdata curl wget ca-certificates fontconfig locales p11-kit binutils     && echo "en_US.UTF-8 UTF-8" >> /etc/locale.gen     && locale-gen en_US.UTF-8     && rm -rf /var/lib/apt/lists/*
# Tue, 08 Aug 2023 19:42:25 GMT
ENV JAVA_VERSION=jdk-17.0.8+7
# Tue, 08 Aug 2023 19:42:52 GMT
RUN set -eux;     ARCH="$(dpkg --print-architecture)";     case "${ARCH}" in        aarch64|arm64)          ESUM='42525ae2951a669803c75ba5987dc8333c664dae50c3e12174f736a506b4aa15';          BINARY_URL='https://github.com/adoptium/temurin17-binaries/releases/download/jdk-17.0.8%2B7/OpenJDK17U-jre_aarch64_linux_hotspot_17.0.8_7.tar.gz';          ;;        armhf|arm)          ESUM='20fa06a86e1647f5997c511dd19e4d1c9839d2500f835973fc9b3c86b87030a0';          BINARY_URL='https://github.com/adoptium/temurin17-binaries/releases/download/jdk-17.0.8%2B7/OpenJDK17U-jre_arm_linux_hotspot_17.0.8_7.tar.gz';          ;;        ppc64el|powerpc:common64)          ESUM='1cf2cf7dca98c74860799b162b9f2eeaaf1ad1e78f5cb7479fe7bd1ccfea3227';          BINARY_URL='https://github.com/adoptium/temurin17-binaries/releases/download/jdk-17.0.8%2B7/OpenJDK17U-jre_ppc64le_linux_hotspot_17.0.8_7.tar.gz';          ;;        s390x|s390:64-bit)          ESUM='4df17b19510864651c1d620baaf13766a448d43ee7848ea9ff69db10d26467b6';          BINARY_URL='https://github.com/adoptium/temurin17-binaries/releases/download/jdk-17.0.8%2B7/OpenJDK17U-jre_s390x_linux_hotspot_17.0.8_7.tar.gz';          ;;        amd64|i386:x86-64)          ESUM='dddbb5f817a77445711528a414678806b00b83c92701fe595c50cdb207758ae9';          BINARY_URL='https://github.com/adoptium/temurin17-binaries/releases/download/jdk-17.0.8%2B7/OpenJDK17U-jre_x64_linux_hotspot_17.0.8_7.tar.gz';          ;;        *)          echo "Unsupported arch: ${ARCH}";          exit 1;          ;;     esac; 	  wget -O /tmp/openjdk.tar.gz ${BINARY_URL}; 	  echo "${ESUM} */tmp/openjdk.tar.gz" | sha256sum -c -; 	  mkdir -p "$JAVA_HOME"; 	  tar --extract 	      --file /tmp/openjdk.tar.gz 	      --directory "$JAVA_HOME" 	      --strip-components 1 	      --no-same-owner 	  ;     rm -f /tmp/openjdk.tar.gz ${JAVA_HOME}/lib/src.zip;     find "$JAVA_HOME/lib" -name '*.so' -exec dirname '{}' ';' | sort -u > /etc/ld.so.conf.d/docker-openjdk.conf;     ldconfig;     java -Xshare:dump;
# Tue, 08 Aug 2023 19:42:53 GMT
RUN echo Verifying install ...     && fileEncoding="$(echo 'System.out.println(System.getProperty("file.encoding"))' | jshell -s -)"; [ "$fileEncoding" = 'UTF-8' ]; rm -rf ~/.java     && echo java --version && java --version     && echo Complete.
# Mon, 14 Aug 2023 18:09:31 GMT
COPY file:8b8864b3e02a33a579dc216fd51b28a6047bc8eeaa03045b258980fe0cf7fcb3 in /__cacert_entrypoint.sh 
# Mon, 14 Aug 2023 18:09:31 GMT
ENTRYPOINT ["/__cacert_entrypoint.sh"]
# Mon, 14 Aug 2023 20:03:40 GMT
ENV CATALINA_HOME=/usr/local/tomcat
# Mon, 14 Aug 2023 20:03:40 GMT
ENV PATH=/usr/local/tomcat/bin:/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Mon, 14 Aug 2023 20:03:40 GMT
RUN mkdir -p "$CATALINA_HOME"
# Mon, 14 Aug 2023 20:03:40 GMT
WORKDIR /usr/local/tomcat
# Mon, 14 Aug 2023 20:03:40 GMT
ENV TOMCAT_NATIVE_LIBDIR=/usr/local/tomcat/native-jni-lib
# Mon, 14 Aug 2023 20:03:41 GMT
ENV LD_LIBRARY_PATH=/usr/local/tomcat/native-jni-lib
# Mon, 14 Aug 2023 20:09:52 GMT
ENV GPG_KEYS=05AB33110949707C93A279E3D3EFE6B686867BA6 07E48665A34DCAFAE522E5E6266191C37C037D42 47309207D818FFD8DCD3F83F1931D684307A10A5 541FBE7D8F78B25E055DDEE13C370389288584E7 5C3C5F3E314C866292F359A8F3AD5C94A67F707E 765908099ACF92702C7D949BFA0C35EA8AA299F1 79F7026C690BAA50B92CD8B66A3AD3F4F22C4FED 9BA44C2621385CB966EBA586F72C284D731FABEE A27677289986DB50844682F8ACB77FC2E86E29AC A9C5DF4D22E99998D9875A5110C01C5A2F6059E7 DCFD35E0BF8CA7344752DE8B6FB21E8933C60243 F3A04C595DB5B6A5F1ECA43E3B7BBB100D811BBE F7DA48BB64BCB84ECBA7EE6935CD23C10D498E23
# Mon, 14 Aug 2023 20:09:52 GMT
ENV TOMCAT_MAJOR=8
# Mon, 14 Aug 2023 20:09:52 GMT
ENV TOMCAT_VERSION=8.5.91
# Mon, 14 Aug 2023 20:09:53 GMT
ENV TOMCAT_SHA512=9e6770e9c9c3b630011c0f0e320b31bb0ea3700d52247a12d544ea25f9ee4d93613ad6ccb7939f97fb05e1760978a7547eccb16352d73fa28886134ba58f3f8c
# Mon, 14 Aug 2023 20:09:53 GMT
COPY dir:fbc1f013162a72e13d69aa8494a3eb50ec48e767d74c314a2dd591937f7ff161 in /usr/local/tomcat 
# Mon, 14 Aug 2023 20:09:56 GMT
RUN set -eux; 	apt-get update; 	xargs -rt apt-get install -y --no-install-recommends < "$TOMCAT_NATIVE_LIBDIR/.dependencies.txt"; 	rm -rf /var/lib/apt/lists/*
# Mon, 14 Aug 2023 20:09:57 GMT
RUN set -eux; 	nativeLines="$(catalina.sh configtest 2>&1)"; 	nativeLines="$(echo "$nativeLines" | grep 'Apache Tomcat Native')"; 	nativeLines="$(echo "$nativeLines" | sort -u)"; 	if ! echo "$nativeLines" | grep -E 'INFO: Loaded( APR based)? Apache Tomcat Native library' >&2; then 		echo >&2 "$nativeLines"; 		exit 1; 	fi
# Mon, 14 Aug 2023 20:09:57 GMT
EXPOSE 8080
# Mon, 14 Aug 2023 20:09:57 GMT
ENTRYPOINT []
# Mon, 14 Aug 2023 20:09:57 GMT
CMD ["catalina.sh" "run"]
```

-	Layers:
	-	`sha256:ac34a2e0269ced3acc355be706239ee0f3f1e73a035c40dd2fac74827164ee53`  
		Last Modified: Wed, 28 Jun 2023 23:23:40 GMT  
		Size: 28.4 MB (28391011 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4df65dff856d09c8b168dd7068823e6f97f3afb0fc6276b56a61cfbc2fc700d4`  
		Last Modified: Thu, 03 Aug 2023 01:12:32 GMT  
		Size: 18.9 MB (18858729 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b113754ab3194cfcda1ea6102eee0f1430256f28cb13fe17439779ebeba8c4a5`  
		Last Modified: Tue, 08 Aug 2023 19:48:50 GMT  
		Size: 46.7 MB (46660687 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0fe6729cede2ddb3b3fdcaf62f9f920074e9f805d07224010a6753482377b86d`  
		Last Modified: Tue, 08 Aug 2023 19:48:45 GMT  
		Size: 159.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:997856411f95501e35b81f436bfbb355adec054d1f7709093ae4fd2114c6c35b`  
		Last Modified: Mon, 14 Aug 2023 18:13:54 GMT  
		Size: 733.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a4a415ed118dd1e239876257ba77d50b29e9a5818cc9952a547588df12624af0`  
		Last Modified: Mon, 14 Aug 2023 20:16:31 GMT  
		Size: 173.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e225fdbc253ea3c6086f2f1bbad39054a530efacdd0c12f7556209b46538599c`  
		Last Modified: Mon, 14 Aug 2023 20:22:38 GMT  
		Size: 11.3 MB (11331147 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fae91625f804f424e324f4700c0ade5d07444bc810b74b3d28921e5c4bb217d8`  
		Last Modified: Mon, 14 Aug 2023 20:22:37 GMT  
		Size: 458.4 KB (458377 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e37913a6f49d7603b1a5515efde98bab8a6d260c2f99b4ba86bda582d311d139`  
		Last Modified: Mon, 14 Aug 2023 20:22:37 GMT  
		Size: 130.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `tomcat:8-jre17-temurin-jammy` - linux; ppc64le

```console
$ docker pull tomcat@sha256:202f85609975c3766b2a7dc44a63349144afa745640c4351e57fb2f00cce7e23
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **113.3 MB (113335832 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a242e84ff47a3b109f7a3c114db1f4d3062f797b34e30a0731dc26b37af314bf`
-	Default Command: `["catalina.sh","run"]`

```dockerfile
# Wed, 28 Jun 2023 08:45:53 GMT
ARG RELEASE
# Wed, 28 Jun 2023 08:45:53 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Wed, 28 Jun 2023 08:45:53 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Wed, 28 Jun 2023 08:45:54 GMT
LABEL org.opencontainers.image.version=22.04
# Wed, 28 Jun 2023 08:45:56 GMT
ADD file:8c2fc380378944326d602742fde0e30458cd3e82012847b0f7e09c7184bfd135 in / 
# Wed, 28 Jun 2023 08:45:57 GMT
CMD ["/bin/bash"]
# Wed, 05 Jul 2023 00:18:18 GMT
ENV JAVA_HOME=/opt/java/openjdk
# Wed, 05 Jul 2023 00:18:18 GMT
ENV PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 05 Jul 2023 00:18:19 GMT
ENV LANG=en_US.UTF-8 LANGUAGE=en_US:en LC_ALL=en_US.UTF-8
# Tue, 08 Aug 2023 19:25:06 GMT
RUN apt-get update     && DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends tzdata curl wget ca-certificates fontconfig locales p11-kit binutils     && echo "en_US.UTF-8 UTF-8" >> /etc/locale.gen     && locale-gen en_US.UTF-8     && rm -rf /var/lib/apt/lists/*
# Tue, 08 Aug 2023 19:25:11 GMT
ENV JAVA_VERSION=jdk-17.0.8+7
# Tue, 08 Aug 2023 19:26:40 GMT
RUN set -eux;     ARCH="$(dpkg --print-architecture)";     case "${ARCH}" in        aarch64|arm64)          ESUM='42525ae2951a669803c75ba5987dc8333c664dae50c3e12174f736a506b4aa15';          BINARY_URL='https://github.com/adoptium/temurin17-binaries/releases/download/jdk-17.0.8%2B7/OpenJDK17U-jre_aarch64_linux_hotspot_17.0.8_7.tar.gz';          ;;        armhf|arm)          ESUM='20fa06a86e1647f5997c511dd19e4d1c9839d2500f835973fc9b3c86b87030a0';          BINARY_URL='https://github.com/adoptium/temurin17-binaries/releases/download/jdk-17.0.8%2B7/OpenJDK17U-jre_arm_linux_hotspot_17.0.8_7.tar.gz';          ;;        ppc64el|powerpc:common64)          ESUM='1cf2cf7dca98c74860799b162b9f2eeaaf1ad1e78f5cb7479fe7bd1ccfea3227';          BINARY_URL='https://github.com/adoptium/temurin17-binaries/releases/download/jdk-17.0.8%2B7/OpenJDK17U-jre_ppc64le_linux_hotspot_17.0.8_7.tar.gz';          ;;        s390x|s390:64-bit)          ESUM='4df17b19510864651c1d620baaf13766a448d43ee7848ea9ff69db10d26467b6';          BINARY_URL='https://github.com/adoptium/temurin17-binaries/releases/download/jdk-17.0.8%2B7/OpenJDK17U-jre_s390x_linux_hotspot_17.0.8_7.tar.gz';          ;;        amd64|i386:x86-64)          ESUM='dddbb5f817a77445711528a414678806b00b83c92701fe595c50cdb207758ae9';          BINARY_URL='https://github.com/adoptium/temurin17-binaries/releases/download/jdk-17.0.8%2B7/OpenJDK17U-jre_x64_linux_hotspot_17.0.8_7.tar.gz';          ;;        *)          echo "Unsupported arch: ${ARCH}";          exit 1;          ;;     esac; 	  wget -O /tmp/openjdk.tar.gz ${BINARY_URL}; 	  echo "${ESUM} */tmp/openjdk.tar.gz" | sha256sum -c -; 	  mkdir -p "$JAVA_HOME"; 	  tar --extract 	      --file /tmp/openjdk.tar.gz 	      --directory "$JAVA_HOME" 	      --strip-components 1 	      --no-same-owner 	  ;     rm -f /tmp/openjdk.tar.gz ${JAVA_HOME}/lib/src.zip;     find "$JAVA_HOME/lib" -name '*.so' -exec dirname '{}' ';' | sort -u > /etc/ld.so.conf.d/docker-openjdk.conf;     ldconfig;     java -Xshare:dump;
# Tue, 08 Aug 2023 19:26:44 GMT
RUN echo Verifying install ...     && fileEncoding="$(echo 'System.out.println(System.getProperty("file.encoding"))' | jshell -s -)"; [ "$fileEncoding" = 'UTF-8' ]; rm -rf ~/.java     && echo java --version && java --version     && echo Complete.
# Mon, 14 Aug 2023 18:10:26 GMT
COPY file:8b8864b3e02a33a579dc216fd51b28a6047bc8eeaa03045b258980fe0cf7fcb3 in /__cacert_entrypoint.sh 
# Mon, 14 Aug 2023 18:10:27 GMT
ENTRYPOINT ["/__cacert_entrypoint.sh"]
# Mon, 14 Aug 2023 19:39:05 GMT
ENV CATALINA_HOME=/usr/local/tomcat
# Mon, 14 Aug 2023 19:39:06 GMT
ENV PATH=/usr/local/tomcat/bin:/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Mon, 14 Aug 2023 19:39:07 GMT
RUN mkdir -p "$CATALINA_HOME"
# Mon, 14 Aug 2023 19:39:08 GMT
WORKDIR /usr/local/tomcat
# Mon, 14 Aug 2023 19:39:08 GMT
ENV TOMCAT_NATIVE_LIBDIR=/usr/local/tomcat/native-jni-lib
# Mon, 14 Aug 2023 19:39:08 GMT
ENV LD_LIBRARY_PATH=/usr/local/tomcat/native-jni-lib
# Mon, 14 Aug 2023 19:57:19 GMT
ENV GPG_KEYS=05AB33110949707C93A279E3D3EFE6B686867BA6 07E48665A34DCAFAE522E5E6266191C37C037D42 47309207D818FFD8DCD3F83F1931D684307A10A5 541FBE7D8F78B25E055DDEE13C370389288584E7 5C3C5F3E314C866292F359A8F3AD5C94A67F707E 765908099ACF92702C7D949BFA0C35EA8AA299F1 79F7026C690BAA50B92CD8B66A3AD3F4F22C4FED 9BA44C2621385CB966EBA586F72C284D731FABEE A27677289986DB50844682F8ACB77FC2E86E29AC A9C5DF4D22E99998D9875A5110C01C5A2F6059E7 DCFD35E0BF8CA7344752DE8B6FB21E8933C60243 F3A04C595DB5B6A5F1ECA43E3B7BBB100D811BBE F7DA48BB64BCB84ECBA7EE6935CD23C10D498E23
# Mon, 14 Aug 2023 19:57:20 GMT
ENV TOMCAT_MAJOR=8
# Mon, 14 Aug 2023 19:57:21 GMT
ENV TOMCAT_VERSION=8.5.91
# Mon, 14 Aug 2023 19:57:21 GMT
ENV TOMCAT_SHA512=9e6770e9c9c3b630011c0f0e320b31bb0ea3700d52247a12d544ea25f9ee4d93613ad6ccb7939f97fb05e1760978a7547eccb16352d73fa28886134ba58f3f8c
# Mon, 14 Aug 2023 19:57:22 GMT
COPY dir:c655389f7ed905c22686e5af3e5209dee0eec83e222078002079020ba6dc2951 in /usr/local/tomcat 
# Mon, 14 Aug 2023 19:57:32 GMT
RUN set -eux; 	apt-get update; 	xargs -rt apt-get install -y --no-install-recommends < "$TOMCAT_NATIVE_LIBDIR/.dependencies.txt"; 	rm -rf /var/lib/apt/lists/*
# Mon, 14 Aug 2023 19:57:36 GMT
RUN set -eux; 	nativeLines="$(catalina.sh configtest 2>&1)"; 	nativeLines="$(echo "$nativeLines" | grep 'Apache Tomcat Native')"; 	nativeLines="$(echo "$nativeLines" | sort -u)"; 	if ! echo "$nativeLines" | grep -E 'INFO: Loaded( APR based)? Apache Tomcat Native library' >&2; then 		echo >&2 "$nativeLines"; 		exit 1; 	fi
# Mon, 14 Aug 2023 19:57:36 GMT
EXPOSE 8080
# Mon, 14 Aug 2023 19:57:37 GMT
ENTRYPOINT []
# Mon, 14 Aug 2023 19:57:37 GMT
CMD ["catalina.sh" "run"]
```

-	Layers:
	-	`sha256:7faa46ce6b6f5c34485980029504c3995e38149d0bca67d8b976c5dbb3673644`  
		Last Modified: Tue, 04 Jul 2023 04:42:31 GMT  
		Size: 35.7 MB (35711469 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5db77a9bc80a636be0a061681aa78957c506eea6993305fe871da82fd4a2d8e5`  
		Last Modified: Tue, 08 Aug 2023 19:34:25 GMT  
		Size: 18.7 MB (18729537 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e7209170f5ee5b1f6b7430a41687d0b4623dd6a45b90c174d760fe2464c461f6`  
		Last Modified: Tue, 08 Aug 2023 19:35:58 GMT  
		Size: 47.1 MB (47053226 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:294b37a4c64d6b60d80d6f60fa26991d5bc87b7fefd46bd48b4195bfd12f8630`  
		Last Modified: Tue, 08 Aug 2023 19:35:46 GMT  
		Size: 160.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5b5de702898874688381ecd4779b9d0d8df8abdccef888811fc78321518172b1`  
		Last Modified: Mon, 14 Aug 2023 18:16:15 GMT  
		Size: 734.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:789c4731a70151a8057bdb2a94e968ce6891226c03ec191bb897bf3d8bc12d94`  
		Last Modified: Mon, 14 Aug 2023 20:12:10 GMT  
		Size: 172.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3ec3826b36677db4f6502ff91dab098f1b851b23519886125663bf3a2f9cbb42`  
		Last Modified: Mon, 14 Aug 2023 20:21:28 GMT  
		Size: 11.4 MB (11350896 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:07a6d13b384c49347dde0ed1f8b046e643412c84150bf98e19808bd77fbd9266`  
		Last Modified: Mon, 14 Aug 2023 20:21:27 GMT  
		Size: 489.5 KB (489508 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1ffaff62bb809d6ccc0592dd2da75bbfa76224bd090f3922e4a611c9baf690b7`  
		Last Modified: Mon, 14 Aug 2023 20:21:27 GMT  
		Size: 130.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `tomcat:8-jre17-temurin-jammy` - linux; s390x

```console
$ docker pull tomcat@sha256:6e3ef016168e8e1e496895709b4a70519cbd988044c8503f81338bfcdd748fb5
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **101.5 MB (101539684 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:82a65202cd97ff50addf7ca2da993f7695e7d5d65bdabcdfa8f85eeeb56b76f3`
-	Default Command: `["catalina.sh","run"]`

```dockerfile
# Wed, 28 Jun 2023 08:53:20 GMT
ARG RELEASE
# Wed, 28 Jun 2023 08:53:20 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Wed, 28 Jun 2023 08:53:20 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Wed, 28 Jun 2023 08:53:20 GMT
LABEL org.opencontainers.image.version=22.04
# Wed, 28 Jun 2023 08:53:22 GMT
ADD file:fa0aef35be7808c8fd6751a52bdec4dd81057e2fcaa075c547a1db53640dae9a in / 
# Wed, 28 Jun 2023 08:53:22 GMT
CMD ["/bin/bash"]
# Tue, 04 Jul 2023 16:24:17 GMT
ENV JAVA_HOME=/opt/java/openjdk
# Tue, 04 Jul 2023 16:24:18 GMT
ENV PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 04 Jul 2023 16:24:18 GMT
ENV LANG=en_US.UTF-8 LANGUAGE=en_US:en LC_ALL=en_US.UTF-8
# Tue, 08 Aug 2023 19:44:31 GMT
RUN apt-get update     && DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends tzdata curl wget ca-certificates fontconfig locales p11-kit binutils     && echo "en_US.UTF-8 UTF-8" >> /etc/locale.gen     && locale-gen en_US.UTF-8     && rm -rf /var/lib/apt/lists/*
# Tue, 08 Aug 2023 19:44:32 GMT
ENV JAVA_VERSION=jdk-17.0.8+7
# Tue, 08 Aug 2023 19:45:13 GMT
RUN set -eux;     ARCH="$(dpkg --print-architecture)";     case "${ARCH}" in        aarch64|arm64)          ESUM='42525ae2951a669803c75ba5987dc8333c664dae50c3e12174f736a506b4aa15';          BINARY_URL='https://github.com/adoptium/temurin17-binaries/releases/download/jdk-17.0.8%2B7/OpenJDK17U-jre_aarch64_linux_hotspot_17.0.8_7.tar.gz';          ;;        armhf|arm)          ESUM='20fa06a86e1647f5997c511dd19e4d1c9839d2500f835973fc9b3c86b87030a0';          BINARY_URL='https://github.com/adoptium/temurin17-binaries/releases/download/jdk-17.0.8%2B7/OpenJDK17U-jre_arm_linux_hotspot_17.0.8_7.tar.gz';          ;;        ppc64el|powerpc:common64)          ESUM='1cf2cf7dca98c74860799b162b9f2eeaaf1ad1e78f5cb7479fe7bd1ccfea3227';          BINARY_URL='https://github.com/adoptium/temurin17-binaries/releases/download/jdk-17.0.8%2B7/OpenJDK17U-jre_ppc64le_linux_hotspot_17.0.8_7.tar.gz';          ;;        s390x|s390:64-bit)          ESUM='4df17b19510864651c1d620baaf13766a448d43ee7848ea9ff69db10d26467b6';          BINARY_URL='https://github.com/adoptium/temurin17-binaries/releases/download/jdk-17.0.8%2B7/OpenJDK17U-jre_s390x_linux_hotspot_17.0.8_7.tar.gz';          ;;        amd64|i386:x86-64)          ESUM='dddbb5f817a77445711528a414678806b00b83c92701fe595c50cdb207758ae9';          BINARY_URL='https://github.com/adoptium/temurin17-binaries/releases/download/jdk-17.0.8%2B7/OpenJDK17U-jre_x64_linux_hotspot_17.0.8_7.tar.gz';          ;;        *)          echo "Unsupported arch: ${ARCH}";          exit 1;          ;;     esac; 	  wget -O /tmp/openjdk.tar.gz ${BINARY_URL}; 	  echo "${ESUM} */tmp/openjdk.tar.gz" | sha256sum -c -; 	  mkdir -p "$JAVA_HOME"; 	  tar --extract 	      --file /tmp/openjdk.tar.gz 	      --directory "$JAVA_HOME" 	      --strip-components 1 	      --no-same-owner 	  ;     rm -f /tmp/openjdk.tar.gz ${JAVA_HOME}/lib/src.zip;     find "$JAVA_HOME/lib" -name '*.so' -exec dirname '{}' ';' | sort -u > /etc/ld.so.conf.d/docker-openjdk.conf;     ldconfig;     java -Xshare:dump;
# Tue, 08 Aug 2023 19:45:15 GMT
RUN echo Verifying install ...     && fileEncoding="$(echo 'System.out.println(System.getProperty("file.encoding"))' | jshell -s -)"; [ "$fileEncoding" = 'UTF-8' ]; rm -rf ~/.java     && echo java --version && java --version     && echo Complete.
# Mon, 14 Aug 2023 18:10:06 GMT
COPY file:8b8864b3e02a33a579dc216fd51b28a6047bc8eeaa03045b258980fe0cf7fcb3 in /__cacert_entrypoint.sh 
# Mon, 14 Aug 2023 18:10:07 GMT
ENTRYPOINT ["/__cacert_entrypoint.sh"]
# Mon, 14 Aug 2023 18:46:19 GMT
ENV CATALINA_HOME=/usr/local/tomcat
# Mon, 14 Aug 2023 18:46:19 GMT
ENV PATH=/usr/local/tomcat/bin:/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Mon, 14 Aug 2023 18:46:20 GMT
RUN mkdir -p "$CATALINA_HOME"
# Mon, 14 Aug 2023 18:46:20 GMT
WORKDIR /usr/local/tomcat
# Mon, 14 Aug 2023 18:46:20 GMT
ENV TOMCAT_NATIVE_LIBDIR=/usr/local/tomcat/native-jni-lib
# Mon, 14 Aug 2023 18:46:20 GMT
ENV LD_LIBRARY_PATH=/usr/local/tomcat/native-jni-lib
# Mon, 14 Aug 2023 18:53:30 GMT
ENV GPG_KEYS=05AB33110949707C93A279E3D3EFE6B686867BA6 07E48665A34DCAFAE522E5E6266191C37C037D42 47309207D818FFD8DCD3F83F1931D684307A10A5 541FBE7D8F78B25E055DDEE13C370389288584E7 5C3C5F3E314C866292F359A8F3AD5C94A67F707E 765908099ACF92702C7D949BFA0C35EA8AA299F1 79F7026C690BAA50B92CD8B66A3AD3F4F22C4FED 9BA44C2621385CB966EBA586F72C284D731FABEE A27677289986DB50844682F8ACB77FC2E86E29AC A9C5DF4D22E99998D9875A5110C01C5A2F6059E7 DCFD35E0BF8CA7344752DE8B6FB21E8933C60243 F3A04C595DB5B6A5F1ECA43E3B7BBB100D811BBE F7DA48BB64BCB84ECBA7EE6935CD23C10D498E23
# Mon, 14 Aug 2023 18:53:30 GMT
ENV TOMCAT_MAJOR=8
# Mon, 14 Aug 2023 18:53:30 GMT
ENV TOMCAT_VERSION=8.5.91
# Mon, 14 Aug 2023 18:53:30 GMT
ENV TOMCAT_SHA512=9e6770e9c9c3b630011c0f0e320b31bb0ea3700d52247a12d544ea25f9ee4d93613ad6ccb7939f97fb05e1760978a7547eccb16352d73fa28886134ba58f3f8c
# Mon, 14 Aug 2023 18:53:31 GMT
COPY dir:e030267fb4202cb63130e6da824f54c408aef500a4343badd8bb89a16674fd6a in /usr/local/tomcat 
# Mon, 14 Aug 2023 18:53:34 GMT
RUN set -eux; 	apt-get update; 	xargs -rt apt-get install -y --no-install-recommends < "$TOMCAT_NATIVE_LIBDIR/.dependencies.txt"; 	rm -rf /var/lib/apt/lists/*
# Mon, 14 Aug 2023 18:53:35 GMT
RUN set -eux; 	nativeLines="$(catalina.sh configtest 2>&1)"; 	nativeLines="$(echo "$nativeLines" | grep 'Apache Tomcat Native')"; 	nativeLines="$(echo "$nativeLines" | sort -u)"; 	if ! echo "$nativeLines" | grep -E 'INFO: Loaded( APR based)? Apache Tomcat Native library' >&2; then 		echo >&2 "$nativeLines"; 		exit 1; 	fi
# Mon, 14 Aug 2023 18:53:36 GMT
EXPOSE 8080
# Mon, 14 Aug 2023 18:53:36 GMT
ENTRYPOINT []
# Mon, 14 Aug 2023 18:53:36 GMT
CMD ["catalina.sh" "run"]
```

-	Layers:
	-	`sha256:ce02ee0330980398d6a84a50abfa1a8c4d1cba27cbd7442b79f4aa1b1a14020d`  
		Last Modified: Tue, 04 Jul 2023 13:08:30 GMT  
		Size: 28.6 MB (28645696 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fbbc3ca72e7c73374cf85ad35ee727d2bb1efa34f74596d738251b2541906c7b`  
		Last Modified: Tue, 08 Aug 2023 19:47:44 GMT  
		Size: 17.3 MB (17255716 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ab2b5808d175613308c480033ee4e5f96b27e32ccfc88e47fa5ab3cea15a54a2`  
		Last Modified: Tue, 08 Aug 2023 19:48:27 GMT  
		Size: 43.9 MB (43859738 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:154f45391e40d1749b8abe1eee183080a644f03d4df3df574047821580f8cfd1`  
		Last Modified: Tue, 08 Aug 2023 19:48:20 GMT  
		Size: 160.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4f7f6819c0c02d68da47dceda1a6986861343cb4f771692753f02143bca02792`  
		Last Modified: Mon, 14 Aug 2023 18:12:08 GMT  
		Size: 734.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d92d5fe74136aa1497cce4d11d4c3cd13a47b86ca0ba6e7597c521caae970b4c`  
		Last Modified: Mon, 14 Aug 2023 18:58:39 GMT  
		Size: 172.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:15e006fea1206162275cd2da574f81d9641687f7741f13a27587383fa446feb3`  
		Last Modified: Mon, 14 Aug 2023 19:01:48 GMT  
		Size: 11.3 MB (11317483 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d28aa1718123ef86fd88792750d2f2ce96d3230e3a9b13001f474fa6199f2fca`  
		Last Modified: Mon, 14 Aug 2023 19:01:47 GMT  
		Size: 459.9 KB (459856 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1ad9a58799371f6468e5151c0dc77a5b60ebb92750c79d557196093eeccaaa5d`  
		Last Modified: Mon, 14 Aug 2023 19:01:47 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
