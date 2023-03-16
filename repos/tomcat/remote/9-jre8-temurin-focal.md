## `tomcat:9-jre8-temurin-focal`

```console
$ docker pull tomcat@sha256:1340f80acbc167c7984b96a3b485da677d6e3147f8a155ce7f3ea3a5d8f50821
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 4
	-	linux; amd64
	-	linux; arm variant v7
	-	linux; arm64 variant v8
	-	linux; ppc64le

### `tomcat:9-jre8-temurin-focal` - linux; amd64

```console
$ docker pull tomcat@sha256:f08637358aa16e352ce890d80151849bbdc453b4260ba59ddcd9e5e13c74dea7
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **99.5 MB (99475482 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:9c4b6c886fbc4bec2dc0c9e728d34f1a9b9088531c78931277f8f4afdd336a14`
-	Default Command: `["catalina.sh","run"]`

```dockerfile
# Wed, 01 Mar 2023 04:53:01 GMT
ARG RELEASE
# Wed, 01 Mar 2023 04:53:01 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Wed, 01 Mar 2023 04:53:01 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Wed, 01 Mar 2023 04:53:02 GMT
LABEL org.opencontainers.image.version=20.04
# Wed, 01 Mar 2023 04:53:03 GMT
ADD file:3478fb5bdcf8ad03d450d48901a6a8452c0ab253f24d21b1e27f99259db2d26b in / 
# Wed, 01 Mar 2023 04:53:04 GMT
CMD ["/bin/bash"]
# Thu, 02 Mar 2023 04:01:09 GMT
ENV JAVA_HOME=/opt/java/openjdk
# Thu, 02 Mar 2023 04:01:09 GMT
ENV PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 02 Mar 2023 04:01:09 GMT
ENV LANG=en_US.UTF-8 LANGUAGE=en_US:en LC_ALL=en_US.UTF-8
# Thu, 02 Mar 2023 04:01:25 GMT
RUN apt-get update     && DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends tzdata curl wget ca-certificates fontconfig locales     && echo "en_US.UTF-8 UTF-8" >> /etc/locale.gen     && locale-gen en_US.UTF-8     && rm -rf /var/lib/apt/lists/*
# Thu, 02 Mar 2023 04:01:25 GMT
ENV JAVA_VERSION=jdk8u362-b09
# Thu, 02 Mar 2023 04:02:12 GMT
RUN set -eux;     ARCH="$(dpkg --print-architecture)";     case "${ARCH}" in        aarch64|arm64)          ESUM='cbe45788fa2d9d04d6b10f8aec7dbb15a018dbafe897ed75e31876d0367d56a5';          BINARY_URL='https://github.com/adoptium/temurin8-binaries/releases/download/jdk8u362-b09/OpenJDK8U-jre_aarch64_linux_hotspot_8u362b09.tar.gz';          ;;        armhf|arm)          ESUM='82d8524838b07ee438d42f4c33b6ecfe89ae83efac9af0605c76d75195bdcd99';          BINARY_URL='https://github.com/adoptium/temurin8-binaries/releases/download/jdk8u362-b09/OpenJDK8U-jre_arm_linux_hotspot_8u362b09.tar.gz';          apt-get update          && DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends libatomic1          && rm -rf /var/lib/apt/lists/*          ;;        ppc64el|powerpc:common64)          ESUM='5ec3e07126fedc23b58bb0f5b2dd05b5e9599ce1a3567fc2c7b27587f39faa3b';          BINARY_URL='https://github.com/adoptium/temurin8-binaries/releases/download/jdk8u362-b09/OpenJDK8U-jre_ppc64le_linux_hotspot_8u362b09.tar.gz';          ;;        amd64|i386:x86-64)          ESUM='c8c4e180f915fc7c163240bf363dcdf2b481cd2723fabfc3d08ccf12e049611f';          BINARY_URL='https://github.com/adoptium/temurin8-binaries/releases/download/jdk8u362-b09/OpenJDK8U-jre_x64_linux_hotspot_8u362b09.tar.gz';          ;;        *)          echo "Unsupported arch: ${ARCH}";          exit 1;          ;;     esac; 	  wget -O /tmp/openjdk.tar.gz ${BINARY_URL}; 	  echo "${ESUM} */tmp/openjdk.tar.gz" | sha256sum -c -; 	  mkdir -p "$JAVA_HOME"; 	  tar --extract 	      --file /tmp/openjdk.tar.gz 	      --directory "$JAVA_HOME" 	      --strip-components 1 	      --no-same-owner 	  ;     rm -f /tmp/openjdk.tar.gz ${JAVA_HOME}/src.zip;     find "$JAVA_HOME/lib" -name '*.so' -exec dirname '{}' ';' | sort -u > /etc/ld.so.conf.d/docker-openjdk.conf;     ldconfig;
# Thu, 02 Mar 2023 04:02:13 GMT
RUN echo Verifying install ...     && echo java -version && java -version     && echo Complete.
# Thu, 02 Mar 2023 10:52:20 GMT
ENV CATALINA_HOME=/usr/local/tomcat
# Thu, 02 Mar 2023 10:52:20 GMT
ENV PATH=/usr/local/tomcat/bin:/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 02 Mar 2023 10:52:21 GMT
RUN mkdir -p "$CATALINA_HOME"
# Thu, 02 Mar 2023 10:52:21 GMT
WORKDIR /usr/local/tomcat
# Thu, 02 Mar 2023 10:52:21 GMT
ENV TOMCAT_NATIVE_LIBDIR=/usr/local/tomcat/native-jni-lib
# Thu, 02 Mar 2023 10:52:21 GMT
ENV LD_LIBRARY_PATH=/usr/local/tomcat/native-jni-lib
# Thu, 02 Mar 2023 10:52:21 GMT
ENV GPG_KEYS=48F8E69F6390C9F25CFEDCD268248959359E722B A9C5DF4D22E99998D9875A5110C01C5A2F6059E7 DCFD35E0BF8CA7344752DE8B6FB21E8933C60243
# Thu, 02 Mar 2023 10:52:21 GMT
ENV TOMCAT_MAJOR=9
# Sat, 04 Mar 2023 02:39:55 GMT
ENV TOMCAT_VERSION=9.0.73
# Sat, 04 Mar 2023 02:39:55 GMT
ENV TOMCAT_SHA512=d43fbd6c5ae00bc0ffc2559743f91abd3547c827426cb0acdc8428e060e8659b6bb41b3877deb061ab6202980de39b9558525a4256725b647d5bff93e47a5664
# Sat, 04 Mar 2023 02:39:55 GMT
COPY dir:1fd19ca3e4c2bdb6857b72e05947a6b9b2a2e5198157d7cb81cb5a7c14e01ad5 in /usr/local/tomcat 
# Sat, 04 Mar 2023 02:40:00 GMT
RUN set -eux; 	apt-get update; 	xargs -rt apt-get install -y --no-install-recommends < "$TOMCAT_NATIVE_LIBDIR/.dependencies.txt"; 	rm -rf /var/lib/apt/lists/*
# Sat, 04 Mar 2023 02:40:02 GMT
RUN set -eux; 	nativeLines="$(catalina.sh configtest 2>&1)"; 	nativeLines="$(echo "$nativeLines" | grep 'Apache Tomcat Native')"; 	nativeLines="$(echo "$nativeLines" | sort -u)"; 	if ! echo "$nativeLines" | grep -E 'INFO: Loaded( APR based)? Apache Tomcat Native library' >&2; then 		echo >&2 "$nativeLines"; 		exit 1; 	fi
# Sat, 04 Mar 2023 02:40:02 GMT
EXPOSE 8080
# Sat, 04 Mar 2023 02:40:02 GMT
CMD ["catalina.sh" "run"]
```

-	Layers:
	-	`sha256:df6635ed1257a768a4cf0fba31ebc5c8a6a03ae7d5b9b079bfd9df9eb89e0f81`  
		Last Modified: Wed, 01 Mar 2023 09:05:18 GMT  
		Size: 28.6 MB (28578002 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a7015360bd1b0c50709c39c29445410d9103f250a78c1f0067f535569434606e`  
		Last Modified: Thu, 02 Mar 2023 04:07:42 GMT  
		Size: 16.3 MB (16341483 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:74f153beee3524c1bc9661095592c903191f04b8ef3698a9521e77e52e0ca368`  
		Last Modified: Thu, 02 Mar 2023 04:08:21 GMT  
		Size: 41.8 MB (41824184 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8ba0921a1f8f7441b2c3b8b01a8cd7bf0b310630be3dd9245196ebccc60b7053`  
		Last Modified: Thu, 02 Mar 2023 04:08:16 GMT  
		Size: 159.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:88d22129084f2f0f3233bc2ff69ac1f665aaafa3b8333d4bb22d8aacde2b0893`  
		Last Modified: Thu, 02 Mar 2023 11:07:53 GMT  
		Size: 174.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1754115d4ed9d26696efd7f64e8dd95ca462c1f440c928736cda86dc63284b28`  
		Last Modified: Sat, 04 Mar 2023 02:49:30 GMT  
		Size: 12.3 MB (12283090 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3fdc00d5117ab6c68baab330f1fbb39fbb83f94542efc6a3c9683f7ce9cb9144`  
		Last Modified: Sat, 04 Mar 2023 02:49:29 GMT  
		Size: 448.3 KB (448259 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:82949342acaa38a7debc073a7f0aff63f19184382c326b55dcb5313600b14ffd`  
		Last Modified: Sat, 04 Mar 2023 02:49:29 GMT  
		Size: 131.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `tomcat:9-jre8-temurin-focal` - linux; arm variant v7

```console
$ docker pull tomcat@sha256:72d0c8a08560eb6233210620b75e53eaeeb385a1500a2fc5d325d9e00ee311f0
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **92.0 MB (91965009 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e6012f7299e03d8041fb479cd106c04e85a662c5ef0a3390dd618f2aab597af2`
-	Default Command: `["catalina.sh","run"]`

```dockerfile
# Wed, 08 Mar 2023 04:31:43 GMT
ARG RELEASE
# Wed, 08 Mar 2023 04:31:43 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Wed, 08 Mar 2023 04:31:43 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Wed, 08 Mar 2023 04:31:43 GMT
LABEL org.opencontainers.image.version=20.04
# Wed, 08 Mar 2023 04:31:46 GMT
ADD file:99d501af7a191308f8fe3dc3f33c63bd8b54fb749d061b1a901c423b85f8cec2 in / 
# Wed, 08 Mar 2023 04:31:46 GMT
CMD ["/bin/bash"]
# Thu, 16 Mar 2023 02:45:16 GMT
ENV JAVA_HOME=/opt/java/openjdk
# Thu, 16 Mar 2023 02:45:16 GMT
ENV PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 16 Mar 2023 02:45:16 GMT
ENV LANG=en_US.UTF-8 LANGUAGE=en_US:en LC_ALL=en_US.UTF-8
# Thu, 16 Mar 2023 02:45:58 GMT
RUN apt-get update     && DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends tzdata curl wget ca-certificates fontconfig locales     && echo "en_US.UTF-8 UTF-8" >> /etc/locale.gen     && locale-gen en_US.UTF-8     && rm -rf /var/lib/apt/lists/*
# Thu, 16 Mar 2023 02:45:58 GMT
ENV JAVA_VERSION=jdk8u362-b09
# Thu, 16 Mar 2023 02:47:21 GMT
RUN set -eux;     ARCH="$(dpkg --print-architecture)";     case "${ARCH}" in        aarch64|arm64)          ESUM='cbe45788fa2d9d04d6b10f8aec7dbb15a018dbafe897ed75e31876d0367d56a5';          BINARY_URL='https://github.com/adoptium/temurin8-binaries/releases/download/jdk8u362-b09/OpenJDK8U-jre_aarch64_linux_hotspot_8u362b09.tar.gz';          ;;        armhf|arm)          ESUM='82d8524838b07ee438d42f4c33b6ecfe89ae83efac9af0605c76d75195bdcd99';          BINARY_URL='https://github.com/adoptium/temurin8-binaries/releases/download/jdk8u362-b09/OpenJDK8U-jre_arm_linux_hotspot_8u362b09.tar.gz';          apt-get update          && DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends libatomic1          && rm -rf /var/lib/apt/lists/*          ;;        ppc64el|powerpc:common64)          ESUM='5ec3e07126fedc23b58bb0f5b2dd05b5e9599ce1a3567fc2c7b27587f39faa3b';          BINARY_URL='https://github.com/adoptium/temurin8-binaries/releases/download/jdk8u362-b09/OpenJDK8U-jre_ppc64le_linux_hotspot_8u362b09.tar.gz';          ;;        amd64|i386:x86-64)          ESUM='c8c4e180f915fc7c163240bf363dcdf2b481cd2723fabfc3d08ccf12e049611f';          BINARY_URL='https://github.com/adoptium/temurin8-binaries/releases/download/jdk8u362-b09/OpenJDK8U-jre_x64_linux_hotspot_8u362b09.tar.gz';          ;;        *)          echo "Unsupported arch: ${ARCH}";          exit 1;          ;;     esac; 	  wget -O /tmp/openjdk.tar.gz ${BINARY_URL}; 	  echo "${ESUM} */tmp/openjdk.tar.gz" | sha256sum -c -; 	  mkdir -p "$JAVA_HOME"; 	  tar --extract 	      --file /tmp/openjdk.tar.gz 	      --directory "$JAVA_HOME" 	      --strip-components 1 	      --no-same-owner 	  ;     rm -f /tmp/openjdk.tar.gz ${JAVA_HOME}/src.zip;     find "$JAVA_HOME/lib" -name '*.so' -exec dirname '{}' ';' | sort -u > /etc/ld.so.conf.d/docker-openjdk.conf;     ldconfig;
# Thu, 16 Mar 2023 02:47:22 GMT
RUN echo Verifying install ...     && echo java -version && java -version     && echo Complete.
# Thu, 16 Mar 2023 04:56:50 GMT
ENV CATALINA_HOME=/usr/local/tomcat
# Thu, 16 Mar 2023 04:56:50 GMT
ENV PATH=/usr/local/tomcat/bin:/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 16 Mar 2023 04:56:50 GMT
RUN mkdir -p "$CATALINA_HOME"
# Thu, 16 Mar 2023 04:56:50 GMT
WORKDIR /usr/local/tomcat
# Thu, 16 Mar 2023 04:56:50 GMT
ENV TOMCAT_NATIVE_LIBDIR=/usr/local/tomcat/native-jni-lib
# Thu, 16 Mar 2023 04:56:50 GMT
ENV LD_LIBRARY_PATH=/usr/local/tomcat/native-jni-lib
# Thu, 16 Mar 2023 04:56:50 GMT
ENV GPG_KEYS=48F8E69F6390C9F25CFEDCD268248959359E722B A9C5DF4D22E99998D9875A5110C01C5A2F6059E7 DCFD35E0BF8CA7344752DE8B6FB21E8933C60243
# Thu, 16 Mar 2023 04:56:50 GMT
ENV TOMCAT_MAJOR=9
# Thu, 16 Mar 2023 04:56:51 GMT
ENV TOMCAT_VERSION=9.0.73
# Thu, 16 Mar 2023 04:56:51 GMT
ENV TOMCAT_SHA512=d43fbd6c5ae00bc0ffc2559743f91abd3547c827426cb0acdc8428e060e8659b6bb41b3877deb061ab6202980de39b9558525a4256725b647d5bff93e47a5664
# Thu, 16 Mar 2023 04:56:51 GMT
COPY dir:3eef13ed8e9ceae0e4146f20d40a175562020df6230c4a700b3f642cc26df5e8 in /usr/local/tomcat 
# Thu, 16 Mar 2023 04:56:55 GMT
RUN set -eux; 	apt-get update; 	xargs -rt apt-get install -y --no-install-recommends < "$TOMCAT_NATIVE_LIBDIR/.dependencies.txt"; 	rm -rf /var/lib/apt/lists/*
# Thu, 16 Mar 2023 04:56:56 GMT
RUN set -eux; 	nativeLines="$(catalina.sh configtest 2>&1)"; 	nativeLines="$(echo "$nativeLines" | grep 'Apache Tomcat Native')"; 	nativeLines="$(echo "$nativeLines" | sort -u)"; 	if ! echo "$nativeLines" | grep -E 'INFO: Loaded( APR based)? Apache Tomcat Native library' >&2; then 		echo >&2 "$nativeLines"; 		exit 1; 	fi
# Thu, 16 Mar 2023 04:56:56 GMT
EXPOSE 8080
# Thu, 16 Mar 2023 04:56:57 GMT
CMD ["catalina.sh" "run"]
```

-	Layers:
	-	`sha256:5806a4b978689b82c0b1e370978a89d1fb81519414294a062ee8cdaae68d4cf9`  
		Last Modified: Thu, 09 Mar 2023 05:45:04 GMT  
		Size: 24.6 MB (24586482 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:75a83f4fecfbc7e7f11467e3143f3a281108df95027e781d9ccaf4fa910c15f1`  
		Last Modified: Thu, 16 Mar 2023 02:53:15 GMT  
		Size: 15.2 MB (15175904 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bf81d6d5446a1dbddc6fd07c159d3ee4220e114ac569274f3d7fed2d2a12dd27`  
		Last Modified: Thu, 16 Mar 2023 02:53:57 GMT  
		Size: 39.5 MB (39545218 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:449598bae26513fed24ea998cea5006ceaee2dabe8da484b663574771ef3cdc3`  
		Last Modified: Thu, 16 Mar 2023 02:53:52 GMT  
		Size: 160.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d142c15487d84fbd35c8fd23ac9336519383181697eec3a6be5af922cd83f63e`  
		Last Modified: Thu, 16 Mar 2023 05:19:13 GMT  
		Size: 171.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a8849c069bfc4b9732e55187109c4fc28e6359bf17e5e6c3bbb7dcbd637cb00a`  
		Last Modified: Thu, 16 Mar 2023 05:19:14 GMT  
		Size: 12.2 MB (12232148 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:244c7b96ec5d741d30c7c56b9b64f91eba88a35e1264909cdfb8577c6e30f246`  
		Last Modified: Thu, 16 Mar 2023 05:19:13 GMT  
		Size: 424.8 KB (424795 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a484959023794a7c5e673ccd7b43f7069e4511bff60117e059d2dc90e9d2e154`  
		Last Modified: Thu, 16 Mar 2023 05:19:13 GMT  
		Size: 131.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `tomcat:9-jre8-temurin-focal` - linux; arm64 variant v8

```console
$ docker pull tomcat@sha256:3f2ff3501280ba641ce0fdb7813a8af3f43f8b341b48f886ae0504e65961785b
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **97.0 MB (96966532 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:5164a960d6629e2f1c231614b2d1861fc9026a2de9be80b30559a5148279afa6`
-	Default Command: `["catalina.sh","run"]`

```dockerfile
# Wed, 08 Mar 2023 04:34:20 GMT
ARG RELEASE
# Wed, 08 Mar 2023 04:34:20 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Wed, 08 Mar 2023 04:34:20 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Wed, 08 Mar 2023 04:34:20 GMT
LABEL org.opencontainers.image.version=20.04
# Wed, 08 Mar 2023 04:34:24 GMT
ADD file:e73d5d005a3ba2c2fb3d8585a1f19daf5ea9ed75af5a2f97b1cc6f7f03db0cdc in / 
# Wed, 08 Mar 2023 04:34:24 GMT
CMD ["/bin/bash"]
# Thu, 16 Mar 2023 01:51:45 GMT
ENV JAVA_HOME=/opt/java/openjdk
# Thu, 16 Mar 2023 01:51:45 GMT
ENV PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 16 Mar 2023 01:51:45 GMT
ENV LANG=en_US.UTF-8 LANGUAGE=en_US:en LC_ALL=en_US.UTF-8
# Thu, 16 Mar 2023 01:52:13 GMT
RUN apt-get update     && DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends tzdata curl wget ca-certificates fontconfig locales     && echo "en_US.UTF-8 UTF-8" >> /etc/locale.gen     && locale-gen en_US.UTF-8     && rm -rf /var/lib/apt/lists/*
# Thu, 16 Mar 2023 01:52:13 GMT
ENV JAVA_VERSION=jdk8u362-b09
# Thu, 16 Mar 2023 01:53:12 GMT
RUN set -eux;     ARCH="$(dpkg --print-architecture)";     case "${ARCH}" in        aarch64|arm64)          ESUM='cbe45788fa2d9d04d6b10f8aec7dbb15a018dbafe897ed75e31876d0367d56a5';          BINARY_URL='https://github.com/adoptium/temurin8-binaries/releases/download/jdk8u362-b09/OpenJDK8U-jre_aarch64_linux_hotspot_8u362b09.tar.gz';          ;;        armhf|arm)          ESUM='82d8524838b07ee438d42f4c33b6ecfe89ae83efac9af0605c76d75195bdcd99';          BINARY_URL='https://github.com/adoptium/temurin8-binaries/releases/download/jdk8u362-b09/OpenJDK8U-jre_arm_linux_hotspot_8u362b09.tar.gz';          apt-get update          && DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends libatomic1          && rm -rf /var/lib/apt/lists/*          ;;        ppc64el|powerpc:common64)          ESUM='5ec3e07126fedc23b58bb0f5b2dd05b5e9599ce1a3567fc2c7b27587f39faa3b';          BINARY_URL='https://github.com/adoptium/temurin8-binaries/releases/download/jdk8u362-b09/OpenJDK8U-jre_ppc64le_linux_hotspot_8u362b09.tar.gz';          ;;        amd64|i386:x86-64)          ESUM='c8c4e180f915fc7c163240bf363dcdf2b481cd2723fabfc3d08ccf12e049611f';          BINARY_URL='https://github.com/adoptium/temurin8-binaries/releases/download/jdk8u362-b09/OpenJDK8U-jre_x64_linux_hotspot_8u362b09.tar.gz';          ;;        *)          echo "Unsupported arch: ${ARCH}";          exit 1;          ;;     esac; 	  wget -O /tmp/openjdk.tar.gz ${BINARY_URL}; 	  echo "${ESUM} */tmp/openjdk.tar.gz" | sha256sum -c -; 	  mkdir -p "$JAVA_HOME"; 	  tar --extract 	      --file /tmp/openjdk.tar.gz 	      --directory "$JAVA_HOME" 	      --strip-components 1 	      --no-same-owner 	  ;     rm -f /tmp/openjdk.tar.gz ${JAVA_HOME}/src.zip;     find "$JAVA_HOME/lib" -name '*.so' -exec dirname '{}' ';' | sort -u > /etc/ld.so.conf.d/docker-openjdk.conf;     ldconfig;
# Thu, 16 Mar 2023 01:53:13 GMT
RUN echo Verifying install ...     && echo java -version && java -version     && echo Complete.
# Thu, 16 Mar 2023 06:31:37 GMT
ENV CATALINA_HOME=/usr/local/tomcat
# Thu, 16 Mar 2023 06:31:37 GMT
ENV PATH=/usr/local/tomcat/bin:/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 16 Mar 2023 06:31:37 GMT
RUN mkdir -p "$CATALINA_HOME"
# Thu, 16 Mar 2023 06:31:38 GMT
WORKDIR /usr/local/tomcat
# Thu, 16 Mar 2023 06:31:38 GMT
ENV TOMCAT_NATIVE_LIBDIR=/usr/local/tomcat/native-jni-lib
# Thu, 16 Mar 2023 06:31:38 GMT
ENV LD_LIBRARY_PATH=/usr/local/tomcat/native-jni-lib
# Thu, 16 Mar 2023 06:31:38 GMT
ENV GPG_KEYS=48F8E69F6390C9F25CFEDCD268248959359E722B A9C5DF4D22E99998D9875A5110C01C5A2F6059E7 DCFD35E0BF8CA7344752DE8B6FB21E8933C60243
# Thu, 16 Mar 2023 06:31:38 GMT
ENV TOMCAT_MAJOR=9
# Thu, 16 Mar 2023 06:31:38 GMT
ENV TOMCAT_VERSION=9.0.73
# Thu, 16 Mar 2023 06:31:38 GMT
ENV TOMCAT_SHA512=d43fbd6c5ae00bc0ffc2559743f91abd3547c827426cb0acdc8428e060e8659b6bb41b3877deb061ab6202980de39b9558525a4256725b647d5bff93e47a5664
# Thu, 16 Mar 2023 06:31:38 GMT
COPY dir:4619cf24725868a52d393a284c5c233ba9b5337cfddc7ee895ac0c32fb9c66a9 in /usr/local/tomcat 
# Thu, 16 Mar 2023 06:31:42 GMT
RUN set -eux; 	apt-get update; 	xargs -rt apt-get install -y --no-install-recommends < "$TOMCAT_NATIVE_LIBDIR/.dependencies.txt"; 	rm -rf /var/lib/apt/lists/*
# Thu, 16 Mar 2023 06:31:43 GMT
RUN set -eux; 	nativeLines="$(catalina.sh configtest 2>&1)"; 	nativeLines="$(echo "$nativeLines" | grep 'Apache Tomcat Native')"; 	nativeLines="$(echo "$nativeLines" | sort -u)"; 	if ! echo "$nativeLines" | grep -E 'INFO: Loaded( APR based)? Apache Tomcat Native library' >&2; then 		echo >&2 "$nativeLines"; 		exit 1; 	fi
# Thu, 16 Mar 2023 06:31:43 GMT
EXPOSE 8080
# Thu, 16 Mar 2023 06:31:43 GMT
CMD ["catalina.sh" "run"]
```

-	Layers:
	-	`sha256:0c68957c744181d1b5cae80a96971c651cec74faeade53191985b92abff361da`  
		Last Modified: Wed, 08 Mar 2023 20:37:17 GMT  
		Size: 27.2 MB (27196161 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:468a568d00c266348e3fcc790b81f74ef5577ea655a9f4ee8c5950aa335c610d`  
		Last Modified: Thu, 16 Mar 2023 01:58:03 GMT  
		Size: 16.2 MB (16210991 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9ed36cc0aa028036d8a20174a8cc7121e1dde43da15551ed046d758e469fc362`  
		Last Modified: Thu, 16 Mar 2023 01:58:39 GMT  
		Size: 40.8 MB (40808830 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f350e0dfdcb8a98a29d0886395ee2d5144ca20879ebcd8f5f7222eda97c0a00e`  
		Last Modified: Thu, 16 Mar 2023 01:58:35 GMT  
		Size: 160.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ac4c35757806b92fa6aa2a6381dcca2db0129b2f15d1196ab856de8fb4970a33`  
		Last Modified: Thu, 16 Mar 2023 06:46:31 GMT  
		Size: 171.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9b3484052add4ef3481758bc7df082023f53bb135698a7d2c71a85ddce25a929`  
		Last Modified: Thu, 16 Mar 2023 06:46:32 GMT  
		Size: 12.3 MB (12301229 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a33e8ee51c7f8991f17b76b0bbed12224f2fe2e5b8b346be586106d20e6d9a03`  
		Last Modified: Thu, 16 Mar 2023 06:46:31 GMT  
		Size: 448.9 KB (448861 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b4dd9b053937329641b3270b9fe448c0726d95484d5189401275da76901bd655`  
		Last Modified: Thu, 16 Mar 2023 06:46:31 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `tomcat:9-jre8-temurin-focal` - linux; ppc64le

```console
$ docker pull tomcat@sha256:7b976a5e405e77bf11d0c029fce1df3d03a9569fc5aa8479d7cd2e7aa586c08c
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **104.9 MB (104891096 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:6421882ee6108125fe913aa94fe3668cbc7ffbc850398dc4a9c97856b2f185ce`
-	Default Command: `["catalina.sh","run"]`

```dockerfile
# Wed, 01 Mar 2023 05:25:21 GMT
ARG RELEASE
# Wed, 01 Mar 2023 05:25:21 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Wed, 01 Mar 2023 05:25:22 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Wed, 01 Mar 2023 05:25:22 GMT
LABEL org.opencontainers.image.version=20.04
# Wed, 01 Mar 2023 05:25:25 GMT
ADD file:8ec53343ee3a54689d663a250c785fbf7b8ac0c74de561582d2e54878e2d73b5 in / 
# Wed, 01 Mar 2023 05:25:25 GMT
CMD ["/bin/bash"]
# Thu, 02 Mar 2023 04:03:25 GMT
ENV JAVA_HOME=/opt/java/openjdk
# Thu, 02 Mar 2023 04:03:25 GMT
ENV PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 02 Mar 2023 04:03:26 GMT
ENV LANG=en_US.UTF-8 LANGUAGE=en_US:en LC_ALL=en_US.UTF-8
# Thu, 02 Mar 2023 04:04:14 GMT
RUN apt-get update     && DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends tzdata curl wget ca-certificates fontconfig locales     && echo "en_US.UTF-8 UTF-8" >> /etc/locale.gen     && locale-gen en_US.UTF-8     && rm -rf /var/lib/apt/lists/*
# Thu, 02 Mar 2023 04:04:16 GMT
ENV JAVA_VERSION=jdk8u362-b09
# Thu, 02 Mar 2023 04:06:17 GMT
RUN set -eux;     ARCH="$(dpkg --print-architecture)";     case "${ARCH}" in        aarch64|arm64)          ESUM='cbe45788fa2d9d04d6b10f8aec7dbb15a018dbafe897ed75e31876d0367d56a5';          BINARY_URL='https://github.com/adoptium/temurin8-binaries/releases/download/jdk8u362-b09/OpenJDK8U-jre_aarch64_linux_hotspot_8u362b09.tar.gz';          ;;        armhf|arm)          ESUM='82d8524838b07ee438d42f4c33b6ecfe89ae83efac9af0605c76d75195bdcd99';          BINARY_URL='https://github.com/adoptium/temurin8-binaries/releases/download/jdk8u362-b09/OpenJDK8U-jre_arm_linux_hotspot_8u362b09.tar.gz';          apt-get update          && DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends libatomic1          && rm -rf /var/lib/apt/lists/*          ;;        ppc64el|powerpc:common64)          ESUM='5ec3e07126fedc23b58bb0f5b2dd05b5e9599ce1a3567fc2c7b27587f39faa3b';          BINARY_URL='https://github.com/adoptium/temurin8-binaries/releases/download/jdk8u362-b09/OpenJDK8U-jre_ppc64le_linux_hotspot_8u362b09.tar.gz';          ;;        amd64|i386:x86-64)          ESUM='c8c4e180f915fc7c163240bf363dcdf2b481cd2723fabfc3d08ccf12e049611f';          BINARY_URL='https://github.com/adoptium/temurin8-binaries/releases/download/jdk8u362-b09/OpenJDK8U-jre_x64_linux_hotspot_8u362b09.tar.gz';          ;;        *)          echo "Unsupported arch: ${ARCH}";          exit 1;          ;;     esac; 	  wget -O /tmp/openjdk.tar.gz ${BINARY_URL}; 	  echo "${ESUM} */tmp/openjdk.tar.gz" | sha256sum -c -; 	  mkdir -p "$JAVA_HOME"; 	  tar --extract 	      --file /tmp/openjdk.tar.gz 	      --directory "$JAVA_HOME" 	      --strip-components 1 	      --no-same-owner 	  ;     rm -f /tmp/openjdk.tar.gz ${JAVA_HOME}/src.zip;     find "$JAVA_HOME/lib" -name '*.so' -exec dirname '{}' ';' | sort -u > /etc/ld.so.conf.d/docker-openjdk.conf;     ldconfig;
# Thu, 02 Mar 2023 04:06:20 GMT
RUN echo Verifying install ...     && echo java -version && java -version     && echo Complete.
# Thu, 02 Mar 2023 06:55:05 GMT
ENV CATALINA_HOME=/usr/local/tomcat
# Thu, 02 Mar 2023 06:55:06 GMT
ENV PATH=/usr/local/tomcat/bin:/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 02 Mar 2023 06:55:07 GMT
RUN mkdir -p "$CATALINA_HOME"
# Thu, 02 Mar 2023 06:55:08 GMT
WORKDIR /usr/local/tomcat
# Thu, 02 Mar 2023 06:55:08 GMT
ENV TOMCAT_NATIVE_LIBDIR=/usr/local/tomcat/native-jni-lib
# Thu, 02 Mar 2023 06:55:09 GMT
ENV LD_LIBRARY_PATH=/usr/local/tomcat/native-jni-lib
# Thu, 02 Mar 2023 06:55:09 GMT
ENV GPG_KEYS=48F8E69F6390C9F25CFEDCD268248959359E722B A9C5DF4D22E99998D9875A5110C01C5A2F6059E7 DCFD35E0BF8CA7344752DE8B6FB21E8933C60243
# Thu, 02 Mar 2023 06:55:10 GMT
ENV TOMCAT_MAJOR=9
# Sat, 04 Mar 2023 02:37:35 GMT
ENV TOMCAT_VERSION=9.0.73
# Sat, 04 Mar 2023 02:37:35 GMT
ENV TOMCAT_SHA512=d43fbd6c5ae00bc0ffc2559743f91abd3547c827426cb0acdc8428e060e8659b6bb41b3877deb061ab6202980de39b9558525a4256725b647d5bff93e47a5664
# Sat, 04 Mar 2023 02:37:36 GMT
COPY dir:87ced27d03b54eceac02f7ca61765ba1c626aa16fba97b0ea756dd0a1e1f9588 in /usr/local/tomcat 
# Sat, 04 Mar 2023 02:37:45 GMT
RUN set -eux; 	apt-get update; 	xargs -rt apt-get install -y --no-install-recommends < "$TOMCAT_NATIVE_LIBDIR/.dependencies.txt"; 	rm -rf /var/lib/apt/lists/*
# Sat, 04 Mar 2023 02:37:49 GMT
RUN set -eux; 	nativeLines="$(catalina.sh configtest 2>&1)"; 	nativeLines="$(echo "$nativeLines" | grep 'Apache Tomcat Native')"; 	nativeLines="$(echo "$nativeLines" | sort -u)"; 	if ! echo "$nativeLines" | grep -E 'INFO: Loaded( APR based)? Apache Tomcat Native library' >&2; then 		echo >&2 "$nativeLines"; 		exit 1; 	fi
# Sat, 04 Mar 2023 02:37:49 GMT
EXPOSE 8080
# Sat, 04 Mar 2023 02:37:50 GMT
CMD ["catalina.sh" "run"]
```

-	Layers:
	-	`sha256:4ecbbabc4a8d11d32aa94bd1d645cba73ad91f59060b872eaf684de51310281b`  
		Last Modified: Thu, 02 Mar 2023 03:56:04 GMT  
		Size: 33.3 MB (33300379 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:86bf781428c54e99ccbf1268ef9774419ef70853536b11e51069c5ce69a81411`  
		Last Modified: Thu, 02 Mar 2023 04:17:41 GMT  
		Size: 17.6 MB (17577844 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:38ed241fb085c44d6c1e8d524e97350ed5286126d2020db5d72908a99d4af45a`  
		Last Modified: Thu, 02 Mar 2023 04:18:38 GMT  
		Size: 41.2 MB (41214796 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:54ee1da147a00b751df8204f38135873b823769f0338ecf653213ebc1a25c7cf`  
		Last Modified: Thu, 02 Mar 2023 04:18:30 GMT  
		Size: 159.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:acf9200e82594a3f509ba24e961012bdfb56ee05e03ad4201248d94c4b797d3d`  
		Last Modified: Thu, 02 Mar 2023 07:28:22 GMT  
		Size: 172.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:571f6b9f99d49f14681597e1f2dc97ab57982704ca655d3bd78b621f659dd7eb`  
		Last Modified: Sat, 04 Mar 2023 02:50:56 GMT  
		Size: 12.3 MB (12323702 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:22664bd0c629b88a907c7428cfafa89267525ed3eadd0030f2683551601bc2c4`  
		Last Modified: Sat, 04 Mar 2023 02:50:54 GMT  
		Size: 473.9 KB (473914 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d66ad25feacc104d765f39d85a17389aaf86a73926880a6761366c9d6deab337`  
		Last Modified: Sat, 04 Mar 2023 02:50:54 GMT  
		Size: 130.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
