## `tomcat:9-jre8-temurin`

```console
$ docker pull tomcat@sha256:2869ce1cc95616fbb5157d40d24a8c4e1a333d49cc0ac826ed51f0cd407c4699
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 4
	-	linux; amd64
	-	linux; arm variant v7
	-	linux; arm64 variant v8
	-	linux; ppc64le

### `tomcat:9-jre8-temurin` - linux; amd64

```console
$ docker pull tomcat@sha256:9ddf01c48c3522022fa3383c8b4c97ffba7d05933518b15444f4d2d4356a0e53
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **99.9 MB (99864903 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:19eeab0dd0260c46f669c633b5f4324fec66dab7631d715a262cfa8279fafc5b`
-	Default Command: `["catalina.sh","run"]`

```dockerfile
# Thu, 26 Jan 2023 04:57:59 GMT
ARG RELEASE
# Thu, 26 Jan 2023 04:57:59 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Thu, 26 Jan 2023 04:58:00 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Thu, 26 Jan 2023 04:58:00 GMT
LABEL org.opencontainers.image.version=22.04
# Thu, 26 Jan 2023 04:58:02 GMT
ADD file:18e71f049606f6339ce7a995839623f50e6ec6474bfd0a3a7ca799db726f47f6 in / 
# Thu, 26 Jan 2023 04:58:02 GMT
CMD ["/bin/bash"]
# Tue, 31 Jan 2023 20:27:05 GMT
ENV JAVA_HOME=/opt/java/openjdk
# Tue, 31 Jan 2023 20:27:05 GMT
ENV PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 31 Jan 2023 20:27:05 GMT
ENV LANG=en_US.UTF-8 LANGUAGE=en_US:en LC_ALL=en_US.UTF-8
# Tue, 31 Jan 2023 20:27:28 GMT
RUN apt-get update     && DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends tzdata curl wget ca-certificates fontconfig locales     && echo "en_US.UTF-8 UTF-8" >> /etc/locale.gen     && locale-gen en_US.UTF-8     && rm -rf /var/lib/apt/lists/*
# Tue, 31 Jan 2023 20:27:28 GMT
ENV JAVA_VERSION=jdk8u362-b09
# Tue, 31 Jan 2023 20:27:55 GMT
RUN set -eux;     ARCH="$(dpkg --print-architecture)";     case "${ARCH}" in        aarch64|arm64)          ESUM='cbe45788fa2d9d04d6b10f8aec7dbb15a018dbafe897ed75e31876d0367d56a5';          BINARY_URL='https://github.com/adoptium/temurin8-binaries/releases/download/jdk8u362-b09/OpenJDK8U-jre_aarch64_linux_hotspot_8u362b09.tar.gz';          ;;        armhf|arm)          ESUM='82d8524838b07ee438d42f4c33b6ecfe89ae83efac9af0605c76d75195bdcd99';          BINARY_URL='https://github.com/adoptium/temurin8-binaries/releases/download/jdk8u362-b09/OpenJDK8U-jre_arm_linux_hotspot_8u362b09.tar.gz';          apt-get update          && DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends libatomic1          && rm -rf /var/lib/apt/lists/*          ;;        ppc64el|powerpc:common64)          ESUM='5ec3e07126fedc23b58bb0f5b2dd05b5e9599ce1a3567fc2c7b27587f39faa3b';          BINARY_URL='https://github.com/adoptium/temurin8-binaries/releases/download/jdk8u362-b09/OpenJDK8U-jre_ppc64le_linux_hotspot_8u362b09.tar.gz';          ;;        amd64|i386:x86-64)          ESUM='c8c4e180f915fc7c163240bf363dcdf2b481cd2723fabfc3d08ccf12e049611f';          BINARY_URL='https://github.com/adoptium/temurin8-binaries/releases/download/jdk8u362-b09/OpenJDK8U-jre_x64_linux_hotspot_8u362b09.tar.gz';          ;;        *)          echo "Unsupported arch: ${ARCH}";          exit 1;          ;;     esac; 	  wget -O /tmp/openjdk.tar.gz ${BINARY_URL}; 	  echo "${ESUM} */tmp/openjdk.tar.gz" | sha256sum -c -; 	  mkdir -p "$JAVA_HOME"; 	  tar --extract 	      --file /tmp/openjdk.tar.gz 	      --directory "$JAVA_HOME" 	      --strip-components 1 	      --no-same-owner 	  ;     rm -f /tmp/openjdk.tar.gz ${JAVA_HOME}/src.zip;     find "$JAVA_HOME/lib" -name '*.so' -exec dirname '{}' ';' | sort -u > /etc/ld.so.conf.d/docker-openjdk.conf;     ldconfig;
# Tue, 31 Jan 2023 20:27:56 GMT
RUN echo Verifying install ...     && echo java -version && java -version     && echo Complete.
# Wed, 01 Feb 2023 02:45:37 GMT
ENV CATALINA_HOME=/usr/local/tomcat
# Wed, 01 Feb 2023 02:45:37 GMT
ENV PATH=/usr/local/tomcat/bin:/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 01 Feb 2023 02:45:38 GMT
RUN mkdir -p "$CATALINA_HOME"
# Wed, 01 Feb 2023 02:45:38 GMT
WORKDIR /usr/local/tomcat
# Wed, 01 Feb 2023 02:45:38 GMT
ENV TOMCAT_NATIVE_LIBDIR=/usr/local/tomcat/native-jni-lib
# Wed, 01 Feb 2023 02:45:38 GMT
ENV LD_LIBRARY_PATH=/usr/local/tomcat/native-jni-lib
# Wed, 01 Feb 2023 02:45:38 GMT
ENV GPG_KEYS=48F8E69F6390C9F25CFEDCD268248959359E722B A9C5DF4D22E99998D9875A5110C01C5A2F6059E7 DCFD35E0BF8CA7344752DE8B6FB21E8933C60243
# Wed, 01 Feb 2023 02:45:39 GMT
ENV TOMCAT_MAJOR=9
# Sat, 25 Feb 2023 00:50:19 GMT
ENV TOMCAT_VERSION=9.0.72
# Sat, 25 Feb 2023 00:50:19 GMT
ENV TOMCAT_SHA512=43c8fb109d130035d57e0e942f90ff9447ee0f71d9f1ab816f2ad9dd8b73c14f1457dbd26d50e31e09101b0629543f595a661a11ef0b43b16934e40052f18f4a
# Sat, 25 Feb 2023 00:50:19 GMT
COPY dir:ae57570c312ab2f33fb4afb2ed3764ad7879fbb29924972f2eaa99e995de5d69 in /usr/local/tomcat 
# Sat, 25 Feb 2023 00:50:24 GMT
RUN set -eux; 	apt-get update; 	xargs -rt apt-get install -y --no-install-recommends < "$TOMCAT_NATIVE_LIBDIR/.dependencies.txt"; 	rm -rf /var/lib/apt/lists/*
# Sat, 25 Feb 2023 00:50:26 GMT
RUN set -eux; 	nativeLines="$(catalina.sh configtest 2>&1)"; 	nativeLines="$(echo "$nativeLines" | grep 'Apache Tomcat Native')"; 	nativeLines="$(echo "$nativeLines" | sort -u)"; 	if ! echo "$nativeLines" | grep -E 'INFO: Loaded( APR based)? Apache Tomcat Native library' >&2; then 		echo >&2 "$nativeLines"; 		exit 1; 	fi
# Sat, 25 Feb 2023 00:50:26 GMT
EXPOSE 8080
# Sat, 25 Feb 2023 00:50:26 GMT
CMD ["catalina.sh" "run"]
```

-	Layers:
	-	`sha256:10ac4908093d4325f2c94b2c9a571fa1071a17a72dd9c21c1ffb2c86f68ca028`  
		Last Modified: Thu, 26 Jan 2023 08:46:26 GMT  
		Size: 30.4 MB (30429004 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c5b99dc26ba300e0f809f00511dcac6ceb6c9dde4a5c0a7288225868d3a7df21`  
		Last Modified: Tue, 31 Jan 2023 20:33:44 GMT  
		Size: 12.4 MB (12431335 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:116c17a3b264f68996820a7f816c5bb6ef454c707799764c02e8df98152c24d9`  
		Last Modified: Tue, 31 Jan 2023 20:34:20 GMT  
		Size: 41.8 MB (41823534 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1b87b193a7de07f59b50c2019f8269b4589edde682c02941448d02b0195133ed`  
		Last Modified: Tue, 31 Jan 2023 20:34:15 GMT  
		Size: 161.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4024db7a76038e700c0ec0f7c5898c696c528a8ae895188befa455d4c05e8bad`  
		Last Modified: Wed, 01 Feb 2023 03:02:30 GMT  
		Size: 172.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0dfc5894b72b9bae9cec09be1a4aa4c84924a2ffabe2c2ea82927e48772334b6`  
		Last Modified: Sat, 25 Feb 2023 01:10:23 GMT  
		Size: 12.2 MB (12214652 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8d813d342a6c632bbe304e5c63a2a65da5c6e30442d4712d86bc619e28a734a3`  
		Last Modified: Sat, 25 Feb 2023 01:10:22 GMT  
		Size: 3.0 MB (2965914 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:001d30a940d73e840798d0c22eabaa95c4365043e5d222c3f56aa1256cb44f6a`  
		Last Modified: Sat, 25 Feb 2023 01:10:21 GMT  
		Size: 131.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `tomcat:9-jre8-temurin` - linux; arm variant v7

```console
$ docker pull tomcat@sha256:67d65ce29736bc1adc230f1e8a5ced9add86f3b5e114d832b6baab209afec305
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **93.2 MB (93154546 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:353d244b84f905b4ccffbbaa0bf1ca8e5767cbfa073b2e7d73af10127b179038`
-	Default Command: `["catalina.sh","run"]`

```dockerfile
# Thu, 26 Jan 2023 05:05:40 GMT
ARG RELEASE
# Thu, 26 Jan 2023 05:05:40 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Thu, 26 Jan 2023 05:05:40 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Thu, 26 Jan 2023 05:05:40 GMT
LABEL org.opencontainers.image.version=22.04
# Thu, 26 Jan 2023 05:05:43 GMT
ADD file:12d2a7ddc8445b8f97c960075216eb8e8cd226b84259c7343ef15c65a440b500 in / 
# Thu, 26 Jan 2023 05:05:43 GMT
CMD ["/bin/bash"]
# Tue, 31 Jan 2023 18:54:58 GMT
ENV JAVA_HOME=/opt/java/openjdk
# Tue, 31 Jan 2023 18:54:58 GMT
ENV PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 31 Jan 2023 18:54:58 GMT
ENV LANG=en_US.UTF-8 LANGUAGE=en_US:en LC_ALL=en_US.UTF-8
# Tue, 31 Jan 2023 18:55:41 GMT
RUN apt-get update     && DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends tzdata curl wget ca-certificates fontconfig locales     && echo "en_US.UTF-8 UTF-8" >> /etc/locale.gen     && locale-gen en_US.UTF-8     && rm -rf /var/lib/apt/lists/*
# Tue, 31 Jan 2023 18:55:42 GMT
ENV JAVA_VERSION=jdk8u362-b09
# Tue, 31 Jan 2023 18:56:31 GMT
RUN set -eux;     ARCH="$(dpkg --print-architecture)";     case "${ARCH}" in        aarch64|arm64)          ESUM='cbe45788fa2d9d04d6b10f8aec7dbb15a018dbafe897ed75e31876d0367d56a5';          BINARY_URL='https://github.com/adoptium/temurin8-binaries/releases/download/jdk8u362-b09/OpenJDK8U-jre_aarch64_linux_hotspot_8u362b09.tar.gz';          ;;        armhf|arm)          ESUM='82d8524838b07ee438d42f4c33b6ecfe89ae83efac9af0605c76d75195bdcd99';          BINARY_URL='https://github.com/adoptium/temurin8-binaries/releases/download/jdk8u362-b09/OpenJDK8U-jre_arm_linux_hotspot_8u362b09.tar.gz';          apt-get update          && DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends libatomic1          && rm -rf /var/lib/apt/lists/*          ;;        ppc64el|powerpc:common64)          ESUM='5ec3e07126fedc23b58bb0f5b2dd05b5e9599ce1a3567fc2c7b27587f39faa3b';          BINARY_URL='https://github.com/adoptium/temurin8-binaries/releases/download/jdk8u362-b09/OpenJDK8U-jre_ppc64le_linux_hotspot_8u362b09.tar.gz';          ;;        amd64|i386:x86-64)          ESUM='c8c4e180f915fc7c163240bf363dcdf2b481cd2723fabfc3d08ccf12e049611f';          BINARY_URL='https://github.com/adoptium/temurin8-binaries/releases/download/jdk8u362-b09/OpenJDK8U-jre_x64_linux_hotspot_8u362b09.tar.gz';          ;;        *)          echo "Unsupported arch: ${ARCH}";          exit 1;          ;;     esac; 	  wget -O /tmp/openjdk.tar.gz ${BINARY_URL}; 	  echo "${ESUM} */tmp/openjdk.tar.gz" | sha256sum -c -; 	  mkdir -p "$JAVA_HOME"; 	  tar --extract 	      --file /tmp/openjdk.tar.gz 	      --directory "$JAVA_HOME" 	      --strip-components 1 	      --no-same-owner 	  ;     rm -f /tmp/openjdk.tar.gz ${JAVA_HOME}/src.zip;     find "$JAVA_HOME/lib" -name '*.so' -exec dirname '{}' ';' | sort -u > /etc/ld.so.conf.d/docker-openjdk.conf;     ldconfig;
# Tue, 31 Jan 2023 18:56:32 GMT
RUN echo Verifying install ...     && echo java -version && java -version     && echo Complete.
# Sat, 25 Feb 2023 06:07:30 GMT
ENV CATALINA_HOME=/usr/local/tomcat
# Sat, 25 Feb 2023 06:07:30 GMT
ENV PATH=/usr/local/tomcat/bin:/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Sat, 25 Feb 2023 06:07:30 GMT
RUN mkdir -p "$CATALINA_HOME"
# Sat, 25 Feb 2023 06:07:31 GMT
WORKDIR /usr/local/tomcat
# Sat, 25 Feb 2023 06:07:31 GMT
ENV TOMCAT_NATIVE_LIBDIR=/usr/local/tomcat/native-jni-lib
# Sat, 25 Feb 2023 06:07:31 GMT
ENV LD_LIBRARY_PATH=/usr/local/tomcat/native-jni-lib
# Sat, 25 Feb 2023 06:07:31 GMT
ENV GPG_KEYS=48F8E69F6390C9F25CFEDCD268248959359E722B A9C5DF4D22E99998D9875A5110C01C5A2F6059E7 DCFD35E0BF8CA7344752DE8B6FB21E8933C60243
# Sat, 25 Feb 2023 06:07:31 GMT
ENV TOMCAT_MAJOR=9
# Sat, 25 Feb 2023 06:07:31 GMT
ENV TOMCAT_VERSION=9.0.72
# Sat, 25 Feb 2023 06:07:31 GMT
ENV TOMCAT_SHA512=43c8fb109d130035d57e0e942f90ff9447ee0f71d9f1ab816f2ad9dd8b73c14f1457dbd26d50e31e09101b0629543f595a661a11ef0b43b16934e40052f18f4a
# Sat, 25 Feb 2023 06:07:32 GMT
COPY dir:e422adcba4ec68e1494a9ad76815d422828bdc83555e07923841776f4d034bcd in /usr/local/tomcat 
# Sat, 25 Feb 2023 06:07:36 GMT
RUN set -eux; 	apt-get update; 	xargs -rt apt-get install -y --no-install-recommends < "$TOMCAT_NATIVE_LIBDIR/.dependencies.txt"; 	rm -rf /var/lib/apt/lists/*
# Sat, 25 Feb 2023 06:07:37 GMT
RUN set -eux; 	nativeLines="$(catalina.sh configtest 2>&1)"; 	nativeLines="$(echo "$nativeLines" | grep 'Apache Tomcat Native')"; 	nativeLines="$(echo "$nativeLines" | sort -u)"; 	if ! echo "$nativeLines" | grep -E 'INFO: Loaded( APR based)? Apache Tomcat Native library' >&2; then 		echo >&2 "$nativeLines"; 		exit 1; 	fi
# Sat, 25 Feb 2023 06:07:37 GMT
EXPOSE 8080
# Sat, 25 Feb 2023 06:07:37 GMT
CMD ["catalina.sh" "run"]
```

-	Layers:
	-	`sha256:d0210273e3495988f639f6164118a5bba55666799ba86ac3e60a001cf7be3b31`  
		Last Modified: Thu, 26 Jan 2023 18:27:33 GMT  
		Size: 27.0 MB (27022323 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9eb09753c13f1f9b683897d309c55f7a5432a5785ebd23f9231dd98fbb14ee46`  
		Last Modified: Tue, 31 Jan 2023 19:04:18 GMT  
		Size: 12.0 MB (11992694 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4ae677ab7734effc42fe4bc7672d655c86459ed83789631d868f6423cc848623`  
		Last Modified: Tue, 31 Jan 2023 19:04:59 GMT  
		Size: 39.5 MB (39544483 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6736e2a2ad790b8939aef2eaf344ce6a871c91ba0950884d9a629208d68a3654`  
		Last Modified: Tue, 31 Jan 2023 19:04:53 GMT  
		Size: 128.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f9e8a98518381868f48f8f246870767be12bc72fe3e3a744230a2d1249209259`  
		Last Modified: Sat, 25 Feb 2023 06:30:13 GMT  
		Size: 171.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8d38f8892ac64280d25b826781dd55382fb525cc8d6b54fac033de292f03feb3`  
		Last Modified: Sat, 25 Feb 2023 06:30:14 GMT  
		Size: 12.1 MB (12146578 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8c9c44104e39c50879001376b99644b9727b8e42a95c11ca640fa776b9992582`  
		Last Modified: Sat, 25 Feb 2023 06:30:14 GMT  
		Size: 2.4 MB (2448038 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6c923adba290009d32ac1f8fbdbac45cb8e1e2e61b98c3999c9178a9d78a354f`  
		Last Modified: Sat, 25 Feb 2023 06:30:13 GMT  
		Size: 131.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `tomcat:9-jre8-temurin` - linux; arm64 variant v8

```console
$ docker pull tomcat@sha256:2ab89a125d5892eaa42cb4761339c949ca20a90382f4877934c1be36e276e8af
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **96.6 MB (96613844 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:4867e9097e9af2bed0ff8cbdbd25ff1719c6605c4cc2eb7c77daa0d9f29e68d7`
-	Default Command: `["catalina.sh","run"]`

```dockerfile
# Thu, 26 Jan 2023 05:05:49 GMT
ARG RELEASE
# Thu, 26 Jan 2023 05:05:49 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Thu, 26 Jan 2023 05:05:49 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Thu, 26 Jan 2023 05:05:50 GMT
LABEL org.opencontainers.image.version=22.04
# Thu, 26 Jan 2023 05:05:51 GMT
ADD file:55486a91f732042dd4e81ecfd8457d23e04dcd7dd80a0bb06cc7c44873fac838 in / 
# Thu, 26 Jan 2023 05:05:51 GMT
CMD ["/bin/bash"]
# Tue, 31 Jan 2023 17:43:57 GMT
ENV JAVA_HOME=/opt/java/openjdk
# Tue, 31 Jan 2023 17:43:57 GMT
ENV PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 31 Jan 2023 17:43:57 GMT
ENV LANG=en_US.UTF-8 LANGUAGE=en_US:en LC_ALL=en_US.UTF-8
# Tue, 31 Jan 2023 17:44:32 GMT
RUN apt-get update     && DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends tzdata curl wget ca-certificates fontconfig locales     && echo "en_US.UTF-8 UTF-8" >> /etc/locale.gen     && locale-gen en_US.UTF-8     && rm -rf /var/lib/apt/lists/*
# Tue, 31 Jan 2023 17:44:32 GMT
ENV JAVA_VERSION=jdk8u362-b09
# Tue, 31 Jan 2023 17:44:58 GMT
RUN set -eux;     ARCH="$(dpkg --print-architecture)";     case "${ARCH}" in        aarch64|arm64)          ESUM='cbe45788fa2d9d04d6b10f8aec7dbb15a018dbafe897ed75e31876d0367d56a5';          BINARY_URL='https://github.com/adoptium/temurin8-binaries/releases/download/jdk8u362-b09/OpenJDK8U-jre_aarch64_linux_hotspot_8u362b09.tar.gz';          ;;        armhf|arm)          ESUM='82d8524838b07ee438d42f4c33b6ecfe89ae83efac9af0605c76d75195bdcd99';          BINARY_URL='https://github.com/adoptium/temurin8-binaries/releases/download/jdk8u362-b09/OpenJDK8U-jre_arm_linux_hotspot_8u362b09.tar.gz';          apt-get update          && DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends libatomic1          && rm -rf /var/lib/apt/lists/*          ;;        ppc64el|powerpc:common64)          ESUM='5ec3e07126fedc23b58bb0f5b2dd05b5e9599ce1a3567fc2c7b27587f39faa3b';          BINARY_URL='https://github.com/adoptium/temurin8-binaries/releases/download/jdk8u362-b09/OpenJDK8U-jre_ppc64le_linux_hotspot_8u362b09.tar.gz';          ;;        amd64|i386:x86-64)          ESUM='c8c4e180f915fc7c163240bf363dcdf2b481cd2723fabfc3d08ccf12e049611f';          BINARY_URL='https://github.com/adoptium/temurin8-binaries/releases/download/jdk8u362-b09/OpenJDK8U-jre_x64_linux_hotspot_8u362b09.tar.gz';          ;;        *)          echo "Unsupported arch: ${ARCH}";          exit 1;          ;;     esac; 	  wget -O /tmp/openjdk.tar.gz ${BINARY_URL}; 	  echo "${ESUM} */tmp/openjdk.tar.gz" | sha256sum -c -; 	  mkdir -p "$JAVA_HOME"; 	  tar --extract 	      --file /tmp/openjdk.tar.gz 	      --directory "$JAVA_HOME" 	      --strip-components 1 	      --no-same-owner 	  ;     rm -f /tmp/openjdk.tar.gz ${JAVA_HOME}/src.zip;     find "$JAVA_HOME/lib" -name '*.so' -exec dirname '{}' ';' | sort -u > /etc/ld.so.conf.d/docker-openjdk.conf;     ldconfig;
# Tue, 31 Jan 2023 17:44:59 GMT
RUN echo Verifying install ...     && echo java -version && java -version     && echo Complete.
# Tue, 31 Jan 2023 22:17:51 GMT
ENV CATALINA_HOME=/usr/local/tomcat
# Tue, 31 Jan 2023 22:17:51 GMT
ENV PATH=/usr/local/tomcat/bin:/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 31 Jan 2023 22:17:51 GMT
RUN mkdir -p "$CATALINA_HOME"
# Tue, 31 Jan 2023 22:17:52 GMT
WORKDIR /usr/local/tomcat
# Tue, 31 Jan 2023 22:17:52 GMT
ENV TOMCAT_NATIVE_LIBDIR=/usr/local/tomcat/native-jni-lib
# Tue, 31 Jan 2023 22:17:52 GMT
ENV LD_LIBRARY_PATH=/usr/local/tomcat/native-jni-lib
# Tue, 31 Jan 2023 22:17:52 GMT
ENV GPG_KEYS=48F8E69F6390C9F25CFEDCD268248959359E722B A9C5DF4D22E99998D9875A5110C01C5A2F6059E7 DCFD35E0BF8CA7344752DE8B6FB21E8933C60243
# Tue, 31 Jan 2023 22:17:52 GMT
ENV TOMCAT_MAJOR=9
# Sat, 25 Feb 2023 00:15:00 GMT
ENV TOMCAT_VERSION=9.0.72
# Sat, 25 Feb 2023 00:15:00 GMT
ENV TOMCAT_SHA512=43c8fb109d130035d57e0e942f90ff9447ee0f71d9f1ab816f2ad9dd8b73c14f1457dbd26d50e31e09101b0629543f595a661a11ef0b43b16934e40052f18f4a
# Sat, 25 Feb 2023 00:15:00 GMT
COPY dir:ca0ab857b289cd8697890fcba3dde2a958b8388e8c7ef00ee2620266382b1811 in /usr/local/tomcat 
# Sat, 25 Feb 2023 00:15:04 GMT
RUN set -eux; 	apt-get update; 	xargs -rt apt-get install -y --no-install-recommends < "$TOMCAT_NATIVE_LIBDIR/.dependencies.txt"; 	rm -rf /var/lib/apt/lists/*
# Sat, 25 Feb 2023 00:15:06 GMT
RUN set -eux; 	nativeLines="$(catalina.sh configtest 2>&1)"; 	nativeLines="$(echo "$nativeLines" | grep 'Apache Tomcat Native')"; 	nativeLines="$(echo "$nativeLines" | sort -u)"; 	if ! echo "$nativeLines" | grep -E 'INFO: Loaded( APR based)? Apache Tomcat Native library' >&2; then 		echo >&2 "$nativeLines"; 		exit 1; 	fi
# Sat, 25 Feb 2023 00:15:06 GMT
EXPOSE 8080
# Sat, 25 Feb 2023 00:15:06 GMT
CMD ["catalina.sh" "run"]
```

-	Layers:
	-	`sha256:565cb979c5c01279efcd69c4457a9954801b6be6da65894374260ec92d993891`  
		Last Modified: Thu, 26 Jan 2023 16:22:40 GMT  
		Size: 28.4 MB (28384974 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e1c6471d4f305436bdd6e09ea64bdf7a303979f4d8cdb6c9606715fc21afa9ad`  
		Last Modified: Tue, 31 Jan 2023 17:50:26 GMT  
		Size: 12.4 MB (12391264 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9d0dec898a875fc378d2ce3ac7d0168af3e02e277fd627395209667315094cff`  
		Last Modified: Tue, 31 Jan 2023 17:50:59 GMT  
		Size: 40.8 MB (40807793 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3a04f642480a15c275f6fa2fbe854115d13bb23077e4195e066a277041ff9bee`  
		Last Modified: Tue, 31 Jan 2023 17:50:55 GMT  
		Size: 161.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d994113a4199ff1630f097248771aa5c333037e10832653a10878490df63b012`  
		Last Modified: Tue, 31 Jan 2023 22:33:50 GMT  
		Size: 174.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:37bf37a9d71f1b445aeb179ac6aa080bef3face9a5f114c7a237d2b98d9cd88e`  
		Last Modified: Sat, 25 Feb 2023 00:34:39 GMT  
		Size: 12.2 MB (12220284 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2622cdffbc2916226dccec14a4ab29153a36821ade268e4891f146824f893507`  
		Last Modified: Sat, 25 Feb 2023 00:34:39 GMT  
		Size: 2.8 MB (2809064 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f59c0073e9b60d8be57b7b1e120479e410fdd8fca3245c9964bc6c2596be44dc`  
		Last Modified: Sat, 25 Feb 2023 00:34:38 GMT  
		Size: 130.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `tomcat:9-jre8-temurin` - linux; ppc64le

```console
$ docker pull tomcat@sha256:248c96361e1883d1b804c1ff05c50f32495bb4574fb57955ae71bf4222231288
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **105.8 MB (105768576 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:2d3c9e5bb8fd3bda9256bc5bc92d1d7ff4876dd982fb792c1504740dcf033818`
-	Default Command: `["catalina.sh","run"]`

```dockerfile
# Thu, 26 Jan 2023 04:58:24 GMT
ARG RELEASE
# Thu, 26 Jan 2023 04:58:24 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Thu, 26 Jan 2023 04:58:24 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Thu, 26 Jan 2023 04:58:24 GMT
LABEL org.opencontainers.image.version=22.04
# Thu, 26 Jan 2023 04:58:28 GMT
ADD file:f0400001a50847feb579e66e804ec9daaaaeb9a414b4b5cca8bb0c8e9c7fa8f9 in / 
# Thu, 26 Jan 2023 04:58:28 GMT
CMD ["/bin/bash"]
# Tue, 31 Jan 2023 18:22:58 GMT
ENV JAVA_HOME=/opt/java/openjdk
# Tue, 31 Jan 2023 18:22:58 GMT
ENV PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 31 Jan 2023 18:22:59 GMT
ENV LANG=en_US.UTF-8 LANGUAGE=en_US:en LC_ALL=en_US.UTF-8
# Tue, 31 Jan 2023 18:23:22 GMT
RUN apt-get update     && DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends tzdata curl wget ca-certificates fontconfig locales     && echo "en_US.UTF-8 UTF-8" >> /etc/locale.gen     && locale-gen en_US.UTF-8     && rm -rf /var/lib/apt/lists/*
# Tue, 31 Jan 2023 18:23:23 GMT
ENV JAVA_VERSION=jdk8u362-b09
# Tue, 31 Jan 2023 18:24:12 GMT
RUN set -eux;     ARCH="$(dpkg --print-architecture)";     case "${ARCH}" in        aarch64|arm64)          ESUM='cbe45788fa2d9d04d6b10f8aec7dbb15a018dbafe897ed75e31876d0367d56a5';          BINARY_URL='https://github.com/adoptium/temurin8-binaries/releases/download/jdk8u362-b09/OpenJDK8U-jre_aarch64_linux_hotspot_8u362b09.tar.gz';          ;;        armhf|arm)          ESUM='82d8524838b07ee438d42f4c33b6ecfe89ae83efac9af0605c76d75195bdcd99';          BINARY_URL='https://github.com/adoptium/temurin8-binaries/releases/download/jdk8u362-b09/OpenJDK8U-jre_arm_linux_hotspot_8u362b09.tar.gz';          apt-get update          && DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends libatomic1          && rm -rf /var/lib/apt/lists/*          ;;        ppc64el|powerpc:common64)          ESUM='5ec3e07126fedc23b58bb0f5b2dd05b5e9599ce1a3567fc2c7b27587f39faa3b';          BINARY_URL='https://github.com/adoptium/temurin8-binaries/releases/download/jdk8u362-b09/OpenJDK8U-jre_ppc64le_linux_hotspot_8u362b09.tar.gz';          ;;        amd64|i386:x86-64)          ESUM='c8c4e180f915fc7c163240bf363dcdf2b481cd2723fabfc3d08ccf12e049611f';          BINARY_URL='https://github.com/adoptium/temurin8-binaries/releases/download/jdk8u362-b09/OpenJDK8U-jre_x64_linux_hotspot_8u362b09.tar.gz';          ;;        *)          echo "Unsupported arch: ${ARCH}";          exit 1;          ;;     esac; 	  wget -O /tmp/openjdk.tar.gz ${BINARY_URL}; 	  echo "${ESUM} */tmp/openjdk.tar.gz" | sha256sum -c -; 	  mkdir -p "$JAVA_HOME"; 	  tar --extract 	      --file /tmp/openjdk.tar.gz 	      --directory "$JAVA_HOME" 	      --strip-components 1 	      --no-same-owner 	  ;     rm -f /tmp/openjdk.tar.gz ${JAVA_HOME}/src.zip;     find "$JAVA_HOME/lib" -name '*.so' -exec dirname '{}' ';' | sort -u > /etc/ld.so.conf.d/docker-openjdk.conf;     ldconfig;
# Tue, 31 Jan 2023 18:24:14 GMT
RUN echo Verifying install ...     && echo java -version && java -version     && echo Complete.
# Tue, 31 Jan 2023 21:10:07 GMT
ENV CATALINA_HOME=/usr/local/tomcat
# Tue, 31 Jan 2023 21:10:07 GMT
ENV PATH=/usr/local/tomcat/bin:/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 31 Jan 2023 21:10:08 GMT
RUN mkdir -p "$CATALINA_HOME"
# Tue, 31 Jan 2023 21:10:08 GMT
WORKDIR /usr/local/tomcat
# Tue, 31 Jan 2023 21:10:09 GMT
ENV TOMCAT_NATIVE_LIBDIR=/usr/local/tomcat/native-jni-lib
# Tue, 31 Jan 2023 21:10:09 GMT
ENV LD_LIBRARY_PATH=/usr/local/tomcat/native-jni-lib
# Tue, 31 Jan 2023 21:10:09 GMT
ENV GPG_KEYS=48F8E69F6390C9F25CFEDCD268248959359E722B A9C5DF4D22E99998D9875A5110C01C5A2F6059E7 DCFD35E0BF8CA7344752DE8B6FB21E8933C60243
# Tue, 31 Jan 2023 21:10:10 GMT
ENV TOMCAT_MAJOR=9
# Sat, 25 Feb 2023 01:06:29 GMT
ENV TOMCAT_VERSION=9.0.72
# Sat, 25 Feb 2023 01:06:29 GMT
ENV TOMCAT_SHA512=43c8fb109d130035d57e0e942f90ff9447ee0f71d9f1ab816f2ad9dd8b73c14f1457dbd26d50e31e09101b0629543f595a661a11ef0b43b16934e40052f18f4a
# Sat, 25 Feb 2023 01:06:30 GMT
COPY dir:593c96ff3dac192e4b5651ecc7186a443a81c6549a4202a85bfa37892ac5fd17 in /usr/local/tomcat 
# Sat, 25 Feb 2023 01:06:40 GMT
RUN set -eux; 	apt-get update; 	xargs -rt apt-get install -y --no-install-recommends < "$TOMCAT_NATIVE_LIBDIR/.dependencies.txt"; 	rm -rf /var/lib/apt/lists/*
# Sat, 25 Feb 2023 01:06:44 GMT
RUN set -eux; 	nativeLines="$(catalina.sh configtest 2>&1)"; 	nativeLines="$(echo "$nativeLines" | grep 'Apache Tomcat Native')"; 	nativeLines="$(echo "$nativeLines" | sort -u)"; 	if ! echo "$nativeLines" | grep -E 'INFO: Loaded( APR based)? Apache Tomcat Native library' >&2; then 		echo >&2 "$nativeLines"; 		exit 1; 	fi
# Sat, 25 Feb 2023 01:06:44 GMT
EXPOSE 8080
# Sat, 25 Feb 2023 01:06:45 GMT
CMD ["catalina.sh" "run"]
```

-	Layers:
	-	`sha256:b919bd9d6c8a596b3ac4fb9ee1cc6727efdd1f1b05e5c130efec5deaae53ae60`  
		Last Modified: Tue, 31 Jan 2023 17:52:02 GMT  
		Size: 35.7 MB (35708930 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c07cad39c2b79771ce4c5729f09dda98f7002a92d03d36b9fc6cd85658070de0`  
		Last Modified: Tue, 31 Jan 2023 18:35:12 GMT  
		Size: 13.2 MB (13245674 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f33f0850707ee89f22f953201b74d7bd0877147ebbefb55d9edabb51413b82de`  
		Last Modified: Tue, 31 Jan 2023 18:36:07 GMT  
		Size: 41.2 MB (41213517 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e9a0a49bc3bdd7db968764dd8ae8a9700d95a64bc38ed21edbf21f9438cdc920`  
		Last Modified: Tue, 31 Jan 2023 18:35:58 GMT  
		Size: 160.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6d33c292cb43cc161d3aa0b2896a533a398d2d6fc369c9d21ce7686406adc5d3`  
		Last Modified: Tue, 31 Jan 2023 21:38:52 GMT  
		Size: 171.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4387f1370ebdfb82b5e24023327fb36334ca0a6da38e27a3d89e998311ca5f0b`  
		Last Modified: Sat, 25 Feb 2023 01:37:38 GMT  
		Size: 12.2 MB (12243757 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6765ee7ed79542648af206ae08d88a8fa596edfdcf40e19f6b02a82165767a37`  
		Last Modified: Sat, 25 Feb 2023 01:37:37 GMT  
		Size: 3.4 MB (3356236 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:50d135ee198d4191f9cbb3f9175f0ba2dd31950ce3972dd1c4e5249418e45880`  
		Last Modified: Sat, 25 Feb 2023 01:37:36 GMT  
		Size: 131.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
