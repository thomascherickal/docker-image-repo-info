## `tomcat:9-jre8-temurin`

```console
$ docker pull tomcat@sha256:22ee40db1b9f7d0b8f992931e9eb4d5cc4bb474b9d530480647cc276bdc681e4
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 4
	-	linux; amd64
	-	linux; arm variant v7
	-	linux; arm64 variant v8
	-	linux; ppc64le

### `tomcat:9-jre8-temurin` - linux; amd64

```console
$ docker pull tomcat@sha256:5c1e6b12a7037efde54ddfed9511a82147aca9ae0fe1ded1d5dd02dcc73bddf2
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **97.9 MB (97933798 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d5fd442dc6f42cd3ee769f47b56ea67bb50a63f55ea841642545b8eab7227556`
-	Default Command: `["catalina.sh","run"]`

```dockerfile
# Fri, 04 Aug 2023 04:52:57 GMT
ARG RELEASE
# Fri, 04 Aug 2023 04:52:57 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Fri, 04 Aug 2023 04:52:58 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Fri, 04 Aug 2023 04:52:58 GMT
LABEL org.opencontainers.image.version=22.04
# Fri, 04 Aug 2023 04:52:59 GMT
ADD file:bb1fa1d9d012ae826908afdce8c9fa2feebf221b2ab032e1535255905144411a in / 
# Fri, 04 Aug 2023 04:53:00 GMT
CMD ["/bin/bash"]
# Wed, 16 Aug 2023 15:39:01 GMT
ENV JAVA_HOME=/opt/java/openjdk
# Wed, 16 Aug 2023 15:39:01 GMT
ENV PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 16 Aug 2023 15:39:01 GMT
ENV LANG=en_US.UTF-8 LANGUAGE=en_US:en LC_ALL=en_US.UTF-8
# Wed, 16 Aug 2023 15:39:13 GMT
RUN apt-get update     && DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends tzdata curl wget ca-certificates fontconfig locales p11-kit     && echo "en_US.UTF-8 UTF-8" >> /etc/locale.gen     && locale-gen en_US.UTF-8     && rm -rf /var/lib/apt/lists/*
# Wed, 16 Aug 2023 15:39:13 GMT
ENV JAVA_VERSION=jdk8u382-b05
# Wed, 16 Aug 2023 15:39:38 GMT
RUN set -eux;     ARCH="$(dpkg --print-architecture)";     case "${ARCH}" in        aarch64|arm64)          ESUM='8cf329aa76d5b6abe35dd94e5087d9d14993fa13b43bbaed3b26bda4c57162c4';          BINARY_URL='https://github.com/adoptium/temurin8-binaries/releases/download/jdk8u382-b05/OpenJDK8U-jre_aarch64_linux_hotspot_8u382b05.tar.gz';          ;;        armhf|arm)          ESUM='b92fb3972372b5d1f9fb51815def903105722b747f680b7ecf2ba2ba863ab156';          BINARY_URL='https://github.com/adoptium/temurin8-binaries/releases/download/jdk8u382-b05/OpenJDK8U-jre_arm_linux_hotspot_8u382b05.tar.gz';          apt-get update          && DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends libatomic1          && rm -rf /var/lib/apt/lists/*          ;;        ppc64el|powerpc:common64)          ESUM='8f0706f16373078e46666a6035325792584cd565b4cc5a793a37312599f3af0b';          BINARY_URL='https://github.com/adoptium/temurin8-binaries/releases/download/jdk8u382-b05/OpenJDK8U-jre_ppc64le_linux_hotspot_8u382b05.tar.gz';          ;;        amd64|i386:x86-64)          ESUM='1fad165cc243e8db1b9cf226134acdfe3dc5919cd98c5fd9210de3cf9edeabd7';          BINARY_URL='https://github.com/adoptium/temurin8-binaries/releases/download/jdk8u382-b05/OpenJDK8U-jre_x64_linux_hotspot_8u382b05.tar.gz';          ;;        *)          echo "Unsupported arch: ${ARCH}";          exit 1;          ;;     esac; 	  wget -O /tmp/openjdk.tar.gz ${BINARY_URL}; 	  echo "${ESUM} */tmp/openjdk.tar.gz" | sha256sum -c -; 	  mkdir -p "$JAVA_HOME"; 	  tar --extract 	      --file /tmp/openjdk.tar.gz 	      --directory "$JAVA_HOME" 	      --strip-components 1 	      --no-same-owner 	  ;     rm -f /tmp/openjdk.tar.gz ${JAVA_HOME}/lib/src.zip;     find "$JAVA_HOME/lib" -name '*.so' -exec dirname '{}' ';' | sort -u > /etc/ld.so.conf.d/docker-openjdk.conf;     ldconfig;
# Wed, 16 Aug 2023 15:39:39 GMT
RUN echo Verifying install ...     && echo java -version && java -version     && echo Complete.
# Wed, 16 Aug 2023 15:39:39 GMT
COPY file:8b8864b3e02a33a579dc216fd51b28a6047bc8eeaa03045b258980fe0cf7fcb3 in /__cacert_entrypoint.sh 
# Wed, 16 Aug 2023 15:39:39 GMT
ENTRYPOINT ["/__cacert_entrypoint.sh"]
# Wed, 16 Aug 2023 18:29:49 GMT
ENV CATALINA_HOME=/usr/local/tomcat
# Wed, 16 Aug 2023 18:29:49 GMT
ENV PATH=/usr/local/tomcat/bin:/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 16 Aug 2023 18:29:50 GMT
RUN mkdir -p "$CATALINA_HOME"
# Wed, 16 Aug 2023 18:29:50 GMT
WORKDIR /usr/local/tomcat
# Wed, 16 Aug 2023 18:29:50 GMT
ENV TOMCAT_NATIVE_LIBDIR=/usr/local/tomcat/native-jni-lib
# Wed, 16 Aug 2023 18:29:50 GMT
ENV LD_LIBRARY_PATH=/usr/local/tomcat/native-jni-lib
# Wed, 16 Aug 2023 18:29:50 GMT
ENV GPG_KEYS=48F8E69F6390C9F25CFEDCD268248959359E722B A9C5DF4D22E99998D9875A5110C01C5A2F6059E7 DCFD35E0BF8CA7344752DE8B6FB21E8933C60243
# Wed, 16 Aug 2023 18:29:50 GMT
ENV TOMCAT_MAJOR=9
# Sat, 26 Aug 2023 04:24:54 GMT
ENV TOMCAT_VERSION=9.0.80
# Sat, 26 Aug 2023 04:24:54 GMT
ENV TOMCAT_SHA512=24014441b0ccdd2dda238efa56e1a039476488943e6cf04f8a372a340a49dd21ce174ed68e2f5fcc43401e85fae6d00c5eac3d357653e91601737b6fa94476de
# Sat, 26 Aug 2023 04:24:55 GMT
COPY dir:c570ea3dc09e62fe49b3a55b3d240f6cd03b0456c11298d67f205d04fec1b9f4 in /usr/local/tomcat 
# Sat, 26 Aug 2023 04:24:59 GMT
RUN set -eux; 	apt-get update; 	xargs -rt apt-get install -y --no-install-recommends < "$TOMCAT_NATIVE_LIBDIR/.dependencies.txt"; 	rm -rf /var/lib/apt/lists/*
# Sat, 26 Aug 2023 04:25:00 GMT
RUN set -eux; 	nativeLines="$(catalina.sh configtest 2>&1)"; 	nativeLines="$(echo "$nativeLines" | grep 'Apache Tomcat Native')"; 	nativeLines="$(echo "$nativeLines" | sort -u)"; 	if ! echo "$nativeLines" | grep -E 'INFO: Loaded( APR based)? Apache Tomcat Native library' >&2; then 		echo >&2 "$nativeLines"; 		exit 1; 	fi
# Sat, 26 Aug 2023 04:25:00 GMT
EXPOSE 8080
# Sat, 26 Aug 2023 04:25:00 GMT
ENTRYPOINT []
# Sat, 26 Aug 2023 04:25:00 GMT
CMD ["catalina.sh" "run"]
```

-	Layers:
	-	`sha256:99de9192b4afd13ed65aeae58d55b38e5231eb97a743921357b7d5b4c0c903c4`  
		Last Modified: Fri, 04 Aug 2023 09:25:19 GMT  
		Size: 30.4 MB (30437960 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dabb03f19f5a305a4162b2dadb7942d094cb8ae82bfbb4ac13d4df822a60ffe3`  
		Last Modified: Wed, 16 Aug 2023 15:43:09 GMT  
		Size: 12.9 MB (12902780 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c428299586ef52fd07d7c0d5f704db673cb4e5fee15d57f0660f51caa19063a2`  
		Last Modified: Wed, 16 Aug 2023 15:43:37 GMT  
		Size: 41.9 MB (41851953 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:251696f718446151beda6737dde2edfa5168af192406e3c7e583e0e81be3cc63`  
		Last Modified: Wed, 16 Aug 2023 15:43:32 GMT  
		Size: 160.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7ea682eac76ec559e73c2933dccc1180b2397ba5126267f15568edbb8a713aa0`  
		Last Modified: Wed, 16 Aug 2023 15:43:32 GMT  
		Size: 734.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8cac71830742ddd7e868ad53b18adfea65964904e3d401a34823840842bd61fc`  
		Last Modified: Wed, 16 Aug 2023 18:44:12 GMT  
		Size: 170.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7fcfaf2804539f13cce57c02cfc234081429891a957ef4b9c7ddff7b07bfcddf`  
		Last Modified: Sat, 26 Aug 2023 04:46:56 GMT  
		Size: 12.3 MB (12284322 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2d147ad9e1da9590c8d72aa2f5db5110244bdabe5ad39b3bd819bb8573e6dba7`  
		Last Modified: Sat, 26 Aug 2023 04:46:55 GMT  
		Size: 455.6 KB (455589 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8ea1532dada061b856d0b2ea4e5e2ff99aa9369ef6508b4c40aec9f61cd16faa`  
		Last Modified: Sat, 26 Aug 2023 04:46:55 GMT  
		Size: 130.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `tomcat:9-jre8-temurin` - linux; arm variant v7

```console
$ docker pull tomcat@sha256:e09c1627b47854dff50d39a23511019598ad70f078787d704e654ef55de73d30
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **91.7 MB (91732600 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:49955acb212fe984bf6495705e070d744e94efb78ab4e93e4c39fa7543a66567`
-	Default Command: `["catalina.sh","run"]`

```dockerfile
# Fri, 04 Aug 2023 05:03:19 GMT
ARG RELEASE
# Fri, 04 Aug 2023 05:03:19 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Fri, 04 Aug 2023 05:03:19 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Fri, 04 Aug 2023 05:03:19 GMT
LABEL org.opencontainers.image.version=22.04
# Fri, 04 Aug 2023 05:03:24 GMT
ADD file:ca783750060711e8590ab362921bae8d7b02201c48fa3d2cb3fdf6aac045a793 in / 
# Fri, 04 Aug 2023 05:03:25 GMT
CMD ["/bin/bash"]
# Wed, 16 Aug 2023 16:00:56 GMT
ENV JAVA_HOME=/opt/java/openjdk
# Wed, 16 Aug 2023 16:00:56 GMT
ENV PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 16 Aug 2023 16:00:56 GMT
ENV LANG=en_US.UTF-8 LANGUAGE=en_US:en LC_ALL=en_US.UTF-8
# Wed, 16 Aug 2023 16:01:41 GMT
RUN apt-get update     && DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends tzdata curl wget ca-certificates fontconfig locales p11-kit     && echo "en_US.UTF-8 UTF-8" >> /etc/locale.gen     && locale-gen en_US.UTF-8     && rm -rf /var/lib/apt/lists/*
# Wed, 16 Aug 2023 16:01:41 GMT
ENV JAVA_VERSION=jdk8u382-b05
# Wed, 16 Aug 2023 16:02:14 GMT
RUN set -eux;     ARCH="$(dpkg --print-architecture)";     case "${ARCH}" in        aarch64|arm64)          ESUM='8cf329aa76d5b6abe35dd94e5087d9d14993fa13b43bbaed3b26bda4c57162c4';          BINARY_URL='https://github.com/adoptium/temurin8-binaries/releases/download/jdk8u382-b05/OpenJDK8U-jre_aarch64_linux_hotspot_8u382b05.tar.gz';          ;;        armhf|arm)          ESUM='b92fb3972372b5d1f9fb51815def903105722b747f680b7ecf2ba2ba863ab156';          BINARY_URL='https://github.com/adoptium/temurin8-binaries/releases/download/jdk8u382-b05/OpenJDK8U-jre_arm_linux_hotspot_8u382b05.tar.gz';          apt-get update          && DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends libatomic1          && rm -rf /var/lib/apt/lists/*          ;;        ppc64el|powerpc:common64)          ESUM='8f0706f16373078e46666a6035325792584cd565b4cc5a793a37312599f3af0b';          BINARY_URL='https://github.com/adoptium/temurin8-binaries/releases/download/jdk8u382-b05/OpenJDK8U-jre_ppc64le_linux_hotspot_8u382b05.tar.gz';          ;;        amd64|i386:x86-64)          ESUM='1fad165cc243e8db1b9cf226134acdfe3dc5919cd98c5fd9210de3cf9edeabd7';          BINARY_URL='https://github.com/adoptium/temurin8-binaries/releases/download/jdk8u382-b05/OpenJDK8U-jre_x64_linux_hotspot_8u382b05.tar.gz';          ;;        *)          echo "Unsupported arch: ${ARCH}";          exit 1;          ;;     esac; 	  wget -O /tmp/openjdk.tar.gz ${BINARY_URL}; 	  echo "${ESUM} */tmp/openjdk.tar.gz" | sha256sum -c -; 	  mkdir -p "$JAVA_HOME"; 	  tar --extract 	      --file /tmp/openjdk.tar.gz 	      --directory "$JAVA_HOME" 	      --strip-components 1 	      --no-same-owner 	  ;     rm -f /tmp/openjdk.tar.gz ${JAVA_HOME}/lib/src.zip;     find "$JAVA_HOME/lib" -name '*.so' -exec dirname '{}' ';' | sort -u > /etc/ld.so.conf.d/docker-openjdk.conf;     ldconfig;
# Wed, 16 Aug 2023 16:02:15 GMT
RUN echo Verifying install ...     && echo java -version && java -version     && echo Complete.
# Wed, 16 Aug 2023 16:02:15 GMT
COPY file:8b8864b3e02a33a579dc216fd51b28a6047bc8eeaa03045b258980fe0cf7fcb3 in /__cacert_entrypoint.sh 
# Wed, 16 Aug 2023 16:02:15 GMT
ENTRYPOINT ["/__cacert_entrypoint.sh"]
# Thu, 17 Aug 2023 03:16:44 GMT
ENV CATALINA_HOME=/usr/local/tomcat
# Thu, 17 Aug 2023 03:16:44 GMT
ENV PATH=/usr/local/tomcat/bin:/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 17 Aug 2023 03:16:44 GMT
RUN mkdir -p "$CATALINA_HOME"
# Thu, 17 Aug 2023 03:16:44 GMT
WORKDIR /usr/local/tomcat
# Thu, 17 Aug 2023 03:16:44 GMT
ENV TOMCAT_NATIVE_LIBDIR=/usr/local/tomcat/native-jni-lib
# Thu, 17 Aug 2023 03:16:44 GMT
ENV LD_LIBRARY_PATH=/usr/local/tomcat/native-jni-lib
# Thu, 17 Aug 2023 03:16:45 GMT
ENV GPG_KEYS=48F8E69F6390C9F25CFEDCD268248959359E722B A9C5DF4D22E99998D9875A5110C01C5A2F6059E7 DCFD35E0BF8CA7344752DE8B6FB21E8933C60243
# Thu, 17 Aug 2023 03:16:45 GMT
ENV TOMCAT_MAJOR=9
# Sat, 26 Aug 2023 04:05:17 GMT
ENV TOMCAT_VERSION=9.0.80
# Sat, 26 Aug 2023 04:05:18 GMT
ENV TOMCAT_SHA512=24014441b0ccdd2dda238efa56e1a039476488943e6cf04f8a372a340a49dd21ce174ed68e2f5fcc43401e85fae6d00c5eac3d357653e91601737b6fa94476de
# Sat, 26 Aug 2023 04:05:18 GMT
COPY dir:a0c6936df7a02b72189b3243775d7aa52ad86b2a634e1a02690625cc9ed7b835 in /usr/local/tomcat 
# Sat, 26 Aug 2023 04:05:22 GMT
RUN set -eux; 	apt-get update; 	xargs -rt apt-get install -y --no-install-recommends < "$TOMCAT_NATIVE_LIBDIR/.dependencies.txt"; 	rm -rf /var/lib/apt/lists/*
# Sat, 26 Aug 2023 04:05:24 GMT
RUN set -eux; 	nativeLines="$(catalina.sh configtest 2>&1)"; 	nativeLines="$(echo "$nativeLines" | grep 'Apache Tomcat Native')"; 	nativeLines="$(echo "$nativeLines" | sort -u)"; 	if ! echo "$nativeLines" | grep -E 'INFO: Loaded( APR based)? Apache Tomcat Native library' >&2; then 		echo >&2 "$nativeLines"; 		exit 1; 	fi
# Sat, 26 Aug 2023 04:05:24 GMT
EXPOSE 8080
# Sat, 26 Aug 2023 04:05:24 GMT
ENTRYPOINT []
# Sat, 26 Aug 2023 04:05:24 GMT
CMD ["catalina.sh" "run"]
```

-	Layers:
	-	`sha256:24758824a30b6e1f6132a6b6740dec1fc5723821f0f2b5b6513379480e0f74f9`  
		Last Modified: Sat, 05 Aug 2023 02:03:56 GMT  
		Size: 27.0 MB (27029194 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:96febab4cea6e23abf5057ef3e013cc162d11740829a21fd4045f347e961dcf7`  
		Last Modified: Wed, 16 Aug 2023 16:04:10 GMT  
		Size: 12.5 MB (12491781 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9e7ddcfb1dfed5a8cace443aa940f921c5fd8c324390c57d2a6453f99c12103e`  
		Last Modified: Wed, 16 Aug 2023 16:04:35 GMT  
		Size: 39.6 MB (39563902 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:651ffef3b3f983ec1e9ab8fe5f2141d0fc69611b049d818cd6faad047c4f6823`  
		Last Modified: Wed, 16 Aug 2023 16:04:29 GMT  
		Size: 159.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:54883ad29e5df41d3152677d112be2d88b0ab32d98882f87d1c978f5c610e13f`  
		Last Modified: Wed, 16 Aug 2023 16:04:29 GMT  
		Size: 734.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b1cc8a463f8073f092ce194cc8c3c4a521846ca92b528dfb86bbad14a7d7d059`  
		Last Modified: Thu, 17 Aug 2023 03:25:38 GMT  
		Size: 171.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1ffbdfb444c29cb65df94e7b3bc2d82406e9bc9ad42b662e3bcddd1556244bb6`  
		Last Modified: Sat, 26 Aug 2023 04:17:07 GMT  
		Size: 12.2 MB (12216466 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:60908051786172c32128ae7adfc58389f49aeb6fce29a9ca63d6eeb61bcc2ae1`  
		Last Modified: Sat, 26 Aug 2023 04:17:06 GMT  
		Size: 430.1 KB (430065 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c9ed55b4b58b8c7f0088ae81e830e95ed690de53f58fafd3175ea227e7775195`  
		Last Modified: Sat, 26 Aug 2023 04:17:05 GMT  
		Size: 128.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `tomcat:9-jre8-temurin` - linux; arm64 variant v8

```console
$ docker pull tomcat@sha256:28df589bc0c463bed9749af33e116f7a638ffbb9c9e66050f1f1ea35ed5a8041
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **94.8 MB (94828980 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ef12e0e9e25da8f8da52866e3ad4e2260121f6a2f731c051ceb5a4ff6d3fb1c2`
-	Default Command: `["catalina.sh","run"]`

```dockerfile
# Fri, 04 Aug 2023 04:51:14 GMT
ARG RELEASE
# Fri, 04 Aug 2023 04:51:14 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Fri, 04 Aug 2023 04:51:14 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Fri, 04 Aug 2023 04:51:14 GMT
LABEL org.opencontainers.image.version=22.04
# Fri, 04 Aug 2023 04:51:18 GMT
ADD file:5cf7797cf86362218d2bd85debeff136ee897af7eef95a0b8baab9f9457c3e89 in / 
# Fri, 04 Aug 2023 04:51:18 GMT
CMD ["/bin/bash"]
# Wed, 16 Aug 2023 14:23:25 GMT
ENV JAVA_HOME=/opt/java/openjdk
# Wed, 16 Aug 2023 14:23:25 GMT
ENV PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 16 Aug 2023 14:23:25 GMT
ENV LANG=en_US.UTF-8 LANGUAGE=en_US:en LC_ALL=en_US.UTF-8
# Wed, 16 Aug 2023 14:23:38 GMT
RUN apt-get update     && DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends tzdata curl wget ca-certificates fontconfig locales p11-kit     && echo "en_US.UTF-8 UTF-8" >> /etc/locale.gen     && locale-gen en_US.UTF-8     && rm -rf /var/lib/apt/lists/*
# Wed, 16 Aug 2023 14:23:39 GMT
ENV JAVA_VERSION=jdk8u382-b05
# Wed, 16 Aug 2023 14:23:56 GMT
RUN set -eux;     ARCH="$(dpkg --print-architecture)";     case "${ARCH}" in        aarch64|arm64)          ESUM='8cf329aa76d5b6abe35dd94e5087d9d14993fa13b43bbaed3b26bda4c57162c4';          BINARY_URL='https://github.com/adoptium/temurin8-binaries/releases/download/jdk8u382-b05/OpenJDK8U-jre_aarch64_linux_hotspot_8u382b05.tar.gz';          ;;        armhf|arm)          ESUM='b92fb3972372b5d1f9fb51815def903105722b747f680b7ecf2ba2ba863ab156';          BINARY_URL='https://github.com/adoptium/temurin8-binaries/releases/download/jdk8u382-b05/OpenJDK8U-jre_arm_linux_hotspot_8u382b05.tar.gz';          apt-get update          && DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends libatomic1          && rm -rf /var/lib/apt/lists/*          ;;        ppc64el|powerpc:common64)          ESUM='8f0706f16373078e46666a6035325792584cd565b4cc5a793a37312599f3af0b';          BINARY_URL='https://github.com/adoptium/temurin8-binaries/releases/download/jdk8u382-b05/OpenJDK8U-jre_ppc64le_linux_hotspot_8u382b05.tar.gz';          ;;        amd64|i386:x86-64)          ESUM='1fad165cc243e8db1b9cf226134acdfe3dc5919cd98c5fd9210de3cf9edeabd7';          BINARY_URL='https://github.com/adoptium/temurin8-binaries/releases/download/jdk8u382-b05/OpenJDK8U-jre_x64_linux_hotspot_8u382b05.tar.gz';          ;;        *)          echo "Unsupported arch: ${ARCH}";          exit 1;          ;;     esac; 	  wget -O /tmp/openjdk.tar.gz ${BINARY_URL}; 	  echo "${ESUM} */tmp/openjdk.tar.gz" | sha256sum -c -; 	  mkdir -p "$JAVA_HOME"; 	  tar --extract 	      --file /tmp/openjdk.tar.gz 	      --directory "$JAVA_HOME" 	      --strip-components 1 	      --no-same-owner 	  ;     rm -f /tmp/openjdk.tar.gz ${JAVA_HOME}/lib/src.zip;     find "$JAVA_HOME/lib" -name '*.so' -exec dirname '{}' ';' | sort -u > /etc/ld.so.conf.d/docker-openjdk.conf;     ldconfig;
# Wed, 16 Aug 2023 14:23:57 GMT
RUN echo Verifying install ...     && echo java -version && java -version     && echo Complete.
# Wed, 16 Aug 2023 14:23:57 GMT
COPY file:8b8864b3e02a33a579dc216fd51b28a6047bc8eeaa03045b258980fe0cf7fcb3 in /__cacert_entrypoint.sh 
# Wed, 16 Aug 2023 14:23:57 GMT
ENTRYPOINT ["/__cacert_entrypoint.sh"]
# Wed, 16 Aug 2023 22:01:39 GMT
ENV CATALINA_HOME=/usr/local/tomcat
# Wed, 16 Aug 2023 22:01:39 GMT
ENV PATH=/usr/local/tomcat/bin:/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 16 Aug 2023 22:01:39 GMT
RUN mkdir -p "$CATALINA_HOME"
# Wed, 16 Aug 2023 22:01:39 GMT
WORKDIR /usr/local/tomcat
# Wed, 16 Aug 2023 22:01:39 GMT
ENV TOMCAT_NATIVE_LIBDIR=/usr/local/tomcat/native-jni-lib
# Wed, 16 Aug 2023 22:01:39 GMT
ENV LD_LIBRARY_PATH=/usr/local/tomcat/native-jni-lib
# Wed, 16 Aug 2023 22:01:39 GMT
ENV GPG_KEYS=48F8E69F6390C9F25CFEDCD268248959359E722B A9C5DF4D22E99998D9875A5110C01C5A2F6059E7 DCFD35E0BF8CA7344752DE8B6FB21E8933C60243
# Wed, 16 Aug 2023 22:01:40 GMT
ENV TOMCAT_MAJOR=9
# Sat, 26 Aug 2023 03:28:02 GMT
ENV TOMCAT_VERSION=9.0.80
# Sat, 26 Aug 2023 03:28:02 GMT
ENV TOMCAT_SHA512=24014441b0ccdd2dda238efa56e1a039476488943e6cf04f8a372a340a49dd21ce174ed68e2f5fcc43401e85fae6d00c5eac3d357653e91601737b6fa94476de
# Sat, 26 Aug 2023 03:28:02 GMT
COPY dir:b591a6e57476e1de0a9cfe70425688909230f2285e401d23b142f82cda787f03 in /usr/local/tomcat 
# Sat, 26 Aug 2023 03:28:05 GMT
RUN set -eux; 	apt-get update; 	xargs -rt apt-get install -y --no-install-recommends < "$TOMCAT_NATIVE_LIBDIR/.dependencies.txt"; 	rm -rf /var/lib/apt/lists/*
# Sat, 26 Aug 2023 03:28:07 GMT
RUN set -eux; 	nativeLines="$(catalina.sh configtest 2>&1)"; 	nativeLines="$(echo "$nativeLines" | grep 'Apache Tomcat Native')"; 	nativeLines="$(echo "$nativeLines" | sort -u)"; 	if ! echo "$nativeLines" | grep -E 'INFO: Loaded( APR based)? Apache Tomcat Native library' >&2; then 		echo >&2 "$nativeLines"; 		exit 1; 	fi
# Sat, 26 Aug 2023 03:28:07 GMT
EXPOSE 8080
# Sat, 26 Aug 2023 03:28:07 GMT
ENTRYPOINT []
# Sat, 26 Aug 2023 03:28:07 GMT
CMD ["catalina.sh" "run"]
```

-	Layers:
	-	`sha256:9ea365e1e52efb9567c56f02f2200f0e95ddffd579225cc5b20a6333119d2811`  
		Last Modified: Fri, 04 Aug 2023 13:35:19 GMT  
		Size: 28.4 MB (28391903 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c9820f088487afe4c2ad735189bd2cca7b6b80af8efbaf6103e1ba1ae78d9f50`  
		Last Modified: Wed, 16 Aug 2023 14:26:46 GMT  
		Size: 12.8 MB (12843960 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1842eb90ddefb56c65cee49204f2ff2b8ece981dd3eff4e3400c905a8bbfecf9`  
		Last Modified: Wed, 16 Aug 2023 14:27:12 GMT  
		Size: 40.8 MB (40845875 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:526de63fdf58a686f90b02d93bf4f21da7fabebafc1c29ccc164ad58d87fe2c6`  
		Last Modified: Wed, 16 Aug 2023 14:27:08 GMT  
		Size: 159.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ea3cba925c676ed5ceb2b3eb77d1791ee96304c5e207062b2d14655c58e75a55`  
		Last Modified: Wed, 16 Aug 2023 14:27:08 GMT  
		Size: 734.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5717c5a3f42cc42bc36393059a3ddf96fa851ef37d3f808ae11b384b9965b37c`  
		Last Modified: Wed, 16 Aug 2023 22:15:53 GMT  
		Size: 173.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e4dca124ddb663325a68d1af2572f18533963219a2a68ab312a903d8c03bbc31`  
		Last Modified: Sat, 26 Aug 2023 03:47:22 GMT  
		Size: 12.3 MB (12290189 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3f326a34a29ebf54acb73e2547378ac45f8fd1dda314a7e872e262063ee2c72b`  
		Last Modified: Sat, 26 Aug 2023 03:47:21 GMT  
		Size: 455.9 KB (455858 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:69afcadea3c8cf98c5ad1a6623f3007428690c98be105639bee7180f702d02ac`  
		Last Modified: Sat, 26 Aug 2023 03:47:21 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `tomcat:9-jre8-temurin` - linux; ppc64le

```console
$ docker pull tomcat@sha256:d7ba1cb148d4b75c20c1b5bb9dda593f75158e5ba3cf4c6fd3ae525eb17c6589
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **103.5 MB (103511917 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:0b880cbe59f86480133b64485cdf90bff6616944a838416ee87e785860d7a3b4`
-	Default Command: `["catalina.sh","run"]`

```dockerfile
# Fri, 04 Aug 2023 04:56:16 GMT
ARG RELEASE
# Fri, 04 Aug 2023 04:56:17 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Fri, 04 Aug 2023 04:56:17 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Fri, 04 Aug 2023 04:56:17 GMT
LABEL org.opencontainers.image.version=22.04
# Fri, 04 Aug 2023 04:56:20 GMT
ADD file:0e9b840e6824ee009acbddc2d337fd5083ebe606393cf7532cdca4f108813ca3 in / 
# Fri, 04 Aug 2023 04:56:20 GMT
CMD ["/bin/bash"]
# Thu, 17 Aug 2023 07:21:24 GMT
ENV JAVA_HOME=/opt/java/openjdk
# Thu, 17 Aug 2023 07:21:25 GMT
ENV PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 17 Aug 2023 07:21:25 GMT
ENV LANG=en_US.UTF-8 LANGUAGE=en_US:en LC_ALL=en_US.UTF-8
# Thu, 17 Aug 2023 07:22:07 GMT
RUN apt-get update     && DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends tzdata curl wget ca-certificates fontconfig locales p11-kit     && echo "en_US.UTF-8 UTF-8" >> /etc/locale.gen     && locale-gen en_US.UTF-8     && rm -rf /var/lib/apt/lists/*
# Thu, 17 Aug 2023 07:22:08 GMT
ENV JAVA_VERSION=jdk8u382-b05
# Thu, 17 Aug 2023 07:22:47 GMT
RUN set -eux;     ARCH="$(dpkg --print-architecture)";     case "${ARCH}" in        aarch64|arm64)          ESUM='8cf329aa76d5b6abe35dd94e5087d9d14993fa13b43bbaed3b26bda4c57162c4';          BINARY_URL='https://github.com/adoptium/temurin8-binaries/releases/download/jdk8u382-b05/OpenJDK8U-jre_aarch64_linux_hotspot_8u382b05.tar.gz';          ;;        armhf|arm)          ESUM='b92fb3972372b5d1f9fb51815def903105722b747f680b7ecf2ba2ba863ab156';          BINARY_URL='https://github.com/adoptium/temurin8-binaries/releases/download/jdk8u382-b05/OpenJDK8U-jre_arm_linux_hotspot_8u382b05.tar.gz';          apt-get update          && DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends libatomic1          && rm -rf /var/lib/apt/lists/*          ;;        ppc64el|powerpc:common64)          ESUM='8f0706f16373078e46666a6035325792584cd565b4cc5a793a37312599f3af0b';          BINARY_URL='https://github.com/adoptium/temurin8-binaries/releases/download/jdk8u382-b05/OpenJDK8U-jre_ppc64le_linux_hotspot_8u382b05.tar.gz';          ;;        amd64|i386:x86-64)          ESUM='1fad165cc243e8db1b9cf226134acdfe3dc5919cd98c5fd9210de3cf9edeabd7';          BINARY_URL='https://github.com/adoptium/temurin8-binaries/releases/download/jdk8u382-b05/OpenJDK8U-jre_x64_linux_hotspot_8u382b05.tar.gz';          ;;        *)          echo "Unsupported arch: ${ARCH}";          exit 1;          ;;     esac; 	  wget -O /tmp/openjdk.tar.gz ${BINARY_URL}; 	  echo "${ESUM} */tmp/openjdk.tar.gz" | sha256sum -c -; 	  mkdir -p "$JAVA_HOME"; 	  tar --extract 	      --file /tmp/openjdk.tar.gz 	      --directory "$JAVA_HOME" 	      --strip-components 1 	      --no-same-owner 	  ;     rm -f /tmp/openjdk.tar.gz ${JAVA_HOME}/lib/src.zip;     find "$JAVA_HOME/lib" -name '*.so' -exec dirname '{}' ';' | sort -u > /etc/ld.so.conf.d/docker-openjdk.conf;     ldconfig;
# Thu, 17 Aug 2023 07:22:49 GMT
RUN echo Verifying install ...     && echo java -version && java -version     && echo Complete.
# Thu, 17 Aug 2023 07:22:50 GMT
COPY file:8b8864b3e02a33a579dc216fd51b28a6047bc8eeaa03045b258980fe0cf7fcb3 in /__cacert_entrypoint.sh 
# Thu, 17 Aug 2023 07:22:50 GMT
ENTRYPOINT ["/__cacert_entrypoint.sh"]
# Thu, 17 Aug 2023 12:47:11 GMT
ENV CATALINA_HOME=/usr/local/tomcat
# Thu, 17 Aug 2023 12:47:11 GMT
ENV PATH=/usr/local/tomcat/bin:/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 17 Aug 2023 12:47:12 GMT
RUN mkdir -p "$CATALINA_HOME"
# Thu, 17 Aug 2023 12:47:13 GMT
WORKDIR /usr/local/tomcat
# Thu, 17 Aug 2023 12:47:13 GMT
ENV TOMCAT_NATIVE_LIBDIR=/usr/local/tomcat/native-jni-lib
# Thu, 17 Aug 2023 12:47:13 GMT
ENV LD_LIBRARY_PATH=/usr/local/tomcat/native-jni-lib
# Thu, 17 Aug 2023 12:47:13 GMT
ENV GPG_KEYS=48F8E69F6390C9F25CFEDCD268248959359E722B A9C5DF4D22E99998D9875A5110C01C5A2F6059E7 DCFD35E0BF8CA7344752DE8B6FB21E8933C60243
# Thu, 17 Aug 2023 12:47:13 GMT
ENV TOMCAT_MAJOR=9
# Thu, 17 Aug 2023 12:47:14 GMT
ENV TOMCAT_VERSION=9.0.79
# Thu, 17 Aug 2023 12:47:14 GMT
ENV TOMCAT_SHA512=7a0d99b5fc37c9e9ac26b554fab9147ce0a2ba59fad41e2565b15e9f6e137bf0105f5c9cd6b7b508837ff24feb7b95b2aba49e0abc7b1480a30a11606e79802a
# Thu, 17 Aug 2023 12:47:15 GMT
COPY dir:5c848abb2e44267ee98218d715537833abdfc314a3d3507fb53532a8c8a8767a in /usr/local/tomcat 
# Thu, 17 Aug 2023 12:47:23 GMT
RUN set -eux; 	apt-get update; 	xargs -rt apt-get install -y --no-install-recommends < "$TOMCAT_NATIVE_LIBDIR/.dependencies.txt"; 	rm -rf /var/lib/apt/lists/*
# Thu, 17 Aug 2023 12:47:26 GMT
RUN set -eux; 	nativeLines="$(catalina.sh configtest 2>&1)"; 	nativeLines="$(echo "$nativeLines" | grep 'Apache Tomcat Native')"; 	nativeLines="$(echo "$nativeLines" | sort -u)"; 	if ! echo "$nativeLines" | grep -E 'INFO: Loaded( APR based)? Apache Tomcat Native library' >&2; then 		echo >&2 "$nativeLines"; 		exit 1; 	fi
# Thu, 17 Aug 2023 12:47:26 GMT
EXPOSE 8080
# Thu, 17 Aug 2023 12:47:26 GMT
ENTRYPOINT []
# Thu, 17 Aug 2023 12:47:27 GMT
CMD ["catalina.sh" "run"]
```

-	Layers:
	-	`sha256:09f4821f68917c7929419fff8bc583c406640180ea7d58eea03a95e463b8fb21`  
		Last Modified: Wed, 16 Aug 2023 02:15:01 GMT  
		Size: 35.7 MB (35712693 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9bf21ae1b3c5ce2350f829cd1faaad0127a2120d13c5833028ede5e9089d22bf`  
		Last Modified: Thu, 17 Aug 2023 07:26:45 GMT  
		Size: 13.8 MB (13770562 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:743257d4c1ea66345104cb7a4880ed045228dcc348a4d8beaacae180bd79d452`  
		Last Modified: Thu, 17 Aug 2023 07:27:28 GMT  
		Size: 41.2 MB (41229715 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a436e71d8177078b7eab3cc5313c8170ab47bc97e75c5abfee37b2ea3c5eab6b`  
		Last Modified: Thu, 17 Aug 2023 07:27:20 GMT  
		Size: 160.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7d73f08ecacec15962e21b7943751b973020b69b7282be734d3eec8cba52a313`  
		Last Modified: Thu, 17 Aug 2023 07:27:20 GMT  
		Size: 733.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:625daa53452d96a7a1c14d7ce5076220852f858290744070b1917dc5e63cff36`  
		Last Modified: Thu, 17 Aug 2023 13:03:39 GMT  
		Size: 173.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:09d5927e62c827a9e6bfb4513e7efdf5f814edc3e008569eac2d9f68c0b6b1d1`  
		Last Modified: Thu, 17 Aug 2023 13:03:51 GMT  
		Size: 12.3 MB (12310849 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cb9d8cf91b42a32ee74052da83795a8dc47285fe0caf4f538a8582f12bcccf7b`  
		Last Modified: Thu, 17 Aug 2023 13:03:39 GMT  
		Size: 486.9 KB (486902 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4eea5ba1e8d7e78d9a43a79c636d0a077bd48975b7d05e644ebbaaec72edcee4`  
		Last Modified: Thu, 17 Aug 2023 13:03:39 GMT  
		Size: 130.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
