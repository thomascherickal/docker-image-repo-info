## `tomcat:9-jre11-temurin-jammy`

```console
$ docker pull tomcat@sha256:ef6c34197b54f14f63dbfb2054de0c8c746d9f5a7b5b4cf863630184647480df
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 5
	-	linux; amd64
	-	linux; arm variant v7
	-	linux; arm64 variant v8
	-	linux; ppc64le
	-	linux; s390x

### `tomcat:9-jre11-temurin-jammy` - linux; amd64

```console
$ docker pull tomcat@sha256:a0f8294404dead7e337dd8b249a0dc6b6b94e7829cee0c31b8991c1c627b0431
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **102.9 MB (102930032 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:889cd608000d17e20e6ee6297c189b4b6a8fff42828a1cb6ddfe596c5b430e0d`
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
# Tue, 08 Aug 2023 19:21:02 GMT
RUN apt-get update     && DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends tzdata curl wget ca-certificates fontconfig locales p11-kit     && echo "en_US.UTF-8 UTF-8" >> /etc/locale.gen     && locale-gen en_US.UTF-8     && rm -rf /var/lib/apt/lists/*
# Tue, 08 Aug 2023 19:22:14 GMT
ENV JAVA_VERSION=jdk-11.0.20+8
# Tue, 08 Aug 2023 19:22:53 GMT
RUN set -eux;     ARCH="$(dpkg --print-architecture)";     case "${ARCH}" in        aarch64|arm64)          ESUM='45e190920fb3ec61ee5213a7bd98553abf2ae7692eb9daa504fcdc9d59a7cfc4';          BINARY_URL='https://github.com/adoptium/temurin11-binaries/releases/download/jdk-11.0.20%2B8/OpenJDK11U-jre_aarch64_linux_hotspot_11.0.20_8.tar.gz';          ;;        armhf|arm)          ESUM='1e2a02364084b2d054e88a871f3efaa4450ae4f087b8f806fd95c15d5affcc7b';          BINARY_URL='https://github.com/adoptium/temurin11-binaries/releases/download/jdk-11.0.20%2B8/OpenJDK11U-jre_arm_linux_hotspot_11.0.20_8.tar.gz';          ;;        ppc64el|powerpc:common64)          ESUM='61034834b61bf080392218b25dcac2d9e3505b5e4f53539704d496be4181aadf';          BINARY_URL='https://github.com/adoptium/temurin11-binaries/releases/download/jdk-11.0.20%2B8/OpenJDK11U-jre_ppc64le_linux_hotspot_11.0.20_8.tar.gz';          ;;        s390x|s390:64-bit)          ESUM='0c7050976914e0613179446de62bb20d2845ae809f6d31bc0ed8d136f8fd3d9b';          BINARY_URL='https://github.com/adoptium/temurin11-binaries/releases/download/jdk-11.0.20%2B8/OpenJDK11U-jre_s390x_linux_hotspot_11.0.20_8.tar.gz';          ;;        amd64|i386:x86-64)          ESUM='ffb070c26ea22771f78769c569c9db3412e6486434dc6df1fd3c3438285766e7';          BINARY_URL='https://github.com/adoptium/temurin11-binaries/releases/download/jdk-11.0.20%2B8/OpenJDK11U-jre_x64_linux_hotspot_11.0.20_8.tar.gz';          ;;        *)          echo "Unsupported arch: ${ARCH}";          exit 1;          ;;     esac; 	  wget -O /tmp/openjdk.tar.gz ${BINARY_URL}; 	  echo "${ESUM} */tmp/openjdk.tar.gz" | sha256sum -c -; 	  mkdir -p "$JAVA_HOME"; 	  tar --extract 	      --file /tmp/openjdk.tar.gz 	      --directory "$JAVA_HOME" 	      --strip-components 1 	      --no-same-owner 	  ;     rm -f /tmp/openjdk.tar.gz ${JAVA_HOME}/lib/src.zip;     find "$JAVA_HOME/lib" -name '*.so' -exec dirname '{}' ';' | sort -u > /etc/ld.so.conf.d/docker-openjdk.conf;     ldconfig;     java -Xshare:dump;
# Tue, 08 Aug 2023 19:22:53 GMT
RUN echo Verifying install ...     && fileEncoding="$(echo 'System.out.println(System.getProperty("file.encoding"))' | jshell -s -)"; [ "$fileEncoding" = 'UTF-8' ]; rm -rf ~/.java     && echo java --version && java --version     && echo Complete.
# Tue, 08 Aug 2023 19:22:53 GMT
COPY file:0673fe0a4a716089bcd96321c8de60149aea8a94ae7c4ba827ecc4a74a9789a3 in / 
# Tue, 08 Aug 2023 19:22:54 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Tue, 08 Aug 2023 21:19:42 GMT
ENV CATALINA_HOME=/usr/local/tomcat
# Tue, 08 Aug 2023 21:19:42 GMT
ENV PATH=/usr/local/tomcat/bin:/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 08 Aug 2023 21:19:43 GMT
RUN mkdir -p "$CATALINA_HOME"
# Tue, 08 Aug 2023 21:19:43 GMT
WORKDIR /usr/local/tomcat
# Tue, 08 Aug 2023 21:19:43 GMT
ENV TOMCAT_NATIVE_LIBDIR=/usr/local/tomcat/native-jni-lib
# Tue, 08 Aug 2023 21:19:43 GMT
ENV LD_LIBRARY_PATH=/usr/local/tomcat/native-jni-lib
# Tue, 08 Aug 2023 21:22:15 GMT
ENV GPG_KEYS=48F8E69F6390C9F25CFEDCD268248959359E722B A9C5DF4D22E99998D9875A5110C01C5A2F6059E7 DCFD35E0BF8CA7344752DE8B6FB21E8933C60243
# Tue, 08 Aug 2023 21:22:15 GMT
ENV TOMCAT_MAJOR=9
# Tue, 08 Aug 2023 21:22:15 GMT
ENV TOMCAT_VERSION=9.0.78
# Tue, 08 Aug 2023 21:22:15 GMT
ENV TOMCAT_SHA512=c9f2e60489d07f25b53f715918f4b082c5bb69dbc497e0a9d3d5e3a0d351ff2e0ec8dfc5657de840ee5b3dea6174b27630033b38e36fa4c06b08664e70dec8df
# Tue, 08 Aug 2023 21:22:15 GMT
COPY dir:d66496f959d43496b9c89d017704f51d788e255b57452ccab2d07540cee6752d in /usr/local/tomcat 
# Tue, 08 Aug 2023 21:22:19 GMT
RUN set -eux; 	apt-get update; 	xargs -rt apt-get install -y --no-install-recommends < "$TOMCAT_NATIVE_LIBDIR/.dependencies.txt"; 	rm -rf /var/lib/apt/lists/*
# Tue, 08 Aug 2023 21:22:20 GMT
RUN set -eux; 	nativeLines="$(catalina.sh configtest 2>&1)"; 	nativeLines="$(echo "$nativeLines" | grep 'Apache Tomcat Native')"; 	nativeLines="$(echo "$nativeLines" | sort -u)"; 	if ! echo "$nativeLines" | grep -E 'INFO: Loaded( APR based)? Apache Tomcat Native library' >&2; then 		echo >&2 "$nativeLines"; 		exit 1; 	fi
# Tue, 08 Aug 2023 21:22:20 GMT
EXPOSE 8080
# Sat, 12 Aug 2023 00:18:57 GMT
ENTRYPOINT []
# Sat, 12 Aug 2023 00:18:57 GMT
CMD ["catalina.sh" "run"]
```

-	Layers:
	-	`sha256:9d19ee268e0d7bcf6716e6658ee1b0384a71d6f2f9aa1ae2085610cf7c7b316f`  
		Last Modified: Wed, 28 Jun 2023 11:50:41 GMT  
		Size: 30.4 MB (30431229 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8a1d9603a2223f0c0337b5489031adc59113c119d64dfce6852f6114f42f2f05`  
		Last Modified: Tue, 08 Aug 2023 19:27:08 GMT  
		Size: 12.9 MB (12902861 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:29ec547f8ce2155ce58a25da4ddaaffb94bbba064f0491bbc9535447779218de`  
		Last Modified: Tue, 08 Aug 2023 19:30:50 GMT  
		Size: 46.9 MB (46864855 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:83c96886bebf4fd42e9a6622257a11b02a6c388c2a8b5dda93d1087b4f6ee1fd`  
		Last Modified: Tue, 08 Aug 2023 19:30:44 GMT  
		Size: 160.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fcf16da19f8ed2a380e226c2910876175263f8b9faadec9dc54ce22afa3d1af2`  
		Last Modified: Tue, 08 Aug 2023 19:30:44 GMT  
		Size: 666.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a61848075b315b207168c2fe1398dab9d0ec71c4fbb107cb79e1905a1f8a45f6`  
		Last Modified: Tue, 08 Aug 2023 21:33:54 GMT  
		Size: 172.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:928e90d0ce80b80986c163e5d27976d9000f8fba5759d15dbff9a6c98c62860d`  
		Last Modified: Tue, 08 Aug 2023 21:36:19 GMT  
		Size: 12.3 MB (12274307 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bd42be45972fcd990bfba93301420655a6804161314648dde0c06c7ba8a6de18`  
		Last Modified: Tue, 08 Aug 2023 21:36:18 GMT  
		Size: 455.7 KB (455652 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3e5fa1cef704c1b3f628af0ef6c845b11be06d2f32c207d9854bcd5b3f22fe64`  
		Last Modified: Tue, 08 Aug 2023 21:36:18 GMT  
		Size: 130.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `tomcat:9-jre11-temurin-jammy` - linux; arm variant v7

```console
$ docker pull tomcat@sha256:0041d5ae6812f05c7490c51ea67bb1c28c3b560e1ffc026344fd0f4dc6fedb20
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **97.2 MB (97172696 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:de6a359504a38f64af78742d117135ff6c3b4ecff6a3d3eb48a3b5b654be274a`
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
# Tue, 08 Aug 2023 18:59:01 GMT
RUN apt-get update     && DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends tzdata curl wget ca-certificates fontconfig locales p11-kit     && echo "en_US.UTF-8 UTF-8" >> /etc/locale.gen     && locale-gen en_US.UTF-8     && rm -rf /var/lib/apt/lists/*
# Tue, 08 Aug 2023 19:00:03 GMT
ENV JAVA_VERSION=jdk-11.0.20+8
# Tue, 08 Aug 2023 19:00:32 GMT
RUN set -eux;     ARCH="$(dpkg --print-architecture)";     case "${ARCH}" in        aarch64|arm64)          ESUM='45e190920fb3ec61ee5213a7bd98553abf2ae7692eb9daa504fcdc9d59a7cfc4';          BINARY_URL='https://github.com/adoptium/temurin11-binaries/releases/download/jdk-11.0.20%2B8/OpenJDK11U-jre_aarch64_linux_hotspot_11.0.20_8.tar.gz';          ;;        armhf|arm)          ESUM='1e2a02364084b2d054e88a871f3efaa4450ae4f087b8f806fd95c15d5affcc7b';          BINARY_URL='https://github.com/adoptium/temurin11-binaries/releases/download/jdk-11.0.20%2B8/OpenJDK11U-jre_arm_linux_hotspot_11.0.20_8.tar.gz';          ;;        ppc64el|powerpc:common64)          ESUM='61034834b61bf080392218b25dcac2d9e3505b5e4f53539704d496be4181aadf';          BINARY_URL='https://github.com/adoptium/temurin11-binaries/releases/download/jdk-11.0.20%2B8/OpenJDK11U-jre_ppc64le_linux_hotspot_11.0.20_8.tar.gz';          ;;        s390x|s390:64-bit)          ESUM='0c7050976914e0613179446de62bb20d2845ae809f6d31bc0ed8d136f8fd3d9b';          BINARY_URL='https://github.com/adoptium/temurin11-binaries/releases/download/jdk-11.0.20%2B8/OpenJDK11U-jre_s390x_linux_hotspot_11.0.20_8.tar.gz';          ;;        amd64|i386:x86-64)          ESUM='ffb070c26ea22771f78769c569c9db3412e6486434dc6df1fd3c3438285766e7';          BINARY_URL='https://github.com/adoptium/temurin11-binaries/releases/download/jdk-11.0.20%2B8/OpenJDK11U-jre_x64_linux_hotspot_11.0.20_8.tar.gz';          ;;        *)          echo "Unsupported arch: ${ARCH}";          exit 1;          ;;     esac; 	  wget -O /tmp/openjdk.tar.gz ${BINARY_URL}; 	  echo "${ESUM} */tmp/openjdk.tar.gz" | sha256sum -c -; 	  mkdir -p "$JAVA_HOME"; 	  tar --extract 	      --file /tmp/openjdk.tar.gz 	      --directory "$JAVA_HOME" 	      --strip-components 1 	      --no-same-owner 	  ;     rm -f /tmp/openjdk.tar.gz ${JAVA_HOME}/lib/src.zip;     find "$JAVA_HOME/lib" -name '*.so' -exec dirname '{}' ';' | sort -u > /etc/ld.so.conf.d/docker-openjdk.conf;     ldconfig;     java -Xshare:dump;
# Tue, 08 Aug 2023 19:00:33 GMT
RUN echo Verifying install ...     && fileEncoding="$(echo 'System.out.println(System.getProperty("file.encoding"))' | jshell -s -)"; [ "$fileEncoding" = 'UTF-8' ]; rm -rf ~/.java     && echo java --version && java --version     && echo Complete.
# Tue, 08 Aug 2023 19:00:33 GMT
COPY file:0673fe0a4a716089bcd96321c8de60149aea8a94ae7c4ba827ecc4a74a9789a3 in / 
# Tue, 08 Aug 2023 19:00:33 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Tue, 08 Aug 2023 19:56:27 GMT
ENV CATALINA_HOME=/usr/local/tomcat
# Tue, 08 Aug 2023 19:56:27 GMT
ENV PATH=/usr/local/tomcat/bin:/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 08 Aug 2023 19:56:27 GMT
RUN mkdir -p "$CATALINA_HOME"
# Tue, 08 Aug 2023 19:56:27 GMT
WORKDIR /usr/local/tomcat
# Tue, 08 Aug 2023 19:56:28 GMT
ENV TOMCAT_NATIVE_LIBDIR=/usr/local/tomcat/native-jni-lib
# Tue, 08 Aug 2023 19:56:28 GMT
ENV LD_LIBRARY_PATH=/usr/local/tomcat/native-jni-lib
# Tue, 08 Aug 2023 19:59:11 GMT
ENV GPG_KEYS=48F8E69F6390C9F25CFEDCD268248959359E722B A9C5DF4D22E99998D9875A5110C01C5A2F6059E7 DCFD35E0BF8CA7344752DE8B6FB21E8933C60243
# Tue, 08 Aug 2023 19:59:11 GMT
ENV TOMCAT_MAJOR=9
# Tue, 08 Aug 2023 19:59:11 GMT
ENV TOMCAT_VERSION=9.0.78
# Tue, 08 Aug 2023 19:59:11 GMT
ENV TOMCAT_SHA512=c9f2e60489d07f25b53f715918f4b082c5bb69dbc497e0a9d3d5e3a0d351ff2e0ec8dfc5657de840ee5b3dea6174b27630033b38e36fa4c06b08664e70dec8df
# Tue, 08 Aug 2023 19:59:12 GMT
COPY dir:c860baa2f52c933a18753ebf273c9ec250d1ebc217264b85026a035d7a65401f in /usr/local/tomcat 
# Tue, 08 Aug 2023 19:59:16 GMT
RUN set -eux; 	apt-get update; 	xargs -rt apt-get install -y --no-install-recommends < "$TOMCAT_NATIVE_LIBDIR/.dependencies.txt"; 	rm -rf /var/lib/apt/lists/*
# Tue, 08 Aug 2023 19:59:18 GMT
RUN set -eux; 	nativeLines="$(catalina.sh configtest 2>&1)"; 	nativeLines="$(echo "$nativeLines" | grep 'Apache Tomcat Native')"; 	nativeLines="$(echo "$nativeLines" | sort -u)"; 	if ! echo "$nativeLines" | grep -E 'INFO: Loaded( APR based)? Apache Tomcat Native library' >&2; then 		echo >&2 "$nativeLines"; 		exit 1; 	fi
# Tue, 08 Aug 2023 19:59:18 GMT
EXPOSE 8080
# Sat, 12 Aug 2023 00:25:42 GMT
ENTRYPOINT []
# Sat, 12 Aug 2023 00:25:42 GMT
CMD ["catalina.sh" "run"]
```

-	Layers:
	-	`sha256:63b96265cfe95b9cec847027033d4226b783ecd042036f5c809a7386027f56b0`  
		Last Modified: Fri, 30 Jun 2023 02:08:02 GMT  
		Size: 27.0 MB (27026961 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:791f420277f117d4cbc9798bac0e3991df4d76dcb209a6289b5474d81f4c32d0`  
		Last Modified: Tue, 08 Aug 2023 19:02:56 GMT  
		Size: 12.5 MB (12491020 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:488129ff542f9219b30a6eeb605366757b9f8a1ded3e35478e46e293c8c0702d`  
		Last Modified: Tue, 08 Aug 2023 19:04:54 GMT  
		Size: 45.0 MB (45013047 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b9327b04613d69a7cfb1d735b350938d15b93139ebc371bca95df06821c0ff23`  
		Last Modified: Tue, 08 Aug 2023 19:04:47 GMT  
		Size: 160.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:afcf4e3ac40244e0a4c3d631e214005a21c6af63accecd7cd1b70cbd1eae57f8`  
		Last Modified: Tue, 08 Aug 2023 19:04:47 GMT  
		Size: 666.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7966203b4d51d7c30d8b666be073bf177511881157c202cd86c01fdc8b81e0ae`  
		Last Modified: Tue, 08 Aug 2023 20:10:23 GMT  
		Size: 172.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a466d79f90497a37a8f6f22c807e100ad25717774b57b61742063541f22bfec7`  
		Last Modified: Tue, 08 Aug 2023 20:12:46 GMT  
		Size: 12.2 MB (12211620 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f75796241edb387a51a7c433fb6970e6d7ad31e1b8858ab0e74d087c343dab75`  
		Last Modified: Tue, 08 Aug 2023 20:12:44 GMT  
		Size: 428.9 KB (428920 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a04e20fb3387af2646ba443d195dcc6afada39f34b1cf72bb78cbb1f495e7d10`  
		Last Modified: Tue, 08 Aug 2023 20:12:44 GMT  
		Size: 130.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `tomcat:9-jre11-temurin-jammy` - linux; arm64 variant v8

```console
$ docker pull tomcat@sha256:242760f32fea6919c3b5bbff4c0e1353b46da2f2005c0db9dc2b7bc3f1f53edc
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **99.2 MB (99165950 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:3026b6170ce201add70ea13abbafc3190291c4db4b2e5f9c02a74a4e973c4803`
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
# Tue, 08 Aug 2023 19:40:41 GMT
RUN apt-get update     && DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends tzdata curl wget ca-certificates fontconfig locales p11-kit     && echo "en_US.UTF-8 UTF-8" >> /etc/locale.gen     && locale-gen en_US.UTF-8     && rm -rf /var/lib/apt/lists/*
# Tue, 08 Aug 2023 19:41:25 GMT
ENV JAVA_VERSION=jdk-11.0.20+8
# Tue, 08 Aug 2023 19:41:50 GMT
RUN set -eux;     ARCH="$(dpkg --print-architecture)";     case "${ARCH}" in        aarch64|arm64)          ESUM='45e190920fb3ec61ee5213a7bd98553abf2ae7692eb9daa504fcdc9d59a7cfc4';          BINARY_URL='https://github.com/adoptium/temurin11-binaries/releases/download/jdk-11.0.20%2B8/OpenJDK11U-jre_aarch64_linux_hotspot_11.0.20_8.tar.gz';          ;;        armhf|arm)          ESUM='1e2a02364084b2d054e88a871f3efaa4450ae4f087b8f806fd95c15d5affcc7b';          BINARY_URL='https://github.com/adoptium/temurin11-binaries/releases/download/jdk-11.0.20%2B8/OpenJDK11U-jre_arm_linux_hotspot_11.0.20_8.tar.gz';          ;;        ppc64el|powerpc:common64)          ESUM='61034834b61bf080392218b25dcac2d9e3505b5e4f53539704d496be4181aadf';          BINARY_URL='https://github.com/adoptium/temurin11-binaries/releases/download/jdk-11.0.20%2B8/OpenJDK11U-jre_ppc64le_linux_hotspot_11.0.20_8.tar.gz';          ;;        s390x|s390:64-bit)          ESUM='0c7050976914e0613179446de62bb20d2845ae809f6d31bc0ed8d136f8fd3d9b';          BINARY_URL='https://github.com/adoptium/temurin11-binaries/releases/download/jdk-11.0.20%2B8/OpenJDK11U-jre_s390x_linux_hotspot_11.0.20_8.tar.gz';          ;;        amd64|i386:x86-64)          ESUM='ffb070c26ea22771f78769c569c9db3412e6486434dc6df1fd3c3438285766e7';          BINARY_URL='https://github.com/adoptium/temurin11-binaries/releases/download/jdk-11.0.20%2B8/OpenJDK11U-jre_x64_linux_hotspot_11.0.20_8.tar.gz';          ;;        *)          echo "Unsupported arch: ${ARCH}";          exit 1;          ;;     esac; 	  wget -O /tmp/openjdk.tar.gz ${BINARY_URL}; 	  echo "${ESUM} */tmp/openjdk.tar.gz" | sha256sum -c -; 	  mkdir -p "$JAVA_HOME"; 	  tar --extract 	      --file /tmp/openjdk.tar.gz 	      --directory "$JAVA_HOME" 	      --strip-components 1 	      --no-same-owner 	  ;     rm -f /tmp/openjdk.tar.gz ${JAVA_HOME}/lib/src.zip;     find "$JAVA_HOME/lib" -name '*.so' -exec dirname '{}' ';' | sort -u > /etc/ld.so.conf.d/docker-openjdk.conf;     ldconfig;     java -Xshare:dump;
# Tue, 08 Aug 2023 19:41:51 GMT
RUN echo Verifying install ...     && fileEncoding="$(echo 'System.out.println(System.getProperty("file.encoding"))' | jshell -s -)"; [ "$fileEncoding" = 'UTF-8' ]; rm -rf ~/.java     && echo java --version && java --version     && echo Complete.
# Tue, 08 Aug 2023 19:41:51 GMT
COPY file:0673fe0a4a716089bcd96321c8de60149aea8a94ae7c4ba827ecc4a74a9789a3 in / 
# Tue, 08 Aug 2023 19:41:51 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Tue, 08 Aug 2023 22:35:53 GMT
ENV CATALINA_HOME=/usr/local/tomcat
# Tue, 08 Aug 2023 22:35:54 GMT
ENV PATH=/usr/local/tomcat/bin:/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 08 Aug 2023 22:35:54 GMT
RUN mkdir -p "$CATALINA_HOME"
# Tue, 08 Aug 2023 22:35:54 GMT
WORKDIR /usr/local/tomcat
# Tue, 08 Aug 2023 22:35:54 GMT
ENV TOMCAT_NATIVE_LIBDIR=/usr/local/tomcat/native-jni-lib
# Tue, 08 Aug 2023 22:35:54 GMT
ENV LD_LIBRARY_PATH=/usr/local/tomcat/native-jni-lib
# Tue, 08 Aug 2023 22:37:54 GMT
ENV GPG_KEYS=48F8E69F6390C9F25CFEDCD268248959359E722B A9C5DF4D22E99998D9875A5110C01C5A2F6059E7 DCFD35E0BF8CA7344752DE8B6FB21E8933C60243
# Tue, 08 Aug 2023 22:37:54 GMT
ENV TOMCAT_MAJOR=9
# Tue, 08 Aug 2023 22:37:55 GMT
ENV TOMCAT_VERSION=9.0.78
# Tue, 08 Aug 2023 22:37:55 GMT
ENV TOMCAT_SHA512=c9f2e60489d07f25b53f715918f4b082c5bb69dbc497e0a9d3d5e3a0d351ff2e0ec8dfc5657de840ee5b3dea6174b27630033b38e36fa4c06b08664e70dec8df
# Tue, 08 Aug 2023 22:37:55 GMT
COPY dir:23f889a3b2cdecd072883d6baeea265beefc3c494a4ddd10e12998f99db2d38d in /usr/local/tomcat 
# Tue, 08 Aug 2023 22:37:58 GMT
RUN set -eux; 	apt-get update; 	xargs -rt apt-get install -y --no-install-recommends < "$TOMCAT_NATIVE_LIBDIR/.dependencies.txt"; 	rm -rf /var/lib/apt/lists/*
# Tue, 08 Aug 2023 22:37:59 GMT
RUN set -eux; 	nativeLines="$(catalina.sh configtest 2>&1)"; 	nativeLines="$(echo "$nativeLines" | grep 'Apache Tomcat Native')"; 	nativeLines="$(echo "$nativeLines" | sort -u)"; 	if ! echo "$nativeLines" | grep -E 'INFO: Loaded( APR based)? Apache Tomcat Native library' >&2; then 		echo >&2 "$nativeLines"; 		exit 1; 	fi
# Tue, 08 Aug 2023 22:37:59 GMT
EXPOSE 8080
# Sat, 12 Aug 2023 01:04:47 GMT
ENTRYPOINT []
# Sat, 12 Aug 2023 01:04:47 GMT
CMD ["catalina.sh" "run"]
```

-	Layers:
	-	`sha256:ac34a2e0269ced3acc355be706239ee0f3f1e73a035c40dd2fac74827164ee53`  
		Last Modified: Wed, 28 Jun 2023 23:23:40 GMT  
		Size: 28.4 MB (28391011 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:91712d801b234a271df55fd60b35e7d2918ce5ae0fb7ce56a8de0edb8151fd0e`  
		Last Modified: Tue, 08 Aug 2023 19:44:21 GMT  
		Size: 12.8 MB (12844180 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3aeb71c3e8ddfbdbcdf7f366fa14814e5ae4bc3c34c81ee51cd629b818bbedac`  
		Last Modified: Tue, 08 Aug 2023 19:46:59 GMT  
		Size: 45.2 MB (45190380 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e29f50935a8980aae448b158b40171ce38beb0eaaac6885c4f54cce54e91111d`  
		Last Modified: Tue, 08 Aug 2023 19:46:54 GMT  
		Size: 159.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:78f0a93a82bda1755bff5d618fe66a84d7a66aa14b6a354e0cba1523e594c088`  
		Last Modified: Tue, 08 Aug 2023 19:46:53 GMT  
		Size: 667.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:639e7d04c7fcfd6d278fdb6171706187682498b6aad235b3be91c12e45773392`  
		Last Modified: Tue, 08 Aug 2023 22:48:06 GMT  
		Size: 171.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2fab5a9be0f480900f45cc3e1a364d2da24d2c6ca62ffbb7e8ccef48613cd6b0`  
		Last Modified: Tue, 08 Aug 2023 22:50:25 GMT  
		Size: 12.3 MB (12283319 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:889320135f678f7e560593d20199b21f028fd6f71833b407ad81b29d5bb00c38`  
		Last Modified: Tue, 08 Aug 2023 22:50:24 GMT  
		Size: 455.9 KB (455934 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b7c3de513603e59f45336e577748f3ad5b60db679562c7d5c5d86988bf598fc4`  
		Last Modified: Tue, 08 Aug 2023 22:50:23 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `tomcat:9-jre11-temurin-jammy` - linux; ppc64le

```console
$ docker pull tomcat@sha256:6d5eb27280087370fe45211529aae200c9b112a6625eab26322cd25674c8bb17
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **104.6 MB (104567962 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:7b25009ad5058e62ebedb32d90c3f04dd65eb483a48a96d3ce16eb9d55f7ede2`
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
# Tue, 08 Aug 2023 19:19:30 GMT
RUN apt-get update     && DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends tzdata curl wget ca-certificates fontconfig locales p11-kit     && echo "en_US.UTF-8 UTF-8" >> /etc/locale.gen     && locale-gen en_US.UTF-8     && rm -rf /var/lib/apt/lists/*
# Tue, 08 Aug 2023 19:21:25 GMT
ENV JAVA_VERSION=jdk-11.0.20+8
# Tue, 08 Aug 2023 19:22:34 GMT
RUN set -eux;     ARCH="$(dpkg --print-architecture)";     case "${ARCH}" in        aarch64|arm64)          ESUM='45e190920fb3ec61ee5213a7bd98553abf2ae7692eb9daa504fcdc9d59a7cfc4';          BINARY_URL='https://github.com/adoptium/temurin11-binaries/releases/download/jdk-11.0.20%2B8/OpenJDK11U-jre_aarch64_linux_hotspot_11.0.20_8.tar.gz';          ;;        armhf|arm)          ESUM='1e2a02364084b2d054e88a871f3efaa4450ae4f087b8f806fd95c15d5affcc7b';          BINARY_URL='https://github.com/adoptium/temurin11-binaries/releases/download/jdk-11.0.20%2B8/OpenJDK11U-jre_arm_linux_hotspot_11.0.20_8.tar.gz';          ;;        ppc64el|powerpc:common64)          ESUM='61034834b61bf080392218b25dcac2d9e3505b5e4f53539704d496be4181aadf';          BINARY_URL='https://github.com/adoptium/temurin11-binaries/releases/download/jdk-11.0.20%2B8/OpenJDK11U-jre_ppc64le_linux_hotspot_11.0.20_8.tar.gz';          ;;        s390x|s390:64-bit)          ESUM='0c7050976914e0613179446de62bb20d2845ae809f6d31bc0ed8d136f8fd3d9b';          BINARY_URL='https://github.com/adoptium/temurin11-binaries/releases/download/jdk-11.0.20%2B8/OpenJDK11U-jre_s390x_linux_hotspot_11.0.20_8.tar.gz';          ;;        amd64|i386:x86-64)          ESUM='ffb070c26ea22771f78769c569c9db3412e6486434dc6df1fd3c3438285766e7';          BINARY_URL='https://github.com/adoptium/temurin11-binaries/releases/download/jdk-11.0.20%2B8/OpenJDK11U-jre_x64_linux_hotspot_11.0.20_8.tar.gz';          ;;        *)          echo "Unsupported arch: ${ARCH}";          exit 1;          ;;     esac; 	  wget -O /tmp/openjdk.tar.gz ${BINARY_URL}; 	  echo "${ESUM} */tmp/openjdk.tar.gz" | sha256sum -c -; 	  mkdir -p "$JAVA_HOME"; 	  tar --extract 	      --file /tmp/openjdk.tar.gz 	      --directory "$JAVA_HOME" 	      --strip-components 1 	      --no-same-owner 	  ;     rm -f /tmp/openjdk.tar.gz ${JAVA_HOME}/lib/src.zip;     find "$JAVA_HOME/lib" -name '*.so' -exec dirname '{}' ';' | sort -u > /etc/ld.so.conf.d/docker-openjdk.conf;     ldconfig;     java -Xshare:dump;
# Tue, 08 Aug 2023 19:22:37 GMT
RUN echo Verifying install ...     && fileEncoding="$(echo 'System.out.println(System.getProperty("file.encoding"))' | jshell -s -)"; [ "$fileEncoding" = 'UTF-8' ]; rm -rf ~/.java     && echo java --version && java --version     && echo Complete.
# Tue, 08 Aug 2023 19:22:38 GMT
COPY file:0673fe0a4a716089bcd96321c8de60149aea8a94ae7c4ba827ecc4a74a9789a3 in / 
# Tue, 08 Aug 2023 19:22:38 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Tue, 08 Aug 2023 21:03:30 GMT
ENV CATALINA_HOME=/usr/local/tomcat
# Tue, 08 Aug 2023 21:03:30 GMT
ENV PATH=/usr/local/tomcat/bin:/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 08 Aug 2023 21:03:32 GMT
RUN mkdir -p "$CATALINA_HOME"
# Tue, 08 Aug 2023 21:03:32 GMT
WORKDIR /usr/local/tomcat
# Tue, 08 Aug 2023 21:03:33 GMT
ENV TOMCAT_NATIVE_LIBDIR=/usr/local/tomcat/native-jni-lib
# Tue, 08 Aug 2023 21:03:33 GMT
ENV LD_LIBRARY_PATH=/usr/local/tomcat/native-jni-lib
# Tue, 08 Aug 2023 21:12:07 GMT
ENV GPG_KEYS=48F8E69F6390C9F25CFEDCD268248959359E722B A9C5DF4D22E99998D9875A5110C01C5A2F6059E7 DCFD35E0BF8CA7344752DE8B6FB21E8933C60243
# Tue, 08 Aug 2023 21:12:08 GMT
ENV TOMCAT_MAJOR=9
# Tue, 08 Aug 2023 21:12:09 GMT
ENV TOMCAT_VERSION=9.0.78
# Tue, 08 Aug 2023 21:12:10 GMT
ENV TOMCAT_SHA512=c9f2e60489d07f25b53f715918f4b082c5bb69dbc497e0a9d3d5e3a0d351ff2e0ec8dfc5657de840ee5b3dea6174b27630033b38e36fa4c06b08664e70dec8df
# Tue, 08 Aug 2023 21:12:11 GMT
COPY dir:3c3b7f5b97fcb009860309cd08fc3c59362da6c2cd2c2e295481152f361d3465 in /usr/local/tomcat 
# Tue, 08 Aug 2023 21:12:21 GMT
RUN set -eux; 	apt-get update; 	xargs -rt apt-get install -y --no-install-recommends < "$TOMCAT_NATIVE_LIBDIR/.dependencies.txt"; 	rm -rf /var/lib/apt/lists/*
# Tue, 08 Aug 2023 21:12:24 GMT
RUN set -eux; 	nativeLines="$(catalina.sh configtest 2>&1)"; 	nativeLines="$(echo "$nativeLines" | grep 'Apache Tomcat Native')"; 	nativeLines="$(echo "$nativeLines" | sort -u)"; 	if ! echo "$nativeLines" | grep -E 'INFO: Loaded( APR based)? Apache Tomcat Native library' >&2; then 		echo >&2 "$nativeLines"; 		exit 1; 	fi
# Tue, 08 Aug 2023 21:12:24 GMT
EXPOSE 8080
# Sat, 12 Aug 2023 00:15:47 GMT
ENTRYPOINT []
# Sat, 12 Aug 2023 00:15:48 GMT
CMD ["catalina.sh" "run"]
```

-	Layers:
	-	`sha256:7faa46ce6b6f5c34485980029504c3995e38149d0bca67d8b976c5dbb3673644`  
		Last Modified: Tue, 04 Jul 2023 04:42:31 GMT  
		Size: 35.7 MB (35711469 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bc2f5a106d782ce62a5cf92c2a7f53d1b6067d5198e321d1c74bf914ae7b208f`  
		Last Modified: Tue, 08 Aug 2023 19:28:59 GMT  
		Size: 13.8 MB (13770640 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:165a80cbdb7b61d7a95bcc244443e23a3069edb8cf8f0552be6581117a7fb3c3`  
		Last Modified: Tue, 08 Aug 2023 19:33:10 GMT  
		Size: 42.3 MB (42295309 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ad547ccf5a7181bed1599a10c0225336c8544a8fb637b97dd9c901fcb54fa33e`  
		Last Modified: Tue, 08 Aug 2023 19:32:59 GMT  
		Size: 162.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a1943e298b8799c3be0cd6731d681795316d3b4a21ec0e099e765625a3a2eada`  
		Last Modified: Tue, 08 Aug 2023 19:32:59 GMT  
		Size: 667.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8629aea934a23d6e284a17d7018a2034b72174ef59389e5fc3ba0b56b6d500be`  
		Last Modified: Tue, 08 Aug 2023 21:40:35 GMT  
		Size: 173.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:00e6b44ac8e418a50d8f2f178e64177a17a9d1547bd39c8baae48d6904b2fc97`  
		Last Modified: Tue, 08 Aug 2023 21:44:07 GMT  
		Size: 12.3 MB (12302528 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d001f8c487271684c37dc7c90797fd49f16b1141553b862a34708f00440c7243`  
		Last Modified: Tue, 08 Aug 2023 21:44:05 GMT  
		Size: 486.9 KB (486884 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f6a681cd4b52714b1efb501a830968c3ffba0713fe262e469f34e22cd61cd4d8`  
		Last Modified: Tue, 08 Aug 2023 21:44:05 GMT  
		Size: 130.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `tomcat:9-jre11-temurin-jammy` - linux; s390x

```console
$ docker pull tomcat@sha256:0872d74d67c7e7bb84802facac010ca9d7147f8cd4ae81ba465e999e4187b283
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **95.0 MB (94991308 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:415897dd95488ae04c429a17f7079997b04f07e30c86972f040d05cf2593a601`
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
# Tue, 08 Aug 2023 19:42:55 GMT
RUN apt-get update     && DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends tzdata curl wget ca-certificates fontconfig locales p11-kit     && echo "en_US.UTF-8 UTF-8" >> /etc/locale.gen     && locale-gen en_US.UTF-8     && rm -rf /var/lib/apt/lists/*
# Tue, 08 Aug 2023 19:42:56 GMT
ENV JAVA_VERSION=jdk-11.0.20+8
# Tue, 08 Aug 2023 19:43:34 GMT
RUN set -eux;     ARCH="$(dpkg --print-architecture)";     case "${ARCH}" in        aarch64|arm64)          ESUM='45e190920fb3ec61ee5213a7bd98553abf2ae7692eb9daa504fcdc9d59a7cfc4';          BINARY_URL='https://github.com/adoptium/temurin11-binaries/releases/download/jdk-11.0.20%2B8/OpenJDK11U-jre_aarch64_linux_hotspot_11.0.20_8.tar.gz';          ;;        armhf|arm)          ESUM='1e2a02364084b2d054e88a871f3efaa4450ae4f087b8f806fd95c15d5affcc7b';          BINARY_URL='https://github.com/adoptium/temurin11-binaries/releases/download/jdk-11.0.20%2B8/OpenJDK11U-jre_arm_linux_hotspot_11.0.20_8.tar.gz';          ;;        ppc64el|powerpc:common64)          ESUM='61034834b61bf080392218b25dcac2d9e3505b5e4f53539704d496be4181aadf';          BINARY_URL='https://github.com/adoptium/temurin11-binaries/releases/download/jdk-11.0.20%2B8/OpenJDK11U-jre_ppc64le_linux_hotspot_11.0.20_8.tar.gz';          ;;        s390x|s390:64-bit)          ESUM='0c7050976914e0613179446de62bb20d2845ae809f6d31bc0ed8d136f8fd3d9b';          BINARY_URL='https://github.com/adoptium/temurin11-binaries/releases/download/jdk-11.0.20%2B8/OpenJDK11U-jre_s390x_linux_hotspot_11.0.20_8.tar.gz';          ;;        amd64|i386:x86-64)          ESUM='ffb070c26ea22771f78769c569c9db3412e6486434dc6df1fd3c3438285766e7';          BINARY_URL='https://github.com/adoptium/temurin11-binaries/releases/download/jdk-11.0.20%2B8/OpenJDK11U-jre_x64_linux_hotspot_11.0.20_8.tar.gz';          ;;        *)          echo "Unsupported arch: ${ARCH}";          exit 1;          ;;     esac; 	  wget -O /tmp/openjdk.tar.gz ${BINARY_URL}; 	  echo "${ESUM} */tmp/openjdk.tar.gz" | sha256sum -c -; 	  mkdir -p "$JAVA_HOME"; 	  tar --extract 	      --file /tmp/openjdk.tar.gz 	      --directory "$JAVA_HOME" 	      --strip-components 1 	      --no-same-owner 	  ;     rm -f /tmp/openjdk.tar.gz ${JAVA_HOME}/lib/src.zip;     find "$JAVA_HOME/lib" -name '*.so' -exec dirname '{}' ';' | sort -u > /etc/ld.so.conf.d/docker-openjdk.conf;     ldconfig;     java -Xshare:dump;
# Tue, 08 Aug 2023 19:43:36 GMT
RUN echo Verifying install ...     && fileEncoding="$(echo 'System.out.println(System.getProperty("file.encoding"))' | jshell -s -)"; [ "$fileEncoding" = 'UTF-8' ]; rm -rf ~/.java     && echo java --version && java --version     && echo Complete.
# Tue, 08 Aug 2023 19:43:36 GMT
COPY file:0673fe0a4a716089bcd96321c8de60149aea8a94ae7c4ba827ecc4a74a9789a3 in / 
# Tue, 08 Aug 2023 19:43:36 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Tue, 08 Aug 2023 20:09:17 GMT
ENV CATALINA_HOME=/usr/local/tomcat
# Tue, 08 Aug 2023 20:09:17 GMT
ENV PATH=/usr/local/tomcat/bin:/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 08 Aug 2023 20:09:18 GMT
RUN mkdir -p "$CATALINA_HOME"
# Tue, 08 Aug 2023 20:09:18 GMT
WORKDIR /usr/local/tomcat
# Tue, 08 Aug 2023 20:09:18 GMT
ENV TOMCAT_NATIVE_LIBDIR=/usr/local/tomcat/native-jni-lib
# Tue, 08 Aug 2023 20:09:18 GMT
ENV LD_LIBRARY_PATH=/usr/local/tomcat/native-jni-lib
# Tue, 08 Aug 2023 20:11:57 GMT
ENV GPG_KEYS=48F8E69F6390C9F25CFEDCD268248959359E722B A9C5DF4D22E99998D9875A5110C01C5A2F6059E7 DCFD35E0BF8CA7344752DE8B6FB21E8933C60243
# Tue, 08 Aug 2023 20:11:58 GMT
ENV TOMCAT_MAJOR=9
# Tue, 08 Aug 2023 20:11:58 GMT
ENV TOMCAT_VERSION=9.0.78
# Tue, 08 Aug 2023 20:11:58 GMT
ENV TOMCAT_SHA512=c9f2e60489d07f25b53f715918f4b082c5bb69dbc497e0a9d3d5e3a0d351ff2e0ec8dfc5657de840ee5b3dea6174b27630033b38e36fa4c06b08664e70dec8df
# Tue, 08 Aug 2023 20:11:58 GMT
COPY dir:579d6d5c1e73de092b8aee24d8dbcee04abadc0f37f5f76aa3e470b31ad9db96 in /usr/local/tomcat 
# Tue, 08 Aug 2023 20:12:03 GMT
RUN set -eux; 	apt-get update; 	xargs -rt apt-get install -y --no-install-recommends < "$TOMCAT_NATIVE_LIBDIR/.dependencies.txt"; 	rm -rf /var/lib/apt/lists/*
# Tue, 08 Aug 2023 20:12:04 GMT
RUN set -eux; 	nativeLines="$(catalina.sh configtest 2>&1)"; 	nativeLines="$(echo "$nativeLines" | grep 'Apache Tomcat Native')"; 	nativeLines="$(echo "$nativeLines" | sort -u)"; 	if ! echo "$nativeLines" | grep -E 'INFO: Loaded( APR based)? Apache Tomcat Native library' >&2; then 		echo >&2 "$nativeLines"; 		exit 1; 	fi
# Tue, 08 Aug 2023 20:12:04 GMT
EXPOSE 8080
# Sat, 12 Aug 2023 00:06:21 GMT
ENTRYPOINT []
# Sat, 12 Aug 2023 00:06:21 GMT
CMD ["catalina.sh" "run"]
```

-	Layers:
	-	`sha256:ce02ee0330980398d6a84a50abfa1a8c4d1cba27cbd7442b79f4aa1b1a14020d`  
		Last Modified: Tue, 04 Jul 2023 13:08:30 GMT  
		Size: 28.6 MB (28645696 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:10c50c1c8dac118ab286a3daca746c31d4f16f57d4a01f96c6538eeca886cafd`  
		Last Modified: Tue, 08 Aug 2023 19:46:30 GMT  
		Size: 13.0 MB (12981935 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6d424bed4049f5cf52f12697efc3fe523bc4707130adfb89345709da2e4e8ca9`  
		Last Modified: Tue, 08 Aug 2023 19:47:11 GMT  
		Size: 40.6 MB (40631193 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a3def242509c79c9ab5ad5c0d8bc6f938bccc2cb6bb3c44cb5f26670034581ef`  
		Last Modified: Tue, 08 Aug 2023 19:47:05 GMT  
		Size: 160.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fc77f682b0e12c84d69e1ab6735b311b61f235d127d06a7b80d50e2e2215bce1`  
		Last Modified: Tue, 08 Aug 2023 19:47:05 GMT  
		Size: 667.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:92d999e748c081631ed8d85c88cc3d5046200a1f8aeb54d2fb5f22a237054702`  
		Last Modified: Tue, 08 Aug 2023 20:18:40 GMT  
		Size: 172.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:74aa1ba02744a26fdd7d8c07788bd8a8243d8ed2b2f5fbe8caa81771c189e161`  
		Last Modified: Tue, 08 Aug 2023 20:20:09 GMT  
		Size: 12.3 MB (12274084 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:500a4dde45e83a6cf146194054957132879f4828787a9c9f1f8d9c7590be81c4`  
		Last Modified: Tue, 08 Aug 2023 20:20:08 GMT  
		Size: 457.3 KB (457271 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f78958e9095e526aec1fa460aab3532fb13781b52198eeef098980a28f376291`  
		Last Modified: Tue, 08 Aug 2023 20:20:08 GMT  
		Size: 130.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
