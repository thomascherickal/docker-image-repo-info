## `eclipse-temurin:8-jdk`

```console
$ docker pull eclipse-temurin@sha256:a239363b3c5f06ce52fd2cfd50c6d092c33400ba827842e49f206c72e5a7b287
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 6
	-	linux; amd64
	-	linux; arm variant v7
	-	linux; arm64 variant v8
	-	linux; ppc64le
	-	windows version 10.0.20348.1906; amd64
	-	windows version 10.0.17763.4737; amd64

### `eclipse-temurin:8-jdk` - linux; amd64

```console
$ docker pull eclipse-temurin@sha256:4cc902119753d44b3581647395db332d9496e21ad8799902cd4c33de0e5b84cf
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **146.9 MB (146931329 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d34accc95da2538ac2a3b1d6b1a4181151836d317799796e5b54b42073e960bd`
-	Entrypoint: `["\/__cacert_entrypoint.sh"]`

```dockerfile
# Wed, 16 Aug 2023 06:01:52 GMT
ARG RELEASE
# Wed, 16 Aug 2023 06:01:52 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Wed, 16 Aug 2023 06:01:52 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Wed, 16 Aug 2023 06:01:52 GMT
LABEL org.opencontainers.image.version=22.04
# Wed, 16 Aug 2023 06:01:54 GMT
ADD file:aa9b51e9f0067860cebbc9930374452d1384ec3c59badb5e4733130eedc90329 in / 
# Wed, 16 Aug 2023 06:01:54 GMT
CMD ["/bin/bash"]
# Sat, 02 Sep 2023 00:37:45 GMT
ENV JAVA_HOME=/opt/java/openjdk
# Sat, 02 Sep 2023 00:37:45 GMT
ENV PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Sat, 02 Sep 2023 00:37:45 GMT
ENV LANG=en_US.UTF-8 LANGUAGE=en_US:en LC_ALL=en_US.UTF-8
# Sat, 02 Sep 2023 00:37:58 GMT
RUN apt-get update     && DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends tzdata curl wget ca-certificates fontconfig locales p11-kit     && echo "en_US.UTF-8 UTF-8" >> /etc/locale.gen     && locale-gen en_US.UTF-8     && rm -rf /var/lib/apt/lists/*
# Sat, 02 Sep 2023 00:37:58 GMT
ENV JAVA_VERSION=jdk8u382-b05
# Sat, 02 Sep 2023 00:38:04 GMT
RUN set -eux;     ARCH="$(dpkg --print-architecture)";     case "${ARCH}" in        aarch64|arm64)          ESUM='0951398197b7bef39ab987b59c22852812ee2c2da6549953eed7fced4c08e13d';          BINARY_URL='https://github.com/adoptium/temurin8-binaries/releases/download/jdk8u382-b05/OpenJDK8U-jdk_aarch64_linux_hotspot_8u382b05.tar.gz';          ;;        armhf|arm)          ESUM='5d805ff157f272acf0f7d192f21af4a3b68c840333ca95568e4e07142efc369d';          BINARY_URL='https://github.com/adoptium/temurin8-binaries/releases/download/jdk8u382-b05/OpenJDK8U-jdk_arm_linux_hotspot_8u382b05.tar.gz';          apt-get update          && DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends libatomic1          && rm -rf /var/lib/apt/lists/*          ;;        ppc64el|powerpc:common64)          ESUM='509c923c308d1f4f28fd0068831a59250a05b8ca173ca92fb2be2e2e1f9ff3f9';          BINARY_URL='https://github.com/adoptium/temurin8-binaries/releases/download/jdk8u382-b05/OpenJDK8U-jdk_ppc64le_linux_hotspot_8u382b05.tar.gz';          ;;        amd64|i386:x86-64)          ESUM='789ad24dc0d9618294e3ba564c9bfda9d3f3a218604350e0ce0381bbc8f28db3';          BINARY_URL='https://github.com/adoptium/temurin8-binaries/releases/download/jdk8u382-b05/OpenJDK8U-jdk_x64_linux_hotspot_8u382b05.tar.gz';          ;;        *)          echo "Unsupported arch: ${ARCH}";          exit 1;          ;;     esac; 	  wget -O /tmp/openjdk.tar.gz ${BINARY_URL}; 	  echo "${ESUM} */tmp/openjdk.tar.gz" | sha256sum -c -; 	  mkdir -p "$JAVA_HOME"; 	  tar --extract 	      --file /tmp/openjdk.tar.gz 	      --directory "$JAVA_HOME" 	      --strip-components 1 	      --no-same-owner 	  ;     rm -f /tmp/openjdk.tar.gz ${JAVA_HOME}/lib/src.zip;     find "$JAVA_HOME/lib" -name '*.so' -exec dirname '{}' ';' | sort -u > /etc/ld.so.conf.d/docker-openjdk.conf;     ldconfig;
# Sat, 02 Sep 2023 00:38:05 GMT
RUN echo Verifying install ...     && echo javac -version && javac -version     && echo java -version && java -version     && echo Complete.
# Sat, 02 Sep 2023 00:38:05 GMT
COPY file:8b8864b3e02a33a579dc216fd51b28a6047bc8eeaa03045b258980fe0cf7fcb3 in /__cacert_entrypoint.sh 
# Sat, 02 Sep 2023 00:38:05 GMT
ENTRYPOINT ["/__cacert_entrypoint.sh"]
```

-	Layers:
	-	`sha256:44ba2882f8eb14264e5f2f9f6ec55bcf5306527b637279f2cd9d4858762388af`  
		Last Modified: Wed, 16 Aug 2023 10:32:51 GMT  
		Size: 30.4 MB (30438977 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:274fb0278626020650ff7c358074255903c792176a61a1ebce3055ba27e11436`  
		Last Modified: Sat, 02 Sep 2023 00:41:34 GMT  
		Size: 12.9 MB (12902882 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:11ad034c908965635a64fab34307a658280a305549ae76fa885e0d3aed44ed4d`  
		Last Modified: Sat, 02 Sep 2023 00:41:40 GMT  
		Size: 103.6 MB (103588579 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:96082a3fe734749b7256bffdf8e8aeca730269b34b313b250143d58f1352d99a`  
		Last Modified: Sat, 02 Sep 2023 00:41:31 GMT  
		Size: 158.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:053cb8db5f878f8abdfac5d22052688868723a0a412111faca43a82b4141cd9e`  
		Last Modified: Sat, 02 Sep 2023 00:41:31 GMT  
		Size: 733.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `eclipse-temurin:8-jdk` - linux; arm variant v7

```console
$ docker pull eclipse-temurin@sha256:7abed7ca9a94e63698f9b6176b0f474d807d456a7c242cf830cca5fbfe898078
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **138.7 MB (138744196 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b0cd6b1e00e9a54ad174dda16f48851e3958a860f983063ff483422214641542`
-	Entrypoint: `["\/__cacert_entrypoint.sh"]`

```dockerfile
# Wed, 16 Aug 2023 06:08:27 GMT
ARG RELEASE
# Wed, 16 Aug 2023 06:08:27 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Wed, 16 Aug 2023 06:08:27 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Wed, 16 Aug 2023 06:08:27 GMT
LABEL org.opencontainers.image.version=22.04
# Wed, 16 Aug 2023 06:08:32 GMT
ADD file:e61c6bbfc8728cb119b4cfd4a35d1e5aad76e84c0ac8f2ff9850a7ceec9f3dc5 in / 
# Wed, 16 Aug 2023 06:08:32 GMT
CMD ["/bin/bash"]
# Fri, 01 Sep 2023 23:34:53 GMT
ENV JAVA_HOME=/opt/java/openjdk
# Fri, 01 Sep 2023 23:34:53 GMT
ENV PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Fri, 01 Sep 2023 23:34:53 GMT
ENV LANG=en_US.UTF-8 LANGUAGE=en_US:en LC_ALL=en_US.UTF-8
# Fri, 01 Sep 2023 23:35:38 GMT
RUN apt-get update     && DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends tzdata curl wget ca-certificates fontconfig locales p11-kit     && echo "en_US.UTF-8 UTF-8" >> /etc/locale.gen     && locale-gen en_US.UTF-8     && rm -rf /var/lib/apt/lists/*
# Fri, 01 Sep 2023 23:35:38 GMT
ENV JAVA_VERSION=jdk8u382-b05
# Fri, 01 Sep 2023 23:35:49 GMT
RUN set -eux;     ARCH="$(dpkg --print-architecture)";     case "${ARCH}" in        aarch64|arm64)          ESUM='0951398197b7bef39ab987b59c22852812ee2c2da6549953eed7fced4c08e13d';          BINARY_URL='https://github.com/adoptium/temurin8-binaries/releases/download/jdk8u382-b05/OpenJDK8U-jdk_aarch64_linux_hotspot_8u382b05.tar.gz';          ;;        armhf|arm)          ESUM='5d805ff157f272acf0f7d192f21af4a3b68c840333ca95568e4e07142efc369d';          BINARY_URL='https://github.com/adoptium/temurin8-binaries/releases/download/jdk8u382-b05/OpenJDK8U-jdk_arm_linux_hotspot_8u382b05.tar.gz';          apt-get update          && DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends libatomic1          && rm -rf /var/lib/apt/lists/*          ;;        ppc64el|powerpc:common64)          ESUM='509c923c308d1f4f28fd0068831a59250a05b8ca173ca92fb2be2e2e1f9ff3f9';          BINARY_URL='https://github.com/adoptium/temurin8-binaries/releases/download/jdk8u382-b05/OpenJDK8U-jdk_ppc64le_linux_hotspot_8u382b05.tar.gz';          ;;        amd64|i386:x86-64)          ESUM='789ad24dc0d9618294e3ba564c9bfda9d3f3a218604350e0ce0381bbc8f28db3';          BINARY_URL='https://github.com/adoptium/temurin8-binaries/releases/download/jdk8u382-b05/OpenJDK8U-jdk_x64_linux_hotspot_8u382b05.tar.gz';          ;;        *)          echo "Unsupported arch: ${ARCH}";          exit 1;          ;;     esac; 	  wget -O /tmp/openjdk.tar.gz ${BINARY_URL}; 	  echo "${ESUM} */tmp/openjdk.tar.gz" | sha256sum -c -; 	  mkdir -p "$JAVA_HOME"; 	  tar --extract 	      --file /tmp/openjdk.tar.gz 	      --directory "$JAVA_HOME" 	      --strip-components 1 	      --no-same-owner 	  ;     rm -f /tmp/openjdk.tar.gz ${JAVA_HOME}/lib/src.zip;     find "$JAVA_HOME/lib" -name '*.so' -exec dirname '{}' ';' | sort -u > /etc/ld.so.conf.d/docker-openjdk.conf;     ldconfig;
# Fri, 01 Sep 2023 23:35:50 GMT
RUN echo Verifying install ...     && echo javac -version && javac -version     && echo java -version && java -version     && echo Complete.
# Fri, 01 Sep 2023 23:35:51 GMT
COPY file:8b8864b3e02a33a579dc216fd51b28a6047bc8eeaa03045b258980fe0cf7fcb3 in /__cacert_entrypoint.sh 
# Fri, 01 Sep 2023 23:35:51 GMT
ENTRYPOINT ["/__cacert_entrypoint.sh"]
```

-	Layers:
	-	`sha256:5987bac23899c422dbd7b7045113aa103f4d6856141a3f9098850e6328563e42`  
		Last Modified: Wed, 16 Aug 2023 13:31:19 GMT  
		Size: 27.0 MB (27027892 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7d351a285b1ff5e9027d7ca8fa1bb3eb48c9515c406c2908cb97b7e6efccc4a0`  
		Last Modified: Fri, 01 Sep 2023 23:37:49 GMT  
		Size: 12.5 MB (12492076 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8a81ed58e1d965b21b63805a1a69c0e86432a18377d8522f30a09ef3623038cd`  
		Last Modified: Fri, 01 Sep 2023 23:37:57 GMT  
		Size: 99.2 MB (99223334 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:086f5e6f8b9f6c429d11da91791d70d73a2420ad2993b49ffa1afd97113d4730`  
		Last Modified: Fri, 01 Sep 2023 23:37:47 GMT  
		Size: 160.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7f5ffc4ab54138f046378983f1bc952e51921c112d84fd6abe701cb100a285f5`  
		Last Modified: Fri, 01 Sep 2023 23:37:47 GMT  
		Size: 734.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `eclipse-temurin:8-jdk` - linux; arm64 variant v8

```console
$ docker pull eclipse-temurin@sha256:b6fd685cd805595288640ff9fe26a02012bf6053c9c2762acbc0c0d182c9d4dc
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **143.9 MB (143929578 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:eed25339cd17296f553148aa4cfd6653187fc1061f312799a55369b3ca277762`
-	Entrypoint: `["\/__cacert_entrypoint.sh"]`

```dockerfile
# Wed, 16 Aug 2023 06:19:52 GMT
ARG RELEASE
# Wed, 16 Aug 2023 06:19:52 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Wed, 16 Aug 2023 06:19:52 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Wed, 16 Aug 2023 06:19:53 GMT
LABEL org.opencontainers.image.version=22.04
# Wed, 16 Aug 2023 06:19:59 GMT
ADD file:3fcf00866c55150f1ea0a5ef7b8473c39275c1fdbf6aba0acd84cacb83d0c564 in / 
# Wed, 16 Aug 2023 06:19:59 GMT
CMD ["/bin/bash"]
# Fri, 01 Sep 2023 23:28:53 GMT
ENV JAVA_HOME=/opt/java/openjdk
# Fri, 01 Sep 2023 23:28:53 GMT
ENV PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Fri, 01 Sep 2023 23:28:53 GMT
ENV LANG=en_US.UTF-8 LANGUAGE=en_US:en LC_ALL=en_US.UTF-8
# Fri, 01 Sep 2023 23:29:07 GMT
RUN apt-get update     && DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends tzdata curl wget ca-certificates fontconfig locales p11-kit     && echo "en_US.UTF-8 UTF-8" >> /etc/locale.gen     && locale-gen en_US.UTF-8     && rm -rf /var/lib/apt/lists/*
# Fri, 01 Sep 2023 23:29:07 GMT
ENV JAVA_VERSION=jdk8u382-b05
# Fri, 01 Sep 2023 23:29:13 GMT
RUN set -eux;     ARCH="$(dpkg --print-architecture)";     case "${ARCH}" in        aarch64|arm64)          ESUM='0951398197b7bef39ab987b59c22852812ee2c2da6549953eed7fced4c08e13d';          BINARY_URL='https://github.com/adoptium/temurin8-binaries/releases/download/jdk8u382-b05/OpenJDK8U-jdk_aarch64_linux_hotspot_8u382b05.tar.gz';          ;;        armhf|arm)          ESUM='5d805ff157f272acf0f7d192f21af4a3b68c840333ca95568e4e07142efc369d';          BINARY_URL='https://github.com/adoptium/temurin8-binaries/releases/download/jdk8u382-b05/OpenJDK8U-jdk_arm_linux_hotspot_8u382b05.tar.gz';          apt-get update          && DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends libatomic1          && rm -rf /var/lib/apt/lists/*          ;;        ppc64el|powerpc:common64)          ESUM='509c923c308d1f4f28fd0068831a59250a05b8ca173ca92fb2be2e2e1f9ff3f9';          BINARY_URL='https://github.com/adoptium/temurin8-binaries/releases/download/jdk8u382-b05/OpenJDK8U-jdk_ppc64le_linux_hotspot_8u382b05.tar.gz';          ;;        amd64|i386:x86-64)          ESUM='789ad24dc0d9618294e3ba564c9bfda9d3f3a218604350e0ce0381bbc8f28db3';          BINARY_URL='https://github.com/adoptium/temurin8-binaries/releases/download/jdk8u382-b05/OpenJDK8U-jdk_x64_linux_hotspot_8u382b05.tar.gz';          ;;        *)          echo "Unsupported arch: ${ARCH}";          exit 1;          ;;     esac; 	  wget -O /tmp/openjdk.tar.gz ${BINARY_URL}; 	  echo "${ESUM} */tmp/openjdk.tar.gz" | sha256sum -c -; 	  mkdir -p "$JAVA_HOME"; 	  tar --extract 	      --file /tmp/openjdk.tar.gz 	      --directory "$JAVA_HOME" 	      --strip-components 1 	      --no-same-owner 	  ;     rm -f /tmp/openjdk.tar.gz ${JAVA_HOME}/lib/src.zip;     find "$JAVA_HOME/lib" -name '*.so' -exec dirname '{}' ';' | sort -u > /etc/ld.so.conf.d/docker-openjdk.conf;     ldconfig;
# Fri, 01 Sep 2023 23:29:14 GMT
RUN echo Verifying install ...     && echo javac -version && javac -version     && echo java -version && java -version     && echo Complete.
# Fri, 01 Sep 2023 23:29:14 GMT
COPY file:8b8864b3e02a33a579dc216fd51b28a6047bc8eeaa03045b258980fe0cf7fcb3 in /__cacert_entrypoint.sh 
# Fri, 01 Sep 2023 23:29:14 GMT
ENTRYPOINT ["/__cacert_entrypoint.sh"]
```

-	Layers:
	-	`sha256:8b5db5f6400d85199afbfde601a9e3c2051ebceb1ed9cc0fe25fe6b91e79afa9`  
		Last Modified: Thu, 17 Aug 2023 19:55:40 GMT  
		Size: 28.4 MB (28392978 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3c8624f6e9281a23943755ff078ce7c91b6b23aa7887445c9345622a3fdb3f32`  
		Last Modified: Fri, 01 Sep 2023 23:31:56 GMT  
		Size: 12.8 MB (12845046 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:59ec0f8ef15a061593461df6d7c68134566bdde84233e2eec62a72e489037702`  
		Last Modified: Fri, 01 Sep 2023 23:32:05 GMT  
		Size: 102.7 MB (102690664 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cee37ad20f503f1c4ef79a983cc1cf2226dcff8b1580f97f9f5593bb57390089`  
		Last Modified: Fri, 01 Sep 2023 23:31:54 GMT  
		Size: 159.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2e5251544da96b3c8875a1def75c772da40c19b881af9590f7820224d5b5ab9d`  
		Last Modified: Fri, 01 Sep 2023 23:31:54 GMT  
		Size: 731.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `eclipse-temurin:8-jdk` - linux; ppc64le

```console
$ docker pull eclipse-temurin@sha256:d6e40269de94129d78e399a41518ad7c82df1df2f32d2bf33c3577cec0286a1c
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **150.5 MB (150528410 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:3bcc9b4067f074d927de1ace1af61f89d1e4cbb080153a569ed7b46f7e9d4076`
-	Entrypoint: `["\/__cacert_entrypoint.sh"]`

```dockerfile
# Wed, 16 Aug 2023 06:03:07 GMT
ARG RELEASE
# Wed, 16 Aug 2023 06:03:07 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Wed, 16 Aug 2023 06:03:08 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Wed, 16 Aug 2023 06:03:08 GMT
LABEL org.opencontainers.image.version=22.04
# Wed, 16 Aug 2023 06:03:11 GMT
ADD file:632018deeaeb9e42f0026fb331dfb08381e46bd414b2b470b18ea22ac0653bf6 in / 
# Wed, 16 Aug 2023 06:03:11 GMT
CMD ["/bin/bash"]
# Sat, 02 Sep 2023 00:03:15 GMT
ENV JAVA_HOME=/opt/java/openjdk
# Sat, 02 Sep 2023 00:03:16 GMT
ENV PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Sat, 02 Sep 2023 00:03:18 GMT
ENV LANG=en_US.UTF-8 LANGUAGE=en_US:en LC_ALL=en_US.UTF-8
# Sat, 02 Sep 2023 00:04:06 GMT
RUN apt-get update     && DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends tzdata curl wget ca-certificates fontconfig locales p11-kit     && echo "en_US.UTF-8 UTF-8" >> /etc/locale.gen     && locale-gen en_US.UTF-8     && rm -rf /var/lib/apt/lists/*
# Sat, 02 Sep 2023 00:04:09 GMT
ENV JAVA_VERSION=jdk8u382-b05
# Sat, 02 Sep 2023 00:04:20 GMT
RUN set -eux;     ARCH="$(dpkg --print-architecture)";     case "${ARCH}" in        aarch64|arm64)          ESUM='0951398197b7bef39ab987b59c22852812ee2c2da6549953eed7fced4c08e13d';          BINARY_URL='https://github.com/adoptium/temurin8-binaries/releases/download/jdk8u382-b05/OpenJDK8U-jdk_aarch64_linux_hotspot_8u382b05.tar.gz';          ;;        armhf|arm)          ESUM='5d805ff157f272acf0f7d192f21af4a3b68c840333ca95568e4e07142efc369d';          BINARY_URL='https://github.com/adoptium/temurin8-binaries/releases/download/jdk8u382-b05/OpenJDK8U-jdk_arm_linux_hotspot_8u382b05.tar.gz';          apt-get update          && DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends libatomic1          && rm -rf /var/lib/apt/lists/*          ;;        ppc64el|powerpc:common64)          ESUM='509c923c308d1f4f28fd0068831a59250a05b8ca173ca92fb2be2e2e1f9ff3f9';          BINARY_URL='https://github.com/adoptium/temurin8-binaries/releases/download/jdk8u382-b05/OpenJDK8U-jdk_ppc64le_linux_hotspot_8u382b05.tar.gz';          ;;        amd64|i386:x86-64)          ESUM='789ad24dc0d9618294e3ba564c9bfda9d3f3a218604350e0ce0381bbc8f28db3';          BINARY_URL='https://github.com/adoptium/temurin8-binaries/releases/download/jdk8u382-b05/OpenJDK8U-jdk_x64_linux_hotspot_8u382b05.tar.gz';          ;;        *)          echo "Unsupported arch: ${ARCH}";          exit 1;          ;;     esac; 	  wget -O /tmp/openjdk.tar.gz ${BINARY_URL}; 	  echo "${ESUM} */tmp/openjdk.tar.gz" | sha256sum -c -; 	  mkdir -p "$JAVA_HOME"; 	  tar --extract 	      --file /tmp/openjdk.tar.gz 	      --directory "$JAVA_HOME" 	      --strip-components 1 	      --no-same-owner 	  ;     rm -f /tmp/openjdk.tar.gz ${JAVA_HOME}/lib/src.zip;     find "$JAVA_HOME/lib" -name '*.so' -exec dirname '{}' ';' | sort -u > /etc/ld.so.conf.d/docker-openjdk.conf;     ldconfig;
# Sat, 02 Sep 2023 00:04:26 GMT
RUN echo Verifying install ...     && echo javac -version && javac -version     && echo java -version && java -version     && echo Complete.
# Sat, 02 Sep 2023 00:04:27 GMT
COPY file:8b8864b3e02a33a579dc216fd51b28a6047bc8eeaa03045b258980fe0cf7fcb3 in /__cacert_entrypoint.sh 
# Sat, 02 Sep 2023 00:04:28 GMT
ENTRYPOINT ["/__cacert_entrypoint.sh"]
```

-	Layers:
	-	`sha256:5d4cfc5435802883c4aaa9fa4afcc1b07f40e20bee68f058f0671804ab6bc3a0`  
		Last Modified: Sat, 02 Sep 2023 00:08:58 GMT  
		Size: 35.7 MB (35705651 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:20bbdfadf6550699bed2516a6d795d42d07af539ddc96ec121092535bbfefc27`  
		Last Modified: Sat, 02 Sep 2023 00:08:53 GMT  
		Size: 13.8 MB (13770760 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b84846b873917d9d8ca07c8c6395bd5952ea46089c0e16b30cb4969767df5895`  
		Last Modified: Sat, 02 Sep 2023 00:09:04 GMT  
		Size: 101.1 MB (101051104 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:47f8204539dc3be057440dc32d7524420a1edea03a3c6b8805d9ba58c100c71a`  
		Last Modified: Sat, 02 Sep 2023 00:08:49 GMT  
		Size: 161.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:37ffba40b193db865ea4030d086227e7ce90829ea749c4fcf339f3179a224f79`  
		Last Modified: Sat, 02 Sep 2023 00:08:49 GMT  
		Size: 734.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `eclipse-temurin:8-jdk` - windows version 10.0.20348.1906; amd64

```console
$ docker pull eclipse-temurin@sha256:5bb246d74d5695a7ee04bcc7471b0a427ee63742746717de8a7330f3840c3c83
```

-	Docker Version: 20.10.21
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.0 GB (1988875783 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:1231cd9c02de4ec74493e4bae72ccef87718bc8550596c574935207710f8038d`
-	Default Command: `["c:\\windows\\system32\\cmd.exe"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Thu, 08 Jun 2023 12:55:20 GMT
RUN Apply image 10.0.20348.1787
# Thu, 03 Aug 2023 10:01:10 GMT
RUN Install update 10.0.20348.1906
# Wed, 09 Aug 2023 23:35:07 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Wed, 09 Aug 2023 23:35:08 GMT
ENV JAVA_VERSION=jdk8u382-b05
# Wed, 09 Aug 2023 23:36:07 GMT
RUN Write-Host ('Downloading https://github.com/adoptium/temurin8-binaries/releases/download/jdk8u382-b05/OpenJDK8U-jdk_x64_windows_hotspot_8u382b05.msi ...');     curl.exe -LfsSo openjdk.msi https://github.com/adoptium/temurin8-binaries/releases/download/jdk8u382-b05/OpenJDK8U-jdk_x64_windows_hotspot_8u382b05.msi ;     Write-Host ('Verifying sha256 (da10c23aa318764adc8361df0e0363fa50f885abe97b229fb0e4d4fe8c9f9679) ...');     if ((Get-FileHash openjdk.msi -Algorithm sha256).Hash -ne 'da10c23aa318764adc8361df0e0363fa50f885abe97b229fb0e4d4fe8c9f9679') {         Write-Host 'FAILED!';         exit 1;     };         New-Item -ItemType Directory -Path C:\temp | Out-Null;         Write-Host 'Installing using MSI ...';     $proc = Start-Process -FilePath "msiexec.exe" -ArgumentList '/i', 'openjdk.msi', '/L*V', 'C:\temp\OpenJDK.log',     '/quiet', 'ADDLOCAL=FeatureEnvironment,FeatureJarFileRunWith,FeatureJavaHome', 'INSTALLDIR=C:\openjdk-8' -Wait -Passthru;     $proc.WaitForExit() ;     if ($proc.ExitCode -ne 0) {         Write-Host 'FAILED installing MSI!' ;         exit 1;     };         Remove-Item -Path C:\temp -Recurse | Out-Null;     Write-Host 'Removing openjdk.msi ...';     Remove-Item openjdk.msi -Force
# Wed, 09 Aug 2023 23:36:30 GMT
RUN Write-Host 'Verifying install ...';     Write-Host 'javac -version'; javac -version;     Write-Host 'java -version'; java -version;         Write-Host 'Complete.'
```

-	Layers:
	-	`sha256:7c76e5cf7755ce357ffb737715b0da6799a50ea468cc252c094f4d915d426b3f`  
		Last Modified: Tue, 13 Jun 2023 17:55:32 GMT  
		Size: 1.4 GB (1388598786 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:22a441455ace20af58f01367d769afc2b25c3db3e4a7aee67a634d14826f6f19`  
		Last Modified: Tue, 08 Aug 2023 18:20:41 GMT  
		Size: 408.8 MB (408765102 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a53d0f5bc5dd4cb7976f788ee32f7195b84c7964cb22bc38a49eb55673629149`  
		Last Modified: Thu, 10 Aug 2023 00:18:32 GMT  
		Size: 1.4 KB (1413 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4be361cd0475de61a76b439cd920c0b3eebd6feb424a862b502fc11deb216e30`  
		Last Modified: Thu, 10 Aug 2023 00:18:32 GMT  
		Size: 1.4 KB (1437 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b84e8ca282bfa9e4f112d6ab729fc10b98dc803bf9852e8f442148d7a4274858`  
		Last Modified: Thu, 10 Aug 2023 00:18:51 GMT  
		Size: 191.2 MB (191244285 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6298e107d6f9d8d49c4fe963747ae7d2c4ae6500dd010b138ebfa6ba445a03b7`  
		Last Modified: Thu, 10 Aug 2023 00:18:32 GMT  
		Size: 264.8 KB (264760 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `eclipse-temurin:8-jdk` - windows version 10.0.17763.4737; amd64

```console
$ docker pull eclipse-temurin@sha256:9dbf5d2da2714ad6816a4b0dff1ac3a2660fc09b2c795ca7f61e34bc255a05a5
```

-	Docker Version: 20.10.21
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.2 GB (2187488736 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:497f12f3018921415922d3d82ab607abed9af3a16dc978b5de5b7a3739be7193`
-	Default Command: `["c:\\windows\\system32\\cmd.exe"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Thu, 08 Jun 2023 12:58:24 GMT
RUN Apply image 10.0.17763.4499
# Wed, 02 Aug 2023 09:07:15 GMT
RUN Install update 10.0.17763.4737
# Wed, 09 Aug 2023 23:36:50 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Wed, 09 Aug 2023 23:36:51 GMT
ENV JAVA_VERSION=jdk8u382-b05
# Wed, 09 Aug 2023 23:38:37 GMT
RUN Write-Host ('Downloading https://github.com/adoptium/temurin8-binaries/releases/download/jdk8u382-b05/OpenJDK8U-jdk_x64_windows_hotspot_8u382b05.msi ...');     curl.exe -LfsSo openjdk.msi https://github.com/adoptium/temurin8-binaries/releases/download/jdk8u382-b05/OpenJDK8U-jdk_x64_windows_hotspot_8u382b05.msi ;     Write-Host ('Verifying sha256 (da10c23aa318764adc8361df0e0363fa50f885abe97b229fb0e4d4fe8c9f9679) ...');     if ((Get-FileHash openjdk.msi -Algorithm sha256).Hash -ne 'da10c23aa318764adc8361df0e0363fa50f885abe97b229fb0e4d4fe8c9f9679') {         Write-Host 'FAILED!';         exit 1;     };         New-Item -ItemType Directory -Path C:\temp | Out-Null;         Write-Host 'Installing using MSI ...';     $proc = Start-Process -FilePath "msiexec.exe" -ArgumentList '/i', 'openjdk.msi', '/L*V', 'C:\temp\OpenJDK.log',     '/quiet', 'ADDLOCAL=FeatureEnvironment,FeatureJarFileRunWith,FeatureJavaHome', 'INSTALLDIR=C:\openjdk-8' -Wait -Passthru;     $proc.WaitForExit() ;     if ($proc.ExitCode -ne 0) {         Write-Host 'FAILED installing MSI!' ;         exit 1;     };         Remove-Item -Path C:\temp -Recurse | Out-Null;     Write-Host 'Removing openjdk.msi ...';     Remove-Item openjdk.msi -Force
# Wed, 09 Aug 2023 23:39:40 GMT
RUN Write-Host 'Verifying install ...';     Write-Host 'javac -version'; javac -version;     Write-Host 'java -version'; java -version;         Write-Host 'Complete.'
```

-	Layers:
	-	`sha256:c9226d61d3bdbf9f09821b32f5878623b8daaa5fb4f875cb63c199f87a26d57e`  
		Last Modified: Tue, 13 Jun 2023 18:25:35 GMT  
		Size: 1.7 GB (1650620357 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b95f433aa7d90194e65f6b08a599b3ee12292e124d47c204107baedfd71054c1`  
		Last Modified: Tue, 08 Aug 2023 18:31:16 GMT  
		Size: 345.3 MB (345334986 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a03d23fbbd4f650b6f60106a3cc28d711efce2f97cfb80b67e2dec305e011aa3`  
		Last Modified: Thu, 10 Aug 2023 00:19:47 GMT  
		Size: 1.4 KB (1414 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:95bee61ee62c6402944a7a93c2f07bbbbbece6873406b91d78be74c5c1e0bc2c`  
		Last Modified: Thu, 10 Aug 2023 00:19:48 GMT  
		Size: 1.4 KB (1437 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:90c03dddd5dd3dfc278f8295e44930ee5d7ab46f66e5d6ea2da60dc32412d824`  
		Last Modified: Thu, 10 Aug 2023 00:20:07 GMT  
		Size: 191.3 MB (191306441 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bdc8b7ed80fbdfc5c50dbb99a52af7826c117b976451250ea98c700780e96ef7`  
		Last Modified: Thu, 10 Aug 2023 00:19:48 GMT  
		Size: 224.1 KB (224101 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
