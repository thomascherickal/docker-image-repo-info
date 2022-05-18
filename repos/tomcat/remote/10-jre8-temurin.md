## `tomcat:10-jre8-temurin`

```console
$ docker pull tomcat@sha256:0e768d2a6bceb83591a1387f9b915ef94cac3ba221f615160789cf1fdd7862fc
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 4
	-	linux; amd64
	-	linux; arm variant v7
	-	linux; arm64 variant v8
	-	linux; ppc64le

### `tomcat:10-jre8-temurin` - linux; amd64

```console
$ docker pull tomcat@sha256:2fa0d3a0fea7d0a681cdfc83725451cac1a145abe78bb4df8a3b613fe36bc92c
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **101.3 MB (101340387 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:cf1f7033e1369f6bb02242bd65e23d58cfbbade76265bc1109d00e5b2b15522b`
-	Default Command: `["catalina.sh","run"]`

```dockerfile
# Fri, 29 Apr 2022 23:20:59 GMT
ADD file:7009ad0ee0bbe5ed7f381792e07347e260e6896aeee0d80597808065120fa96b in / 
# Fri, 29 Apr 2022 23:20:59 GMT
CMD ["bash"]
# Sat, 30 Apr 2022 00:22:32 GMT
ENV LANG=en_US.UTF-8 LANGUAGE=en_US:en LC_ALL=en_US.UTF-8
# Sat, 30 Apr 2022 00:22:47 GMT
RUN apt-get update     && DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends tzdata curl ca-certificates fontconfig locales     && echo "en_US.UTF-8 UTF-8" >> /etc/locale.gen     && locale-gen en_US.UTF-8     && rm -rf /var/lib/apt/lists/*
# Thu, 05 May 2022 18:27:10 GMT
ENV JAVA_VERSION=jdk8u332-b09
# Thu, 05 May 2022 18:27:46 GMT
RUN set -eux;     ARCH="$(dpkg --print-architecture)";     case "${ARCH}" in        aarch64|arm64)          ESUM='be92e658ed7f6b14b3b945700d7a4f87467c682b70dfbf682ca4562b93cfc8e0';          BINARY_URL='https://github.com/adoptium/temurin8-binaries/releases/download/jdk8u332-b09/OpenJDK8U-jre_aarch64_linux_hotspot_8u332b09.tar.gz';          ;;        armhf|arm)          ESUM='72adfae646b7866aedd28c20a874181c8f3835ccb16610c47e0ca0780f8f9a9c';          BINARY_URL='https://github.com/adoptium/temurin8-binaries/releases/download/jdk8u332-b09/OpenJDK8U-jre_arm_linux_hotspot_8u332b09.tar.gz';          apt-get update          && DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends libatomic1          && rm -rf /var/lib/apt/lists/*          ;;        ppc64el|powerpc:common64)          ESUM='3c7434b248b0edd23a5ac0d8244382725d90e1214f0ddc73a0ead5ad5ceffdaa';          BINARY_URL='https://github.com/adoptium/temurin8-binaries/releases/download/jdk8u332-b09/OpenJDK8U-jre_ppc64le_linux_hotspot_8u332b09.tar.gz';          ;;        amd64|i386:x86-64)          ESUM='34454309b43d585047baaefc36c1850d0192cccc8b52cdc4aadb192b8e3e4c81';          BINARY_URL='https://github.com/adoptium/temurin8-binaries/releases/download/jdk8u332-b09/OpenJDK8U-jre_x64_linux_hotspot_8u332b09.tar.gz';          ;;        *)          echo "Unsupported arch: ${ARCH}";          exit 1;          ;;     esac;     curl -LfsSo /tmp/openjdk.tar.gz ${BINARY_URL};     echo "${ESUM} */tmp/openjdk.tar.gz" | sha256sum -c -;     mkdir -p /opt/java/openjdk;     cd /opt/java/openjdk;     tar -xf /tmp/openjdk.tar.gz --strip-components=1;     rm -rf /tmp/openjdk.tar.gz;
# Thu, 05 May 2022 18:27:46 GMT
ENV JAVA_HOME=/opt/java/openjdk PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 05 May 2022 18:27:47 GMT
RUN echo Verifying install ...     && echo java -version && java -version     && echo Complete.
# Thu, 05 May 2022 19:08:14 GMT
ENV CATALINA_HOME=/usr/local/tomcat
# Thu, 05 May 2022 19:08:14 GMT
ENV PATH=/usr/local/tomcat/bin:/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 05 May 2022 19:08:15 GMT
RUN mkdir -p "$CATALINA_HOME"
# Thu, 05 May 2022 19:08:15 GMT
WORKDIR /usr/local/tomcat
# Thu, 05 May 2022 19:08:15 GMT
ENV TOMCAT_NATIVE_LIBDIR=/usr/local/tomcat/native-jni-lib
# Thu, 05 May 2022 19:08:15 GMT
ENV LD_LIBRARY_PATH=/usr/local/tomcat/native-jni-lib
# Thu, 05 May 2022 19:08:15 GMT
ENV GPG_KEYS=A9C5DF4D22E99998D9875A5110C01C5A2F6059E7
# Thu, 05 May 2022 19:08:15 GMT
ENV TOMCAT_MAJOR=10
# Wed, 18 May 2022 03:13:35 GMT
ENV TOMCAT_VERSION=10.0.21
# Wed, 18 May 2022 03:13:35 GMT
ENV TOMCAT_SHA512=a20d905486fc446bcc67501418520ab8a30425944fe30f30fb3306ef975573cd0a6c439c0b764bcec9144083684668ebe4aa0c80ccc7dd931af6c2f487f2fdba
# Wed, 18 May 2022 03:13:36 GMT
COPY dir:442f5b7c480097189a15e630d632574c981f9e7eba1a8c9d3f2a109c43809746 in /usr/local/tomcat 
# Wed, 18 May 2022 03:13:40 GMT
RUN set -eux; 	apt-get update; 	xargs -rt apt-get install -y --no-install-recommends < "$TOMCAT_NATIVE_LIBDIR/.dependencies.txt"; 	rm -rf /var/lib/apt/lists/*
# Wed, 18 May 2022 03:13:42 GMT
RUN set -eux; 	nativeLines="$(catalina.sh configtest 2>&1)"; 	nativeLines="$(echo "$nativeLines" | grep 'Apache Tomcat Native')"; 	nativeLines="$(echo "$nativeLines" | sort -u)"; 	if ! echo "$nativeLines" | grep -E 'INFO: Loaded( APR based)? Apache Tomcat Native library' >&2; then 		echo >&2 "$nativeLines"; 		exit 1; 	fi
# Wed, 18 May 2022 03:13:42 GMT
EXPOSE 8080
# Wed, 18 May 2022 03:13:42 GMT
CMD ["catalina.sh" "run"]
```

-	Layers:
	-	`sha256:d5fd17ec1767521cf97f61568096bfc9a7cd9c2d149576a7b43930c5a97062b0`  
		Last Modified: Thu, 28 Apr 2022 03:03:21 GMT  
		Size: 28.6 MB (28566230 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8e94d254f3c4d0b302d167dc31edd456d3f663ed337bc99fdd2fd0a21025340e`  
		Last Modified: Sat, 30 Apr 2022 00:26:11 GMT  
		Size: 16.0 MB (16030310 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a2db2e8276849402c1b8e9aad20b1d0c8a07ae127bda53919348a4ace443cbc7`  
		Last Modified: Thu, 05 May 2022 18:31:03 GMT  
		Size: 41.8 MB (41798998 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c73a56a81b0c3a1789d1e7542d3ddf9fd5c5bc61c3590aad7e18eec5f9e3cd4a`  
		Last Modified: Thu, 05 May 2022 18:30:58 GMT  
		Size: 160.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:be7817cdedb999f183a0521b454277013b2be09528cc0a77bd0bd40cac868bdf`  
		Last Modified: Thu, 05 May 2022 19:20:30 GMT  
		Size: 172.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e08f51b23f20b462a530f5359c9de3a72410d92957b6b57c5cb3105f08380557`  
		Last Modified: Wed, 18 May 2022 03:46:02 GMT  
		Size: 12.6 MB (12592306 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5af1f4e9271a7350f4cd52d5c069e3d4de8f8356fdb888cd08dd36159b2ecc6a`  
		Last Modified: Wed, 18 May 2022 03:46:01 GMT  
		Size: 2.4 MB (2352081 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a8e7ba40010317884e776f2694c6b1eae4a0cf0326a39526336de55995d51185`  
		Last Modified: Wed, 18 May 2022 03:46:01 GMT  
		Size: 130.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `tomcat:10-jre8-temurin` - linux; arm variant v7

```console
$ docker pull tomcat@sha256:3b38130376e406df6d20dd2e800987714509b96f19e5057c74db0f6426210a36
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **93.0 MB (93019492 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:93780f696a194fea19e78761a703c555b7c9bd8156c35bbe121d663adf7244de`
-	Default Command: `["catalina.sh","run"]`

```dockerfile
# Fri, 29 Apr 2022 22:58:46 GMT
ADD file:5f12bea85a1ebe365907ca3979b0e31e6043dccfcb9a3cdf62be46e054494147 in / 
# Fri, 29 Apr 2022 22:58:47 GMT
CMD ["bash"]
# Fri, 29 Apr 2022 23:56:03 GMT
ENV LANG=en_US.UTF-8 LANGUAGE=en_US:en LC_ALL=en_US.UTF-8
# Fri, 29 Apr 2022 23:56:45 GMT
RUN apt-get update     && DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends tzdata curl ca-certificates fontconfig locales     && echo "en_US.UTF-8 UTF-8" >> /etc/locale.gen     && locale-gen en_US.UTF-8     && rm -rf /var/lib/apt/lists/*
# Thu, 05 May 2022 17:57:50 GMT
ENV JAVA_VERSION=jdk8u332-b09
# Thu, 05 May 2022 17:58:47 GMT
RUN set -eux;     ARCH="$(dpkg --print-architecture)";     case "${ARCH}" in        aarch64|arm64)          ESUM='be92e658ed7f6b14b3b945700d7a4f87467c682b70dfbf682ca4562b93cfc8e0';          BINARY_URL='https://github.com/adoptium/temurin8-binaries/releases/download/jdk8u332-b09/OpenJDK8U-jre_aarch64_linux_hotspot_8u332b09.tar.gz';          ;;        armhf|arm)          ESUM='72adfae646b7866aedd28c20a874181c8f3835ccb16610c47e0ca0780f8f9a9c';          BINARY_URL='https://github.com/adoptium/temurin8-binaries/releases/download/jdk8u332-b09/OpenJDK8U-jre_arm_linux_hotspot_8u332b09.tar.gz';          apt-get update          && DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends libatomic1          && rm -rf /var/lib/apt/lists/*          ;;        ppc64el|powerpc:common64)          ESUM='3c7434b248b0edd23a5ac0d8244382725d90e1214f0ddc73a0ead5ad5ceffdaa';          BINARY_URL='https://github.com/adoptium/temurin8-binaries/releases/download/jdk8u332-b09/OpenJDK8U-jre_ppc64le_linux_hotspot_8u332b09.tar.gz';          ;;        amd64|i386:x86-64)          ESUM='34454309b43d585047baaefc36c1850d0192cccc8b52cdc4aadb192b8e3e4c81';          BINARY_URL='https://github.com/adoptium/temurin8-binaries/releases/download/jdk8u332-b09/OpenJDK8U-jre_x64_linux_hotspot_8u332b09.tar.gz';          ;;        *)          echo "Unsupported arch: ${ARCH}";          exit 1;          ;;     esac;     curl -LfsSo /tmp/openjdk.tar.gz ${BINARY_URL};     echo "${ESUM} */tmp/openjdk.tar.gz" | sha256sum -c -;     mkdir -p /opt/java/openjdk;     cd /opt/java/openjdk;     tar -xf /tmp/openjdk.tar.gz --strip-components=1;     rm -rf /tmp/openjdk.tar.gz;
# Thu, 05 May 2022 17:58:47 GMT
ENV JAVA_HOME=/opt/java/openjdk PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 05 May 2022 17:58:49 GMT
RUN echo Verifying install ...     && echo java -version && java -version     && echo Complete.
# Thu, 05 May 2022 18:48:29 GMT
ENV CATALINA_HOME=/usr/local/tomcat
# Thu, 05 May 2022 18:48:30 GMT
ENV PATH=/usr/local/tomcat/bin:/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 05 May 2022 18:48:31 GMT
RUN mkdir -p "$CATALINA_HOME"
# Thu, 05 May 2022 18:48:32 GMT
WORKDIR /usr/local/tomcat
# Thu, 05 May 2022 18:48:32 GMT
ENV TOMCAT_NATIVE_LIBDIR=/usr/local/tomcat/native-jni-lib
# Thu, 05 May 2022 18:48:33 GMT
ENV LD_LIBRARY_PATH=/usr/local/tomcat/native-jni-lib
# Thu, 05 May 2022 18:48:33 GMT
ENV GPG_KEYS=A9C5DF4D22E99998D9875A5110C01C5A2F6059E7
# Thu, 05 May 2022 18:48:33 GMT
ENV TOMCAT_MAJOR=10
# Wed, 18 May 2022 08:45:00 GMT
ENV TOMCAT_VERSION=10.0.21
# Wed, 18 May 2022 08:45:01 GMT
ENV TOMCAT_SHA512=a20d905486fc446bcc67501418520ab8a30425944fe30f30fb3306ef975573cd0a6c439c0b764bcec9144083684668ebe4aa0c80ccc7dd931af6c2f487f2fdba
# Wed, 18 May 2022 08:45:03 GMT
COPY dir:cd2bdc9562b201cef701cab7b4498ad8299b769fe6dfdd3c9b0aface5b7cdb59 in /usr/local/tomcat 
# Wed, 18 May 2022 08:45:15 GMT
RUN set -eux; 	apt-get update; 	xargs -rt apt-get install -y --no-install-recommends < "$TOMCAT_NATIVE_LIBDIR/.dependencies.txt"; 	rm -rf /var/lib/apt/lists/*
# Wed, 18 May 2022 08:45:18 GMT
RUN set -eux; 	nativeLines="$(catalina.sh configtest 2>&1)"; 	nativeLines="$(echo "$nativeLines" | grep 'Apache Tomcat Native')"; 	nativeLines="$(echo "$nativeLines" | sort -u)"; 	if ! echo "$nativeLines" | grep -E 'INFO: Loaded( APR based)? Apache Tomcat Native library' >&2; then 		echo >&2 "$nativeLines"; 		exit 1; 	fi
# Wed, 18 May 2022 08:45:18 GMT
EXPOSE 8080
# Wed, 18 May 2022 08:45:19 GMT
CMD ["catalina.sh" "run"]
```

-	Layers:
	-	`sha256:b20724a4297c7ca8b89f31d6ad53e7ead0c17c7908a4592871cdc97332193580`  
		Last Modified: Fri, 29 Apr 2022 23:03:00 GMT  
		Size: 24.1 MB (24073650 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:142d50dc2d1479b31402efb7588259cffeca2de60159fa16b540aa20dcf0cd3f`  
		Last Modified: Sat, 30 Apr 2022 00:04:04 GMT  
		Size: 14.9 MB (14901951 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5ae1e7e22a40525923a76679a6295576bfb573768f7d50e75be310747e6ca9c0`  
		Last Modified: Thu, 05 May 2022 18:04:02 GMT  
		Size: 39.5 MB (39530275 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:adddf73f472e79bf81d9cb541f0809ae75fd7568416e19538a83b777765816b5`  
		Last Modified: Thu, 05 May 2022 18:03:40 GMT  
		Size: 159.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6885083ea01fddc701a2af5837bc2b5044207599551945fe80b6e8ccb0076f96`  
		Last Modified: Thu, 05 May 2022 19:06:50 GMT  
		Size: 171.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:47238aa4e1c03e0c685060e73845ca9a0aab1a332f04e5588fd8cf10164e6e40`  
		Last Modified: Wed, 18 May 2022 09:09:16 GMT  
		Size: 12.5 MB (12542405 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:290bc884ee6f0805de9933bf05fc95a9988d2d8687d390cc16cc8076698e28d9`  
		Last Modified: Wed, 18 May 2022 09:09:13 GMT  
		Size: 2.0 MB (1970751 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:638f2b0eb9b16c50a8eb199a1554727b99522bb457648a253d6b1ea023e6bd8a`  
		Last Modified: Wed, 18 May 2022 09:09:12 GMT  
		Size: 130.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `tomcat:10-jre8-temurin` - linux; arm64 variant v8

```console
$ docker pull tomcat@sha256:27340a95d705514df215b7d502802c26a987c4072b70cc061db5ddbf0e013956
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **98.7 MB (98677967 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a9bd80821291efb575952bcde75740d8c8ddf30f170422e92589e8cd08266b9e`
-	Default Command: `["catalina.sh","run"]`

```dockerfile
# Fri, 29 Apr 2022 22:49:34 GMT
ADD file:ccdde790bb849fe101367f2b541f1062b3544d21f99a5acc535bf2b0884cc0eb in / 
# Fri, 29 Apr 2022 22:49:35 GMT
CMD ["bash"]
# Fri, 29 Apr 2022 23:28:34 GMT
ENV LANG=en_US.UTF-8 LANGUAGE=en_US:en LC_ALL=en_US.UTF-8
# Fri, 29 Apr 2022 23:28:52 GMT
RUN apt-get update     && DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends tzdata curl ca-certificates fontconfig locales     && echo "en_US.UTF-8 UTF-8" >> /etc/locale.gen     && locale-gen en_US.UTF-8     && rm -rf /var/lib/apt/lists/*
# Thu, 05 May 2022 17:44:46 GMT
ENV JAVA_VERSION=jdk8u332-b09
# Thu, 05 May 2022 17:45:23 GMT
RUN set -eux;     ARCH="$(dpkg --print-architecture)";     case "${ARCH}" in        aarch64|arm64)          ESUM='be92e658ed7f6b14b3b945700d7a4f87467c682b70dfbf682ca4562b93cfc8e0';          BINARY_URL='https://github.com/adoptium/temurin8-binaries/releases/download/jdk8u332-b09/OpenJDK8U-jre_aarch64_linux_hotspot_8u332b09.tar.gz';          ;;        armhf|arm)          ESUM='72adfae646b7866aedd28c20a874181c8f3835ccb16610c47e0ca0780f8f9a9c';          BINARY_URL='https://github.com/adoptium/temurin8-binaries/releases/download/jdk8u332-b09/OpenJDK8U-jre_arm_linux_hotspot_8u332b09.tar.gz';          apt-get update          && DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends libatomic1          && rm -rf /var/lib/apt/lists/*          ;;        ppc64el|powerpc:common64)          ESUM='3c7434b248b0edd23a5ac0d8244382725d90e1214f0ddc73a0ead5ad5ceffdaa';          BINARY_URL='https://github.com/adoptium/temurin8-binaries/releases/download/jdk8u332-b09/OpenJDK8U-jre_ppc64le_linux_hotspot_8u332b09.tar.gz';          ;;        amd64|i386:x86-64)          ESUM='34454309b43d585047baaefc36c1850d0192cccc8b52cdc4aadb192b8e3e4c81';          BINARY_URL='https://github.com/adoptium/temurin8-binaries/releases/download/jdk8u332-b09/OpenJDK8U-jre_x64_linux_hotspot_8u332b09.tar.gz';          ;;        *)          echo "Unsupported arch: ${ARCH}";          exit 1;          ;;     esac;     curl -LfsSo /tmp/openjdk.tar.gz ${BINARY_URL};     echo "${ESUM} */tmp/openjdk.tar.gz" | sha256sum -c -;     mkdir -p /opt/java/openjdk;     cd /opt/java/openjdk;     tar -xf /tmp/openjdk.tar.gz --strip-components=1;     rm -rf /tmp/openjdk.tar.gz;
# Thu, 05 May 2022 17:45:23 GMT
ENV JAVA_HOME=/opt/java/openjdk PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 05 May 2022 17:45:24 GMT
RUN echo Verifying install ...     && echo java -version && java -version     && echo Complete.
# Thu, 05 May 2022 18:43:31 GMT
ENV CATALINA_HOME=/usr/local/tomcat
# Thu, 05 May 2022 18:43:32 GMT
ENV PATH=/usr/local/tomcat/bin:/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 05 May 2022 18:43:33 GMT
RUN mkdir -p "$CATALINA_HOME"
# Thu, 05 May 2022 18:43:34 GMT
WORKDIR /usr/local/tomcat
# Thu, 05 May 2022 18:43:35 GMT
ENV TOMCAT_NATIVE_LIBDIR=/usr/local/tomcat/native-jni-lib
# Thu, 05 May 2022 18:43:36 GMT
ENV LD_LIBRARY_PATH=/usr/local/tomcat/native-jni-lib
# Thu, 05 May 2022 18:43:37 GMT
ENV GPG_KEYS=A9C5DF4D22E99998D9875A5110C01C5A2F6059E7
# Thu, 05 May 2022 18:43:38 GMT
ENV TOMCAT_MAJOR=10
# Wed, 18 May 2022 02:36:14 GMT
ENV TOMCAT_VERSION=10.0.21
# Wed, 18 May 2022 02:36:15 GMT
ENV TOMCAT_SHA512=a20d905486fc446bcc67501418520ab8a30425944fe30f30fb3306ef975573cd0a6c439c0b764bcec9144083684668ebe4aa0c80ccc7dd931af6c2f487f2fdba
# Wed, 18 May 2022 02:36:17 GMT
COPY dir:cb6042eda12c16c9560bcc300403b88511e8eed755787a363d7ee993bfb64fb7 in /usr/local/tomcat 
# Wed, 18 May 2022 02:36:24 GMT
RUN set -eux; 	apt-get update; 	xargs -rt apt-get install -y --no-install-recommends < "$TOMCAT_NATIVE_LIBDIR/.dependencies.txt"; 	rm -rf /var/lib/apt/lists/*
# Wed, 18 May 2022 02:36:26 GMT
RUN set -eux; 	nativeLines="$(catalina.sh configtest 2>&1)"; 	nativeLines="$(echo "$nativeLines" | grep 'Apache Tomcat Native')"; 	nativeLines="$(echo "$nativeLines" | sort -u)"; 	if ! echo "$nativeLines" | grep -E 'INFO: Loaded( APR based)? Apache Tomcat Native library' >&2; then 		echo >&2 "$nativeLines"; 		exit 1; 	fi
# Wed, 18 May 2022 02:36:27 GMT
EXPOSE 8080
# Wed, 18 May 2022 02:36:28 GMT
CMD ["catalina.sh" "run"]
```

-	Layers:
	-	`sha256:d4ba87bb7858f0dd4a60003f011338f3a58b87d0add985652856007fe5ca5034`  
		Last Modified: Fri, 29 Apr 2022 22:51:32 GMT  
		Size: 27.2 MB (27169388 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0ce33c7cb386794b97371bf23d6db512379e04036ae033b076a599f51f6416b6`  
		Last Modified: Fri, 29 Apr 2022 23:33:40 GMT  
		Size: 15.9 MB (15897301 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e80901725afa7411c05d2a5149e9b62712820c52e3ffaf9aed0b7324bdb82aef`  
		Last Modified: Thu, 05 May 2022 17:49:16 GMT  
		Size: 40.8 MB (40785896 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cdbac92c0520c944c2b1cedf6fc76390e5d9d035e6de66bd2e6d3ebe35e32da0`  
		Last Modified: Thu, 05 May 2022 17:49:11 GMT  
		Size: 127.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1f0bb848174124e83aa510d9bfca60c928ad49f6d9e8be744ea42f31d412892b`  
		Last Modified: Thu, 05 May 2022 19:08:40 GMT  
		Size: 137.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d28620c03be8f2fcdf58efa0bccd4dfb55afb85bd87362efc579b20ab0ccce7f`  
		Last Modified: Wed, 18 May 2022 03:23:13 GMT  
		Size: 12.6 MB (12609668 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d947a5e316758b7ddcd359bb1fe33dae7efd75030e99f5c25ca77268d27b6552`  
		Last Modified: Wed, 18 May 2022 03:23:12 GMT  
		Size: 2.2 MB (2215450 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `tomcat:10-jre8-temurin` - linux; ppc64le

```console
$ docker pull tomcat@sha256:f49f0bd30ec1872a28187df21b50cfb3437bd8a60fb79391c06f535ab6ecd5fe
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **106.9 MB (106882013 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c57fe39fe1c92db00290716e377a9c6fbc6b1cda4c69600e490db402132c42cd`
-	Default Command: `["catalina.sh","run"]`

```dockerfile
# Fri, 29 Apr 2022 23:22:28 GMT
ADD file:55691ac7d76af0fcfafc39ebd1e5a4f2d7018147d6db6f89812db33fbaffc2f9 in / 
# Fri, 29 Apr 2022 23:22:33 GMT
CMD ["bash"]
# Sat, 30 Apr 2022 00:29:48 GMT
ENV LANG=en_US.UTF-8 LANGUAGE=en_US:en LC_ALL=en_US.UTF-8
# Sat, 30 Apr 2022 00:32:16 GMT
RUN apt-get update     && DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends tzdata curl ca-certificates fontconfig locales     && echo "en_US.UTF-8 UTF-8" >> /etc/locale.gen     && locale-gen en_US.UTF-8     && rm -rf /var/lib/apt/lists/*
# Thu, 05 May 2022 18:16:57 GMT
ENV JAVA_VERSION=jdk8u332-b09
# Thu, 05 May 2022 18:19:04 GMT
RUN set -eux;     ARCH="$(dpkg --print-architecture)";     case "${ARCH}" in        aarch64|arm64)          ESUM='be92e658ed7f6b14b3b945700d7a4f87467c682b70dfbf682ca4562b93cfc8e0';          BINARY_URL='https://github.com/adoptium/temurin8-binaries/releases/download/jdk8u332-b09/OpenJDK8U-jre_aarch64_linux_hotspot_8u332b09.tar.gz';          ;;        armhf|arm)          ESUM='72adfae646b7866aedd28c20a874181c8f3835ccb16610c47e0ca0780f8f9a9c';          BINARY_URL='https://github.com/adoptium/temurin8-binaries/releases/download/jdk8u332-b09/OpenJDK8U-jre_arm_linux_hotspot_8u332b09.tar.gz';          apt-get update          && DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends libatomic1          && rm -rf /var/lib/apt/lists/*          ;;        ppc64el|powerpc:common64)          ESUM='3c7434b248b0edd23a5ac0d8244382725d90e1214f0ddc73a0ead5ad5ceffdaa';          BINARY_URL='https://github.com/adoptium/temurin8-binaries/releases/download/jdk8u332-b09/OpenJDK8U-jre_ppc64le_linux_hotspot_8u332b09.tar.gz';          ;;        amd64|i386:x86-64)          ESUM='34454309b43d585047baaefc36c1850d0192cccc8b52cdc4aadb192b8e3e4c81';          BINARY_URL='https://github.com/adoptium/temurin8-binaries/releases/download/jdk8u332-b09/OpenJDK8U-jre_x64_linux_hotspot_8u332b09.tar.gz';          ;;        *)          echo "Unsupported arch: ${ARCH}";          exit 1;          ;;     esac;     curl -LfsSo /tmp/openjdk.tar.gz ${BINARY_URL};     echo "${ESUM} */tmp/openjdk.tar.gz" | sha256sum -c -;     mkdir -p /opt/java/openjdk;     cd /opt/java/openjdk;     tar -xf /tmp/openjdk.tar.gz --strip-components=1;     rm -rf /tmp/openjdk.tar.gz;
# Thu, 05 May 2022 18:19:10 GMT
ENV JAVA_HOME=/opt/java/openjdk PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 05 May 2022 18:19:18 GMT
RUN echo Verifying install ...     && echo java -version && java -version     && echo Complete.
# Thu, 05 May 2022 19:09:06 GMT
ENV CATALINA_HOME=/usr/local/tomcat
# Thu, 05 May 2022 19:09:12 GMT
ENV PATH=/usr/local/tomcat/bin:/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 05 May 2022 19:09:18 GMT
RUN mkdir -p "$CATALINA_HOME"
# Thu, 05 May 2022 19:09:21 GMT
WORKDIR /usr/local/tomcat
# Thu, 05 May 2022 19:09:22 GMT
ENV TOMCAT_NATIVE_LIBDIR=/usr/local/tomcat/native-jni-lib
# Thu, 05 May 2022 19:09:27 GMT
ENV LD_LIBRARY_PATH=/usr/local/tomcat/native-jni-lib
# Thu, 05 May 2022 19:09:29 GMT
ENV GPG_KEYS=A9C5DF4D22E99998D9875A5110C01C5A2F6059E7
# Thu, 05 May 2022 19:09:32 GMT
ENV TOMCAT_MAJOR=10
# Wed, 18 May 2022 06:36:00 GMT
ENV TOMCAT_VERSION=10.0.21
# Wed, 18 May 2022 06:36:01 GMT
ENV TOMCAT_SHA512=a20d905486fc446bcc67501418520ab8a30425944fe30f30fb3306ef975573cd0a6c439c0b764bcec9144083684668ebe4aa0c80ccc7dd931af6c2f487f2fdba
# Wed, 18 May 2022 06:36:05 GMT
COPY dir:0ac7f51d1dbc2d2981319db2b0f9a58fe6c15d6b08472fb31b264b0fb99e57e3 in /usr/local/tomcat 
# Wed, 18 May 2022 06:36:32 GMT
RUN set -eux; 	apt-get update; 	xargs -rt apt-get install -y --no-install-recommends < "$TOMCAT_NATIVE_LIBDIR/.dependencies.txt"; 	rm -rf /var/lib/apt/lists/*
# Wed, 18 May 2022 06:36:45 GMT
RUN set -eux; 	nativeLines="$(catalina.sh configtest 2>&1)"; 	nativeLines="$(echo "$nativeLines" | grep 'Apache Tomcat Native')"; 	nativeLines="$(echo "$nativeLines" | sort -u)"; 	if ! echo "$nativeLines" | grep -E 'INFO: Loaded( APR based)? Apache Tomcat Native library' >&2; then 		echo >&2 "$nativeLines"; 		exit 1; 	fi
# Wed, 18 May 2022 06:36:49 GMT
EXPOSE 8080
# Wed, 18 May 2022 06:36:50 GMT
CMD ["catalina.sh" "run"]
```

-	Layers:
	-	`sha256:e9c0a77cb9f0f7330e3fc62254e4c8ae89ed4bba21209fdc1088195250f950b9`  
		Last Modified: Fri, 29 Apr 2022 23:25:23 GMT  
		Size: 33.3 MB (33290661 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a436aa11f9f1d03225e672ec1f60e82ddcff2d3b267d9904213f0f01ed5eeba5`  
		Last Modified: Sat, 30 Apr 2022 00:45:44 GMT  
		Size: 17.2 MB (17204116 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f52806fb57ec020c802a4f4cb502d02e7fe9f9e523ee2589b220cf2255dbaf21`  
		Last Modified: Thu, 05 May 2022 18:24:39 GMT  
		Size: 41.2 MB (41205891 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c927ffc56d7be25073d4bf077485eea398ae7e563143fec34567a832e0bc4a24`  
		Last Modified: Thu, 05 May 2022 18:24:32 GMT  
		Size: 161.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fddd318375d0abc69921071bad194d598355a079821bf6806470a863ff9e7495`  
		Last Modified: Thu, 05 May 2022 19:28:45 GMT  
		Size: 172.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e77e5fe240a07d9d529f865c039f1cc36167dda41ec622061de7adf6bdf0628c`  
		Last Modified: Wed, 18 May 2022 07:05:14 GMT  
		Size: 12.6 MB (12632783 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:134a0d1800a0ee2d91054231ae2cf5fdbd7909f34e092386e9bc6d1dbdd581a7`  
		Last Modified: Wed, 18 May 2022 07:05:13 GMT  
		Size: 2.5 MB (2548099 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b0d2d92ad845ca8357889f1fe25528d6f958952d2b554b9df2a87d0f6a3fdb00`  
		Last Modified: Wed, 18 May 2022 07:05:12 GMT  
		Size: 130.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
