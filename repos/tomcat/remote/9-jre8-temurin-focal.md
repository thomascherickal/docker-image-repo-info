## `tomcat:9-jre8-temurin-focal`

```console
$ docker pull tomcat@sha256:ae62ff82a604d4cc0e6ce980b6536e6c3e17d7b27af6a25d8b3e138f4b62729a
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 4
	-	linux; amd64
	-	linux; arm variant v7
	-	linux; arm64 variant v8
	-	linux; ppc64le

### `tomcat:9-jre8-temurin-focal` - linux; amd64

```console
$ docker pull tomcat@sha256:690383c821b16a1a4166b74cca3eb7b65a96470523792061f930855a9f13df2e
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **99.6 MB (99619221 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:63a19db10aef37efa4d5b0f59ecdd923e4aed59df265e28d83881946691af075`
-	Default Command: `["catalina.sh","run"]`

```dockerfile
# Wed, 28 Jun 2023 09:59:08 GMT
ARG RELEASE
# Wed, 28 Jun 2023 09:59:08 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Wed, 28 Jun 2023 09:59:08 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Wed, 28 Jun 2023 09:59:08 GMT
LABEL org.opencontainers.image.version=20.04
# Wed, 28 Jun 2023 09:59:10 GMT
ADD file:12f97b7b044d0d1166dd59408c67f5610a764127aa8a01bc57db23bee48911af in / 
# Wed, 28 Jun 2023 09:59:10 GMT
CMD ["/bin/bash"]
# Tue, 04 Jul 2023 20:33:00 GMT
ENV JAVA_HOME=/opt/java/openjdk
# Tue, 04 Jul 2023 20:33:00 GMT
ENV PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 04 Jul 2023 20:33:00 GMT
ENV LANG=en_US.UTF-8 LANGUAGE=en_US:en LC_ALL=en_US.UTF-8
# Tue, 04 Jul 2023 20:33:34 GMT
RUN apt-get update     && DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends tzdata curl wget ca-certificates fontconfig locales     && echo "en_US.UTF-8 UTF-8" >> /etc/locale.gen     && locale-gen en_US.UTF-8     && rm -rf /var/lib/apt/lists/*
# Tue, 04 Jul 2023 20:33:35 GMT
ENV JAVA_VERSION=jdk8u372-b07
# Tue, 04 Jul 2023 20:34:28 GMT
RUN set -eux;     ARCH="$(dpkg --print-architecture)";     case "${ARCH}" in        aarch64|arm64)          ESUM='f8e440273c8feb3fcfaca88ba18fec291deae18a548adde8a37cd1db08107b95';          BINARY_URL='https://github.com/adoptium/temurin8-binaries/releases/download/jdk8u372-b07/OpenJDK8U-jre_aarch64_linux_hotspot_8u372b07.tar.gz';          ;;        armhf|arm)          ESUM='e58e017012838ae4f0db78293e3246cc09958e6ea9a2393c5947ec003bf736dd';          BINARY_URL='https://github.com/adoptium/temurin8-binaries/releases/download/jdk8u372-b07/OpenJDK8U-jre_arm_linux_hotspot_8u372b07.tar.gz';          apt-get update          && DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends libatomic1          && rm -rf /var/lib/apt/lists/*          ;;        ppc64el|powerpc:common64)          ESUM='ba5f8141a16722e39576bf42b69d2b8ebf95fc2c05441e3200f609af4dd9f1ea';          BINARY_URL='https://github.com/adoptium/temurin8-binaries/releases/download/jdk8u372-b07/OpenJDK8U-jre_ppc64le_linux_hotspot_8u372b07.tar.gz';          ;;        amd64|i386:x86-64)          ESUM='b6fdfe32085a884c11b31f66aa67ac62811df7112fb6fb08beea61376a86fbb4';          BINARY_URL='https://github.com/adoptium/temurin8-binaries/releases/download/jdk8u372-b07/OpenJDK8U-jre_x64_linux_hotspot_8u372b07.tar.gz';          ;;        *)          echo "Unsupported arch: ${ARCH}";          exit 1;          ;;     esac; 	  wget -O /tmp/openjdk.tar.gz ${BINARY_URL}; 	  echo "${ESUM} */tmp/openjdk.tar.gz" | sha256sum -c -; 	  mkdir -p "$JAVA_HOME"; 	  tar --extract 	      --file /tmp/openjdk.tar.gz 	      --directory "$JAVA_HOME" 	      --strip-components 1 	      --no-same-owner 	  ;     rm -f /tmp/openjdk.tar.gz ${JAVA_HOME}/src.zip;     find "$JAVA_HOME/lib" -name '*.so' -exec dirname '{}' ';' | sort -u > /etc/ld.so.conf.d/docker-openjdk.conf;     ldconfig;
# Tue, 04 Jul 2023 20:34:29 GMT
RUN echo Verifying install ...     && echo java -version && java -version     && echo Complete.
# Wed, 05 Jul 2023 08:27:55 GMT
ENV CATALINA_HOME=/usr/local/tomcat
# Wed, 05 Jul 2023 08:27:55 GMT
ENV PATH=/usr/local/tomcat/bin:/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 05 Jul 2023 08:27:55 GMT
RUN mkdir -p "$CATALINA_HOME"
# Wed, 05 Jul 2023 08:27:55 GMT
WORKDIR /usr/local/tomcat
# Wed, 05 Jul 2023 08:27:55 GMT
ENV TOMCAT_NATIVE_LIBDIR=/usr/local/tomcat/native-jni-lib
# Wed, 05 Jul 2023 08:27:56 GMT
ENV LD_LIBRARY_PATH=/usr/local/tomcat/native-jni-lib
# Wed, 05 Jul 2023 08:27:56 GMT
ENV GPG_KEYS=48F8E69F6390C9F25CFEDCD268248959359E722B A9C5DF4D22E99998D9875A5110C01C5A2F6059E7 DCFD35E0BF8CA7344752DE8B6FB21E8933C60243
# Wed, 05 Jul 2023 08:27:56 GMT
ENV TOMCAT_MAJOR=9
# Tue, 11 Jul 2023 00:19:06 GMT
ENV TOMCAT_VERSION=9.0.78
# Tue, 11 Jul 2023 00:19:06 GMT
ENV TOMCAT_SHA512=c9f2e60489d07f25b53f715918f4b082c5bb69dbc497e0a9d3d5e3a0d351ff2e0ec8dfc5657de840ee5b3dea6174b27630033b38e36fa4c06b08664e70dec8df
# Tue, 11 Jul 2023 00:19:06 GMT
COPY dir:1cd14d16e9d065577b4b39ba1d8996d3fe4f1c04222a2df85916138304383c01 in /usr/local/tomcat 
# Tue, 11 Jul 2023 00:19:11 GMT
RUN set -eux; 	apt-get update; 	xargs -rt apt-get install -y --no-install-recommends < "$TOMCAT_NATIVE_LIBDIR/.dependencies.txt"; 	rm -rf /var/lib/apt/lists/*
# Tue, 11 Jul 2023 00:19:13 GMT
RUN set -eux; 	nativeLines="$(catalina.sh configtest 2>&1)"; 	nativeLines="$(echo "$nativeLines" | grep 'Apache Tomcat Native')"; 	nativeLines="$(echo "$nativeLines" | sort -u)"; 	if ! echo "$nativeLines" | grep -E 'INFO: Loaded( APR based)? Apache Tomcat Native library' >&2; then 		echo >&2 "$nativeLines"; 		exit 1; 	fi
# Tue, 11 Jul 2023 00:19:13 GMT
EXPOSE 8080
# Tue, 11 Jul 2023 00:19:13 GMT
CMD ["catalina.sh" "run"]
```

-	Layers:
	-	`sha256:0fb668748fc8bb961f4580895692ae741be788857ac2e8220adc2265ffb38e10`  
		Last Modified: Wed, 28 Jun 2023 18:43:28 GMT  
		Size: 28.6 MB (28580012 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e0c6314534fa2a3b454bddc0f12350fdd16cce9b09f979ce4c7fafd5ec679a69`  
		Last Modified: Tue, 04 Jul 2023 20:38:50 GMT  
		Size: 16.4 MB (16413467 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:87b76ff479c93205426b08c14b79be9ede864e4a601eee59e2aa53c9d1b84331`  
		Last Modified: Tue, 04 Jul 2023 20:39:27 GMT  
		Size: 41.8 MB (41837640 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0fe5e65faa453535c66e7d4e0bdbb200416e054693b3076a1ad9a98aaf2bdb94`  
		Last Modified: Tue, 04 Jul 2023 20:39:23 GMT  
		Size: 160.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cb3e7ebb33d61cf45ec29e4aa0d73de9a97f1d044bde68e014d0d6d50508bd4b`  
		Last Modified: Wed, 05 Jul 2023 08:41:16 GMT  
		Size: 173.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ece362f9d6fd017d116aff99a83d9b9b0763197c5a3b6bbc503e58100af3f7a3`  
		Last Modified: Tue, 11 Jul 2023 00:40:49 GMT  
		Size: 12.3 MB (12339035 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c729c7c7b23cf86b6d87d520ab161125adbefef09ecb75cecc90cd7015bb4812`  
		Last Modified: Tue, 11 Jul 2023 00:40:49 GMT  
		Size: 448.6 KB (448602 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6d423fd7cd7e8cc03ea9376ddedd098b42392d23559591cf3e23d32c8d658a66`  
		Last Modified: Tue, 11 Jul 2023 00:40:48 GMT  
		Size: 132.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `tomcat:9-jre8-temurin-focal` - linux; arm variant v7

```console
$ docker pull tomcat@sha256:5aabad62f5a97f6798bfa530a7b4169929731b3450c8e28be03aa6b0686871c7
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **92.1 MB (92096080 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a640977dd3e001b7e8cf1956b009b89f286933054af16150d4fc09065779200d`
-	Default Command: `["catalina.sh","run"]`

```dockerfile
# Wed, 28 Jun 2023 09:58:19 GMT
ARG RELEASE
# Wed, 28 Jun 2023 09:58:20 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Wed, 28 Jun 2023 09:58:20 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Wed, 28 Jun 2023 09:58:20 GMT
LABEL org.opencontainers.image.version=20.04
# Wed, 28 Jun 2023 09:58:22 GMT
ADD file:8bedca16bf416520f5df29175a99b07585281465c459544b9f9679016f59762a in / 
# Wed, 28 Jun 2023 09:58:22 GMT
CMD ["/bin/bash"]
# Tue, 04 Jul 2023 20:08:56 GMT
ENV JAVA_HOME=/opt/java/openjdk
# Tue, 04 Jul 2023 20:08:56 GMT
ENV PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 04 Jul 2023 20:08:56 GMT
ENV LANG=en_US.UTF-8 LANGUAGE=en_US:en LC_ALL=en_US.UTF-8
# Tue, 04 Jul 2023 20:09:13 GMT
RUN apt-get update     && DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends tzdata curl wget ca-certificates fontconfig locales     && echo "en_US.UTF-8 UTF-8" >> /etc/locale.gen     && locale-gen en_US.UTF-8     && rm -rf /var/lib/apt/lists/*
# Tue, 04 Jul 2023 20:09:14 GMT
ENV JAVA_VERSION=jdk8u372-b07
# Tue, 04 Jul 2023 20:10:17 GMT
RUN set -eux;     ARCH="$(dpkg --print-architecture)";     case "${ARCH}" in        aarch64|arm64)          ESUM='f8e440273c8feb3fcfaca88ba18fec291deae18a548adde8a37cd1db08107b95';          BINARY_URL='https://github.com/adoptium/temurin8-binaries/releases/download/jdk8u372-b07/OpenJDK8U-jre_aarch64_linux_hotspot_8u372b07.tar.gz';          ;;        armhf|arm)          ESUM='e58e017012838ae4f0db78293e3246cc09958e6ea9a2393c5947ec003bf736dd';          BINARY_URL='https://github.com/adoptium/temurin8-binaries/releases/download/jdk8u372-b07/OpenJDK8U-jre_arm_linux_hotspot_8u372b07.tar.gz';          apt-get update          && DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends libatomic1          && rm -rf /var/lib/apt/lists/*          ;;        ppc64el|powerpc:common64)          ESUM='ba5f8141a16722e39576bf42b69d2b8ebf95fc2c05441e3200f609af4dd9f1ea';          BINARY_URL='https://github.com/adoptium/temurin8-binaries/releases/download/jdk8u372-b07/OpenJDK8U-jre_ppc64le_linux_hotspot_8u372b07.tar.gz';          ;;        amd64|i386:x86-64)          ESUM='b6fdfe32085a884c11b31f66aa67ac62811df7112fb6fb08beea61376a86fbb4';          BINARY_URL='https://github.com/adoptium/temurin8-binaries/releases/download/jdk8u372-b07/OpenJDK8U-jre_x64_linux_hotspot_8u372b07.tar.gz';          ;;        *)          echo "Unsupported arch: ${ARCH}";          exit 1;          ;;     esac; 	  wget -O /tmp/openjdk.tar.gz ${BINARY_URL}; 	  echo "${ESUM} */tmp/openjdk.tar.gz" | sha256sum -c -; 	  mkdir -p "$JAVA_HOME"; 	  tar --extract 	      --file /tmp/openjdk.tar.gz 	      --directory "$JAVA_HOME" 	      --strip-components 1 	      --no-same-owner 	  ;     rm -f /tmp/openjdk.tar.gz ${JAVA_HOME}/src.zip;     find "$JAVA_HOME/lib" -name '*.so' -exec dirname '{}' ';' | sort -u > /etc/ld.so.conf.d/docker-openjdk.conf;     ldconfig;
# Tue, 04 Jul 2023 20:10:18 GMT
RUN echo Verifying install ...     && echo java -version && java -version     && echo Complete.
# Wed, 05 Jul 2023 05:38:46 GMT
ENV CATALINA_HOME=/usr/local/tomcat
# Wed, 05 Jul 2023 05:38:47 GMT
ENV PATH=/usr/local/tomcat/bin:/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 05 Jul 2023 05:38:47 GMT
RUN mkdir -p "$CATALINA_HOME"
# Wed, 05 Jul 2023 05:38:47 GMT
WORKDIR /usr/local/tomcat
# Wed, 05 Jul 2023 05:38:47 GMT
ENV TOMCAT_NATIVE_LIBDIR=/usr/local/tomcat/native-jni-lib
# Wed, 05 Jul 2023 05:38:47 GMT
ENV LD_LIBRARY_PATH=/usr/local/tomcat/native-jni-lib
# Wed, 05 Jul 2023 05:38:47 GMT
ENV GPG_KEYS=48F8E69F6390C9F25CFEDCD268248959359E722B A9C5DF4D22E99998D9875A5110C01C5A2F6059E7 DCFD35E0BF8CA7344752DE8B6FB21E8933C60243
# Wed, 05 Jul 2023 05:38:47 GMT
ENV TOMCAT_MAJOR=9
# Tue, 11 Jul 2023 05:14:18 GMT
ENV TOMCAT_VERSION=9.0.78
# Tue, 11 Jul 2023 05:14:18 GMT
ENV TOMCAT_SHA512=c9f2e60489d07f25b53f715918f4b082c5bb69dbc497e0a9d3d5e3a0d351ff2e0ec8dfc5657de840ee5b3dea6174b27630033b38e36fa4c06b08664e70dec8df
# Tue, 11 Jul 2023 05:14:18 GMT
COPY dir:5612d7286681c733ac8fe2c85a7b11971e7d4557322af0f4709c5e88195778ea in /usr/local/tomcat 
# Tue, 11 Jul 2023 05:14:22 GMT
RUN set -eux; 	apt-get update; 	xargs -rt apt-get install -y --no-install-recommends < "$TOMCAT_NATIVE_LIBDIR/.dependencies.txt"; 	rm -rf /var/lib/apt/lists/*
# Tue, 11 Jul 2023 05:14:24 GMT
RUN set -eux; 	nativeLines="$(catalina.sh configtest 2>&1)"; 	nativeLines="$(echo "$nativeLines" | grep 'Apache Tomcat Native')"; 	nativeLines="$(echo "$nativeLines" | sort -u)"; 	if ! echo "$nativeLines" | grep -E 'INFO: Loaded( APR based)? Apache Tomcat Native library' >&2; then 		echo >&2 "$nativeLines"; 		exit 1; 	fi
# Tue, 11 Jul 2023 05:14:24 GMT
EXPOSE 8080
# Tue, 11 Jul 2023 05:14:24 GMT
CMD ["catalina.sh" "run"]
```

-	Layers:
	-	`sha256:06e53fabee8df31622850c604f9242a52a466ec4eb75320019bdfdc8ec311692`  
		Last Modified: Tue, 04 Jul 2023 06:22:20 GMT  
		Size: 24.6 MB (24588135 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c0186b47b0f035fc3bcf39b19dfd039f6fa8694a7e17ba90a3fc477b5753c106`  
		Last Modified: Tue, 04 Jul 2023 20:13:22 GMT  
		Size: 15.2 MB (15239799 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:46108a468090682cd2e7d0a673ea50c7b9c6df2f7650acdd0bf57ec7780ccea2`  
		Last Modified: Tue, 04 Jul 2023 20:13:58 GMT  
		Size: 39.6 MB (39552808 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b1c382716a3eca22f35c8e6ca7f99b1aa161f2b29bf71502c745f119c7132c7e`  
		Last Modified: Tue, 04 Jul 2023 20:13:54 GMT  
		Size: 162.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:562d3d3d74c127e0bd8229345d606f684ea85ae444eb74fcb1387d33ae1fe223`  
		Last Modified: Wed, 05 Jul 2023 05:50:44 GMT  
		Size: 171.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7237ba80b05a6616adf3de5235a2c2a7f1144494fb0c6a72cb1c17e68ec2cc67`  
		Last Modified: Tue, 11 Jul 2023 05:26:47 GMT  
		Size: 12.3 MB (12289808 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:89c5e26a3372649e9ae48e90cb3d28715bfbb9a465d84c576b2cbcc89b5442dc`  
		Last Modified: Tue, 11 Jul 2023 05:26:46 GMT  
		Size: 425.1 KB (425065 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:92b5d0b1ca482dc019f4148f8846fd17b9e6d9aec8daf83c5049e2ba73b5124d`  
		Last Modified: Tue, 11 Jul 2023 05:26:46 GMT  
		Size: 132.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `tomcat:9-jre8-temurin-focal` - linux; arm64 variant v8

```console
$ docker pull tomcat@sha256:5a313dea7561c22adaaf8ee9bdc32d6ffe0f878c9e056296ed3e8282d23a0c71
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **97.1 MB (97094784 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:86ebae9d0d3ad69daef82bfb0b29085fb254836d10c994a6f3cc5c0636bd9614`
-	Default Command: `["catalina.sh","run"]`

```dockerfile
# Wed, 28 Jun 2023 09:54:46 GMT
ARG RELEASE
# Wed, 28 Jun 2023 09:54:46 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Wed, 28 Jun 2023 09:54:46 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Wed, 28 Jun 2023 09:54:46 GMT
LABEL org.opencontainers.image.version=20.04
# Wed, 28 Jun 2023 09:54:48 GMT
ADD file:a6db9f7789e57b7119f68e4e4ec9ec5aab8c3c8bd53fd932f3c59c54b1c20a26 in / 
# Wed, 28 Jun 2023 09:54:49 GMT
CMD ["/bin/bash"]
# Tue, 04 Jul 2023 15:32:11 GMT
ENV JAVA_HOME=/opt/java/openjdk
# Tue, 04 Jul 2023 15:32:12 GMT
ENV PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 04 Jul 2023 15:32:12 GMT
ENV LANG=en_US.UTF-8 LANGUAGE=en_US:en LC_ALL=en_US.UTF-8
# Tue, 04 Jul 2023 15:32:32 GMT
RUN apt-get update     && DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends tzdata curl wget ca-certificates fontconfig locales     && echo "en_US.UTF-8 UTF-8" >> /etc/locale.gen     && locale-gen en_US.UTF-8     && rm -rf /var/lib/apt/lists/*
# Tue, 04 Jul 2023 15:32:32 GMT
ENV JAVA_VERSION=jdk8u372-b07
# Tue, 04 Jul 2023 15:33:14 GMT
RUN set -eux;     ARCH="$(dpkg --print-architecture)";     case "${ARCH}" in        aarch64|arm64)          ESUM='f8e440273c8feb3fcfaca88ba18fec291deae18a548adde8a37cd1db08107b95';          BINARY_URL='https://github.com/adoptium/temurin8-binaries/releases/download/jdk8u372-b07/OpenJDK8U-jre_aarch64_linux_hotspot_8u372b07.tar.gz';          ;;        armhf|arm)          ESUM='e58e017012838ae4f0db78293e3246cc09958e6ea9a2393c5947ec003bf736dd';          BINARY_URL='https://github.com/adoptium/temurin8-binaries/releases/download/jdk8u372-b07/OpenJDK8U-jre_arm_linux_hotspot_8u372b07.tar.gz';          apt-get update          && DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends libatomic1          && rm -rf /var/lib/apt/lists/*          ;;        ppc64el|powerpc:common64)          ESUM='ba5f8141a16722e39576bf42b69d2b8ebf95fc2c05441e3200f609af4dd9f1ea';          BINARY_URL='https://github.com/adoptium/temurin8-binaries/releases/download/jdk8u372-b07/OpenJDK8U-jre_ppc64le_linux_hotspot_8u372b07.tar.gz';          ;;        amd64|i386:x86-64)          ESUM='b6fdfe32085a884c11b31f66aa67ac62811df7112fb6fb08beea61376a86fbb4';          BINARY_URL='https://github.com/adoptium/temurin8-binaries/releases/download/jdk8u372-b07/OpenJDK8U-jre_x64_linux_hotspot_8u372b07.tar.gz';          ;;        *)          echo "Unsupported arch: ${ARCH}";          exit 1;          ;;     esac; 	  wget -O /tmp/openjdk.tar.gz ${BINARY_URL}; 	  echo "${ESUM} */tmp/openjdk.tar.gz" | sha256sum -c -; 	  mkdir -p "$JAVA_HOME"; 	  tar --extract 	      --file /tmp/openjdk.tar.gz 	      --directory "$JAVA_HOME" 	      --strip-components 1 	      --no-same-owner 	  ;     rm -f /tmp/openjdk.tar.gz ${JAVA_HOME}/src.zip;     find "$JAVA_HOME/lib" -name '*.so' -exec dirname '{}' ';' | sort -u > /etc/ld.so.conf.d/docker-openjdk.conf;     ldconfig;
# Tue, 04 Jul 2023 15:33:15 GMT
RUN echo Verifying install ...     && echo java -version && java -version     && echo Complete.
# Wed, 05 Jul 2023 03:02:51 GMT
ENV CATALINA_HOME=/usr/local/tomcat
# Wed, 05 Jul 2023 03:02:51 GMT
ENV PATH=/usr/local/tomcat/bin:/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 05 Jul 2023 03:02:52 GMT
RUN mkdir -p "$CATALINA_HOME"
# Wed, 05 Jul 2023 03:02:52 GMT
WORKDIR /usr/local/tomcat
# Wed, 05 Jul 2023 03:02:52 GMT
ENV TOMCAT_NATIVE_LIBDIR=/usr/local/tomcat/native-jni-lib
# Wed, 05 Jul 2023 03:02:52 GMT
ENV LD_LIBRARY_PATH=/usr/local/tomcat/native-jni-lib
# Wed, 05 Jul 2023 03:02:52 GMT
ENV GPG_KEYS=48F8E69F6390C9F25CFEDCD268248959359E722B A9C5DF4D22E99998D9875A5110C01C5A2F6059E7 DCFD35E0BF8CA7344752DE8B6FB21E8933C60243
# Wed, 05 Jul 2023 03:02:52 GMT
ENV TOMCAT_MAJOR=9
# Tue, 11 Jul 2023 01:21:38 GMT
ENV TOMCAT_VERSION=9.0.78
# Tue, 11 Jul 2023 01:21:38 GMT
ENV TOMCAT_SHA512=c9f2e60489d07f25b53f715918f4b082c5bb69dbc497e0a9d3d5e3a0d351ff2e0ec8dfc5657de840ee5b3dea6174b27630033b38e36fa4c06b08664e70dec8df
# Tue, 11 Jul 2023 01:21:38 GMT
COPY dir:f131c71d14ac3b930ea444762b8e70abd72d85695fc7911850306899f02be03b in /usr/local/tomcat 
# Tue, 11 Jul 2023 01:21:43 GMT
RUN set -eux; 	apt-get update; 	xargs -rt apt-get install -y --no-install-recommends < "$TOMCAT_NATIVE_LIBDIR/.dependencies.txt"; 	rm -rf /var/lib/apt/lists/*
# Tue, 11 Jul 2023 01:21:44 GMT
RUN set -eux; 	nativeLines="$(catalina.sh configtest 2>&1)"; 	nativeLines="$(echo "$nativeLines" | grep 'Apache Tomcat Native')"; 	nativeLines="$(echo "$nativeLines" | sort -u)"; 	if ! echo "$nativeLines" | grep -E 'INFO: Loaded( APR based)? Apache Tomcat Native library' >&2; then 		echo >&2 "$nativeLines"; 		exit 1; 	fi
# Tue, 11 Jul 2023 01:21:44 GMT
EXPOSE 8080
# Tue, 11 Jul 2023 01:21:44 GMT
CMD ["catalina.sh" "run"]
```

-	Layers:
	-	`sha256:1e77eb131c5c9032ce8e6e512f601714ce7ba48e296f5b7a5191703bdcbc904d`  
		Last Modified: Tue, 04 Jul 2023 04:05:23 GMT  
		Size: 27.2 MB (27198330 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f18a6ed3004a374532e52161ba803de458ea0c89faf66c28c12d9858ee1796c1`  
		Last Modified: Tue, 04 Jul 2023 15:36:40 GMT  
		Size: 16.3 MB (16268149 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b8947b151acba43145ea8fba1014dedcab8a14635b00d7d9f4e3dffec9b6949a`  
		Last Modified: Tue, 04 Jul 2023 15:37:14 GMT  
		Size: 40.8 MB (40821398 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c406990b3dfa76a00d7e24ddded8d0cf99e50d5dd230626d5c81de8366e96bac`  
		Last Modified: Tue, 04 Jul 2023 15:37:10 GMT  
		Size: 162.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:01cd2d944ce4457fc315a13c6140e19a1c511ff5f4be79c07d63a90b1efc1f8b`  
		Last Modified: Wed, 05 Jul 2023 03:19:20 GMT  
		Size: 172.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0398b1c57f70017dd886eaab7edb940d31c55c9e640bfe4c458210042a3f935c`  
		Last Modified: Tue, 11 Jul 2023 01:41:29 GMT  
		Size: 12.4 MB (12357682 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:67be4ab7e58cd464a2fc344f79001a5dcc3b980737f4049d0b3ca1726d4d573f`  
		Last Modified: Tue, 11 Jul 2023 01:41:29 GMT  
		Size: 448.8 KB (448761 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:29eb489f3cda2e1111f5e4ee4554326662a81116637ff64d4b1eeb857ab4a521`  
		Last Modified: Tue, 11 Jul 2023 01:41:28 GMT  
		Size: 130.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `tomcat:9-jre8-temurin-focal` - linux; ppc64le

```console
$ docker pull tomcat@sha256:79b30f774cd5d63b1bd07880147d57a4bd1d701376bf2b28c91a9f7b530b2596
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **105.0 MB (105045684 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:eb2f3fedd78d4d688166bbc3994a6e839b00fb5f57c91d91d5bf1b21042996be`
-	Default Command: `["catalina.sh","run"]`

```dockerfile
# Wed, 28 Jun 2023 10:04:43 GMT
ARG RELEASE
# Wed, 28 Jun 2023 10:04:43 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Wed, 28 Jun 2023 10:04:43 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Wed, 28 Jun 2023 10:04:43 GMT
LABEL org.opencontainers.image.version=20.04
# Wed, 28 Jun 2023 10:04:46 GMT
ADD file:df651ead0b69eb261098e765354dbdf5ffca51275c037d8881fedcaa1c91c36d in / 
# Wed, 28 Jun 2023 10:04:46 GMT
CMD ["/bin/bash"]
# Wed, 05 Jul 2023 00:16:24 GMT
ENV JAVA_HOME=/opt/java/openjdk
# Wed, 05 Jul 2023 00:16:25 GMT
ENV PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 05 Jul 2023 00:16:26 GMT
ENV LANG=en_US.UTF-8 LANGUAGE=en_US:en LC_ALL=en_US.UTF-8
# Wed, 05 Jul 2023 00:17:45 GMT
RUN apt-get update     && DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends tzdata curl wget ca-certificates fontconfig locales     && echo "en_US.UTF-8 UTF-8" >> /etc/locale.gen     && locale-gen en_US.UTF-8     && rm -rf /var/lib/apt/lists/*
# Wed, 05 Jul 2023 00:17:46 GMT
ENV JAVA_VERSION=jdk8u372-b07
# Wed, 05 Jul 2023 00:20:10 GMT
RUN set -eux;     ARCH="$(dpkg --print-architecture)";     case "${ARCH}" in        aarch64|arm64)          ESUM='f8e440273c8feb3fcfaca88ba18fec291deae18a548adde8a37cd1db08107b95';          BINARY_URL='https://github.com/adoptium/temurin8-binaries/releases/download/jdk8u372-b07/OpenJDK8U-jre_aarch64_linux_hotspot_8u372b07.tar.gz';          ;;        armhf|arm)          ESUM='e58e017012838ae4f0db78293e3246cc09958e6ea9a2393c5947ec003bf736dd';          BINARY_URL='https://github.com/adoptium/temurin8-binaries/releases/download/jdk8u372-b07/OpenJDK8U-jre_arm_linux_hotspot_8u372b07.tar.gz';          apt-get update          && DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends libatomic1          && rm -rf /var/lib/apt/lists/*          ;;        ppc64el|powerpc:common64)          ESUM='ba5f8141a16722e39576bf42b69d2b8ebf95fc2c05441e3200f609af4dd9f1ea';          BINARY_URL='https://github.com/adoptium/temurin8-binaries/releases/download/jdk8u372-b07/OpenJDK8U-jre_ppc64le_linux_hotspot_8u372b07.tar.gz';          ;;        amd64|i386:x86-64)          ESUM='b6fdfe32085a884c11b31f66aa67ac62811df7112fb6fb08beea61376a86fbb4';          BINARY_URL='https://github.com/adoptium/temurin8-binaries/releases/download/jdk8u372-b07/OpenJDK8U-jre_x64_linux_hotspot_8u372b07.tar.gz';          ;;        *)          echo "Unsupported arch: ${ARCH}";          exit 1;          ;;     esac; 	  wget -O /tmp/openjdk.tar.gz ${BINARY_URL}; 	  echo "${ESUM} */tmp/openjdk.tar.gz" | sha256sum -c -; 	  mkdir -p "$JAVA_HOME"; 	  tar --extract 	      --file /tmp/openjdk.tar.gz 	      --directory "$JAVA_HOME" 	      --strip-components 1 	      --no-same-owner 	  ;     rm -f /tmp/openjdk.tar.gz ${JAVA_HOME}/src.zip;     find "$JAVA_HOME/lib" -name '*.so' -exec dirname '{}' ';' | sort -u > /etc/ld.so.conf.d/docker-openjdk.conf;     ldconfig;
# Wed, 05 Jul 2023 00:20:13 GMT
RUN echo Verifying install ...     && echo java -version && java -version     && echo Complete.
# Wed, 05 Jul 2023 18:10:08 GMT
ENV CATALINA_HOME=/usr/local/tomcat
# Wed, 05 Jul 2023 18:10:09 GMT
ENV PATH=/usr/local/tomcat/bin:/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 05 Jul 2023 18:10:10 GMT
RUN mkdir -p "$CATALINA_HOME"
# Wed, 05 Jul 2023 18:10:11 GMT
WORKDIR /usr/local/tomcat
# Wed, 05 Jul 2023 18:10:12 GMT
ENV TOMCAT_NATIVE_LIBDIR=/usr/local/tomcat/native-jni-lib
# Wed, 05 Jul 2023 18:10:12 GMT
ENV LD_LIBRARY_PATH=/usr/local/tomcat/native-jni-lib
# Wed, 05 Jul 2023 18:10:13 GMT
ENV GPG_KEYS=48F8E69F6390C9F25CFEDCD268248959359E722B A9C5DF4D22E99998D9875A5110C01C5A2F6059E7 DCFD35E0BF8CA7344752DE8B6FB21E8933C60243
# Wed, 05 Jul 2023 18:10:14 GMT
ENV TOMCAT_MAJOR=9
# Tue, 11 Jul 2023 08:54:39 GMT
ENV TOMCAT_VERSION=9.0.78
# Tue, 11 Jul 2023 08:54:40 GMT
ENV TOMCAT_SHA512=c9f2e60489d07f25b53f715918f4b082c5bb69dbc497e0a9d3d5e3a0d351ff2e0ec8dfc5657de840ee5b3dea6174b27630033b38e36fa4c06b08664e70dec8df
# Tue, 11 Jul 2023 08:54:41 GMT
COPY dir:0c4719a8a137e21b2c74f17b694ef40cb84a0a5cf9a44115a46cb8d4b42b7fda in /usr/local/tomcat 
# Tue, 11 Jul 2023 08:55:03 GMT
RUN set -eux; 	apt-get update; 	xargs -rt apt-get install -y --no-install-recommends < "$TOMCAT_NATIVE_LIBDIR/.dependencies.txt"; 	rm -rf /var/lib/apt/lists/*
# Tue, 11 Jul 2023 08:55:21 GMT
RUN set -eux; 	nativeLines="$(catalina.sh configtest 2>&1)"; 	nativeLines="$(echo "$nativeLines" | grep 'Apache Tomcat Native')"; 	nativeLines="$(echo "$nativeLines" | sort -u)"; 	if ! echo "$nativeLines" | grep -E 'INFO: Loaded( APR based)? Apache Tomcat Native library' >&2; then 		echo >&2 "$nativeLines"; 		exit 1; 	fi
# Tue, 11 Jul 2023 08:55:21 GMT
EXPOSE 8080
# Tue, 11 Jul 2023 08:55:24 GMT
CMD ["catalina.sh" "run"]
```

-	Layers:
	-	`sha256:4e95615eadb7a0d90a47ca15a5c0693371494902f54d8d78a50d53e89e7a20de`  
		Last Modified: Tue, 04 Jul 2023 04:40:49 GMT  
		Size: 33.3 MB (33308759 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:900a3bee385ed74b6117be4963259e4ef65f261ee58fc971b7206f32acb0572b`  
		Last Modified: Wed, 05 Jul 2023 00:27:54 GMT  
		Size: 17.6 MB (17648843 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:15478ccefefb96197ef02f10a8c1a8cdb9bc0406f8e8f8284c45c17c57e0845c`  
		Last Modified: Wed, 05 Jul 2023 00:28:54 GMT  
		Size: 41.2 MB (41232958 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e4653f5978add8f5d7ca79945725093bc8caec640275a43bdf97a276dcc64864`  
		Last Modified: Wed, 05 Jul 2023 00:28:46 GMT  
		Size: 160.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d79e01859a06e56f3690e9860549ab37e7fae31fbc7820103947ca806e1a3f6a`  
		Last Modified: Wed, 05 Jul 2023 18:37:01 GMT  
		Size: 171.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c4e9ec960097713fdb2dfa78aa22486c984816693a66159aa70cb68469d449ca`  
		Last Modified: Tue, 11 Jul 2023 09:34:02 GMT  
		Size: 12.4 MB (12380345 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d0621c357f4cd4e2e59534c744faeec0005a277f7aab098b907a055aaa138d94`  
		Last Modified: Tue, 11 Jul 2023 09:34:00 GMT  
		Size: 474.3 KB (474318 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4769cb01b62edc2529927f15698e0bd3f4e2b77b96a770cb59ed87368458f991`  
		Last Modified: Tue, 11 Jul 2023 09:34:00 GMT  
		Size: 130.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
