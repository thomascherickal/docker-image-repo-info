## `tomcat:9-jre8`

```console
$ docker pull tomcat@sha256:8ef547658d187e543c08aab9686e4c9cf07df6ea65f1278bdcbfe93112c62675
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 4
	-	linux; amd64
	-	linux; arm variant v7
	-	linux; arm64 variant v8
	-	linux; ppc64le

### `tomcat:9-jre8` - linux; amd64

```console
$ docker pull tomcat@sha256:048c46d4bd37e4188c27d1c5fe5c58a363c21d8cdbda1f7ca378d166171f56c6
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **97.4 MB (97354977 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:beec77ca91d8708894fb21da385fd5f35aa61e747a918bb884177b321d9a7d05`
-	Default Command: `["catalina.sh","run"]`

```dockerfile
# Wed, 01 Mar 2023 04:38:47 GMT
ARG RELEASE
# Wed, 01 Mar 2023 04:38:47 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Wed, 01 Mar 2023 04:38:47 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Wed, 01 Mar 2023 04:38:47 GMT
LABEL org.opencontainers.image.version=22.04
# Wed, 01 Mar 2023 04:38:48 GMT
ADD file:fb4c8244f4468cdd3f666932f05805a3882d34010d3a0c14b7c20589bf619a9c in / 
# Wed, 01 Mar 2023 04:38:49 GMT
CMD ["/bin/bash"]
# Thu, 02 Mar 2023 04:01:37 GMT
ENV JAVA_HOME=/opt/java/openjdk
# Thu, 02 Mar 2023 04:01:37 GMT
ENV PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 02 Mar 2023 04:01:37 GMT
ENV LANG=en_US.UTF-8 LANGUAGE=en_US:en LC_ALL=en_US.UTF-8
# Thu, 02 Mar 2023 04:01:51 GMT
RUN apt-get update     && DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends tzdata curl wget ca-certificates fontconfig locales     && echo "en_US.UTF-8 UTF-8" >> /etc/locale.gen     && locale-gen en_US.UTF-8     && rm -rf /var/lib/apt/lists/*
# Thu, 02 Mar 2023 04:01:51 GMT
ENV JAVA_VERSION=jdk8u362-b09
# Thu, 02 Mar 2023 04:02:19 GMT
RUN set -eux;     ARCH="$(dpkg --print-architecture)";     case "${ARCH}" in        aarch64|arm64)          ESUM='cbe45788fa2d9d04d6b10f8aec7dbb15a018dbafe897ed75e31876d0367d56a5';          BINARY_URL='https://github.com/adoptium/temurin8-binaries/releases/download/jdk8u362-b09/OpenJDK8U-jre_aarch64_linux_hotspot_8u362b09.tar.gz';          ;;        armhf|arm)          ESUM='82d8524838b07ee438d42f4c33b6ecfe89ae83efac9af0605c76d75195bdcd99';          BINARY_URL='https://github.com/adoptium/temurin8-binaries/releases/download/jdk8u362-b09/OpenJDK8U-jre_arm_linux_hotspot_8u362b09.tar.gz';          apt-get update          && DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends libatomic1          && rm -rf /var/lib/apt/lists/*          ;;        ppc64el|powerpc:common64)          ESUM='5ec3e07126fedc23b58bb0f5b2dd05b5e9599ce1a3567fc2c7b27587f39faa3b';          BINARY_URL='https://github.com/adoptium/temurin8-binaries/releases/download/jdk8u362-b09/OpenJDK8U-jre_ppc64le_linux_hotspot_8u362b09.tar.gz';          ;;        amd64|i386:x86-64)          ESUM='c8c4e180f915fc7c163240bf363dcdf2b481cd2723fabfc3d08ccf12e049611f';          BINARY_URL='https://github.com/adoptium/temurin8-binaries/releases/download/jdk8u362-b09/OpenJDK8U-jre_x64_linux_hotspot_8u362b09.tar.gz';          ;;        *)          echo "Unsupported arch: ${ARCH}";          exit 1;          ;;     esac; 	  wget -O /tmp/openjdk.tar.gz ${BINARY_URL}; 	  echo "${ESUM} */tmp/openjdk.tar.gz" | sha256sum -c -; 	  mkdir -p "$JAVA_HOME"; 	  tar --extract 	      --file /tmp/openjdk.tar.gz 	      --directory "$JAVA_HOME" 	      --strip-components 1 	      --no-same-owner 	  ;     rm -f /tmp/openjdk.tar.gz ${JAVA_HOME}/src.zip;     find "$JAVA_HOME/lib" -name '*.so' -exec dirname '{}' ';' | sort -u > /etc/ld.so.conf.d/docker-openjdk.conf;     ldconfig;
# Thu, 02 Mar 2023 04:02:19 GMT
RUN echo Verifying install ...     && echo java -version && java -version     && echo Complete.
# Thu, 02 Mar 2023 10:51:28 GMT
ENV CATALINA_HOME=/usr/local/tomcat
# Thu, 02 Mar 2023 10:51:28 GMT
ENV PATH=/usr/local/tomcat/bin:/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 02 Mar 2023 10:51:28 GMT
RUN mkdir -p "$CATALINA_HOME"
# Thu, 02 Mar 2023 10:51:28 GMT
WORKDIR /usr/local/tomcat
# Thu, 02 Mar 2023 10:51:28 GMT
ENV TOMCAT_NATIVE_LIBDIR=/usr/local/tomcat/native-jni-lib
# Thu, 02 Mar 2023 10:51:28 GMT
ENV LD_LIBRARY_PATH=/usr/local/tomcat/native-jni-lib
# Thu, 02 Mar 2023 10:51:29 GMT
ENV GPG_KEYS=48F8E69F6390C9F25CFEDCD268248959359E722B A9C5DF4D22E99998D9875A5110C01C5A2F6059E7 DCFD35E0BF8CA7344752DE8B6FB21E8933C60243
# Thu, 02 Mar 2023 10:51:29 GMT
ENV TOMCAT_MAJOR=9
# Thu, 02 Mar 2023 10:51:29 GMT
ENV TOMCAT_VERSION=9.0.72
# Thu, 02 Mar 2023 10:51:29 GMT
ENV TOMCAT_SHA512=43c8fb109d130035d57e0e942f90ff9447ee0f71d9f1ab816f2ad9dd8b73c14f1457dbd26d50e31e09101b0629543f595a661a11ef0b43b16934e40052f18f4a
# Thu, 02 Mar 2023 10:51:29 GMT
COPY dir:6c10af298b72047c736c8dcf5edbb5d991e8562495f542535fbf168e1d0ed178 in /usr/local/tomcat 
# Thu, 02 Mar 2023 10:51:34 GMT
RUN set -eux; 	apt-get update; 	xargs -rt apt-get install -y --no-install-recommends < "$TOMCAT_NATIVE_LIBDIR/.dependencies.txt"; 	rm -rf /var/lib/apt/lists/*
# Thu, 02 Mar 2023 10:51:36 GMT
RUN set -eux; 	nativeLines="$(catalina.sh configtest 2>&1)"; 	nativeLines="$(echo "$nativeLines" | grep 'Apache Tomcat Native')"; 	nativeLines="$(echo "$nativeLines" | sort -u)"; 	if ! echo "$nativeLines" | grep -E 'INFO: Loaded( APR based)? Apache Tomcat Native library' >&2; then 		echo >&2 "$nativeLines"; 		exit 1; 	fi
# Thu, 02 Mar 2023 10:51:36 GMT
EXPOSE 8080
# Thu, 02 Mar 2023 10:51:36 GMT
CMD ["catalina.sh" "run"]
```

-	Layers:
	-	`sha256:b65bcf19d1445822c0d6f15ea82c9ed82ac1d903cfd6c1284ba7b2409a092845`  
		Last Modified: Wed, 01 Mar 2023 09:07:16 GMT  
		Size: 30.4 MB (30430002 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9e3e3d5d30a242b64d6ee4089176f1459cdfe9d3aeb58e2114cc14b420ad71e5`  
		Last Modified: Thu, 02 Mar 2023 04:07:58 GMT  
		Size: 12.4 MB (12432173 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:be66b727d0420bf9ca0a1c4ea43efad105c7cf92d3477ec2be1d236b4c30ea1a`  
		Last Modified: Thu, 02 Mar 2023 04:08:35 GMT  
		Size: 41.8 MB (41823540 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:161f5bd3c987cb3d2ac3105d736dd5e93d631263049c691cd1720f3cf164eace`  
		Last Modified: Thu, 02 Mar 2023 04:08:29 GMT  
		Size: 159.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8e304a3a395480af685dfffb5fab5e891ffcfa8716bdad673c5361ebc7dd6500`  
		Last Modified: Thu, 02 Mar 2023 11:07:17 GMT  
		Size: 172.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:32638e866f63985234e2db9f26c4094dcebc9ca99224b024a98b4b14abb9cce8`  
		Last Modified: Thu, 02 Mar 2023 11:07:18 GMT  
		Size: 12.2 MB (12214666 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:59e4430e2f5736726cbb0f6ea75883c68e86d2af6ddde316351c0cb918178038`  
		Last Modified: Thu, 02 Mar 2023 11:07:18 GMT  
		Size: 454.1 KB (454135 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ebae68dbbc790086d33cdd51a84f1fd3120a19781e2cb254714ad85c2d98e530`  
		Last Modified: Thu, 02 Mar 2023 11:07:17 GMT  
		Size: 130.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `tomcat:9-jre8` - linux; arm variant v7

```console
$ docker pull tomcat@sha256:1929160475a71f8eea76d3c3a65716cde2a711af5daa97f1f6b25ca016f25c7a
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **91.1 MB (91137613 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:806d6295dea5fd1f3ae9e537c97a79fee2e2899726b5e32d40a88568b1ca63af`
-	Default Command: `["catalina.sh","run"]`

```dockerfile
# Wed, 01 Mar 2023 04:45:54 GMT
ARG RELEASE
# Wed, 01 Mar 2023 04:45:54 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Wed, 01 Mar 2023 04:45:54 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Wed, 01 Mar 2023 04:45:54 GMT
LABEL org.opencontainers.image.version=22.04
# Wed, 01 Mar 2023 04:45:58 GMT
ADD file:d8e0c2340f91ec5973c8459c1a917be69f6530fe7f88da02eb5b4dd562c31730 in / 
# Wed, 01 Mar 2023 04:45:59 GMT
CMD ["/bin/bash"]
# Thu, 02 Mar 2023 10:59:46 GMT
ENV JAVA_HOME=/opt/java/openjdk
# Thu, 02 Mar 2023 10:59:46 GMT
ENV PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 02 Mar 2023 10:59:46 GMT
ENV LANG=en_US.UTF-8 LANGUAGE=en_US:en LC_ALL=en_US.UTF-8
# Thu, 02 Mar 2023 11:00:29 GMT
RUN apt-get update     && DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends tzdata curl wget ca-certificates fontconfig locales     && echo "en_US.UTF-8 UTF-8" >> /etc/locale.gen     && locale-gen en_US.UTF-8     && rm -rf /var/lib/apt/lists/*
# Thu, 02 Mar 2023 11:00:29 GMT
ENV JAVA_VERSION=jdk8u362-b09
# Thu, 02 Mar 2023 11:01:04 GMT
RUN set -eux;     ARCH="$(dpkg --print-architecture)";     case "${ARCH}" in        aarch64|arm64)          ESUM='cbe45788fa2d9d04d6b10f8aec7dbb15a018dbafe897ed75e31876d0367d56a5';          BINARY_URL='https://github.com/adoptium/temurin8-binaries/releases/download/jdk8u362-b09/OpenJDK8U-jre_aarch64_linux_hotspot_8u362b09.tar.gz';          ;;        armhf|arm)          ESUM='82d8524838b07ee438d42f4c33b6ecfe89ae83efac9af0605c76d75195bdcd99';          BINARY_URL='https://github.com/adoptium/temurin8-binaries/releases/download/jdk8u362-b09/OpenJDK8U-jre_arm_linux_hotspot_8u362b09.tar.gz';          apt-get update          && DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends libatomic1          && rm -rf /var/lib/apt/lists/*          ;;        ppc64el|powerpc:common64)          ESUM='5ec3e07126fedc23b58bb0f5b2dd05b5e9599ce1a3567fc2c7b27587f39faa3b';          BINARY_URL='https://github.com/adoptium/temurin8-binaries/releases/download/jdk8u362-b09/OpenJDK8U-jre_ppc64le_linux_hotspot_8u362b09.tar.gz';          ;;        amd64|i386:x86-64)          ESUM='c8c4e180f915fc7c163240bf363dcdf2b481cd2723fabfc3d08ccf12e049611f';          BINARY_URL='https://github.com/adoptium/temurin8-binaries/releases/download/jdk8u362-b09/OpenJDK8U-jre_x64_linux_hotspot_8u362b09.tar.gz';          ;;        *)          echo "Unsupported arch: ${ARCH}";          exit 1;          ;;     esac; 	  wget -O /tmp/openjdk.tar.gz ${BINARY_URL}; 	  echo "${ESUM} */tmp/openjdk.tar.gz" | sha256sum -c -; 	  mkdir -p "$JAVA_HOME"; 	  tar --extract 	      --file /tmp/openjdk.tar.gz 	      --directory "$JAVA_HOME" 	      --strip-components 1 	      --no-same-owner 	  ;     rm -f /tmp/openjdk.tar.gz ${JAVA_HOME}/src.zip;     find "$JAVA_HOME/lib" -name '*.so' -exec dirname '{}' ';' | sort -u > /etc/ld.so.conf.d/docker-openjdk.conf;     ldconfig;
# Thu, 02 Mar 2023 11:01:05 GMT
RUN echo Verifying install ...     && echo java -version && java -version     && echo Complete.
# Thu, 02 Mar 2023 13:03:02 GMT
ENV CATALINA_HOME=/usr/local/tomcat
# Thu, 02 Mar 2023 13:03:02 GMT
ENV PATH=/usr/local/tomcat/bin:/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 02 Mar 2023 13:03:02 GMT
RUN mkdir -p "$CATALINA_HOME"
# Thu, 02 Mar 2023 13:03:02 GMT
WORKDIR /usr/local/tomcat
# Thu, 02 Mar 2023 13:03:02 GMT
ENV TOMCAT_NATIVE_LIBDIR=/usr/local/tomcat/native-jni-lib
# Thu, 02 Mar 2023 13:03:02 GMT
ENV LD_LIBRARY_PATH=/usr/local/tomcat/native-jni-lib
# Thu, 02 Mar 2023 13:03:02 GMT
ENV GPG_KEYS=48F8E69F6390C9F25CFEDCD268248959359E722B A9C5DF4D22E99998D9875A5110C01C5A2F6059E7 DCFD35E0BF8CA7344752DE8B6FB21E8933C60243
# Thu, 02 Mar 2023 13:03:03 GMT
ENV TOMCAT_MAJOR=9
# Thu, 02 Mar 2023 13:03:03 GMT
ENV TOMCAT_VERSION=9.0.72
# Thu, 02 Mar 2023 13:03:03 GMT
ENV TOMCAT_SHA512=43c8fb109d130035d57e0e942f90ff9447ee0f71d9f1ab816f2ad9dd8b73c14f1457dbd26d50e31e09101b0629543f595a661a11ef0b43b16934e40052f18f4a
# Thu, 02 Mar 2023 13:03:03 GMT
COPY dir:48fcb64f610ede18fcda89086e9145856a283435da667bf9adbe147e9c005283 in /usr/local/tomcat 
# Thu, 02 Mar 2023 13:03:07 GMT
RUN set -eux; 	apt-get update; 	xargs -rt apt-get install -y --no-install-recommends < "$TOMCAT_NATIVE_LIBDIR/.dependencies.txt"; 	rm -rf /var/lib/apt/lists/*
# Thu, 02 Mar 2023 13:03:09 GMT
RUN set -eux; 	nativeLines="$(catalina.sh configtest 2>&1)"; 	nativeLines="$(echo "$nativeLines" | grep 'Apache Tomcat Native')"; 	nativeLines="$(echo "$nativeLines" | sort -u)"; 	if ! echo "$nativeLines" | grep -E 'INFO: Loaded( APR based)? Apache Tomcat Native library' >&2; then 		echo >&2 "$nativeLines"; 		exit 1; 	fi
# Thu, 02 Mar 2023 13:03:09 GMT
EXPOSE 8080
# Thu, 02 Mar 2023 13:03:09 GMT
CMD ["catalina.sh" "run"]
```

-	Layers:
	-	`sha256:5909c79a6169dfa05f978dbe7f8dfeadbb92a0d4a3a4d792314b3afe271dd793`  
		Last Modified: Wed, 01 Mar 2023 08:59:31 GMT  
		Size: 27.0 MB (27024489 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6d7f8907def135ff9e4431f5006bfdfd54de1a11b40a6400a2ba91bc407d9d89`  
		Last Modified: Thu, 02 Mar 2023 11:07:07 GMT  
		Size: 12.0 MB (11993099 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:80e8029b7ad79b9c65b1253cb18c2013c20671e9684c7231a7ea4f2ab8ff42be`  
		Last Modified: Thu, 02 Mar 2023 11:07:44 GMT  
		Size: 39.5 MB (39544857 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9de267807999c9bb7af883e36e3899339db25f79cb7924017fdb2526f210ae9b`  
		Last Modified: Thu, 02 Mar 2023 11:07:39 GMT  
		Size: 159.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8b8bb6e71a33028f4518abe2f8c83c8836085e82a6ea14ae660955a66d97529f`  
		Last Modified: Thu, 02 Mar 2023 13:25:40 GMT  
		Size: 174.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:788851e16c13c0151ec8c6a0da06ca14d4814d6f06d9427f6c5b2f750f1b7e24`  
		Last Modified: Thu, 02 Mar 2023 13:25:41 GMT  
		Size: 12.1 MB (12146653 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:df040b43f364254c89fbe9f8bfb421ff72bffce3201786b17a9335d6e4ff8fc7`  
		Last Modified: Thu, 02 Mar 2023 13:25:40 GMT  
		Size: 428.1 KB (428053 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d35615f940b5b9d05b8bd989c86334059aca1fb2e18fe3e2440445106f82e721`  
		Last Modified: Thu, 02 Mar 2023 13:25:40 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `tomcat:9-jre8` - linux; arm64 variant v8

```console
$ docker pull tomcat@sha256:8617f9a5b447fbf0ff3e9d5b92072dffcfe9cc47c0f901039b7e3bebe6eda17d
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **94.3 MB (94260276 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e35df57d46deb9acf87fdd88a7041835e81b63251102023ee40cc200ed388ba3`
-	Default Command: `["catalina.sh","run"]`

```dockerfile
# Wed, 01 Mar 2023 04:47:53 GMT
ARG RELEASE
# Wed, 01 Mar 2023 04:47:53 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Wed, 01 Mar 2023 04:47:54 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Wed, 01 Mar 2023 04:47:54 GMT
LABEL org.opencontainers.image.version=22.04
# Wed, 01 Mar 2023 04:48:01 GMT
ADD file:cf91de9ab30abab112d58c0a7f3bbb35853a02b2e406c65c89430ff049573c47 in / 
# Wed, 01 Mar 2023 04:48:01 GMT
CMD ["/bin/bash"]
# Thu, 02 Mar 2023 04:27:42 GMT
ENV JAVA_HOME=/opt/java/openjdk
# Thu, 02 Mar 2023 04:27:42 GMT
ENV PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 02 Mar 2023 04:27:42 GMT
ENV LANG=en_US.UTF-8 LANGUAGE=en_US:en LC_ALL=en_US.UTF-8
# Thu, 02 Mar 2023 04:27:55 GMT
RUN apt-get update     && DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends tzdata curl wget ca-certificates fontconfig locales     && echo "en_US.UTF-8 UTF-8" >> /etc/locale.gen     && locale-gen en_US.UTF-8     && rm -rf /var/lib/apt/lists/*
# Thu, 02 Mar 2023 04:27:55 GMT
ENV JAVA_VERSION=jdk8u362-b09
# Thu, 02 Mar 2023 04:28:18 GMT
RUN set -eux;     ARCH="$(dpkg --print-architecture)";     case "${ARCH}" in        aarch64|arm64)          ESUM='cbe45788fa2d9d04d6b10f8aec7dbb15a018dbafe897ed75e31876d0367d56a5';          BINARY_URL='https://github.com/adoptium/temurin8-binaries/releases/download/jdk8u362-b09/OpenJDK8U-jre_aarch64_linux_hotspot_8u362b09.tar.gz';          ;;        armhf|arm)          ESUM='82d8524838b07ee438d42f4c33b6ecfe89ae83efac9af0605c76d75195bdcd99';          BINARY_URL='https://github.com/adoptium/temurin8-binaries/releases/download/jdk8u362-b09/OpenJDK8U-jre_arm_linux_hotspot_8u362b09.tar.gz';          apt-get update          && DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends libatomic1          && rm -rf /var/lib/apt/lists/*          ;;        ppc64el|powerpc:common64)          ESUM='5ec3e07126fedc23b58bb0f5b2dd05b5e9599ce1a3567fc2c7b27587f39faa3b';          BINARY_URL='https://github.com/adoptium/temurin8-binaries/releases/download/jdk8u362-b09/OpenJDK8U-jre_ppc64le_linux_hotspot_8u362b09.tar.gz';          ;;        amd64|i386:x86-64)          ESUM='c8c4e180f915fc7c163240bf363dcdf2b481cd2723fabfc3d08ccf12e049611f';          BINARY_URL='https://github.com/adoptium/temurin8-binaries/releases/download/jdk8u362-b09/OpenJDK8U-jre_x64_linux_hotspot_8u362b09.tar.gz';          ;;        *)          echo "Unsupported arch: ${ARCH}";          exit 1;          ;;     esac; 	  wget -O /tmp/openjdk.tar.gz ${BINARY_URL}; 	  echo "${ESUM} */tmp/openjdk.tar.gz" | sha256sum -c -; 	  mkdir -p "$JAVA_HOME"; 	  tar --extract 	      --file /tmp/openjdk.tar.gz 	      --directory "$JAVA_HOME" 	      --strip-components 1 	      --no-same-owner 	  ;     rm -f /tmp/openjdk.tar.gz ${JAVA_HOME}/src.zip;     find "$JAVA_HOME/lib" -name '*.so' -exec dirname '{}' ';' | sort -u > /etc/ld.so.conf.d/docker-openjdk.conf;     ldconfig;
# Thu, 02 Mar 2023 04:28:18 GMT
RUN echo Verifying install ...     && echo java -version && java -version     && echo Complete.
# Thu, 02 Mar 2023 07:48:00 GMT
ENV CATALINA_HOME=/usr/local/tomcat
# Thu, 02 Mar 2023 07:48:00 GMT
ENV PATH=/usr/local/tomcat/bin:/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 02 Mar 2023 07:48:00 GMT
RUN mkdir -p "$CATALINA_HOME"
# Thu, 02 Mar 2023 07:48:00 GMT
WORKDIR /usr/local/tomcat
# Thu, 02 Mar 2023 07:48:00 GMT
ENV TOMCAT_NATIVE_LIBDIR=/usr/local/tomcat/native-jni-lib
# Thu, 02 Mar 2023 07:48:01 GMT
ENV LD_LIBRARY_PATH=/usr/local/tomcat/native-jni-lib
# Thu, 02 Mar 2023 07:48:01 GMT
ENV GPG_KEYS=48F8E69F6390C9F25CFEDCD268248959359E722B A9C5DF4D22E99998D9875A5110C01C5A2F6059E7 DCFD35E0BF8CA7344752DE8B6FB21E8933C60243
# Thu, 02 Mar 2023 07:48:01 GMT
ENV TOMCAT_MAJOR=9
# Thu, 02 Mar 2023 07:48:01 GMT
ENV TOMCAT_VERSION=9.0.72
# Thu, 02 Mar 2023 07:48:01 GMT
ENV TOMCAT_SHA512=43c8fb109d130035d57e0e942f90ff9447ee0f71d9f1ab816f2ad9dd8b73c14f1457dbd26d50e31e09101b0629543f595a661a11ef0b43b16934e40052f18f4a
# Thu, 02 Mar 2023 07:48:01 GMT
COPY dir:77d7400dd0b7338ca531c7b1e588e9e36704caf98c0c284e29950790a1bdccf1 in /usr/local/tomcat 
# Thu, 02 Mar 2023 07:48:05 GMT
RUN set -eux; 	apt-get update; 	xargs -rt apt-get install -y --no-install-recommends < "$TOMCAT_NATIVE_LIBDIR/.dependencies.txt"; 	rm -rf /var/lib/apt/lists/*
# Thu, 02 Mar 2023 07:48:06 GMT
RUN set -eux; 	nativeLines="$(catalina.sh configtest 2>&1)"; 	nativeLines="$(echo "$nativeLines" | grep 'Apache Tomcat Native')"; 	nativeLines="$(echo "$nativeLines" | sort -u)"; 	if ! echo "$nativeLines" | grep -E 'INFO: Loaded( APR based)? Apache Tomcat Native library' >&2; then 		echo >&2 "$nativeLines"; 		exit 1; 	fi
# Thu, 02 Mar 2023 07:48:06 GMT
EXPOSE 8080
# Thu, 02 Mar 2023 07:48:06 GMT
CMD ["catalina.sh" "run"]
```

-	Layers:
	-	`sha256:986c4f6be3072d9528a459c780295bd053806536d2295a6de6aad327eaf19fad`  
		Last Modified: Wed, 01 Mar 2023 09:02:52 GMT  
		Size: 28.4 MB (28387922 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:219ba20309dcd99cff3a43c2f3c01df9170ee1fe02df71ead98cfcef30b9c450`  
		Last Modified: Thu, 02 Mar 2023 04:33:24 GMT  
		Size: 12.4 MB (12390219 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:591a50343e8681bd502ff222aecd18d8abefa72d3e7b924186d2591cb3c93c28`  
		Last Modified: Thu, 02 Mar 2023 04:33:56 GMT  
		Size: 40.8 MB (40807778 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ee122a13c2df69f7adef6234e639c81b9eb2cac7e112d9250634ea111c5be448`  
		Last Modified: Thu, 02 Mar 2023 04:33:52 GMT  
		Size: 161.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:48e74561ae1d8beafbd2adb8cca142b82d73349dfe9059fa3b88a564a6449c49`  
		Last Modified: Thu, 02 Mar 2023 08:02:58 GMT  
		Size: 172.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b6a6d5794abac464ad791cefb103bac308623701c85974b47b8f252cd252fef8`  
		Last Modified: Thu, 02 Mar 2023 08:02:59 GMT  
		Size: 12.2 MB (12220239 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ae8dcfd3b009e3cb14e4bf0773cce7c40e1319fbf6c15f8adeb06503ce91fb66`  
		Last Modified: Thu, 02 Mar 2023 08:02:59 GMT  
		Size: 453.7 KB (453655 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5a8843a6236a89597a7caf1df28ff76cdb4a231f7fbfa60364f9d666c3f74289`  
		Last Modified: Thu, 02 Mar 2023 08:02:58 GMT  
		Size: 130.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `tomcat:9-jre8` - linux; ppc64le

```console
$ docker pull tomcat@sha256:085a81d94536df9383221aac2f3d07ad779c8dd38446f5b7236a060d57c1c313
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **102.9 MB (102901150 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:2879f7da7cd6f0a14a20e198d7af810814fbb6e8a9daf79be5f943fb32edb1bf`
-	Default Command: `["catalina.sh","run"]`

```dockerfile
# Wed, 01 Mar 2023 05:09:57 GMT
ARG RELEASE
# Wed, 01 Mar 2023 05:09:57 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Wed, 01 Mar 2023 05:09:57 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Wed, 01 Mar 2023 05:09:57 GMT
LABEL org.opencontainers.image.version=22.04
# Wed, 01 Mar 2023 05:10:01 GMT
ADD file:e4d45fbda8cf3ca1613a11d2b929670e0e12b43c66818636afa9ebcbf6b48b59 in / 
# Wed, 01 Mar 2023 05:10:01 GMT
CMD ["/bin/bash"]
# Thu, 02 Mar 2023 04:04:52 GMT
ENV JAVA_HOME=/opt/java/openjdk
# Thu, 02 Mar 2023 04:04:52 GMT
ENV PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 02 Mar 2023 04:04:53 GMT
ENV LANG=en_US.UTF-8 LANGUAGE=en_US:en LC_ALL=en_US.UTF-8
# Thu, 02 Mar 2023 04:05:37 GMT
RUN apt-get update     && DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends tzdata curl wget ca-certificates fontconfig locales     && echo "en_US.UTF-8 UTF-8" >> /etc/locale.gen     && locale-gen en_US.UTF-8     && rm -rf /var/lib/apt/lists/*
# Thu, 02 Mar 2023 04:05:38 GMT
ENV JAVA_VERSION=jdk8u362-b09
# Thu, 02 Mar 2023 04:06:32 GMT
RUN set -eux;     ARCH="$(dpkg --print-architecture)";     case "${ARCH}" in        aarch64|arm64)          ESUM='cbe45788fa2d9d04d6b10f8aec7dbb15a018dbafe897ed75e31876d0367d56a5';          BINARY_URL='https://github.com/adoptium/temurin8-binaries/releases/download/jdk8u362-b09/OpenJDK8U-jre_aarch64_linux_hotspot_8u362b09.tar.gz';          ;;        armhf|arm)          ESUM='82d8524838b07ee438d42f4c33b6ecfe89ae83efac9af0605c76d75195bdcd99';          BINARY_URL='https://github.com/adoptium/temurin8-binaries/releases/download/jdk8u362-b09/OpenJDK8U-jre_arm_linux_hotspot_8u362b09.tar.gz';          apt-get update          && DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends libatomic1          && rm -rf /var/lib/apt/lists/*          ;;        ppc64el|powerpc:common64)          ESUM='5ec3e07126fedc23b58bb0f5b2dd05b5e9599ce1a3567fc2c7b27587f39faa3b';          BINARY_URL='https://github.com/adoptium/temurin8-binaries/releases/download/jdk8u362-b09/OpenJDK8U-jre_ppc64le_linux_hotspot_8u362b09.tar.gz';          ;;        amd64|i386:x86-64)          ESUM='c8c4e180f915fc7c163240bf363dcdf2b481cd2723fabfc3d08ccf12e049611f';          BINARY_URL='https://github.com/adoptium/temurin8-binaries/releases/download/jdk8u362-b09/OpenJDK8U-jre_x64_linux_hotspot_8u362b09.tar.gz';          ;;        *)          echo "Unsupported arch: ${ARCH}";          exit 1;          ;;     esac; 	  wget -O /tmp/openjdk.tar.gz ${BINARY_URL}; 	  echo "${ESUM} */tmp/openjdk.tar.gz" | sha256sum -c -; 	  mkdir -p "$JAVA_HOME"; 	  tar --extract 	      --file /tmp/openjdk.tar.gz 	      --directory "$JAVA_HOME" 	      --strip-components 1 	      --no-same-owner 	  ;     rm -f /tmp/openjdk.tar.gz ${JAVA_HOME}/src.zip;     find "$JAVA_HOME/lib" -name '*.so' -exec dirname '{}' ';' | sort -u > /etc/ld.so.conf.d/docker-openjdk.conf;     ldconfig;
# Thu, 02 Mar 2023 04:06:34 GMT
RUN echo Verifying install ...     && echo java -version && java -version     && echo Complete.
# Thu, 02 Mar 2023 06:52:52 GMT
ENV CATALINA_HOME=/usr/local/tomcat
# Thu, 02 Mar 2023 06:52:53 GMT
ENV PATH=/usr/local/tomcat/bin:/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 02 Mar 2023 06:52:55 GMT
RUN mkdir -p "$CATALINA_HOME"
# Thu, 02 Mar 2023 06:52:56 GMT
WORKDIR /usr/local/tomcat
# Thu, 02 Mar 2023 06:52:56 GMT
ENV TOMCAT_NATIVE_LIBDIR=/usr/local/tomcat/native-jni-lib
# Thu, 02 Mar 2023 06:52:56 GMT
ENV LD_LIBRARY_PATH=/usr/local/tomcat/native-jni-lib
# Thu, 02 Mar 2023 06:52:57 GMT
ENV GPG_KEYS=48F8E69F6390C9F25CFEDCD268248959359E722B A9C5DF4D22E99998D9875A5110C01C5A2F6059E7 DCFD35E0BF8CA7344752DE8B6FB21E8933C60243
# Thu, 02 Mar 2023 06:52:58 GMT
ENV TOMCAT_MAJOR=9
# Thu, 02 Mar 2023 06:52:59 GMT
ENV TOMCAT_VERSION=9.0.72
# Thu, 02 Mar 2023 06:53:00 GMT
ENV TOMCAT_SHA512=43c8fb109d130035d57e0e942f90ff9447ee0f71d9f1ab816f2ad9dd8b73c14f1457dbd26d50e31e09101b0629543f595a661a11ef0b43b16934e40052f18f4a
# Thu, 02 Mar 2023 06:53:01 GMT
COPY dir:2abb0ec7b5586e60041bc6f37fe26829aa2c18f3900398efb51ce30046e4b8a1 in /usr/local/tomcat 
# Thu, 02 Mar 2023 06:53:12 GMT
RUN set -eux; 	apt-get update; 	xargs -rt apt-get install -y --no-install-recommends < "$TOMCAT_NATIVE_LIBDIR/.dependencies.txt"; 	rm -rf /var/lib/apt/lists/*
# Thu, 02 Mar 2023 06:53:16 GMT
RUN set -eux; 	nativeLines="$(catalina.sh configtest 2>&1)"; 	nativeLines="$(echo "$nativeLines" | grep 'Apache Tomcat Native')"; 	nativeLines="$(echo "$nativeLines" | sort -u)"; 	if ! echo "$nativeLines" | grep -E 'INFO: Loaded( APR based)? Apache Tomcat Native library' >&2; then 		echo >&2 "$nativeLines"; 		exit 1; 	fi
# Thu, 02 Mar 2023 06:53:16 GMT
EXPOSE 8080
# Thu, 02 Mar 2023 06:53:17 GMT
CMD ["catalina.sh" "run"]
```

-	Layers:
	-	`sha256:062a5dd6f1a8faa2ffa6ca3db2cdb7e930e5f49f52c8647b30709399b759b1cb`  
		Last Modified: Thu, 02 Mar 2023 03:35:30 GMT  
		Size: 35.7 MB (35711589 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:121eddcd73312db262a7816616eb5c5d347769495ce897aef3f86e63aa00c644`  
		Last Modified: Thu, 02 Mar 2023 04:18:05 GMT  
		Size: 13.2 MB (13246165 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6e045a617a4c9940437f09fbd0ca46608d7eb936f75006331388678feee9b350`  
		Last Modified: Thu, 02 Mar 2023 04:18:58 GMT  
		Size: 41.2 MB (41213505 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:43073c451a29c40180d1a4934cd68c663c854ecabc11d5f68b0c119017f67ecf`  
		Last Modified: Thu, 02 Mar 2023 04:18:50 GMT  
		Size: 160.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:863950a6ab34097b2482865f9593e360270ff2f085533971b14760b9e1168520`  
		Last Modified: Thu, 02 Mar 2023 07:27:33 GMT  
		Size: 173.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a1c911ae5709d6670fa193aa1a6845e332206986154d8947b152868b08459a31`  
		Last Modified: Thu, 02 Mar 2023 07:27:35 GMT  
		Size: 12.2 MB (12243855 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:64973a254fdf3e1255bd35a1c5430b32bbc03998d38fd2768bd824d07006c344`  
		Last Modified: Thu, 02 Mar 2023 07:27:33 GMT  
		Size: 485.6 KB (485573 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:63bb95661b9f301f64239e8850f85ff47d3d5d0f86161df291c23d19752ddfba`  
		Last Modified: Thu, 02 Mar 2023 07:27:33 GMT  
		Size: 130.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
