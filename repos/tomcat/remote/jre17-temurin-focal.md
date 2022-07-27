## `tomcat:jre17-temurin-focal`

```console
$ docker pull tomcat@sha256:feff2a3276b88a8df5add62b6c147966bcca7fc5a8fb18e77f23c120d3bbf2fa
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 5
	-	linux; amd64
	-	linux; arm variant v7
	-	linux; arm64 variant v8
	-	linux; ppc64le
	-	linux; s390x

### `tomcat:jre17-temurin-focal` - linux; amd64

```console
$ docker pull tomcat@sha256:f5a0df444fe9900ed0348738e6c5ea49c92bbe670e4e4bd7da4a9f6205107535
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **110.2 MB (110175831 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:cc2148c26ef40e09b72a6b9e1abc8c22d331a5b17099d223aff1a167e81e804b`
-	Default Command: `["catalina.sh","run"]`

```dockerfile
# Mon, 06 Jun 2022 22:21:11 GMT
ADD file:00dae10e79b05c4e1a3db053a1f85a4f38a39fe85cbbd88d74201a01a7dd59b5 in / 
# Mon, 06 Jun 2022 22:21:12 GMT
CMD ["bash"]
# Tue, 07 Jun 2022 00:12:30 GMT
ENV LANG=en_US.UTF-8 LANGUAGE=en_US:en LC_ALL=en_US.UTF-8
# Tue, 07 Jun 2022 00:15:30 GMT
RUN apt-get update     && DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends tzdata curl ca-certificates fontconfig locales binutils     && echo "en_US.UTF-8 UTF-8" >> /etc/locale.gen     && locale-gen en_US.UTF-8     && rm -rf /var/lib/apt/lists/*
# Tue, 07 Jun 2022 00:15:30 GMT
ENV JAVA_VERSION=jdk-17.0.3+7
# Tue, 07 Jun 2022 00:16:21 GMT
RUN set -eux;     ARCH="$(dpkg --print-architecture)";     case "${ARCH}" in        aarch64|arm64)          ESUM='b32bf4e18a0befea32c0ff377da7a1753b91477617a9921ceb3dee6964d2799b';          BINARY_URL='https://github.com/adoptium/temurin17-binaries/releases/download/jdk-17.0.3%2B7/OpenJDK17U-jre_aarch64_linux_hotspot_17.0.3_7.tar.gz';          ;;        armhf|arm)          ESUM='fda34743f1ad8b629f42773f6519e87d13876d4b10f98b76cd47b1aa9ad18572';          BINARY_URL='https://github.com/adoptium/temurin17-binaries/releases/download/jdk-17.0.3%2B7/OpenJDK17U-jre_arm_linux_hotspot_17.0.3_7.tar.gz';          ;;        ppc64el|powerpc:common64)          ESUM='257325f38546ce34645f6e8d7e566df401c97a9ae5f107583f9ac71f0f1b04e9';          BINARY_URL='https://github.com/adoptium/temurin17-binaries/releases/download/jdk-17.0.3%2B7/OpenJDK17U-jre_ppc64le_linux_hotspot_17.0.3_7.tar.gz';          ;;        s390x|s390:64-bit)          ESUM='6790e3995a7fb8db99974d213f750bfd1631bfc0dad9946334be34d7b78fdbee';          BINARY_URL='https://github.com/adoptium/temurin17-binaries/releases/download/jdk-17.0.3%2B7/OpenJDK17U-jre_s390x_linux_hotspot_17.0.3_7.tar.gz';          ;;        amd64|i386:x86-64)          ESUM='446b1ac5504d51c2ff9b0cccff079be3ce800cf8c3a3f13bab07f2656aa1fd27';          BINARY_URL='https://github.com/adoptium/temurin17-binaries/releases/download/jdk-17.0.3%2B7/OpenJDK17U-jre_x64_linux_hotspot_17.0.3_7.tar.gz';          ;;        *)          echo "Unsupported arch: ${ARCH}";          exit 1;          ;;     esac;     curl -LfsSo /tmp/openjdk.tar.gz ${BINARY_URL};     echo "${ESUM} */tmp/openjdk.tar.gz" | sha256sum -c -;     mkdir -p /opt/java/openjdk;     cd /opt/java/openjdk;     tar -xf /tmp/openjdk.tar.gz --strip-components=1;     rm -rf /tmp/openjdk.tar.gz;
# Tue, 07 Jun 2022 00:16:22 GMT
ENV JAVA_HOME=/opt/java/openjdk PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 07 Jun 2022 00:16:22 GMT
RUN echo Verifying install ...     && echo java --version && java --version     && echo Complete.
# Tue, 07 Jun 2022 06:29:26 GMT
ENV CATALINA_HOME=/usr/local/tomcat
# Tue, 07 Jun 2022 06:29:26 GMT
ENV PATH=/usr/local/tomcat/bin:/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 07 Jun 2022 06:29:27 GMT
RUN mkdir -p "$CATALINA_HOME"
# Tue, 07 Jun 2022 06:29:27 GMT
WORKDIR /usr/local/tomcat
# Tue, 07 Jun 2022 06:29:27 GMT
ENV TOMCAT_NATIVE_LIBDIR=/usr/local/tomcat/native-jni-lib
# Tue, 07 Jun 2022 06:29:27 GMT
ENV LD_LIBRARY_PATH=/usr/local/tomcat/native-jni-lib
# Tue, 07 Jun 2022 06:29:27 GMT
ENV GPG_KEYS=A9C5DF4D22E99998D9875A5110C01C5A2F6059E7
# Tue, 07 Jun 2022 06:29:27 GMT
ENV TOMCAT_MAJOR=10
# Wed, 27 Jul 2022 01:27:46 GMT
ENV TOMCAT_VERSION=10.0.23
# Wed, 27 Jul 2022 01:27:46 GMT
ENV TOMCAT_SHA512=0e0263e8280f2ccfb4bef916444a6105fef689a3d95c334c8a7bfe59f1e3966d48ea624727f1818a4df331a603f1ac5e21b908dda3cae676ddc1aef90c2d12ab
# Wed, 27 Jul 2022 01:27:47 GMT
COPY dir:ac75a62a42620c530f155a969944682ebebbd5e5a409cdc70d177f5353582993 in /usr/local/tomcat 
# Wed, 27 Jul 2022 01:27:54 GMT
RUN set -eux; 	apt-get update; 	xargs -rt apt-get install -y --no-install-recommends < "$TOMCAT_NATIVE_LIBDIR/.dependencies.txt"; 	rm -rf /var/lib/apt/lists/*
# Wed, 27 Jul 2022 01:27:55 GMT
RUN set -eux; 	nativeLines="$(catalina.sh configtest 2>&1)"; 	nativeLines="$(echo "$nativeLines" | grep 'Apache Tomcat Native')"; 	nativeLines="$(echo "$nativeLines" | sort -u)"; 	if ! echo "$nativeLines" | grep -E 'INFO: Loaded( APR based)? Apache Tomcat Native library' >&2; then 		echo >&2 "$nativeLines"; 		exit 1; 	fi
# Wed, 27 Jul 2022 01:27:55 GMT
EXPOSE 8080
# Wed, 27 Jul 2022 01:27:55 GMT
CMD ["catalina.sh" "run"]
```

-	Layers:
	-	`sha256:d7bfe07ed8476565a440c2113cc64d7c0409dba8ef761fb3ec019d7e6b5952df`  
		Last Modified: Wed, 01 Jun 2022 21:51:10 GMT  
		Size: 28.6 MB (28572632 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a32598539a8f0b55be77078c6637866fc4128a4213ea59e9993662a310a2b711`  
		Last Modified: Tue, 07 Jun 2022 00:22:05 GMT  
		Size: 19.8 MB (19773881 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9c96f165def119d706c2e86c082214c93a07343edb524cc95a4c7701447e5f3d`  
		Last Modified: Tue, 07 Jun 2022 00:23:04 GMT  
		Size: 46.8 MB (46840961 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2880df797d0653bf59426d2fef27e7c6fdb9bb8b8aa0c402b64feac76a60c9a0`  
		Last Modified: Tue, 07 Jun 2022 00:22:57 GMT  
		Size: 162.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b765b1d4f537f62e6522a870bd0db01d08afecdc2e37eb7d6743d461b61e5a24`  
		Last Modified: Tue, 07 Jun 2022 06:47:22 GMT  
		Size: 172.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:356f40b26a179c2e617f039cc677c9a171c2d4d43d656c19f400e0528cf39477`  
		Last Modified: Wed, 27 Jul 2022 01:53:35 GMT  
		Size: 12.6 MB (12632758 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:374cc3af98426771e2b132dc6838587b8759e103bb5205f1d658d5d0af5b2bcc`  
		Last Modified: Wed, 27 Jul 2022 01:53:35 GMT  
		Size: 2.4 MB (2355136 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bf2fc9b38634e82ba9ade125f666c01ba477741c439c8cdcbc63f92d8c768b5e`  
		Last Modified: Wed, 27 Jul 2022 01:53:34 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `tomcat:jre17-temurin-focal` - linux; arm variant v7

```console
$ docker pull tomcat@sha256:3d6aca8e668dab8871afda03c2a733c263fae0e0ada0bdbdbd585e74e535af80
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **102.7 MB (102708263 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:737d35ceeefbad9766a8ebc5c38500730aa6f7ed6220f39d9f3a6a08957ebc99`
-	Default Command: `["catalina.sh","run"]`

```dockerfile
# Tue, 07 Jun 2022 05:50:50 GMT
ADD file:c95d34737ba1f11ac8b92be0125aad2baae46448f0d8ebd85ad69076006a3254 in / 
# Tue, 07 Jun 2022 05:50:51 GMT
CMD ["bash"]
# Tue, 07 Jun 2022 09:33:43 GMT
ENV LANG=en_US.UTF-8 LANGUAGE=en_US:en LC_ALL=en_US.UTF-8
# Tue, 07 Jun 2022 09:41:33 GMT
RUN apt-get update     && DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends tzdata curl ca-certificates fontconfig locales binutils     && echo "en_US.UTF-8 UTF-8" >> /etc/locale.gen     && locale-gen en_US.UTF-8     && rm -rf /var/lib/apt/lists/*
# Tue, 07 Jun 2022 09:41:34 GMT
ENV JAVA_VERSION=jdk-17.0.3+7
# Tue, 07 Jun 2022 09:43:59 GMT
RUN set -eux;     ARCH="$(dpkg --print-architecture)";     case "${ARCH}" in        aarch64|arm64)          ESUM='b32bf4e18a0befea32c0ff377da7a1753b91477617a9921ceb3dee6964d2799b';          BINARY_URL='https://github.com/adoptium/temurin17-binaries/releases/download/jdk-17.0.3%2B7/OpenJDK17U-jre_aarch64_linux_hotspot_17.0.3_7.tar.gz';          ;;        armhf|arm)          ESUM='fda34743f1ad8b629f42773f6519e87d13876d4b10f98b76cd47b1aa9ad18572';          BINARY_URL='https://github.com/adoptium/temurin17-binaries/releases/download/jdk-17.0.3%2B7/OpenJDK17U-jre_arm_linux_hotspot_17.0.3_7.tar.gz';          ;;        ppc64el|powerpc:common64)          ESUM='257325f38546ce34645f6e8d7e566df401c97a9ae5f107583f9ac71f0f1b04e9';          BINARY_URL='https://github.com/adoptium/temurin17-binaries/releases/download/jdk-17.0.3%2B7/OpenJDK17U-jre_ppc64le_linux_hotspot_17.0.3_7.tar.gz';          ;;        s390x|s390:64-bit)          ESUM='6790e3995a7fb8db99974d213f750bfd1631bfc0dad9946334be34d7b78fdbee';          BINARY_URL='https://github.com/adoptium/temurin17-binaries/releases/download/jdk-17.0.3%2B7/OpenJDK17U-jre_s390x_linux_hotspot_17.0.3_7.tar.gz';          ;;        amd64|i386:x86-64)          ESUM='446b1ac5504d51c2ff9b0cccff079be3ce800cf8c3a3f13bab07f2656aa1fd27';          BINARY_URL='https://github.com/adoptium/temurin17-binaries/releases/download/jdk-17.0.3%2B7/OpenJDK17U-jre_x64_linux_hotspot_17.0.3_7.tar.gz';          ;;        *)          echo "Unsupported arch: ${ARCH}";          exit 1;          ;;     esac;     curl -LfsSo /tmp/openjdk.tar.gz ${BINARY_URL};     echo "${ESUM} */tmp/openjdk.tar.gz" | sha256sum -c -;     mkdir -p /opt/java/openjdk;     cd /opt/java/openjdk;     tar -xf /tmp/openjdk.tar.gz --strip-components=1;     rm -rf /tmp/openjdk.tar.gz;
# Tue, 07 Jun 2022 09:44:00 GMT
ENV JAVA_HOME=/opt/java/openjdk PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 07 Jun 2022 09:44:02 GMT
RUN echo Verifying install ...     && echo java --version && java --version     && echo Complete.
# Wed, 27 Jul 2022 11:09:50 GMT
ENV CATALINA_HOME=/usr/local/tomcat
# Wed, 27 Jul 2022 11:09:50 GMT
ENV PATH=/usr/local/tomcat/bin:/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 27 Jul 2022 11:09:50 GMT
RUN mkdir -p "$CATALINA_HOME"
# Wed, 27 Jul 2022 11:09:50 GMT
WORKDIR /usr/local/tomcat
# Wed, 27 Jul 2022 11:09:51 GMT
ENV TOMCAT_NATIVE_LIBDIR=/usr/local/tomcat/native-jni-lib
# Wed, 27 Jul 2022 11:09:51 GMT
ENV LD_LIBRARY_PATH=/usr/local/tomcat/native-jni-lib
# Wed, 27 Jul 2022 11:09:51 GMT
ENV GPG_KEYS=A9C5DF4D22E99998D9875A5110C01C5A2F6059E7
# Wed, 27 Jul 2022 11:09:51 GMT
ENV TOMCAT_MAJOR=10
# Wed, 27 Jul 2022 11:09:51 GMT
ENV TOMCAT_VERSION=10.0.23
# Wed, 27 Jul 2022 11:09:51 GMT
ENV TOMCAT_SHA512=0e0263e8280f2ccfb4bef916444a6105fef689a3d95c334c8a7bfe59f1e3966d48ea624727f1818a4df331a603f1ac5e21b908dda3cae676ddc1aef90c2d12ab
# Wed, 27 Jul 2022 11:09:52 GMT
COPY dir:8aac4b314b853b33e7683c7a1a8aa9f411b708518fcd877a5e2cc126862063ec in /usr/local/tomcat 
# Wed, 27 Jul 2022 11:10:00 GMT
RUN set -eux; 	apt-get update; 	xargs -rt apt-get install -y --no-install-recommends < "$TOMCAT_NATIVE_LIBDIR/.dependencies.txt"; 	rm -rf /var/lib/apt/lists/*
# Wed, 27 Jul 2022 11:10:01 GMT
RUN set -eux; 	nativeLines="$(catalina.sh configtest 2>&1)"; 	nativeLines="$(echo "$nativeLines" | grep 'Apache Tomcat Native')"; 	nativeLines="$(echo "$nativeLines" | sort -u)"; 	if ! echo "$nativeLines" | grep -E 'INFO: Loaded( APR based)? Apache Tomcat Native library' >&2; then 		echo >&2 "$nativeLines"; 		exit 1; 	fi
# Wed, 27 Jul 2022 11:10:02 GMT
EXPOSE 8080
# Wed, 27 Jul 2022 11:10:02 GMT
CMD ["catalina.sh" "run"]
```

-	Layers:
	-	`sha256:36754881d0ec0d456ee49776d62f6f0df47d29956ac7b2231b797e05780c6744`  
		Last Modified: Tue, 07 Jun 2022 05:55:05 GMT  
		Size: 24.6 MB (24592639 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c1a22ec594d8f8b03d4226421978317b6cbae6f7beba70a96500f2934f78da24`  
		Last Modified: Tue, 07 Jun 2022 09:58:12 GMT  
		Size: 19.2 MB (19196476 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9bc76517832621f178ae6932a2085fc084aca7f0b978c12b92c44147e7daa4dd`  
		Last Modified: Tue, 07 Jun 2022 10:01:24 GMT  
		Size: 44.4 MB (44363361 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2965aa4bc8652036619ce48f510ccdff7e5d4fef47b351c5764d130cb26ad140`  
		Last Modified: Tue, 07 Jun 2022 10:00:56 GMT  
		Size: 159.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:07658af84c379eac765656acdc0987d475f33f8f00b04bd0b9d1c8fb025630d1`  
		Last Modified: Wed, 27 Jul 2022 11:47:12 GMT  
		Size: 174.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3a4134a1e9eb57d5dbe253f1c49644dfafe43d39fc5b4cd4b58548c7948ba61f`  
		Last Modified: Wed, 27 Jul 2022 11:47:13 GMT  
		Size: 12.6 MB (12583258 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ce8efe9ad49ff2c0caba5f1dd0db6652f6e33a833dae8e5e50292855475ea604`  
		Last Modified: Wed, 27 Jul 2022 11:47:12 GMT  
		Size: 2.0 MB (1972065 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:832141b3f3f2cdde92fb893fee79065aa0b53ce0b7f7a61668ac8a0c68c58ecd`  
		Last Modified: Wed, 27 Jul 2022 11:47:12 GMT  
		Size: 131.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `tomcat:jre17-temurin-focal` - linux; arm64 variant v8

```console
$ docker pull tomcat@sha256:899bd7e6b3e029ce6480fb1e2e7218c0bc637c48dcdd055b810cb24667240cc9
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **108.8 MB (108835350 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d8043897a75087dcf007bbea54611649f3e999cfef8b309ae39a4285d9439bc4`
-	Default Command: `["catalina.sh","run"]`

```dockerfile
# Tue, 07 Jun 2022 01:25:15 GMT
ADD file:8bb0809a8ac8e978274cf731cff7529372088d22c5b0233a28f01ef414aefbca in / 
# Tue, 07 Jun 2022 01:25:16 GMT
CMD ["bash"]
# Tue, 07 Jun 2022 04:59:51 GMT
ENV LANG=en_US.UTF-8 LANGUAGE=en_US:en LC_ALL=en_US.UTF-8
# Tue, 07 Jun 2022 05:06:48 GMT
RUN apt-get update     && DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends tzdata curl ca-certificates fontconfig locales binutils     && echo "en_US.UTF-8 UTF-8" >> /etc/locale.gen     && locale-gen en_US.UTF-8     && rm -rf /var/lib/apt/lists/*
# Tue, 07 Jun 2022 06:36:39 GMT
ENV JAVA_VERSION=jdk-17.0.3+7
# Tue, 07 Jun 2022 06:37:50 GMT
RUN set -eux;     ARCH="$(dpkg --print-architecture)";     case "${ARCH}" in        aarch64|arm64)          ESUM='b32bf4e18a0befea32c0ff377da7a1753b91477617a9921ceb3dee6964d2799b';          BINARY_URL='https://github.com/adoptium/temurin17-binaries/releases/download/jdk-17.0.3%2B7/OpenJDK17U-jre_aarch64_linux_hotspot_17.0.3_7.tar.gz';          ;;        armhf|arm)          ESUM='fda34743f1ad8b629f42773f6519e87d13876d4b10f98b76cd47b1aa9ad18572';          BINARY_URL='https://github.com/adoptium/temurin17-binaries/releases/download/jdk-17.0.3%2B7/OpenJDK17U-jre_arm_linux_hotspot_17.0.3_7.tar.gz';          ;;        ppc64el|powerpc:common64)          ESUM='257325f38546ce34645f6e8d7e566df401c97a9ae5f107583f9ac71f0f1b04e9';          BINARY_URL='https://github.com/adoptium/temurin17-binaries/releases/download/jdk-17.0.3%2B7/OpenJDK17U-jre_ppc64le_linux_hotspot_17.0.3_7.tar.gz';          ;;        s390x|s390:64-bit)          ESUM='6790e3995a7fb8db99974d213f750bfd1631bfc0dad9946334be34d7b78fdbee';          BINARY_URL='https://github.com/adoptium/temurin17-binaries/releases/download/jdk-17.0.3%2B7/OpenJDK17U-jre_s390x_linux_hotspot_17.0.3_7.tar.gz';          ;;        amd64|i386:x86-64)          ESUM='446b1ac5504d51c2ff9b0cccff079be3ce800cf8c3a3f13bab07f2656aa1fd27';          BINARY_URL='https://github.com/adoptium/temurin17-binaries/releases/download/jdk-17.0.3%2B7/OpenJDK17U-jre_x64_linux_hotspot_17.0.3_7.tar.gz';          ;;        *)          echo "Unsupported arch: ${ARCH}";          exit 1;          ;;     esac;     curl -LfsSo /tmp/openjdk.tar.gz ${BINARY_URL};     echo "${ESUM} */tmp/openjdk.tar.gz" | sha256sum -c -;     mkdir -p /opt/java/openjdk;     cd /opt/java/openjdk;     tar -xf /tmp/openjdk.tar.gz --strip-components=1;     rm -rf /tmp/openjdk.tar.gz;
# Tue, 07 Jun 2022 06:37:50 GMT
ENV JAVA_HOME=/opt/java/openjdk PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 07 Jun 2022 06:37:51 GMT
RUN echo Verifying install ...     && echo java --version && java --version     && echo Complete.
# Tue, 07 Jun 2022 10:47:44 GMT
ENV CATALINA_HOME=/usr/local/tomcat
# Tue, 07 Jun 2022 10:47:45 GMT
ENV PATH=/usr/local/tomcat/bin:/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 07 Jun 2022 10:47:46 GMT
RUN mkdir -p "$CATALINA_HOME"
# Tue, 07 Jun 2022 10:47:47 GMT
WORKDIR /usr/local/tomcat
# Tue, 07 Jun 2022 10:47:48 GMT
ENV TOMCAT_NATIVE_LIBDIR=/usr/local/tomcat/native-jni-lib
# Tue, 07 Jun 2022 10:47:49 GMT
ENV LD_LIBRARY_PATH=/usr/local/tomcat/native-jni-lib
# Tue, 07 Jun 2022 10:47:50 GMT
ENV GPG_KEYS=A9C5DF4D22E99998D9875A5110C01C5A2F6059E7
# Tue, 07 Jun 2022 10:47:51 GMT
ENV TOMCAT_MAJOR=10
# Wed, 27 Jul 2022 02:11:47 GMT
ENV TOMCAT_VERSION=10.0.23
# Wed, 27 Jul 2022 02:11:47 GMT
ENV TOMCAT_SHA512=0e0263e8280f2ccfb4bef916444a6105fef689a3d95c334c8a7bfe59f1e3966d48ea624727f1818a4df331a603f1ac5e21b908dda3cae676ddc1aef90c2d12ab
# Wed, 27 Jul 2022 02:11:49 GMT
COPY dir:7c6d7655dba7fc87e0e7c647a7e2f99efca150f2b61df555bc76a8078612c8f7 in /usr/local/tomcat 
# Wed, 27 Jul 2022 02:11:56 GMT
RUN set -eux; 	apt-get update; 	xargs -rt apt-get install -y --no-install-recommends < "$TOMCAT_NATIVE_LIBDIR/.dependencies.txt"; 	rm -rf /var/lib/apt/lists/*
# Wed, 27 Jul 2022 02:11:58 GMT
RUN set -eux; 	nativeLines="$(catalina.sh configtest 2>&1)"; 	nativeLines="$(echo "$nativeLines" | grep 'Apache Tomcat Native')"; 	nativeLines="$(echo "$nativeLines" | sort -u)"; 	if ! echo "$nativeLines" | grep -E 'INFO: Loaded( APR based)? Apache Tomcat Native library' >&2; then 		echo >&2 "$nativeLines"; 		exit 1; 	fi
# Wed, 27 Jul 2022 02:11:59 GMT
EXPOSE 8080
# Wed, 27 Jul 2022 02:12:00 GMT
CMD ["catalina.sh" "run"]
```

-	Layers:
	-	`sha256:11e23ac719b33170b39b7e30b8027dc09c9cbad6b503b2b6b3ebbd9d33f4adad`  
		Last Modified: Thu, 02 Jun 2022 08:33:07 GMT  
		Size: 27.2 MB (27191210 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:68e4a04805fb472806936ea1417715c9eeb219259a6a6fc44afc367c1d8c5b69`  
		Last Modified: Tue, 07 Jun 2022 05:12:45 GMT  
		Size: 20.5 MB (20500981 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e41ee0d8f3dce0b9899541d38046fddeb37199fc18fd7a0f1bce768cbb028cec`  
		Last Modified: Tue, 07 Jun 2022 06:45:57 GMT  
		Size: 46.3 MB (46273239 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bdd3adec87ea73d8389e852dfa694f418fee963829aa520b51a0c0053b13682f`  
		Last Modified: Tue, 07 Jun 2022 06:45:51 GMT  
		Size: 127.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c1c949faf28852f31b19a153320eb01c7220a7ddc51c2283e34d537b2fc09fa0`  
		Last Modified: Tue, 07 Jun 2022 11:21:48 GMT  
		Size: 138.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a8db2e144fb113e1f4d303d91cc78665ee67c8da2b14de9387be758faff0c86b`  
		Last Modified: Wed, 27 Jul 2022 02:50:30 GMT  
		Size: 12.7 MB (12650714 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:508f2cc03a65b12eb02cf6ff4f78fc2b6d47e6c1925dacbda6f14bda81574edf`  
		Last Modified: Wed, 27 Jul 2022 02:50:29 GMT  
		Size: 2.2 MB (2218941 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `tomcat:jre17-temurin-focal` - linux; ppc64le

```console
$ docker pull tomcat@sha256:571a8b0cc3dfc03e7e8971143210376ab2a3e25a0a1cdd8808581ade3eec5fd6
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **114.8 MB (114823567 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:368c056e99a01edee4121fe850a8aac2f2382b3d8d3c8329f4e467174b037389`
-	Default Command: `["catalina.sh","run"]`

```dockerfile
# Tue, 07 Jun 2022 05:46:02 GMT
ADD file:86506a94b834ba2b6f10dc0d1955bee539be1cf565e4ccc2c4bc074e0375f115 in / 
# Tue, 07 Jun 2022 05:46:06 GMT
CMD ["bash"]
# Wed, 27 Jul 2022 00:33:57 GMT
ENV LANG=en_US.UTF-8 LANGUAGE=en_US:en LC_ALL=en_US.UTF-8
# Wed, 27 Jul 2022 00:41:17 GMT
RUN apt-get update     && DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends tzdata curl ca-certificates fontconfig locales binutils     && echo "en_US.UTF-8 UTF-8" >> /etc/locale.gen     && locale-gen en_US.UTF-8     && rm -rf /var/lib/apt/lists/*
# Wed, 27 Jul 2022 00:41:18 GMT
ENV JAVA_VERSION=jdk-17.0.3+7
# Wed, 27 Jul 2022 00:44:39 GMT
RUN set -eux;     ARCH="$(dpkg --print-architecture)";     case "${ARCH}" in        aarch64|arm64)          ESUM='b32bf4e18a0befea32c0ff377da7a1753b91477617a9921ceb3dee6964d2799b';          BINARY_URL='https://github.com/adoptium/temurin17-binaries/releases/download/jdk-17.0.3%2B7/OpenJDK17U-jre_aarch64_linux_hotspot_17.0.3_7.tar.gz';          ;;        armhf|arm)          ESUM='fda34743f1ad8b629f42773f6519e87d13876d4b10f98b76cd47b1aa9ad18572';          BINARY_URL='https://github.com/adoptium/temurin17-binaries/releases/download/jdk-17.0.3%2B7/OpenJDK17U-jre_arm_linux_hotspot_17.0.3_7.tar.gz';          ;;        ppc64el|powerpc:common64)          ESUM='257325f38546ce34645f6e8d7e566df401c97a9ae5f107583f9ac71f0f1b04e9';          BINARY_URL='https://github.com/adoptium/temurin17-binaries/releases/download/jdk-17.0.3%2B7/OpenJDK17U-jre_ppc64le_linux_hotspot_17.0.3_7.tar.gz';          ;;        s390x|s390:64-bit)          ESUM='6790e3995a7fb8db99974d213f750bfd1631bfc0dad9946334be34d7b78fdbee';          BINARY_URL='https://github.com/adoptium/temurin17-binaries/releases/download/jdk-17.0.3%2B7/OpenJDK17U-jre_s390x_linux_hotspot_17.0.3_7.tar.gz';          ;;        amd64|i386:x86-64)          ESUM='446b1ac5504d51c2ff9b0cccff079be3ce800cf8c3a3f13bab07f2656aa1fd27';          BINARY_URL='https://github.com/adoptium/temurin17-binaries/releases/download/jdk-17.0.3%2B7/OpenJDK17U-jre_x64_linux_hotspot_17.0.3_7.tar.gz';          ;;        *)          echo "Unsupported arch: ${ARCH}";          exit 1;          ;;     esac;     curl -LfsSo /tmp/openjdk.tar.gz ${BINARY_URL};     echo "${ESUM} */tmp/openjdk.tar.gz" | sha256sum -c -;     mkdir -p /opt/java/openjdk;     cd /opt/java/openjdk;     tar -xf /tmp/openjdk.tar.gz --strip-components=1;     rm -rf /tmp/openjdk.tar.gz;
# Wed, 27 Jul 2022 00:44:40 GMT
ENV JAVA_HOME=/opt/java/openjdk PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 27 Jul 2022 00:44:41 GMT
RUN echo Verifying install ...     && echo java --version && java --version     && echo Complete.
# Wed, 27 Jul 2022 14:53:30 GMT
ENV CATALINA_HOME=/usr/local/tomcat
# Wed, 27 Jul 2022 14:53:31 GMT
ENV PATH=/usr/local/tomcat/bin:/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 27 Jul 2022 14:53:32 GMT
RUN mkdir -p "$CATALINA_HOME"
# Wed, 27 Jul 2022 14:53:32 GMT
WORKDIR /usr/local/tomcat
# Wed, 27 Jul 2022 14:53:32 GMT
ENV TOMCAT_NATIVE_LIBDIR=/usr/local/tomcat/native-jni-lib
# Wed, 27 Jul 2022 14:53:33 GMT
ENV LD_LIBRARY_PATH=/usr/local/tomcat/native-jni-lib
# Wed, 27 Jul 2022 14:53:33 GMT
ENV GPG_KEYS=A9C5DF4D22E99998D9875A5110C01C5A2F6059E7
# Wed, 27 Jul 2022 14:53:33 GMT
ENV TOMCAT_MAJOR=10
# Wed, 27 Jul 2022 14:53:34 GMT
ENV TOMCAT_VERSION=10.0.23
# Wed, 27 Jul 2022 14:53:34 GMT
ENV TOMCAT_SHA512=0e0263e8280f2ccfb4bef916444a6105fef689a3d95c334c8a7bfe59f1e3966d48ea624727f1818a4df331a603f1ac5e21b908dda3cae676ddc1aef90c2d12ab
# Wed, 27 Jul 2022 14:53:35 GMT
COPY dir:abe1fdb9feb6ca472e1b8acd3cafbf54ada10f5a9438b1fb213c27700f4772d2 in /usr/local/tomcat 
# Wed, 27 Jul 2022 14:53:44 GMT
RUN set -eux; 	apt-get update; 	xargs -rt apt-get install -y --no-install-recommends < "$TOMCAT_NATIVE_LIBDIR/.dependencies.txt"; 	rm -rf /var/lib/apt/lists/*
# Wed, 27 Jul 2022 14:53:46 GMT
RUN set -eux; 	nativeLines="$(catalina.sh configtest 2>&1)"; 	nativeLines="$(echo "$nativeLines" | grep 'Apache Tomcat Native')"; 	nativeLines="$(echo "$nativeLines" | sort -u)"; 	if ! echo "$nativeLines" | grep -E 'INFO: Loaded( APR based)? Apache Tomcat Native library' >&2; then 		echo >&2 "$nativeLines"; 		exit 1; 	fi
# Wed, 27 Jul 2022 14:53:46 GMT
EXPOSE 8080
# Wed, 27 Jul 2022 14:53:47 GMT
CMD ["catalina.sh" "run"]
```

-	Layers:
	-	`sha256:3f52d061d2d3fdde0d3a099bbeae64080476c9650e9f3ba05de898d5bb5f03e8`  
		Last Modified: Tue, 07 Jun 2022 05:49:10 GMT  
		Size: 33.3 MB (33294345 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:abff6ca525e26e65e4f33725ff2f731fb66f9fa21452fe1cff1f1d65d9860921`  
		Last Modified: Wed, 27 Jul 2022 00:55:32 GMT  
		Size: 21.7 MB (21686416 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1b595bf3d0417ac8157de67621bc5b78ae1f4b5be86c40cc7bff07bde5c5d02c`  
		Last Modified: Wed, 27 Jul 2022 00:57:42 GMT  
		Size: 46.7 MB (46695066 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f1490854d4fe9b684e23626038bb058c78e2f89c469f68bea318d5dd1346cb13`  
		Last Modified: Wed, 27 Jul 2022 00:57:30 GMT  
		Size: 159.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:581124e39a033e27ce031331224a199c5ec158682d94b9da3d3e1da01876cffb`  
		Last Modified: Wed, 27 Jul 2022 15:35:28 GMT  
		Size: 173.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6dfd215a4c66869beb3d523bda2a70a3e27da60e41c65be940a639534384494f`  
		Last Modified: Wed, 27 Jul 2022 15:35:30 GMT  
		Size: 12.7 MB (12673352 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f1f7d538832ce38b045a0f9f2a43a5406950e08eaead440fa4d9458f2e707454`  
		Last Modified: Wed, 27 Jul 2022 15:35:28 GMT  
		Size: 473.9 KB (473926 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:df32d7d1a9d8c2e88b2a1265607513d787d70425279811e9f566797efc9a4873`  
		Last Modified: Wed, 27 Jul 2022 15:35:28 GMT  
		Size: 130.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `tomcat:jre17-temurin-focal` - linux; s390x

```console
$ docker pull tomcat@sha256:82f4a8692b26d99e3998b6dec32f6c61663bb6664c3733e818afd88f3bb46d21
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **104.7 MB (104657394 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:9fa9548ee3ee831f456c7576c257d5eccfc97666d818aa2d46f160a8d78772ce`
-	Default Command: `["catalina.sh","run"]`

```dockerfile
# Tue, 07 Jun 2022 04:05:02 GMT
ADD file:6250f895d7d6c591cfe1b9fc991313d21b02167d94c67991db7c5c1c6814c51e in / 
# Tue, 07 Jun 2022 04:05:06 GMT
CMD ["bash"]
# Tue, 07 Jun 2022 06:11:05 GMT
ENV LANG=en_US.UTF-8 LANGUAGE=en_US:en LC_ALL=en_US.UTF-8
# Tue, 07 Jun 2022 06:19:54 GMT
RUN apt-get update     && DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends tzdata curl ca-certificates fontconfig locales binutils     && echo "en_US.UTF-8 UTF-8" >> /etc/locale.gen     && locale-gen en_US.UTF-8     && rm -rf /var/lib/apt/lists/*
# Tue, 07 Jun 2022 06:36:16 GMT
ENV JAVA_VERSION=jdk-17.0.3+7
# Tue, 07 Jun 2022 06:38:50 GMT
RUN set -eux;     ARCH="$(dpkg --print-architecture)";     case "${ARCH}" in        aarch64|arm64)          ESUM='b32bf4e18a0befea32c0ff377da7a1753b91477617a9921ceb3dee6964d2799b';          BINARY_URL='https://github.com/adoptium/temurin17-binaries/releases/download/jdk-17.0.3%2B7/OpenJDK17U-jre_aarch64_linux_hotspot_17.0.3_7.tar.gz';          ;;        armhf|arm)          ESUM='fda34743f1ad8b629f42773f6519e87d13876d4b10f98b76cd47b1aa9ad18572';          BINARY_URL='https://github.com/adoptium/temurin17-binaries/releases/download/jdk-17.0.3%2B7/OpenJDK17U-jre_arm_linux_hotspot_17.0.3_7.tar.gz';          ;;        ppc64el|powerpc:common64)          ESUM='257325f38546ce34645f6e8d7e566df401c97a9ae5f107583f9ac71f0f1b04e9';          BINARY_URL='https://github.com/adoptium/temurin17-binaries/releases/download/jdk-17.0.3%2B7/OpenJDK17U-jre_ppc64le_linux_hotspot_17.0.3_7.tar.gz';          ;;        s390x|s390:64-bit)          ESUM='6790e3995a7fb8db99974d213f750bfd1631bfc0dad9946334be34d7b78fdbee';          BINARY_URL='https://github.com/adoptium/temurin17-binaries/releases/download/jdk-17.0.3%2B7/OpenJDK17U-jre_s390x_linux_hotspot_17.0.3_7.tar.gz';          ;;        amd64|i386:x86-64)          ESUM='446b1ac5504d51c2ff9b0cccff079be3ce800cf8c3a3f13bab07f2656aa1fd27';          BINARY_URL='https://github.com/adoptium/temurin17-binaries/releases/download/jdk-17.0.3%2B7/OpenJDK17U-jre_x64_linux_hotspot_17.0.3_7.tar.gz';          ;;        *)          echo "Unsupported arch: ${ARCH}";          exit 1;          ;;     esac;     curl -LfsSo /tmp/openjdk.tar.gz ${BINARY_URL};     echo "${ESUM} */tmp/openjdk.tar.gz" | sha256sum -c -;     mkdir -p /opt/java/openjdk;     cd /opt/java/openjdk;     tar -xf /tmp/openjdk.tar.gz --strip-components=1;     rm -rf /tmp/openjdk.tar.gz;
# Tue, 07 Jun 2022 06:38:55 GMT
ENV JAVA_HOME=/opt/java/openjdk PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 07 Jun 2022 06:38:56 GMT
RUN echo Verifying install ...     && echo java --version && java --version     && echo Complete.
# Tue, 07 Jun 2022 10:37:06 GMT
ENV CATALINA_HOME=/usr/local/tomcat
# Tue, 07 Jun 2022 10:37:07 GMT
ENV PATH=/usr/local/tomcat/bin:/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 07 Jun 2022 10:37:09 GMT
RUN mkdir -p "$CATALINA_HOME"
# Tue, 07 Jun 2022 10:37:10 GMT
WORKDIR /usr/local/tomcat
# Tue, 07 Jun 2022 10:37:10 GMT
ENV TOMCAT_NATIVE_LIBDIR=/usr/local/tomcat/native-jni-lib
# Tue, 07 Jun 2022 10:37:11 GMT
ENV LD_LIBRARY_PATH=/usr/local/tomcat/native-jni-lib
# Tue, 07 Jun 2022 10:37:12 GMT
ENV GPG_KEYS=A9C5DF4D22E99998D9875A5110C01C5A2F6059E7
# Tue, 07 Jun 2022 10:37:13 GMT
ENV TOMCAT_MAJOR=10
# Wed, 27 Jul 2022 01:31:04 GMT
ENV TOMCAT_VERSION=10.0.23
# Wed, 27 Jul 2022 01:31:05 GMT
ENV TOMCAT_SHA512=0e0263e8280f2ccfb4bef916444a6105fef689a3d95c334c8a7bfe59f1e3966d48ea624727f1818a4df331a603f1ac5e21b908dda3cae676ddc1aef90c2d12ab
# Wed, 27 Jul 2022 01:31:05 GMT
COPY dir:e59526d057c7e4f39330382ec66581a48efdecb2f41125e8422977a0d5e301c8 in /usr/local/tomcat 
# Wed, 27 Jul 2022 01:31:09 GMT
RUN set -eux; 	apt-get update; 	xargs -rt apt-get install -y --no-install-recommends < "$TOMCAT_NATIVE_LIBDIR/.dependencies.txt"; 	rm -rf /var/lib/apt/lists/*
# Wed, 27 Jul 2022 01:31:10 GMT
RUN set -eux; 	nativeLines="$(catalina.sh configtest 2>&1)"; 	nativeLines="$(echo "$nativeLines" | grep 'Apache Tomcat Native')"; 	nativeLines="$(echo "$nativeLines" | sort -u)"; 	if ! echo "$nativeLines" | grep -E 'INFO: Loaded( APR based)? Apache Tomcat Native library' >&2; then 		echo >&2 "$nativeLines"; 		exit 1; 	fi
# Wed, 27 Jul 2022 01:31:11 GMT
EXPOSE 8080
# Wed, 27 Jul 2022 01:31:11 GMT
CMD ["catalina.sh" "run"]
```

-	Layers:
	-	`sha256:2f1fac119b88f55cd8329458ec27c3d6d6cb324b0fe541feacfd9a4ee621a558`  
		Last Modified: Tue, 07 Jun 2022 04:07:45 GMT  
		Size: 27.1 MB (27056020 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8b03f2d497bd002a5fc2d0070513cb6b5efa08e1c570c55fd15d3d4c89622e29`  
		Last Modified: Tue, 07 Jun 2022 06:25:49 GMT  
		Size: 19.2 MB (19229549 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a157f755a6f207b2c8fc4a018b5cda6d53c448447f84b315daa72b9fed583a61`  
		Last Modified: Tue, 07 Jun 2022 06:44:39 GMT  
		Size: 43.7 MB (43671718 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:93fd41b6f4e1e27165dbca0a198c8d6fa49517a9699f5cad193672434841b380`  
		Last Modified: Tue, 07 Jun 2022 06:44:33 GMT  
		Size: 160.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:13047eefdf206817f87424fa292284ad1661379fc6f93757b7bed2666e0caea8`  
		Last Modified: Tue, 07 Jun 2022 10:54:50 GMT  
		Size: 171.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:432826e12315d88df3827d6536051943ae276acbc2a62fef3de9f88b3b56ae93`  
		Last Modified: Wed, 27 Jul 2022 01:42:55 GMT  
		Size: 12.6 MB (12645835 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f1a05b32d4330782cd8fff6446155bfe836ae232a2b55b7c3692f6a1b63288a3`  
		Last Modified: Wed, 27 Jul 2022 01:42:55 GMT  
		Size: 2.1 MB (2053811 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7ab3d573ab009df476a73434d57c8d4f9f043987cb08c0dd943345badc9e5c82`  
		Last Modified: Wed, 27 Jul 2022 01:42:55 GMT  
		Size: 130.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
