## `tomcat:jre17-temurin`

```console
$ docker pull tomcat@sha256:5e10fd45c5cc7d4a8978ff0634b59b9db29b98ee5d5fb235bf3f5d5187beac49
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 5
	-	linux; amd64
	-	linux; arm variant v7
	-	linux; arm64 variant v8
	-	linux; ppc64le
	-	linux; s390x

### `tomcat:jre17-temurin` - linux; amd64

```console
$ docker pull tomcat@sha256:56b2ac27e46c2d250469693b702ef50e6ae8423ff8b6157912a0bc45998f2db1
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **109.5 MB (109549803 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e393f62ce8b50d4d912b84383d4901662bb7b1fc8c0c447f831e79d7115f8cc8`
-	Default Command: `["catalina.sh","run"]`

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
# Thu, 16 Mar 2023 02:46:48 GMT
RUN apt-get update     && DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends tzdata curl wget ca-certificates fontconfig locales binutils     && echo "en_US.UTF-8 UTF-8" >> /etc/locale.gen     && locale-gen en_US.UTF-8     && rm -rf /var/lib/apt/lists/*
# Wed, 26 Apr 2023 19:23:00 GMT
ENV JAVA_VERSION=jdk-17.0.7+7
# Wed, 26 Apr 2023 19:23:56 GMT
RUN set -eux;     ARCH="$(dpkg --print-architecture)";     case "${ARCH}" in        aarch64|arm64)          ESUM='2ff6a4fd1fa354047c93ba8c3179967156162f27bd683aee1f6e52a480bcbe6a';          BINARY_URL='https://github.com/adoptium/temurin17-binaries/releases/download/jdk-17.0.7%2B7/OpenJDK17U-jre_aarch64_linux_hotspot_17.0.7_7.tar.gz';          ;;        armhf|arm)          ESUM='5b0401199c7c9163b8395ebf25195ed395fec7b7ef7158c36302420cf993825a';          BINARY_URL='https://github.com/adoptium/temurin17-binaries/releases/download/jdk-17.0.7%2B7/OpenJDK17U-jre_arm_linux_hotspot_17.0.7_7.tar.gz';          ;;        ppc64el|powerpc:common64)          ESUM='cc25e74c0817cd4d943bba056b256b86e0e9148bf41d7600c5ec2e1eadb2e470';          BINARY_URL='https://github.com/adoptium/temurin17-binaries/releases/download/jdk-17.0.7%2B7/OpenJDK17U-jre_ppc64le_linux_hotspot_17.0.7_7.tar.gz';          ;;        s390x|s390:64-bit)          ESUM='393f6348c6c0cb12699565cf23a7617fbfce973e6d47584a0920e99fbb1b1e3e';          BINARY_URL='https://github.com/adoptium/temurin17-binaries/releases/download/jdk-17.0.7%2B7/OpenJDK17U-jre_s390x_linux_hotspot_17.0.7_7.tar.gz';          ;;        amd64|i386:x86-64)          ESUM='bb025133b96266f6415d5084bb9b260340a813968007f1d2d14690f20bd021ca';          BINARY_URL='https://github.com/adoptium/temurin17-binaries/releases/download/jdk-17.0.7%2B7/OpenJDK17U-jre_x64_linux_hotspot_17.0.7_7.tar.gz';          ;;        *)          echo "Unsupported arch: ${ARCH}";          exit 1;          ;;     esac; 	  wget -O /tmp/openjdk.tar.gz ${BINARY_URL}; 	  echo "${ESUM} */tmp/openjdk.tar.gz" | sha256sum -c -; 	  mkdir -p "$JAVA_HOME"; 	  tar --extract 	      --file /tmp/openjdk.tar.gz 	      --directory "$JAVA_HOME" 	      --strip-components 1 	      --no-same-owner 	  ;     rm -f /tmp/openjdk.tar.gz ${JAVA_HOME}/src.zip;     find "$JAVA_HOME/lib" -name '*.so' -exec dirname '{}' ';' | sort -u > /etc/ld.so.conf.d/docker-openjdk.conf;     ldconfig;     java -Xshare:dump;
# Wed, 26 Apr 2023 19:23:56 GMT
RUN echo Verifying install ...     && fileEncoding="$(echo 'System.out.println(System.getProperty("file.encoding"))' | jshell -s -)"; [ "$fileEncoding" = 'UTF-8' ]; rm -rf ~/.java     && echo java --version && java --version     && echo Complete.
# Wed, 26 Apr 2023 21:35:51 GMT
ENV CATALINA_HOME=/usr/local/tomcat
# Wed, 26 Apr 2023 21:35:52 GMT
ENV PATH=/usr/local/tomcat/bin:/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 26 Apr 2023 21:35:52 GMT
RUN mkdir -p "$CATALINA_HOME"
# Wed, 26 Apr 2023 21:35:52 GMT
WORKDIR /usr/local/tomcat
# Wed, 26 Apr 2023 21:35:52 GMT
ENV TOMCAT_NATIVE_LIBDIR=/usr/local/tomcat/native-jni-lib
# Wed, 26 Apr 2023 21:35:52 GMT
ENV LD_LIBRARY_PATH=/usr/local/tomcat/native-jni-lib
# Wed, 26 Apr 2023 21:36:35 GMT
ENV GPG_KEYS=5C3C5F3E314C866292F359A8F3AD5C94A67F707E A9C5DF4D22E99998D9875A5110C01C5A2F6059E7
# Wed, 26 Apr 2023 21:36:35 GMT
ENV TOMCAT_MAJOR=10
# Wed, 26 Apr 2023 21:36:35 GMT
ENV TOMCAT_VERSION=10.1.8
# Wed, 26 Apr 2023 21:36:35 GMT
ENV TOMCAT_SHA512=bf1a80582d3fc6e7e32c8b72f6b9c2703d39832a8a337f660b8c201196a555c717647825b495169bef61845a1905507b10d62c2d76dfd8ca180bcd49e44d0d5e
# Wed, 03 May 2023 11:26:45 GMT
COPY dir:1cd643b7c29f7cdafe8d6a1c7417be740c14afde24657fd702d95b5c3f22abb3 in /usr/local/tomcat 
# Wed, 03 May 2023 11:26:50 GMT
RUN set -eux; 	apt-get update; 	xargs -rt apt-get install -y --no-install-recommends < "$TOMCAT_NATIVE_LIBDIR/.dependencies.txt"; 	rm -rf /var/lib/apt/lists/*
# Wed, 03 May 2023 11:26:51 GMT
RUN set -eux; 	nativeLines="$(catalina.sh configtest 2>&1)"; 	nativeLines="$(echo "$nativeLines" | grep 'Apache Tomcat Native')"; 	nativeLines="$(echo "$nativeLines" | sort -u)"; 	if ! echo "$nativeLines" | grep -E 'INFO: Loaded( APR based)? Apache Tomcat Native library' >&2; then 		echo >&2 "$nativeLines"; 		exit 1; 	fi
# Wed, 03 May 2023 11:26:51 GMT
EXPOSE 8080
# Wed, 03 May 2023 11:26:51 GMT
CMD ["catalina.sh" "run"]
```

-	Layers:
	-	`sha256:74ac377868f863e123f24c409f79709f7563fa464557c36a09cf6f85c8b92b7f`  
		Last Modified: Wed, 08 Mar 2023 09:03:15 GMT  
		Size: 30.4 MB (30429963 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a182a611d05b01879f065473c49fb968b8d30312f931350ea07af1c46aa8b4f9`  
		Last Modified: Thu, 16 Mar 2023 02:53:08 GMT  
		Size: 17.0 MB (16975402 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:20cf737c5920a76829f486a52d0506e5082c6f0c10bbb7983c3fe3cc972a8d4d`  
		Last Modified: Wed, 26 Apr 2023 19:34:45 GMT  
		Size: 47.0 MB (47006292 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:08e9ed4ea8fed4bbc7a6b909db9b12ced02c76f3ea22634e6042e38bfebd2a87`  
		Last Modified: Wed, 26 Apr 2023 19:34:38 GMT  
		Size: 161.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a1e9bc1989ca6609d1e658d2eff7510706e3a3c2f4a7e90ebdec1a34351361aa`  
		Last Modified: Wed, 26 Apr 2023 21:49:17 GMT  
		Size: 174.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1b9531237de7ca106d0e925bdacfc3963ee73db4749d4aa94d3508e4683c5070`  
		Last Modified: Wed, 03 May 2023 11:45:01 GMT  
		Size: 12.2 MB (12167126 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:adee126c848f3c93599653ff9b23568436dc144cc6cb95662b061a5d50de0670`  
		Last Modified: Wed, 03 May 2023 11:45:01 GMT  
		Size: 3.0 MB (2970555 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0c65ff36d2673c7edabc9b2ddbd719178fa627e44f136bfee4f2925032156236`  
		Last Modified: Wed, 03 May 2023 11:45:00 GMT  
		Size: 130.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `tomcat:jre17-temurin` - linux; arm variant v7

```console
$ docker pull tomcat@sha256:3f5b17a968b8dd31b5f60bd7e9f12f2b9487e965bb86e73e19c180394a0a0215
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **101.3 MB (101346311 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b3e30267b13addba70a4ec2c2e15f59117283d86a5acee89624d50a7b8fd91d7`
-	Default Command: `["catalina.sh","run"]`

```dockerfile
# Tue, 25 Apr 2023 17:36:58 GMT
ARG RELEASE
# Tue, 25 Apr 2023 17:36:58 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Tue, 25 Apr 2023 17:36:58 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Tue, 25 Apr 2023 17:36:58 GMT
LABEL org.opencontainers.image.version=22.04
# Tue, 25 Apr 2023 17:37:01 GMT
ADD file:08f4534e90f8ffc3bdb6cf9c04b599190ea4e1d39328135a84f4ffcd614bacb4 in / 
# Tue, 25 Apr 2023 17:37:01 GMT
CMD ["/bin/bash"]
# Thu, 04 May 2023 06:51:40 GMT
ENV JAVA_HOME=/opt/java/openjdk
# Thu, 04 May 2023 06:51:40 GMT
ENV PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 04 May 2023 06:51:40 GMT
ENV LANG=en_US.UTF-8 LANGUAGE=en_US:en LC_ALL=en_US.UTF-8
# Thu, 04 May 2023 06:53:21 GMT
RUN apt-get update     && DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends tzdata curl wget ca-certificates fontconfig locales binutils     && echo "en_US.UTF-8 UTF-8" >> /etc/locale.gen     && locale-gen en_US.UTF-8     && rm -rf /var/lib/apt/lists/*
# Thu, 04 May 2023 06:53:21 GMT
ENV JAVA_VERSION=jdk-17.0.7+7
# Thu, 04 May 2023 06:53:47 GMT
RUN set -eux;     ARCH="$(dpkg --print-architecture)";     case "${ARCH}" in        aarch64|arm64)          ESUM='2ff6a4fd1fa354047c93ba8c3179967156162f27bd683aee1f6e52a480bcbe6a';          BINARY_URL='https://github.com/adoptium/temurin17-binaries/releases/download/jdk-17.0.7%2B7/OpenJDK17U-jre_aarch64_linux_hotspot_17.0.7_7.tar.gz';          ;;        armhf|arm)          ESUM='5b0401199c7c9163b8395ebf25195ed395fec7b7ef7158c36302420cf993825a';          BINARY_URL='https://github.com/adoptium/temurin17-binaries/releases/download/jdk-17.0.7%2B7/OpenJDK17U-jre_arm_linux_hotspot_17.0.7_7.tar.gz';          ;;        ppc64el|powerpc:common64)          ESUM='cc25e74c0817cd4d943bba056b256b86e0e9148bf41d7600c5ec2e1eadb2e470';          BINARY_URL='https://github.com/adoptium/temurin17-binaries/releases/download/jdk-17.0.7%2B7/OpenJDK17U-jre_ppc64le_linux_hotspot_17.0.7_7.tar.gz';          ;;        s390x|s390:64-bit)          ESUM='393f6348c6c0cb12699565cf23a7617fbfce973e6d47584a0920e99fbb1b1e3e';          BINARY_URL='https://github.com/adoptium/temurin17-binaries/releases/download/jdk-17.0.7%2B7/OpenJDK17U-jre_s390x_linux_hotspot_17.0.7_7.tar.gz';          ;;        amd64|i386:x86-64)          ESUM='bb025133b96266f6415d5084bb9b260340a813968007f1d2d14690f20bd021ca';          BINARY_URL='https://github.com/adoptium/temurin17-binaries/releases/download/jdk-17.0.7%2B7/OpenJDK17U-jre_x64_linux_hotspot_17.0.7_7.tar.gz';          ;;        *)          echo "Unsupported arch: ${ARCH}";          exit 1;          ;;     esac; 	  wget -O /tmp/openjdk.tar.gz ${BINARY_URL}; 	  echo "${ESUM} */tmp/openjdk.tar.gz" | sha256sum -c -; 	  mkdir -p "$JAVA_HOME"; 	  tar --extract 	      --file /tmp/openjdk.tar.gz 	      --directory "$JAVA_HOME" 	      --strip-components 1 	      --no-same-owner 	  ;     rm -f /tmp/openjdk.tar.gz ${JAVA_HOME}/src.zip;     find "$JAVA_HOME/lib" -name '*.so' -exec dirname '{}' ';' | sort -u > /etc/ld.so.conf.d/docker-openjdk.conf;     ldconfig;     java -Xshare:dump;
# Thu, 04 May 2023 06:53:48 GMT
RUN echo Verifying install ...     && fileEncoding="$(echo 'System.out.println(System.getProperty("file.encoding"))' | jshell -s -)"; [ "$fileEncoding" = 'UTF-8' ]; rm -rf ~/.java     && echo java --version && java --version     && echo Complete.
# Thu, 04 May 2023 12:04:24 GMT
ENV CATALINA_HOME=/usr/local/tomcat
# Thu, 04 May 2023 12:04:24 GMT
ENV PATH=/usr/local/tomcat/bin:/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 04 May 2023 12:04:24 GMT
RUN mkdir -p "$CATALINA_HOME"
# Thu, 04 May 2023 12:04:24 GMT
WORKDIR /usr/local/tomcat
# Thu, 04 May 2023 12:04:24 GMT
ENV TOMCAT_NATIVE_LIBDIR=/usr/local/tomcat/native-jni-lib
# Thu, 04 May 2023 12:04:24 GMT
ENV LD_LIBRARY_PATH=/usr/local/tomcat/native-jni-lib
# Thu, 04 May 2023 12:05:06 GMT
ENV GPG_KEYS=5C3C5F3E314C866292F359A8F3AD5C94A67F707E A9C5DF4D22E99998D9875A5110C01C5A2F6059E7
# Thu, 04 May 2023 12:05:06 GMT
ENV TOMCAT_MAJOR=10
# Thu, 04 May 2023 12:05:06 GMT
ENV TOMCAT_VERSION=10.1.8
# Thu, 04 May 2023 12:05:06 GMT
ENV TOMCAT_SHA512=bf1a80582d3fc6e7e32c8b72f6b9c2703d39832a8a337f660b8c201196a555c717647825b495169bef61845a1905507b10d62c2d76dfd8ca180bcd49e44d0d5e
# Thu, 04 May 2023 12:05:07 GMT
COPY dir:5d4ed86db7599fbd33f175a21e5f1c9781beeaf3954283a810ec3275cc15f5de in /usr/local/tomcat 
# Thu, 04 May 2023 12:05:11 GMT
RUN set -eux; 	apt-get update; 	xargs -rt apt-get install -y --no-install-recommends < "$TOMCAT_NATIVE_LIBDIR/.dependencies.txt"; 	rm -rf /var/lib/apt/lists/*
# Thu, 04 May 2023 12:05:12 GMT
RUN set -eux; 	nativeLines="$(catalina.sh configtest 2>&1)"; 	nativeLines="$(echo "$nativeLines" | grep 'Apache Tomcat Native')"; 	nativeLines="$(echo "$nativeLines" | sort -u)"; 	if ! echo "$nativeLines" | grep -E 'INFO: Loaded( APR based)? Apache Tomcat Native library' >&2; then 		echo >&2 "$nativeLines"; 		exit 1; 	fi
# Thu, 04 May 2023 12:05:12 GMT
EXPOSE 8080
# Thu, 04 May 2023 12:05:12 GMT
CMD ["catalina.sh" "run"]
```

-	Layers:
	-	`sha256:2561bae7e5e30e2beaf0cb6907571e792834948f12d2a8923229e5ac85134ad4`  
		Last Modified: Wed, 26 Apr 2023 02:07:55 GMT  
		Size: 27.0 MB (27026323 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2813bcd6edbef45cf68ef036e0b002ed7c943182304d7236121aea572b1c2de1`  
		Last Modified: Thu, 04 May 2023 06:56:01 GMT  
		Size: 17.2 MB (17166498 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:438449c88c14cc285abcab931964d021d2033d417fd99613f57c4d5ae8df509c`  
		Last Modified: Thu, 04 May 2023 06:56:33 GMT  
		Size: 44.6 MB (44579955 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:728ae3b97b880a9aa699415ed009e373b594d267ee6165e65c9f6a3e0e89a777`  
		Last Modified: Thu, 04 May 2023 06:56:25 GMT  
		Size: 162.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1f4af1b695f5603d53eadc8a6795f0ed5a90b72af2bd8cee57bc45062a55a42d`  
		Last Modified: Thu, 04 May 2023 12:10:32 GMT  
		Size: 170.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e270361ce30ff102254ff59a8004685d104e40ecf8daf8dea314930ed40fa0d2`  
		Last Modified: Thu, 04 May 2023 12:11:30 GMT  
		Size: 12.1 MB (12142152 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:037c8fb188b4006a71e56c4c3865c8facdeaa37256f22ecf4d844df916f3c25d`  
		Last Modified: Thu, 04 May 2023 12:11:29 GMT  
		Size: 430.9 KB (430920 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:87b51ffdcdb6c1eda7456ac028532bc0d7e0b7c1b85901bd26828a1042592b17`  
		Last Modified: Thu, 04 May 2023 12:11:29 GMT  
		Size: 131.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `tomcat:jre17-temurin` - linux; arm64 variant v8

```console
$ docker pull tomcat@sha256:385ae3dfbffc0a7c589d249ce18cc8d0a41e6e7080758853839a4adecfb5316a
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **106.0 MB (105974128 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c1cdf6ac2fedd270240470dca821d8514bf083292388cf4af88b2c2f080a6b4e`
-	Default Command: `["catalina.sh","run"]`

```dockerfile
# Tue, 25 Apr 2023 17:31:58 GMT
ARG RELEASE
# Tue, 25 Apr 2023 17:31:58 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Tue, 25 Apr 2023 17:31:58 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Tue, 25 Apr 2023 17:31:59 GMT
LABEL org.opencontainers.image.version=22.04
# Tue, 25 Apr 2023 17:32:02 GMT
ADD file:aee0d7770ef2f24dc9697e86d391529d001a4013b6e30a3ac90a57932814a57e in / 
# Tue, 25 Apr 2023 17:32:02 GMT
CMD ["/bin/bash"]
# Thu, 04 May 2023 03:25:09 GMT
ENV JAVA_HOME=/opt/java/openjdk
# Thu, 04 May 2023 03:25:09 GMT
ENV PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 04 May 2023 03:25:09 GMT
ENV LANG=en_US.UTF-8 LANGUAGE=en_US:en LC_ALL=en_US.UTF-8
# Thu, 04 May 2023 03:26:25 GMT
RUN apt-get update     && DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends tzdata curl wget ca-certificates fontconfig locales binutils     && echo "en_US.UTF-8 UTF-8" >> /etc/locale.gen     && locale-gen en_US.UTF-8     && rm -rf /var/lib/apt/lists/*
# Thu, 04 May 2023 03:26:25 GMT
ENV JAVA_VERSION=jdk-17.0.7+7
# Thu, 04 May 2023 03:26:51 GMT
RUN set -eux;     ARCH="$(dpkg --print-architecture)";     case "${ARCH}" in        aarch64|arm64)          ESUM='2ff6a4fd1fa354047c93ba8c3179967156162f27bd683aee1f6e52a480bcbe6a';          BINARY_URL='https://github.com/adoptium/temurin17-binaries/releases/download/jdk-17.0.7%2B7/OpenJDK17U-jre_aarch64_linux_hotspot_17.0.7_7.tar.gz';          ;;        armhf|arm)          ESUM='5b0401199c7c9163b8395ebf25195ed395fec7b7ef7158c36302420cf993825a';          BINARY_URL='https://github.com/adoptium/temurin17-binaries/releases/download/jdk-17.0.7%2B7/OpenJDK17U-jre_arm_linux_hotspot_17.0.7_7.tar.gz';          ;;        ppc64el|powerpc:common64)          ESUM='cc25e74c0817cd4d943bba056b256b86e0e9148bf41d7600c5ec2e1eadb2e470';          BINARY_URL='https://github.com/adoptium/temurin17-binaries/releases/download/jdk-17.0.7%2B7/OpenJDK17U-jre_ppc64le_linux_hotspot_17.0.7_7.tar.gz';          ;;        s390x|s390:64-bit)          ESUM='393f6348c6c0cb12699565cf23a7617fbfce973e6d47584a0920e99fbb1b1e3e';          BINARY_URL='https://github.com/adoptium/temurin17-binaries/releases/download/jdk-17.0.7%2B7/OpenJDK17U-jre_s390x_linux_hotspot_17.0.7_7.tar.gz';          ;;        amd64|i386:x86-64)          ESUM='bb025133b96266f6415d5084bb9b260340a813968007f1d2d14690f20bd021ca';          BINARY_URL='https://github.com/adoptium/temurin17-binaries/releases/download/jdk-17.0.7%2B7/OpenJDK17U-jre_x64_linux_hotspot_17.0.7_7.tar.gz';          ;;        *)          echo "Unsupported arch: ${ARCH}";          exit 1;          ;;     esac; 	  wget -O /tmp/openjdk.tar.gz ${BINARY_URL}; 	  echo "${ESUM} */tmp/openjdk.tar.gz" | sha256sum -c -; 	  mkdir -p "$JAVA_HOME"; 	  tar --extract 	      --file /tmp/openjdk.tar.gz 	      --directory "$JAVA_HOME" 	      --strip-components 1 	      --no-same-owner 	  ;     rm -f /tmp/openjdk.tar.gz ${JAVA_HOME}/src.zip;     find "$JAVA_HOME/lib" -name '*.so' -exec dirname '{}' ';' | sort -u > /etc/ld.so.conf.d/docker-openjdk.conf;     ldconfig;     java -Xshare:dump;
# Thu, 04 May 2023 03:26:52 GMT
RUN echo Verifying install ...     && fileEncoding="$(echo 'System.out.println(System.getProperty("file.encoding"))' | jshell -s -)"; [ "$fileEncoding" = 'UTF-8' ]; rm -rf ~/.java     && echo java --version && java --version     && echo Complete.
# Thu, 04 May 2023 11:13:04 GMT
ENV CATALINA_HOME=/usr/local/tomcat
# Thu, 04 May 2023 11:13:04 GMT
ENV PATH=/usr/local/tomcat/bin:/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 04 May 2023 11:13:05 GMT
RUN mkdir -p "$CATALINA_HOME"
# Thu, 04 May 2023 11:13:05 GMT
WORKDIR /usr/local/tomcat
# Thu, 04 May 2023 11:13:05 GMT
ENV TOMCAT_NATIVE_LIBDIR=/usr/local/tomcat/native-jni-lib
# Thu, 04 May 2023 11:13:05 GMT
ENV LD_LIBRARY_PATH=/usr/local/tomcat/native-jni-lib
# Thu, 04 May 2023 11:13:39 GMT
ENV GPG_KEYS=5C3C5F3E314C866292F359A8F3AD5C94A67F707E A9C5DF4D22E99998D9875A5110C01C5A2F6059E7
# Thu, 04 May 2023 11:13:39 GMT
ENV TOMCAT_MAJOR=10
# Thu, 04 May 2023 11:13:39 GMT
ENV TOMCAT_VERSION=10.1.8
# Thu, 04 May 2023 11:13:40 GMT
ENV TOMCAT_SHA512=bf1a80582d3fc6e7e32c8b72f6b9c2703d39832a8a337f660b8c201196a555c717647825b495169bef61845a1905507b10d62c2d76dfd8ca180bcd49e44d0d5e
# Thu, 04 May 2023 11:13:40 GMT
COPY dir:f364c6c35b32b9314da35b7e3e02f8b55fc9c4b520bbb2f77f51c6d50d580b11 in /usr/local/tomcat 
# Thu, 04 May 2023 11:13:43 GMT
RUN set -eux; 	apt-get update; 	xargs -rt apt-get install -y --no-install-recommends < "$TOMCAT_NATIVE_LIBDIR/.dependencies.txt"; 	rm -rf /var/lib/apt/lists/*
# Thu, 04 May 2023 11:13:44 GMT
RUN set -eux; 	nativeLines="$(catalina.sh configtest 2>&1)"; 	nativeLines="$(echo "$nativeLines" | grep 'Apache Tomcat Native')"; 	nativeLines="$(echo "$nativeLines" | sort -u)"; 	if ! echo "$nativeLines" | grep -E 'INFO: Loaded( APR based)? Apache Tomcat Native library' >&2; then 		echo >&2 "$nativeLines"; 		exit 1; 	fi
# Thu, 04 May 2023 11:13:44 GMT
EXPOSE 8080
# Thu, 04 May 2023 11:13:44 GMT
CMD ["catalina.sh" "run"]
```

-	Layers:
	-	`sha256:f3f60f415e9a03eed88bd5dd5268c841cde08dacf16911a3ef1e4e0fcdd76568`  
		Last Modified: Wed, 26 Apr 2023 02:08:37 GMT  
		Size: 28.4 MB (28389440 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2da9c27f8f486373408efc6e2d12bdb650ff3041dc480e2fcd2dd0c7e9be9777`  
		Last Modified: Thu, 04 May 2023 03:29:30 GMT  
		Size: 18.5 MB (18471737 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3634abbba846ac1f9a5583bf63ad7123013aa48dea16d5b2e8f9d56ec2324827`  
		Last Modified: Thu, 04 May 2023 03:29:55 GMT  
		Size: 46.5 MB (46488613 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:806df332a53f1b7492880bdbd41f29c61255518e200531203c319b398aa8076f`  
		Last Modified: Thu, 04 May 2023 03:29:49 GMT  
		Size: 160.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:361f146b34be7bee47334c57558ec692ed07b18d13ab67efcb36868955e1ab69`  
		Last Modified: Thu, 04 May 2023 11:22:32 GMT  
		Size: 171.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5c443825f69bfaf3d218320a2256da60d13d5d4a019ccc8240d6305eb1bc157d`  
		Last Modified: Thu, 04 May 2023 11:23:29 GMT  
		Size: 12.2 MB (12167741 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:16d246189859fc0a3347a07e068b847c97e35e9ca9673cc569b9763d89f3bb72`  
		Last Modified: Thu, 04 May 2023 11:23:28 GMT  
		Size: 456.1 KB (456136 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f0c8be4a552058bff39e310b66ef1d5606cd1f39ca16d34ae145c43f9d5f8a2b`  
		Last Modified: Thu, 04 May 2023 11:23:28 GMT  
		Size: 130.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `tomcat:jre17-temurin` - linux; ppc64le

```console
$ docker pull tomcat@sha256:0bbecdf9e1c131c71139c9cd92cf738be9ab05fc0efb20f941394bfff699c458
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **116.4 MB (116385060 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c948452b53e8ea01304db83e4cde2d5dc93b7b4e9ebddfd03159fe82080f20df`
-	Default Command: `["catalina.sh","run"]`

```dockerfile
# Wed, 08 Mar 2023 04:39:16 GMT
ARG RELEASE
# Wed, 08 Mar 2023 04:39:16 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Wed, 08 Mar 2023 04:39:16 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Wed, 08 Mar 2023 04:39:16 GMT
LABEL org.opencontainers.image.version=22.04
# Wed, 08 Mar 2023 04:39:20 GMT
ADD file:d7434a52d8d8aa6288e788f6fe7e156f0e11bf9b8275efaf70aab0bfc4d919cf in / 
# Wed, 08 Mar 2023 04:39:20 GMT
CMD ["/bin/bash"]
# Thu, 16 Mar 2023 03:57:34 GMT
ENV JAVA_HOME=/opt/java/openjdk
# Thu, 16 Mar 2023 03:57:34 GMT
ENV PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 16 Mar 2023 03:57:35 GMT
ENV LANG=en_US.UTF-8 LANGUAGE=en_US:en LC_ALL=en_US.UTF-8
# Thu, 16 Mar 2023 04:03:27 GMT
RUN apt-get update     && DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends tzdata curl wget ca-certificates fontconfig locales binutils     && echo "en_US.UTF-8 UTF-8" >> /etc/locale.gen     && locale-gen en_US.UTF-8     && rm -rf /var/lib/apt/lists/*
# Wed, 26 Apr 2023 19:23:33 GMT
ENV JAVA_VERSION=jdk-17.0.7+7
# Wed, 26 Apr 2023 19:26:07 GMT
RUN set -eux;     ARCH="$(dpkg --print-architecture)";     case "${ARCH}" in        aarch64|arm64)          ESUM='2ff6a4fd1fa354047c93ba8c3179967156162f27bd683aee1f6e52a480bcbe6a';          BINARY_URL='https://github.com/adoptium/temurin17-binaries/releases/download/jdk-17.0.7%2B7/OpenJDK17U-jre_aarch64_linux_hotspot_17.0.7_7.tar.gz';          ;;        armhf|arm)          ESUM='5b0401199c7c9163b8395ebf25195ed395fec7b7ef7158c36302420cf993825a';          BINARY_URL='https://github.com/adoptium/temurin17-binaries/releases/download/jdk-17.0.7%2B7/OpenJDK17U-jre_arm_linux_hotspot_17.0.7_7.tar.gz';          ;;        ppc64el|powerpc:common64)          ESUM='cc25e74c0817cd4d943bba056b256b86e0e9148bf41d7600c5ec2e1eadb2e470';          BINARY_URL='https://github.com/adoptium/temurin17-binaries/releases/download/jdk-17.0.7%2B7/OpenJDK17U-jre_ppc64le_linux_hotspot_17.0.7_7.tar.gz';          ;;        s390x|s390:64-bit)          ESUM='393f6348c6c0cb12699565cf23a7617fbfce973e6d47584a0920e99fbb1b1e3e';          BINARY_URL='https://github.com/adoptium/temurin17-binaries/releases/download/jdk-17.0.7%2B7/OpenJDK17U-jre_s390x_linux_hotspot_17.0.7_7.tar.gz';          ;;        amd64|i386:x86-64)          ESUM='bb025133b96266f6415d5084bb9b260340a813968007f1d2d14690f20bd021ca';          BINARY_URL='https://github.com/adoptium/temurin17-binaries/releases/download/jdk-17.0.7%2B7/OpenJDK17U-jre_x64_linux_hotspot_17.0.7_7.tar.gz';          ;;        *)          echo "Unsupported arch: ${ARCH}";          exit 1;          ;;     esac; 	  wget -O /tmp/openjdk.tar.gz ${BINARY_URL}; 	  echo "${ESUM} */tmp/openjdk.tar.gz" | sha256sum -c -; 	  mkdir -p "$JAVA_HOME"; 	  tar --extract 	      --file /tmp/openjdk.tar.gz 	      --directory "$JAVA_HOME" 	      --strip-components 1 	      --no-same-owner 	  ;     rm -f /tmp/openjdk.tar.gz ${JAVA_HOME}/src.zip;     find "$JAVA_HOME/lib" -name '*.so' -exec dirname '{}' ';' | sort -u > /etc/ld.so.conf.d/docker-openjdk.conf;     ldconfig;     java -Xshare:dump;
# Wed, 26 Apr 2023 19:26:14 GMT
RUN echo Verifying install ...     && fileEncoding="$(echo 'System.out.println(System.getProperty("file.encoding"))' | jshell -s -)"; [ "$fileEncoding" = 'UTF-8' ]; rm -rf ~/.java     && echo java --version && java --version     && echo Complete.
# Wed, 26 Apr 2023 20:47:46 GMT
ENV CATALINA_HOME=/usr/local/tomcat
# Wed, 26 Apr 2023 20:47:46 GMT
ENV PATH=/usr/local/tomcat/bin:/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 26 Apr 2023 20:47:47 GMT
RUN mkdir -p "$CATALINA_HOME"
# Wed, 26 Apr 2023 20:47:48 GMT
WORKDIR /usr/local/tomcat
# Wed, 26 Apr 2023 20:47:48 GMT
ENV TOMCAT_NATIVE_LIBDIR=/usr/local/tomcat/native-jni-lib
# Wed, 26 Apr 2023 20:47:48 GMT
ENV LD_LIBRARY_PATH=/usr/local/tomcat/native-jni-lib
# Wed, 26 Apr 2023 20:49:17 GMT
ENV GPG_KEYS=5C3C5F3E314C866292F359A8F3AD5C94A67F707E A9C5DF4D22E99998D9875A5110C01C5A2F6059E7
# Wed, 26 Apr 2023 20:49:17 GMT
ENV TOMCAT_MAJOR=10
# Wed, 26 Apr 2023 20:49:18 GMT
ENV TOMCAT_VERSION=10.1.8
# Wed, 26 Apr 2023 20:49:18 GMT
ENV TOMCAT_SHA512=bf1a80582d3fc6e7e32c8b72f6b9c2703d39832a8a337f660b8c201196a555c717647825b495169bef61845a1905507b10d62c2d76dfd8ca180bcd49e44d0d5e
# Wed, 03 May 2023 17:09:10 GMT
COPY dir:9385b0b1c0ab3858d081b53c773be8161f138e683502a8321b6f27fe7dd61cf8 in /usr/local/tomcat 
# Wed, 03 May 2023 17:09:23 GMT
RUN set -eux; 	apt-get update; 	xargs -rt apt-get install -y --no-install-recommends < "$TOMCAT_NATIVE_LIBDIR/.dependencies.txt"; 	rm -rf /var/lib/apt/lists/*
# Wed, 03 May 2023 17:09:28 GMT
RUN set -eux; 	nativeLines="$(catalina.sh configtest 2>&1)"; 	nativeLines="$(echo "$nativeLines" | grep 'Apache Tomcat Native')"; 	nativeLines="$(echo "$nativeLines" | sort -u)"; 	if ! echo "$nativeLines" | grep -E 'INFO: Loaded( APR based)? Apache Tomcat Native library' >&2; then 		echo >&2 "$nativeLines"; 		exit 1; 	fi
# Wed, 03 May 2023 17:09:31 GMT
EXPOSE 8080
# Wed, 03 May 2023 17:09:31 GMT
CMD ["catalina.sh" "run"]
```

-	Layers:
	-	`sha256:deffc758660db3b0ee7a1f211d720633f06f27ab1e4c31db4caf8c27f4a80eeb`  
		Last Modified: Thu, 16 Mar 2023 02:22:27 GMT  
		Size: 35.7 MB (35711728 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:13c06c33e4689e5957d961321ac18da32bea369d2eccc9173c9ad8b517f802ea`  
		Last Modified: Thu, 16 Mar 2023 04:14:09 GMT  
		Size: 18.3 MB (18257665 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:25abdd535a180a29cc8edf36ac17eb237551826124456d77040e4d464bceb120`  
		Last Modified: Wed, 26 Apr 2023 19:37:08 GMT  
		Size: 46.9 MB (46872523 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:be9532e0e54e3616e367a6095c24ff50105415ae0333e1fabc59c04be22f053e`  
		Last Modified: Wed, 26 Apr 2023 19:36:55 GMT  
		Size: 162.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4278acb36120c4587941dc129a702188534e2f62875fb279be8ccf0f89711442`  
		Last Modified: Wed, 26 Apr 2023 21:13:21 GMT  
		Size: 173.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:da8900a514020c9d356fd1cae186f08617c71a9dfb1ce011dd8ee309a0d13214`  
		Last Modified: Wed, 03 May 2023 17:44:31 GMT  
		Size: 12.2 MB (12182862 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9f6393a7137920b972f800ccedccd9710cb076c76b0dbbd89e720c59688e0c91`  
		Last Modified: Wed, 03 May 2023 17:44:30 GMT  
		Size: 3.4 MB (3359817 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c12f46a37cea5ca7e964af6c19d82e3e4d7a3e20cfaaeea02b498222d7a53b8f`  
		Last Modified: Wed, 03 May 2023 17:44:29 GMT  
		Size: 130.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `tomcat:jre17-temurin` - linux; s390x

```console
$ docker pull tomcat@sha256:d8a5c480b5a5bf2d08f5189fefcdd7a29bb6111155a932646fd9ace3cea89130
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **104.0 MB (104001988 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:4ffda9b47f64ece56057d91048463bac0a20188c6bede345cb785e9f81d6664b`
-	Default Command: `["catalina.sh","run"]`

```dockerfile
# Wed, 08 Mar 2023 04:39:24 GMT
ARG RELEASE
# Wed, 08 Mar 2023 04:39:24 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Wed, 08 Mar 2023 04:39:24 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Wed, 08 Mar 2023 04:39:24 GMT
LABEL org.opencontainers.image.version=22.04
# Wed, 08 Mar 2023 04:39:26 GMT
ADD file:630f9865d3d4fd4294d45cac7cbaea83fb549c2e563de454348da964d19fbbba in / 
# Wed, 08 Mar 2023 04:39:26 GMT
CMD ["/bin/bash"]
# Thu, 16 Mar 2023 02:06:17 GMT
ENV JAVA_HOME=/opt/java/openjdk
# Thu, 16 Mar 2023 02:06:17 GMT
ENV PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 16 Mar 2023 02:06:17 GMT
ENV LANG=en_US.UTF-8 LANGUAGE=en_US:en LC_ALL=en_US.UTF-8
# Thu, 16 Mar 2023 02:07:58 GMT
RUN apt-get update     && DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends tzdata curl wget ca-certificates fontconfig locales binutils     && echo "en_US.UTF-8 UTF-8" >> /etc/locale.gen     && locale-gen en_US.UTF-8     && rm -rf /var/lib/apt/lists/*
# Wed, 26 Apr 2023 19:43:50 GMT
ENV JAVA_VERSION=jdk-17.0.7+7
# Wed, 26 Apr 2023 19:44:49 GMT
RUN set -eux;     ARCH="$(dpkg --print-architecture)";     case "${ARCH}" in        aarch64|arm64)          ESUM='2ff6a4fd1fa354047c93ba8c3179967156162f27bd683aee1f6e52a480bcbe6a';          BINARY_URL='https://github.com/adoptium/temurin17-binaries/releases/download/jdk-17.0.7%2B7/OpenJDK17U-jre_aarch64_linux_hotspot_17.0.7_7.tar.gz';          ;;        armhf|arm)          ESUM='5b0401199c7c9163b8395ebf25195ed395fec7b7ef7158c36302420cf993825a';          BINARY_URL='https://github.com/adoptium/temurin17-binaries/releases/download/jdk-17.0.7%2B7/OpenJDK17U-jre_arm_linux_hotspot_17.0.7_7.tar.gz';          ;;        ppc64el|powerpc:common64)          ESUM='cc25e74c0817cd4d943bba056b256b86e0e9148bf41d7600c5ec2e1eadb2e470';          BINARY_URL='https://github.com/adoptium/temurin17-binaries/releases/download/jdk-17.0.7%2B7/OpenJDK17U-jre_ppc64le_linux_hotspot_17.0.7_7.tar.gz';          ;;        s390x|s390:64-bit)          ESUM='393f6348c6c0cb12699565cf23a7617fbfce973e6d47584a0920e99fbb1b1e3e';          BINARY_URL='https://github.com/adoptium/temurin17-binaries/releases/download/jdk-17.0.7%2B7/OpenJDK17U-jre_s390x_linux_hotspot_17.0.7_7.tar.gz';          ;;        amd64|i386:x86-64)          ESUM='bb025133b96266f6415d5084bb9b260340a813968007f1d2d14690f20bd021ca';          BINARY_URL='https://github.com/adoptium/temurin17-binaries/releases/download/jdk-17.0.7%2B7/OpenJDK17U-jre_x64_linux_hotspot_17.0.7_7.tar.gz';          ;;        *)          echo "Unsupported arch: ${ARCH}";          exit 1;          ;;     esac; 	  wget -O /tmp/openjdk.tar.gz ${BINARY_URL}; 	  echo "${ESUM} */tmp/openjdk.tar.gz" | sha256sum -c -; 	  mkdir -p "$JAVA_HOME"; 	  tar --extract 	      --file /tmp/openjdk.tar.gz 	      --directory "$JAVA_HOME" 	      --strip-components 1 	      --no-same-owner 	  ;     rm -f /tmp/openjdk.tar.gz ${JAVA_HOME}/src.zip;     find "$JAVA_HOME/lib" -name '*.so' -exec dirname '{}' ';' | sort -u > /etc/ld.so.conf.d/docker-openjdk.conf;     ldconfig;     java -Xshare:dump;
# Wed, 26 Apr 2023 19:44:51 GMT
RUN echo Verifying install ...     && fileEncoding="$(echo 'System.out.println(System.getProperty("file.encoding"))' | jshell -s -)"; [ "$fileEncoding" = 'UTF-8' ]; rm -rf ~/.java     && echo java --version && java --version     && echo Complete.
# Wed, 26 Apr 2023 20:19:20 GMT
ENV CATALINA_HOME=/usr/local/tomcat
# Wed, 26 Apr 2023 20:19:20 GMT
ENV PATH=/usr/local/tomcat/bin:/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 26 Apr 2023 20:19:20 GMT
RUN mkdir -p "$CATALINA_HOME"
# Wed, 26 Apr 2023 20:19:20 GMT
WORKDIR /usr/local/tomcat
# Wed, 26 Apr 2023 20:19:20 GMT
ENV TOMCAT_NATIVE_LIBDIR=/usr/local/tomcat/native-jni-lib
# Wed, 26 Apr 2023 20:19:20 GMT
ENV LD_LIBRARY_PATH=/usr/local/tomcat/native-jni-lib
# Wed, 26 Apr 2023 20:20:01 GMT
ENV GPG_KEYS=5C3C5F3E314C866292F359A8F3AD5C94A67F707E A9C5DF4D22E99998D9875A5110C01C5A2F6059E7
# Wed, 26 Apr 2023 20:20:01 GMT
ENV TOMCAT_MAJOR=10
# Wed, 26 Apr 2023 20:20:01 GMT
ENV TOMCAT_VERSION=10.1.8
# Wed, 26 Apr 2023 20:20:01 GMT
ENV TOMCAT_SHA512=bf1a80582d3fc6e7e32c8b72f6b9c2703d39832a8a337f660b8c201196a555c717647825b495169bef61845a1905507b10d62c2d76dfd8ca180bcd49e44d0d5e
# Wed, 03 May 2023 18:26:24 GMT
COPY dir:d575dce7bc0065edf6e50b4e8fd8398971b73a62bd074eb508c3831309a59baa in /usr/local/tomcat 
# Wed, 03 May 2023 18:26:28 GMT
RUN set -eux; 	apt-get update; 	xargs -rt apt-get install -y --no-install-recommends < "$TOMCAT_NATIVE_LIBDIR/.dependencies.txt"; 	rm -rf /var/lib/apt/lists/*
# Wed, 03 May 2023 18:26:29 GMT
RUN set -eux; 	nativeLines="$(catalina.sh configtest 2>&1)"; 	nativeLines="$(echo "$nativeLines" | grep 'Apache Tomcat Native')"; 	nativeLines="$(echo "$nativeLines" | sort -u)"; 	if ! echo "$nativeLines" | grep -E 'INFO: Loaded( APR based)? Apache Tomcat Native library' >&2; then 		echo >&2 "$nativeLines"; 		exit 1; 	fi
# Wed, 03 May 2023 18:26:29 GMT
EXPOSE 8080
# Wed, 03 May 2023 18:26:29 GMT
CMD ["catalina.sh" "run"]
```

-	Layers:
	-	`sha256:2c7366af510b72cc0b3456fb93cfa0bfc76f7d383db5cb315967e7b1ce2e0c42`  
		Last Modified: Thu, 16 Mar 2023 02:02:40 GMT  
		Size: 28.6 MB (28647599 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:83d28ae42a862e9773a02317b5a0eeb71ddfe3a887bb001c8f23a2786c926287`  
		Last Modified: Thu, 16 Mar 2023 02:13:35 GMT  
		Size: 16.8 MB (16753284 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ed61af6a2c87d412802d8f160fb683fc3ec859e336bfe78f93cdcc31e81a5d1a`  
		Last Modified: Wed, 26 Apr 2023 19:48:14 GMT  
		Size: 43.8 MB (43774584 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1494ca84bd62528d8f5f078978408f8e5d411da7a46a6065b53e647d1149f5e6`  
		Last Modified: Wed, 26 Apr 2023 19:48:08 GMT  
		Size: 160.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:25f669b151066fa2c8dbb21d7d032d86dc90406dc5580802dbae571df6142610`  
		Last Modified: Wed, 26 Apr 2023 20:28:16 GMT  
		Size: 173.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:517f37b160042db00feb52c99195ceaba34ddaeeb49e6661e2175c8c70f46a40`  
		Last Modified: Wed, 03 May 2023 18:35:36 GMT  
		Size: 12.2 MB (12171765 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f3c3cc369df937ec7e154fbec81210a11b48c138824defe035a2b3953d6dd3b5`  
		Last Modified: Wed, 03 May 2023 18:35:35 GMT  
		Size: 2.7 MB (2654293 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6b9a9e6f8618e5542823677348efb5995bbfd75f8ddaaf3665289a14d36b5a4b`  
		Last Modified: Wed, 03 May 2023 18:35:35 GMT  
		Size: 130.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
