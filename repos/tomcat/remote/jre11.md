## `tomcat:jre11`

```console
$ docker pull tomcat@sha256:3862cc195e07bc8048d856bd3c4575b084fc3b1f763b6e6c3a9af3d33ee1063e
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 5
	-	linux; amd64
	-	linux; arm variant v7
	-	linux; arm64 variant v8
	-	linux; ppc64le
	-	linux; s390x

### `tomcat:jre11` - linux; amd64

```console
$ docker pull tomcat@sha256:ff31bc9c18ac3d0b5b1b5ab677a1a3fcae21a61380067bd3ff45c7b45136bd43
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **101.3 MB (101281257 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:8108fc557bf12735c75aa4db1cac5555ecaefdfc8916890f32b4a64f80a325db`
-	Default Command: `["catalina.sh","run"]`

```dockerfile
# Tue, 02 Aug 2022 01:30:55 GMT
ADD file:396eeb65c8d737180cc1219713cf59efb214027b79d8ea0b7e58a08e7c8d7a21 in / 
# Tue, 02 Aug 2022 01:30:56 GMT
CMD ["bash"]
# Thu, 11 Aug 2022 19:20:28 GMT
ENV JAVA_HOME=/opt/java/openjdk
# Thu, 11 Aug 2022 19:20:28 GMT
ENV PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 11 Aug 2022 19:20:28 GMT
ENV LANG=en_US.UTF-8 LANGUAGE=en_US:en LC_ALL=en_US.UTF-8
# Thu, 11 Aug 2022 19:20:50 GMT
RUN apt-get update     && DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends tzdata wget ca-certificates fontconfig locales     && echo "en_US.UTF-8 UTF-8" >> /etc/locale.gen     && locale-gen en_US.UTF-8     && rm -rf /var/lib/apt/lists/*
# Thu, 11 Aug 2022 19:22:41 GMT
ENV JAVA_VERSION=jdk-11.0.16+8
# Thu, 11 Aug 2022 19:23:30 GMT
RUN set -eux;     ARCH="$(dpkg --print-architecture)";     case "${ARCH}" in        aarch64|arm64)          ESUM='3fa9cb99229ede53d4efddb686106df77794e02b1f4defea6b70b2b53380a8c7';          BINARY_URL='https://github.com/adoptium/temurin11-binaries/releases/download/jdk-11.0.16%2B8/OpenJDK11U-jre_aarch64_linux_hotspot_11.0.16_8.tar.gz';          ;;        armhf|arm)          ESUM='658ee6d797e6ca4d25de24d45072a44ed8462e3a9feaa38ef9f6d033d18401c8';          BINARY_URL='https://github.com/adoptium/temurin11-binaries/releases/download/jdk-11.0.16%2B8/OpenJDK11U-jre_arm_linux_hotspot_11.0.16_8.tar.gz';          ;;        ppc64el|powerpc:common64)          ESUM='6002b8f6c7b3421ac70601d1bf55f355b75c4a193c97e12974b4c2301d737d8d';          BINARY_URL='https://github.com/adoptium/temurin11-binaries/releases/download/jdk-11.0.16%2B8/OpenJDK11U-jre_ppc64le_linux_hotspot_11.0.16_8.tar.gz';          ;;        s390x|s390:64-bit)          ESUM='683902c6429f28c606685f46d628291c989de3effe50eca51889388d65f96b95';          BINARY_URL='https://github.com/adoptium/temurin11-binaries/releases/download/jdk-11.0.16%2B8/OpenJDK11U-jre_s390x_linux_hotspot_11.0.16_8.tar.gz';          ;;        amd64|i386:x86-64)          ESUM='74988677f1e1692f8f482ae5f75814b908bb3cf5a8b7d9872873a42e330e7595';          BINARY_URL='https://github.com/adoptium/temurin11-binaries/releases/download/jdk-11.0.16%2B8/OpenJDK11U-jre_x64_linux_hotspot_11.0.16_8.tar.gz';          ;;        *)          echo "Unsupported arch: ${ARCH}";          exit 1;          ;;     esac; 	  wget -O /tmp/openjdk.tar.gz ${BINARY_URL}; 	  echo "${ESUM} */tmp/openjdk.tar.gz" | sha256sum -c -; 	  mkdir -p "$JAVA_HOME"; 	  tar --extract 	      --file /tmp/openjdk.tar.gz 	      --directory "$JAVA_HOME" 	      --strip-components 1 	      --no-same-owner 	  ;     rm /tmp/openjdk.tar.gz;     find "$JAVA_HOME/lib" -name '*.so' -exec dirname '{}' ';' | sort -u > /etc/ld.so.conf.d/docker-openjdk.conf;     ldconfig;     java -Xshare:dump;
# Thu, 11 Aug 2022 19:23:31 GMT
RUN echo Verifying install ...     && fileEncoding="$(echo 'System.out.println(System.getProperty("file.encoding"))' | jshell -s -)"; [ "$fileEncoding" = 'UTF-8' ]; rm -rf ~/.java     && echo java --version && java --version     && echo Complete.
# Thu, 11 Aug 2022 21:29:54 GMT
ENV CATALINA_HOME=/usr/local/tomcat
# Thu, 11 Aug 2022 21:29:54 GMT
ENV PATH=/usr/local/tomcat/bin:/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 11 Aug 2022 21:29:54 GMT
RUN mkdir -p "$CATALINA_HOME"
# Thu, 11 Aug 2022 21:29:55 GMT
WORKDIR /usr/local/tomcat
# Thu, 11 Aug 2022 21:29:55 GMT
ENV TOMCAT_NATIVE_LIBDIR=/usr/local/tomcat/native-jni-lib
# Thu, 11 Aug 2022 21:29:55 GMT
ENV LD_LIBRARY_PATH=/usr/local/tomcat/native-jni-lib
# Thu, 11 Aug 2022 21:29:55 GMT
ENV GPG_KEYS=A9C5DF4D22E99998D9875A5110C01C5A2F6059E7
# Thu, 11 Aug 2022 21:29:55 GMT
ENV TOMCAT_MAJOR=10
# Thu, 11 Aug 2022 21:32:28 GMT
ENV TOMCAT_VERSION=10.0.23
# Thu, 11 Aug 2022 21:32:28 GMT
ENV TOMCAT_SHA512=0e0263e8280f2ccfb4bef916444a6105fef689a3d95c334c8a7bfe59f1e3966d48ea624727f1818a4df331a603f1ac5e21b908dda3cae676ddc1aef90c2d12ab
# Thu, 11 Aug 2022 21:32:28 GMT
COPY dir:295efba64fb11f555c2efcbe48a1e2b9c52c89deabb412488da748c879789b92 in /usr/local/tomcat 
# Thu, 11 Aug 2022 21:32:32 GMT
RUN set -eux; 	apt-get update; 	xargs -rt apt-get install -y --no-install-recommends < "$TOMCAT_NATIVE_LIBDIR/.dependencies.txt"; 	rm -rf /var/lib/apt/lists/*
# Thu, 11 Aug 2022 21:32:34 GMT
RUN set -eux; 	nativeLines="$(catalina.sh configtest 2>&1)"; 	nativeLines="$(echo "$nativeLines" | grep 'Apache Tomcat Native')"; 	nativeLines="$(echo "$nativeLines" | sort -u)"; 	if ! echo "$nativeLines" | grep -E 'INFO: Loaded( APR based)? Apache Tomcat Native library' >&2; then 		echo >&2 "$nativeLines"; 		exit 1; 	fi
# Thu, 11 Aug 2022 21:32:34 GMT
EXPOSE 8080
# Thu, 11 Aug 2022 21:32:34 GMT
CMD ["catalina.sh" "run"]
```

-	Layers:
	-	`sha256:d19f32bd9e4106d487f1a703fc2f09c8edadd92db4405d477978e8e466ab290d`  
		Last Modified: Tue, 02 Aug 2022 01:32:15 GMT  
		Size: 30.4 MB (30426136 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8cc15e118841a9f177bca811667e37fe099192eb26678de7c0b49e003dac8576`  
		Last Modified: Thu, 11 Aug 2022 19:30:35 GMT  
		Size: 11.3 MB (11343716 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c06f199c59dc441d577e8ab717f37deca9b48cfdc989034d6483f2fe8baba7b6`  
		Last Modified: Thu, 11 Aug 2022 19:34:43 GMT  
		Size: 46.5 MB (46496410 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5db1234d90fb8b714eefb18b0a15fbc0f884f6a81af2f4b88123710936a0e23c`  
		Last Modified: Thu, 11 Aug 2022 19:34:37 GMT  
		Size: 160.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1aeade929514a0cf9b1fa62731ba3a0ab5a74e93af51b4d413764e477404db75`  
		Last Modified: Thu, 11 Aug 2022 21:56:54 GMT  
		Size: 173.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f1d7259e1c2c5a646f00f629b30ad3c9e8dd391a5633404f09b88917744117b3`  
		Last Modified: Thu, 11 Aug 2022 22:00:09 GMT  
		Size: 12.6 MB (12567841 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f4df3660a562404d25137fa31dd53e4362b0bf78633d97cb00ec33aa5aa7688b`  
		Last Modified: Thu, 11 Aug 2022 22:00:08 GMT  
		Size: 446.7 KB (446691 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5497629aeb84524e3102fd9ea5fb7145c580ff795c77e610c5e1395132c4ddd4`  
		Last Modified: Thu, 11 Aug 2022 22:00:08 GMT  
		Size: 130.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `tomcat:jre11` - linux; arm variant v7

```console
$ docker pull tomcat@sha256:98db9f52f73c75db131339f97d8c672c42950b7c1637313ef98256f253375699
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **95.7 MB (95680848 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:aa3d8a8ea7e1b8ac18f7fbd41b5e90377613931a53f3522b6dafe84a3fac255a`
-	Default Command: `["catalina.sh","run"]`

```dockerfile
# Tue, 02 Aug 2022 01:40:56 GMT
ADD file:1bec4ea562c9a42add30f5e3626edc93bdfc0271cbd208a4447842fa31b5c114 in / 
# Tue, 02 Aug 2022 01:40:56 GMT
CMD ["bash"]
# Thu, 11 Aug 2022 18:58:20 GMT
ENV JAVA_HOME=/opt/java/openjdk
# Thu, 11 Aug 2022 18:58:20 GMT
ENV PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 11 Aug 2022 18:58:20 GMT
ENV LANG=en_US.UTF-8 LANGUAGE=en_US:en LC_ALL=en_US.UTF-8
# Thu, 11 Aug 2022 18:58:36 GMT
RUN apt-get update     && DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends tzdata wget ca-certificates fontconfig locales     && echo "en_US.UTF-8 UTF-8" >> /etc/locale.gen     && locale-gen en_US.UTF-8     && rm -rf /var/lib/apt/lists/*
# Thu, 11 Aug 2022 18:59:53 GMT
ENV JAVA_VERSION=jdk-11.0.16+8
# Thu, 11 Aug 2022 19:00:26 GMT
RUN set -eux;     ARCH="$(dpkg --print-architecture)";     case "${ARCH}" in        aarch64|arm64)          ESUM='3fa9cb99229ede53d4efddb686106df77794e02b1f4defea6b70b2b53380a8c7';          BINARY_URL='https://github.com/adoptium/temurin11-binaries/releases/download/jdk-11.0.16%2B8/OpenJDK11U-jre_aarch64_linux_hotspot_11.0.16_8.tar.gz';          ;;        armhf|arm)          ESUM='658ee6d797e6ca4d25de24d45072a44ed8462e3a9feaa38ef9f6d033d18401c8';          BINARY_URL='https://github.com/adoptium/temurin11-binaries/releases/download/jdk-11.0.16%2B8/OpenJDK11U-jre_arm_linux_hotspot_11.0.16_8.tar.gz';          ;;        ppc64el|powerpc:common64)          ESUM='6002b8f6c7b3421ac70601d1bf55f355b75c4a193c97e12974b4c2301d737d8d';          BINARY_URL='https://github.com/adoptium/temurin11-binaries/releases/download/jdk-11.0.16%2B8/OpenJDK11U-jre_ppc64le_linux_hotspot_11.0.16_8.tar.gz';          ;;        s390x|s390:64-bit)          ESUM='683902c6429f28c606685f46d628291c989de3effe50eca51889388d65f96b95';          BINARY_URL='https://github.com/adoptium/temurin11-binaries/releases/download/jdk-11.0.16%2B8/OpenJDK11U-jre_s390x_linux_hotspot_11.0.16_8.tar.gz';          ;;        amd64|i386:x86-64)          ESUM='74988677f1e1692f8f482ae5f75814b908bb3cf5a8b7d9872873a42e330e7595';          BINARY_URL='https://github.com/adoptium/temurin11-binaries/releases/download/jdk-11.0.16%2B8/OpenJDK11U-jre_x64_linux_hotspot_11.0.16_8.tar.gz';          ;;        *)          echo "Unsupported arch: ${ARCH}";          exit 1;          ;;     esac; 	  wget -O /tmp/openjdk.tar.gz ${BINARY_URL}; 	  echo "${ESUM} */tmp/openjdk.tar.gz" | sha256sum -c -; 	  mkdir -p "$JAVA_HOME"; 	  tar --extract 	      --file /tmp/openjdk.tar.gz 	      --directory "$JAVA_HOME" 	      --strip-components 1 	      --no-same-owner 	  ;     rm /tmp/openjdk.tar.gz;     find "$JAVA_HOME/lib" -name '*.so' -exec dirname '{}' ';' | sort -u > /etc/ld.so.conf.d/docker-openjdk.conf;     ldconfig;     java -Xshare:dump;
# Thu, 11 Aug 2022 19:00:27 GMT
RUN echo Verifying install ...     && fileEncoding="$(echo 'System.out.println(System.getProperty("file.encoding"))' | jshell -s -)"; [ "$fileEncoding" = 'UTF-8' ]; rm -rf ~/.java     && echo java --version && java --version     && echo Complete.
# Thu, 11 Aug 2022 20:11:04 GMT
ENV CATALINA_HOME=/usr/local/tomcat
# Thu, 11 Aug 2022 20:11:04 GMT
ENV PATH=/usr/local/tomcat/bin:/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 11 Aug 2022 20:11:05 GMT
RUN mkdir -p "$CATALINA_HOME"
# Thu, 11 Aug 2022 20:11:05 GMT
WORKDIR /usr/local/tomcat
# Thu, 11 Aug 2022 20:11:05 GMT
ENV TOMCAT_NATIVE_LIBDIR=/usr/local/tomcat/native-jni-lib
# Thu, 11 Aug 2022 20:11:05 GMT
ENV LD_LIBRARY_PATH=/usr/local/tomcat/native-jni-lib
# Thu, 11 Aug 2022 20:11:05 GMT
ENV GPG_KEYS=A9C5DF4D22E99998D9875A5110C01C5A2F6059E7
# Thu, 11 Aug 2022 20:11:05 GMT
ENV TOMCAT_MAJOR=10
# Thu, 11 Aug 2022 20:14:36 GMT
ENV TOMCAT_VERSION=10.0.23
# Thu, 11 Aug 2022 20:14:36 GMT
ENV TOMCAT_SHA512=0e0263e8280f2ccfb4bef916444a6105fef689a3d95c334c8a7bfe59f1e3966d48ea624727f1818a4df331a603f1ac5e21b908dda3cae676ddc1aef90c2d12ab
# Thu, 11 Aug 2022 20:14:37 GMT
COPY dir:2677495a2d32dae637a854ed62f94fcb8cf2f0564a2e673adbb9ccdc0481eeeb in /usr/local/tomcat 
# Thu, 11 Aug 2022 20:14:44 GMT
RUN set -eux; 	apt-get update; 	xargs -rt apt-get install -y --no-install-recommends < "$TOMCAT_NATIVE_LIBDIR/.dependencies.txt"; 	rm -rf /var/lib/apt/lists/*
# Thu, 11 Aug 2022 20:14:46 GMT
RUN set -eux; 	nativeLines="$(catalina.sh configtest 2>&1)"; 	nativeLines="$(echo "$nativeLines" | grep 'Apache Tomcat Native')"; 	nativeLines="$(echo "$nativeLines" | sort -u)"; 	if ! echo "$nativeLines" | grep -E 'INFO: Loaded( APR based)? Apache Tomcat Native library' >&2; then 		echo >&2 "$nativeLines"; 		exit 1; 	fi
# Thu, 11 Aug 2022 20:14:46 GMT
EXPOSE 8080
# Thu, 11 Aug 2022 20:14:46 GMT
CMD ["catalina.sh" "run"]
```

-	Layers:
	-	`sha256:f1a5cf9a21e485b0a676c22ced0e80a140055b3ef0d7573caf5be408a10ddb04`  
		Last Modified: Tue, 02 Aug 2022 01:43:32 GMT  
		Size: 27.0 MB (27017015 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:48f83bb11050bc1d50de6dd12d2a1425bd7a5069761fb12910fc0066805ccc5c`  
		Last Modified: Thu, 11 Aug 2022 19:06:03 GMT  
		Size: 11.1 MB (11064474 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:18824beaf598bf76f3f7f146820fb7773ed45f52eb9d6929099f4d5bcadf306b`  
		Last Modified: Thu, 11 Aug 2022 19:08:28 GMT  
		Size: 44.7 MB (44674533 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2d7b15edaa54f78e477be0a8e1c50b26839e7f1ac451936d5060ebe0fb39e15c`  
		Last Modified: Thu, 11 Aug 2022 19:08:21 GMT  
		Size: 160.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e9383955b6dfc918b48b616d3940e2187f88f45837c9db11adfe9a3be93b3c0e`  
		Last Modified: Thu, 11 Aug 2022 20:44:53 GMT  
		Size: 171.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b08a47b572b3dcd90b99d7b839ee6dd6c69fa96477ae33433181d415a482442c`  
		Last Modified: Thu, 11 Aug 2022 20:48:51 GMT  
		Size: 12.5 MB (12503818 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:490adef2973c33b67c95192f32d985228fbe16df69f742304ddf756332674e6d`  
		Last Modified: Thu, 11 Aug 2022 20:48:50 GMT  
		Size: 420.5 KB (420547 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e5cb9f0cbd37f8199849f40534f7e100573d236726cf2f6bf84f93d8c444bfa4`  
		Last Modified: Thu, 11 Aug 2022 20:48:50 GMT  
		Size: 130.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `tomcat:jre11` - linux; arm64 variant v8

```console
$ docker pull tomcat@sha256:57d35e7fe3223aae44fdb21555e6aa1a3083c83b043da8baff8b13778ccb8e70
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **97.3 MB (97304606 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:144e2d63eb22f2d767fd05036088553c5b3dc9a2917ab00c3b4f6260cfca9f23`
-	Default Command: `["catalina.sh","run"]`

```dockerfile
# Tue, 02 Aug 2022 01:18:59 GMT
ADD file:3db67543ea64bf6723921d19cc5d0483db5c6658fc95834d8b2b5ed48a4cbacd in / 
# Tue, 02 Aug 2022 01:18:59 GMT
CMD ["bash"]
# Thu, 11 Aug 2022 18:40:31 GMT
ENV JAVA_HOME=/opt/java/openjdk
# Thu, 11 Aug 2022 18:40:32 GMT
ENV PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 11 Aug 2022 18:40:33 GMT
ENV LANG=en_US.UTF-8 LANGUAGE=en_US:en LC_ALL=en_US.UTF-8
# Thu, 11 Aug 2022 18:40:51 GMT
RUN apt-get update     && DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends tzdata wget ca-certificates fontconfig locales     && echo "en_US.UTF-8 UTF-8" >> /etc/locale.gen     && locale-gen en_US.UTF-8     && rm -rf /var/lib/apt/lists/*
# Thu, 11 Aug 2022 18:43:19 GMT
ENV JAVA_VERSION=jdk-11.0.16+8
# Thu, 11 Aug 2022 18:44:16 GMT
RUN set -eux;     ARCH="$(dpkg --print-architecture)";     case "${ARCH}" in        aarch64|arm64)          ESUM='3fa9cb99229ede53d4efddb686106df77794e02b1f4defea6b70b2b53380a8c7';          BINARY_URL='https://github.com/adoptium/temurin11-binaries/releases/download/jdk-11.0.16%2B8/OpenJDK11U-jre_aarch64_linux_hotspot_11.0.16_8.tar.gz';          ;;        armhf|arm)          ESUM='658ee6d797e6ca4d25de24d45072a44ed8462e3a9feaa38ef9f6d033d18401c8';          BINARY_URL='https://github.com/adoptium/temurin11-binaries/releases/download/jdk-11.0.16%2B8/OpenJDK11U-jre_arm_linux_hotspot_11.0.16_8.tar.gz';          ;;        ppc64el|powerpc:common64)          ESUM='6002b8f6c7b3421ac70601d1bf55f355b75c4a193c97e12974b4c2301d737d8d';          BINARY_URL='https://github.com/adoptium/temurin11-binaries/releases/download/jdk-11.0.16%2B8/OpenJDK11U-jre_ppc64le_linux_hotspot_11.0.16_8.tar.gz';          ;;        s390x|s390:64-bit)          ESUM='683902c6429f28c606685f46d628291c989de3effe50eca51889388d65f96b95';          BINARY_URL='https://github.com/adoptium/temurin11-binaries/releases/download/jdk-11.0.16%2B8/OpenJDK11U-jre_s390x_linux_hotspot_11.0.16_8.tar.gz';          ;;        amd64|i386:x86-64)          ESUM='74988677f1e1692f8f482ae5f75814b908bb3cf5a8b7d9872873a42e330e7595';          BINARY_URL='https://github.com/adoptium/temurin11-binaries/releases/download/jdk-11.0.16%2B8/OpenJDK11U-jre_x64_linux_hotspot_11.0.16_8.tar.gz';          ;;        *)          echo "Unsupported arch: ${ARCH}";          exit 1;          ;;     esac; 	  wget -O /tmp/openjdk.tar.gz ${BINARY_URL}; 	  echo "${ESUM} */tmp/openjdk.tar.gz" | sha256sum -c -; 	  mkdir -p "$JAVA_HOME"; 	  tar --extract 	      --file /tmp/openjdk.tar.gz 	      --directory "$JAVA_HOME" 	      --strip-components 1 	      --no-same-owner 	  ;     rm /tmp/openjdk.tar.gz;     find "$JAVA_HOME/lib" -name '*.so' -exec dirname '{}' ';' | sort -u > /etc/ld.so.conf.d/docker-openjdk.conf;     ldconfig;     java -Xshare:dump;
# Thu, 11 Aug 2022 18:44:17 GMT
RUN echo Verifying install ...     && fileEncoding="$(echo 'System.out.println(System.getProperty("file.encoding"))' | jshell -s -)"; [ "$fileEncoding" = 'UTF-8' ]; rm -rf ~/.java     && echo java --version && java --version     && echo Complete.
# Thu, 11 Aug 2022 20:56:40 GMT
ENV CATALINA_HOME=/usr/local/tomcat
# Thu, 11 Aug 2022 20:56:41 GMT
ENV PATH=/usr/local/tomcat/bin:/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 11 Aug 2022 20:56:42 GMT
RUN mkdir -p "$CATALINA_HOME"
# Thu, 11 Aug 2022 20:56:43 GMT
WORKDIR /usr/local/tomcat
# Thu, 11 Aug 2022 20:56:44 GMT
ENV TOMCAT_NATIVE_LIBDIR=/usr/local/tomcat/native-jni-lib
# Thu, 11 Aug 2022 20:56:45 GMT
ENV LD_LIBRARY_PATH=/usr/local/tomcat/native-jni-lib
# Thu, 11 Aug 2022 20:56:46 GMT
ENV GPG_KEYS=A9C5DF4D22E99998D9875A5110C01C5A2F6059E7
# Thu, 11 Aug 2022 20:56:47 GMT
ENV TOMCAT_MAJOR=10
# Thu, 11 Aug 2022 21:00:57 GMT
ENV TOMCAT_VERSION=10.0.23
# Thu, 11 Aug 2022 21:00:58 GMT
ENV TOMCAT_SHA512=0e0263e8280f2ccfb4bef916444a6105fef689a3d95c334c8a7bfe59f1e3966d48ea624727f1818a4df331a603f1ac5e21b908dda3cae676ddc1aef90c2d12ab
# Thu, 11 Aug 2022 21:01:00 GMT
COPY dir:b229accd7e87ffecb7cb9272f78b7f8aa0ce2b8585f14b7a06f9828bc2db18ab in /usr/local/tomcat 
# Thu, 11 Aug 2022 21:01:07 GMT
RUN set -eux; 	apt-get update; 	xargs -rt apt-get install -y --no-install-recommends < "$TOMCAT_NATIVE_LIBDIR/.dependencies.txt"; 	rm -rf /var/lib/apt/lists/*
# Thu, 11 Aug 2022 21:01:08 GMT
RUN set -eux; 	nativeLines="$(catalina.sh configtest 2>&1)"; 	nativeLines="$(echo "$nativeLines" | grep 'Apache Tomcat Native')"; 	nativeLines="$(echo "$nativeLines" | sort -u)"; 	if ! echo "$nativeLines" | grep -E 'INFO: Loaded( APR based)? Apache Tomcat Native library' >&2; then 		echo >&2 "$nativeLines"; 		exit 1; 	fi
# Thu, 11 Aug 2022 21:01:09 GMT
EXPOSE 8080
# Thu, 11 Aug 2022 21:01:10 GMT
CMD ["catalina.sh" "run"]
```

-	Layers:
	-	`sha256:4a3049d340b7d3651a954fd25a32c42feb1086889d6287e2f15468aef865c5c4`  
		Last Modified: Tue, 02 Aug 2022 01:20:49 GMT  
		Size: 28.4 MB (28381155 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b941860b1b56dff93374f7988debb6b45635d744ea5fe506bdc3aff09ba84e11`  
		Last Modified: Thu, 11 Aug 2022 18:52:53 GMT  
		Size: 11.3 MB (11311183 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d124239d433fcf63e89f26b2341c275998389a5c98e7e35f74756dcfb50eac04`  
		Last Modified: Thu, 11 Aug 2022 18:56:22 GMT  
		Size: 44.8 MB (44827851 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:00dce0813d8cba43018a0f51356f18e76650d59618a1901ca29c80ed4029f546`  
		Last Modified: Thu, 11 Aug 2022 18:56:15 GMT  
		Size: 160.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:00d390143210909030afe77603d328db3fbbefea5a8302afff166bd5473ec917`  
		Last Modified: Thu, 11 Aug 2022 21:44:34 GMT  
		Size: 139.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:53f140da8ffae2adec7eb3452fac380ba58f8ecf826bb6192aef01284636d0c8`  
		Last Modified: Thu, 11 Aug 2022 21:48:20 GMT  
		Size: 12.6 MB (12575148 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e860d134b02f8f51f9729f933c82622fa8df9f8e375f47ee6570dd3bef937df6`  
		Last Modified: Thu, 11 Aug 2022 21:48:19 GMT  
		Size: 209.0 KB (208970 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `tomcat:jre11` - linux; ppc64le

```console
$ docker pull tomcat@sha256:6f0abca2b6b0d45d968e9c57f7552c2af99f9b36404194d4974d7816481caaed
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **102.6 MB (102552348 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f36ac039344f47a76c40c0a1b787fce2c9c90b29d0febbe579629234c28c6ad7`
-	Default Command: `["catalina.sh","run"]`

```dockerfile
# Tue, 02 Aug 2022 01:31:12 GMT
ADD file:b6916c28c03568df4c2efc3da91ea6320f639cdbd2fa3f6741fcea7acad4fd5f in / 
# Tue, 02 Aug 2022 01:31:14 GMT
CMD ["bash"]
# Thu, 11 Aug 2022 19:17:59 GMT
ENV JAVA_HOME=/opt/java/openjdk
# Thu, 11 Aug 2022 19:18:00 GMT
ENV PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 11 Aug 2022 19:18:00 GMT
ENV LANG=en_US.UTF-8 LANGUAGE=en_US:en LC_ALL=en_US.UTF-8
# Thu, 11 Aug 2022 19:18:38 GMT
RUN apt-get update     && DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends tzdata wget ca-certificates fontconfig locales     && echo "en_US.UTF-8 UTF-8" >> /etc/locale.gen     && locale-gen en_US.UTF-8     && rm -rf /var/lib/apt/lists/*
# Thu, 11 Aug 2022 19:21:42 GMT
ENV JAVA_VERSION=jdk-11.0.16+8
# Thu, 11 Aug 2022 19:23:08 GMT
RUN set -eux;     ARCH="$(dpkg --print-architecture)";     case "${ARCH}" in        aarch64|arm64)          ESUM='3fa9cb99229ede53d4efddb686106df77794e02b1f4defea6b70b2b53380a8c7';          BINARY_URL='https://github.com/adoptium/temurin11-binaries/releases/download/jdk-11.0.16%2B8/OpenJDK11U-jre_aarch64_linux_hotspot_11.0.16_8.tar.gz';          ;;        armhf|arm)          ESUM='658ee6d797e6ca4d25de24d45072a44ed8462e3a9feaa38ef9f6d033d18401c8';          BINARY_URL='https://github.com/adoptium/temurin11-binaries/releases/download/jdk-11.0.16%2B8/OpenJDK11U-jre_arm_linux_hotspot_11.0.16_8.tar.gz';          ;;        ppc64el|powerpc:common64)          ESUM='6002b8f6c7b3421ac70601d1bf55f355b75c4a193c97e12974b4c2301d737d8d';          BINARY_URL='https://github.com/adoptium/temurin11-binaries/releases/download/jdk-11.0.16%2B8/OpenJDK11U-jre_ppc64le_linux_hotspot_11.0.16_8.tar.gz';          ;;        s390x|s390:64-bit)          ESUM='683902c6429f28c606685f46d628291c989de3effe50eca51889388d65f96b95';          BINARY_URL='https://github.com/adoptium/temurin11-binaries/releases/download/jdk-11.0.16%2B8/OpenJDK11U-jre_s390x_linux_hotspot_11.0.16_8.tar.gz';          ;;        amd64|i386:x86-64)          ESUM='74988677f1e1692f8f482ae5f75814b908bb3cf5a8b7d9872873a42e330e7595';          BINARY_URL='https://github.com/adoptium/temurin11-binaries/releases/download/jdk-11.0.16%2B8/OpenJDK11U-jre_x64_linux_hotspot_11.0.16_8.tar.gz';          ;;        *)          echo "Unsupported arch: ${ARCH}";          exit 1;          ;;     esac; 	  wget -O /tmp/openjdk.tar.gz ${BINARY_URL}; 	  echo "${ESUM} */tmp/openjdk.tar.gz" | sha256sum -c -; 	  mkdir -p "$JAVA_HOME"; 	  tar --extract 	      --file /tmp/openjdk.tar.gz 	      --directory "$JAVA_HOME" 	      --strip-components 1 	      --no-same-owner 	  ;     rm /tmp/openjdk.tar.gz;     find "$JAVA_HOME/lib" -name '*.so' -exec dirname '{}' ';' | sort -u > /etc/ld.so.conf.d/docker-openjdk.conf;     ldconfig;     java -Xshare:dump;
# Thu, 11 Aug 2022 19:23:10 GMT
RUN echo Verifying install ...     && fileEncoding="$(echo 'System.out.println(System.getProperty("file.encoding"))' | jshell -s -)"; [ "$fileEncoding" = 'UTF-8' ]; rm -rf ~/.java     && echo java --version && java --version     && echo Complete.
# Thu, 11 Aug 2022 20:57:58 GMT
ENV CATALINA_HOME=/usr/local/tomcat
# Thu, 11 Aug 2022 20:57:58 GMT
ENV PATH=/usr/local/tomcat/bin:/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 11 Aug 2022 20:57:59 GMT
RUN mkdir -p "$CATALINA_HOME"
# Thu, 11 Aug 2022 20:58:00 GMT
WORKDIR /usr/local/tomcat
# Thu, 11 Aug 2022 20:58:00 GMT
ENV TOMCAT_NATIVE_LIBDIR=/usr/local/tomcat/native-jni-lib
# Thu, 11 Aug 2022 20:58:00 GMT
ENV LD_LIBRARY_PATH=/usr/local/tomcat/native-jni-lib
# Thu, 11 Aug 2022 20:58:01 GMT
ENV GPG_KEYS=A9C5DF4D22E99998D9875A5110C01C5A2F6059E7
# Thu, 11 Aug 2022 20:58:01 GMT
ENV TOMCAT_MAJOR=10
# Thu, 11 Aug 2022 21:03:06 GMT
ENV TOMCAT_VERSION=10.0.23
# Thu, 11 Aug 2022 21:03:06 GMT
ENV TOMCAT_SHA512=0e0263e8280f2ccfb4bef916444a6105fef689a3d95c334c8a7bfe59f1e3966d48ea624727f1818a4df331a603f1ac5e21b908dda3cae676ddc1aef90c2d12ab
# Thu, 11 Aug 2022 21:03:07 GMT
COPY dir:d37429e19e41a689567a0139cbc11d25f784b65d888be278b71233ee7211be7d in /usr/local/tomcat 
# Thu, 11 Aug 2022 21:03:15 GMT
RUN set -eux; 	apt-get update; 	xargs -rt apt-get install -y --no-install-recommends < "$TOMCAT_NATIVE_LIBDIR/.dependencies.txt"; 	rm -rf /var/lib/apt/lists/*
# Thu, 11 Aug 2022 21:03:17 GMT
RUN set -eux; 	nativeLines="$(catalina.sh configtest 2>&1)"; 	nativeLines="$(echo "$nativeLines" | grep 'Apache Tomcat Native')"; 	nativeLines="$(echo "$nativeLines" | sort -u)"; 	if ! echo "$nativeLines" | grep -E 'INFO: Loaded( APR based)? Apache Tomcat Native library' >&2; then 		echo >&2 "$nativeLines"; 		exit 1; 	fi
# Thu, 11 Aug 2022 21:03:18 GMT
EXPOSE 8080
# Thu, 11 Aug 2022 21:03:18 GMT
CMD ["catalina.sh" "run"]
```

-	Layers:
	-	`sha256:6f8c2fc0a4f976c1c0bd1c0e14022b3ed8b7c83cdb247c83016052c3678aaf28`  
		Last Modified: Tue, 02 Aug 2022 01:33:53 GMT  
		Size: 35.7 MB (35718004 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1beca851dc26aa06b8642a7de984d251e67d42f6e7104fcad4eab7d1664f2090`  
		Last Modified: Thu, 11 Aug 2022 19:33:42 GMT  
		Size: 11.9 MB (11875147 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5c2d9ea429dab9dc0d6aa3a4e4cb2dfcdc46cd3d674174c47a131dc84a64c5cc`  
		Last Modified: Thu, 11 Aug 2022 19:38:05 GMT  
		Size: 41.9 MB (41885516 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9ecf81efed18b64e0203c1da113af51f07bc3db6caed60cde624d200a0632740`  
		Last Modified: Thu, 11 Aug 2022 19:37:55 GMT  
		Size: 160.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fc3fc64f72d1695d348e60d5d15ed2420e3abed87f2d7cc4c1fd0e9188ed109a`  
		Last Modified: Thu, 11 Aug 2022 21:40:16 GMT  
		Size: 173.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ddf54bfa3680d221becca0bf5bfb655f5bf7bd1c04cac90476c24af06bd81639`  
		Last Modified: Thu, 11 Aug 2022 21:44:26 GMT  
		Size: 12.6 MB (12595285 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e678ff65771e4aab82bde16570f811486e41bc2591d7252e68dbeb995bdd5594`  
		Last Modified: Thu, 11 Aug 2022 21:44:24 GMT  
		Size: 477.9 KB (477933 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:67ab030fb84e667ab6596fe3f93f1202e515faa7d581ff725a4890015f4c0fba`  
		Last Modified: Thu, 11 Aug 2022 21:44:24 GMT  
		Size: 130.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `tomcat:jre11` - linux; s390x

```console
$ docker pull tomcat@sha256:a89c5544dc3941ca0ec93b7fd6a06205e694f022dbbd90d793d58da6b24b5816
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **93.5 MB (93548625 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:18f1c56342ee4f51edfb08b89b211e10877002f08874f20a66326c53f7416e83`
-	Default Command: `["catalina.sh","run"]`

```dockerfile
# Tue, 02 Aug 2022 01:02:17 GMT
ADD file:d5a5e56e0ca8287f27b257e3ddbc9675a1bdac1912afbbab6cddd891056cd144 in / 
# Tue, 02 Aug 2022 01:02:19 GMT
CMD ["bash"]
# Thu, 11 Aug 2022 18:42:20 GMT
ENV JAVA_HOME=/opt/java/openjdk
# Thu, 11 Aug 2022 18:42:20 GMT
ENV PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 11 Aug 2022 18:42:20 GMT
ENV LANG=en_US.UTF-8 LANGUAGE=en_US:en LC_ALL=en_US.UTF-8
# Thu, 11 Aug 2022 18:42:35 GMT
RUN apt-get update     && DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends tzdata wget ca-certificates fontconfig locales     && echo "en_US.UTF-8 UTF-8" >> /etc/locale.gen     && locale-gen en_US.UTF-8     && rm -rf /var/lib/apt/lists/*
# Thu, 11 Aug 2022 18:42:36 GMT
ENV JAVA_VERSION=jdk-11.0.16+8
# Thu, 11 Aug 2022 18:43:16 GMT
RUN set -eux;     ARCH="$(dpkg --print-architecture)";     case "${ARCH}" in        aarch64|arm64)          ESUM='3fa9cb99229ede53d4efddb686106df77794e02b1f4defea6b70b2b53380a8c7';          BINARY_URL='https://github.com/adoptium/temurin11-binaries/releases/download/jdk-11.0.16%2B8/OpenJDK11U-jre_aarch64_linux_hotspot_11.0.16_8.tar.gz';          ;;        armhf|arm)          ESUM='658ee6d797e6ca4d25de24d45072a44ed8462e3a9feaa38ef9f6d033d18401c8';          BINARY_URL='https://github.com/adoptium/temurin11-binaries/releases/download/jdk-11.0.16%2B8/OpenJDK11U-jre_arm_linux_hotspot_11.0.16_8.tar.gz';          ;;        ppc64el|powerpc:common64)          ESUM='6002b8f6c7b3421ac70601d1bf55f355b75c4a193c97e12974b4c2301d737d8d';          BINARY_URL='https://github.com/adoptium/temurin11-binaries/releases/download/jdk-11.0.16%2B8/OpenJDK11U-jre_ppc64le_linux_hotspot_11.0.16_8.tar.gz';          ;;        s390x|s390:64-bit)          ESUM='683902c6429f28c606685f46d628291c989de3effe50eca51889388d65f96b95';          BINARY_URL='https://github.com/adoptium/temurin11-binaries/releases/download/jdk-11.0.16%2B8/OpenJDK11U-jre_s390x_linux_hotspot_11.0.16_8.tar.gz';          ;;        amd64|i386:x86-64)          ESUM='74988677f1e1692f8f482ae5f75814b908bb3cf5a8b7d9872873a42e330e7595';          BINARY_URL='https://github.com/adoptium/temurin11-binaries/releases/download/jdk-11.0.16%2B8/OpenJDK11U-jre_x64_linux_hotspot_11.0.16_8.tar.gz';          ;;        *)          echo "Unsupported arch: ${ARCH}";          exit 1;          ;;     esac; 	  wget -O /tmp/openjdk.tar.gz ${BINARY_URL}; 	  echo "${ESUM} */tmp/openjdk.tar.gz" | sha256sum -c -; 	  mkdir -p "$JAVA_HOME"; 	  tar --extract 	      --file /tmp/openjdk.tar.gz 	      --directory "$JAVA_HOME" 	      --strip-components 1 	      --no-same-owner 	  ;     rm /tmp/openjdk.tar.gz;     find "$JAVA_HOME/lib" -name '*.so' -exec dirname '{}' ';' | sort -u > /etc/ld.so.conf.d/docker-openjdk.conf;     ldconfig;     java -Xshare:dump;
# Thu, 11 Aug 2022 18:43:18 GMT
RUN echo Verifying install ...     && fileEncoding="$(echo 'System.out.println(System.getProperty("file.encoding"))' | jshell -s -)"; [ "$fileEncoding" = 'UTF-8' ]; rm -rf ~/.java     && echo java --version && java --version     && echo Complete.
# Thu, 11 Aug 2022 19:45:09 GMT
ENV CATALINA_HOME=/usr/local/tomcat
# Thu, 11 Aug 2022 19:45:09 GMT
ENV PATH=/usr/local/tomcat/bin:/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 11 Aug 2022 19:45:10 GMT
RUN mkdir -p "$CATALINA_HOME"
# Thu, 11 Aug 2022 19:45:11 GMT
WORKDIR /usr/local/tomcat
# Thu, 11 Aug 2022 19:45:11 GMT
ENV TOMCAT_NATIVE_LIBDIR=/usr/local/tomcat/native-jni-lib
# Thu, 11 Aug 2022 19:45:12 GMT
ENV LD_LIBRARY_PATH=/usr/local/tomcat/native-jni-lib
# Thu, 11 Aug 2022 19:45:12 GMT
ENV GPG_KEYS=A9C5DF4D22E99998D9875A5110C01C5A2F6059E7
# Thu, 11 Aug 2022 19:45:13 GMT
ENV TOMCAT_MAJOR=10
# Thu, 11 Aug 2022 19:50:33 GMT
ENV TOMCAT_VERSION=10.0.23
# Thu, 11 Aug 2022 19:50:34 GMT
ENV TOMCAT_SHA512=0e0263e8280f2ccfb4bef916444a6105fef689a3d95c334c8a7bfe59f1e3966d48ea624727f1818a4df331a603f1ac5e21b908dda3cae676ddc1aef90c2d12ab
# Thu, 11 Aug 2022 19:50:35 GMT
COPY dir:29b86f65d98c7a83f2b8805a8152a3e0c31e4b66f2729178b0f819a834b7abee in /usr/local/tomcat 
# Thu, 11 Aug 2022 19:50:44 GMT
RUN set -eux; 	apt-get update; 	xargs -rt apt-get install -y --no-install-recommends < "$TOMCAT_NATIVE_LIBDIR/.dependencies.txt"; 	rm -rf /var/lib/apt/lists/*
# Thu, 11 Aug 2022 19:50:47 GMT
RUN set -eux; 	nativeLines="$(catalina.sh configtest 2>&1)"; 	nativeLines="$(echo "$nativeLines" | grep 'Apache Tomcat Native')"; 	nativeLines="$(echo "$nativeLines" | sort -u)"; 	if ! echo "$nativeLines" | grep -E 'INFO: Loaded( APR based)? Apache Tomcat Native library' >&2; then 		echo >&2 "$nativeLines"; 		exit 1; 	fi
# Thu, 11 Aug 2022 19:50:48 GMT
EXPOSE 8080
# Thu, 11 Aug 2022 19:50:49 GMT
CMD ["catalina.sh" "run"]
```

-	Layers:
	-	`sha256:f97967c51aac02138b615522a1bab9c75addd5896f43ade17ddaac44e0644283`  
		Last Modified: Tue, 02 Aug 2022 01:03:51 GMT  
		Size: 28.6 MB (28642785 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9739633e842cf87e58170d8e9c3754c3a3a79b50ed6fd03fa65bbaf2dabcde04`  
		Last Modified: Thu, 11 Aug 2022 18:49:41 GMT  
		Size: 11.4 MB (11412494 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d546e934e4fbaa88de69ad2d7df9404d12c4c8e0226f64d693d88e545080bc95`  
		Last Modified: Thu, 11 Aug 2022 18:50:22 GMT  
		Size: 40.5 MB (40479895 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2c836e0958febc49e5be83535c64cd2d7df8def1e2c92c9b6a5168776283199f`  
		Last Modified: Thu, 11 Aug 2022 18:50:17 GMT  
		Size: 161.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e3a0a1106f9df170174fd35269f6ff96298121e9232a161b4a35b36768f521b3`  
		Last Modified: Thu, 11 Aug 2022 20:12:25 GMT  
		Size: 172.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1276855402d5db0ca854dc293a12bc075704bbfbc0c42345e4306ec6a4fbea5f`  
		Last Modified: Thu, 11 Aug 2022 20:15:14 GMT  
		Size: 12.6 MB (12564809 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:50953db59719c2b7592cd8f868ae06827f9266a826be09169bc39c207f8a7757`  
		Last Modified: Thu, 11 Aug 2022 20:15:14 GMT  
		Size: 448.2 KB (448179 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:50530178274e398d1c94a46dab738e3bff8642c673373e9a754dc9b369b95e62`  
		Last Modified: Thu, 11 Aug 2022 20:15:14 GMT  
		Size: 130.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
