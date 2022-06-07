## `eclipse-temurin:18-jre-focal`

```console
$ docker pull eclipse-temurin@sha256:7f60aaa43c68395f40b4451e306001cc8869b1e4c97692c87614dd6e37434037
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 5
	-	linux; amd64
	-	linux; arm variant v7
	-	linux; arm64 variant v8
	-	linux; ppc64le
	-	linux; s390x

### `eclipse-temurin:18-jre-focal` - linux; amd64

```console
$ docker pull eclipse-temurin@sha256:c3e022ccea1e83801f400eee06514662999f21e89eefd0aaaadbaa4f0b6bc92c
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **95.0 MB (95003245 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:40069f0f6a1ca917c59e1eff181efb958a946d7422b3e827c0715f94d921d20a`
-	Default Command: `["bash"]`

```dockerfile
# Mon, 06 Jun 2022 22:21:11 GMT
ADD file:00dae10e79b05c4e1a3db053a1f85a4f38a39fe85cbbd88d74201a01a7dd59b5 in / 
# Mon, 06 Jun 2022 22:21:12 GMT
CMD ["bash"]
# Tue, 07 Jun 2022 00:12:30 GMT
ENV LANG=en_US.UTF-8 LANGUAGE=en_US:en LC_ALL=en_US.UTF-8
# Tue, 07 Jun 2022 00:15:30 GMT
RUN apt-get update     && DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends tzdata curl ca-certificates fontconfig locales binutils     && echo "en_US.UTF-8 UTF-8" >> /etc/locale.gen     && locale-gen en_US.UTF-8     && rm -rf /var/lib/apt/lists/*
# Tue, 07 Jun 2022 00:16:35 GMT
ENV JAVA_VERSION=jdk-18.0.1+10
# Tue, 07 Jun 2022 00:17:28 GMT
RUN set -eux;     ARCH="$(dpkg --print-architecture)";     case "${ARCH}" in        aarch64|arm64)          ESUM='cacb261967585ccd3eefe9a44f277b23aaa0b60772589ac220f03941c2bcdad1';          BINARY_URL='https://github.com/adoptium/temurin18-binaries/releases/download/jdk-18.0.1%2B10/OpenJDK18U-jre_aarch64_linux_hotspot_18.0.1_10.tar.gz';          ;;        armhf|arm)          ESUM='24ec0eb692e30c7055cc863e4f47aa9cec2c069849f09b227adb14c87a70e8e7';          BINARY_URL='https://github.com/adoptium/temurin18-binaries/releases/download/jdk-18.0.1%2B10/OpenJDK18U-jre_arm_linux_hotspot_18.0.1_10.tar.gz';          ;;        ppc64el|powerpc:common64)          ESUM='3b43c2a662a88054886c7a89696248c0c99927fe97750c5e7690eddba4fb9645';          BINARY_URL='https://github.com/adoptium/temurin18-binaries/releases/download/jdk-18.0.1%2B10/OpenJDK18U-jre_ppc64le_linux_hotspot_18.0.1_10.tar.gz';          ;;        s390x|s390:64-bit)          ESUM='c9fb7c6fb110ad2e6ffaae9a8c3b8ea51098f98c60eaa1a0fcb0019c980227ab';          BINARY_URL='https://github.com/adoptium/temurin18-binaries/releases/download/jdk-18.0.1%2B10/OpenJDK18U-jre_s390x_linux_hotspot_18.0.1_10.tar.gz';          ;;        amd64|i386:x86-64)          ESUM='67c2cea6040b12c125bb1bea74b3eeb42c94072713b152b720e50c897b946ffa';          BINARY_URL='https://github.com/adoptium/temurin18-binaries/releases/download/jdk-18.0.1%2B10/OpenJDK18U-jre_x64_linux_hotspot_18.0.1_10.tar.gz';          ;;        *)          echo "Unsupported arch: ${ARCH}";          exit 1;          ;;     esac;     curl -LfsSo /tmp/openjdk.tar.gz ${BINARY_URL};     echo "${ESUM} */tmp/openjdk.tar.gz" | sha256sum -c -;     mkdir -p /opt/java/openjdk;     cd /opt/java/openjdk;     tar -xf /tmp/openjdk.tar.gz --strip-components=1;     rm -rf /tmp/openjdk.tar.gz;
# Tue, 07 Jun 2022 00:17:29 GMT
ENV JAVA_HOME=/opt/java/openjdk PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 07 Jun 2022 00:17:29 GMT
RUN echo Verifying install ...     && echo java --version && java --version     && echo Complete.
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
	-	`sha256:e10e8a475e0cc7d41258e49dc8d2c5b1f02962b05eb12abbd338ffd80b2ee757`  
		Last Modified: Tue, 07 Jun 2022 00:24:34 GMT  
		Size: 46.7 MB (46656572 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fadcb54423b5c2eb2be8f449420119cbb52be20032b8f00b46fff12d12973343`  
		Last Modified: Tue, 07 Jun 2022 00:24:27 GMT  
		Size: 160.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `eclipse-temurin:18-jre-focal` - linux; arm variant v7

```console
$ docker pull eclipse-temurin@sha256:d0864e85005c24272ec17697585e6f822584c0f557c657365477d9a54a968535
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **88.1 MB (88099569 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:986be9da0a1bca6134f1b6aec6b779f6e171c5cd92c3604dc396cbec3723e0de`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 07 Jun 2022 05:50:50 GMT
ADD file:c95d34737ba1f11ac8b92be0125aad2baae46448f0d8ebd85ad69076006a3254 in / 
# Tue, 07 Jun 2022 05:50:51 GMT
CMD ["bash"]
# Tue, 07 Jun 2022 09:33:43 GMT
ENV LANG=en_US.UTF-8 LANGUAGE=en_US:en LC_ALL=en_US.UTF-8
# Tue, 07 Jun 2022 09:41:33 GMT
RUN apt-get update     && DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends tzdata curl ca-certificates fontconfig locales binutils     && echo "en_US.UTF-8 UTF-8" >> /etc/locale.gen     && locale-gen en_US.UTF-8     && rm -rf /var/lib/apt/lists/*
# Tue, 07 Jun 2022 09:44:40 GMT
ENV JAVA_VERSION=jdk-18.0.1+10
# Tue, 07 Jun 2022 09:46:32 GMT
RUN set -eux;     ARCH="$(dpkg --print-architecture)";     case "${ARCH}" in        aarch64|arm64)          ESUM='cacb261967585ccd3eefe9a44f277b23aaa0b60772589ac220f03941c2bcdad1';          BINARY_URL='https://github.com/adoptium/temurin18-binaries/releases/download/jdk-18.0.1%2B10/OpenJDK18U-jre_aarch64_linux_hotspot_18.0.1_10.tar.gz';          ;;        armhf|arm)          ESUM='24ec0eb692e30c7055cc863e4f47aa9cec2c069849f09b227adb14c87a70e8e7';          BINARY_URL='https://github.com/adoptium/temurin18-binaries/releases/download/jdk-18.0.1%2B10/OpenJDK18U-jre_arm_linux_hotspot_18.0.1_10.tar.gz';          ;;        ppc64el|powerpc:common64)          ESUM='3b43c2a662a88054886c7a89696248c0c99927fe97750c5e7690eddba4fb9645';          BINARY_URL='https://github.com/adoptium/temurin18-binaries/releases/download/jdk-18.0.1%2B10/OpenJDK18U-jre_ppc64le_linux_hotspot_18.0.1_10.tar.gz';          ;;        s390x|s390:64-bit)          ESUM='c9fb7c6fb110ad2e6ffaae9a8c3b8ea51098f98c60eaa1a0fcb0019c980227ab';          BINARY_URL='https://github.com/adoptium/temurin18-binaries/releases/download/jdk-18.0.1%2B10/OpenJDK18U-jre_s390x_linux_hotspot_18.0.1_10.tar.gz';          ;;        amd64|i386:x86-64)          ESUM='67c2cea6040b12c125bb1bea74b3eeb42c94072713b152b720e50c897b946ffa';          BINARY_URL='https://github.com/adoptium/temurin18-binaries/releases/download/jdk-18.0.1%2B10/OpenJDK18U-jre_x64_linux_hotspot_18.0.1_10.tar.gz';          ;;        *)          echo "Unsupported arch: ${ARCH}";          exit 1;          ;;     esac;     curl -LfsSo /tmp/openjdk.tar.gz ${BINARY_URL};     echo "${ESUM} */tmp/openjdk.tar.gz" | sha256sum -c -;     mkdir -p /opt/java/openjdk;     cd /opt/java/openjdk;     tar -xf /tmp/openjdk.tar.gz --strip-components=1;     rm -rf /tmp/openjdk.tar.gz;
# Tue, 07 Jun 2022 09:46:33 GMT
ENV JAVA_HOME=/opt/java/openjdk PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 07 Jun 2022 09:46:34 GMT
RUN echo Verifying install ...     && echo java --version && java --version     && echo Complete.
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
	-	`sha256:285169e943967fa23d4fc6b29863ce2c6cd47c64439b81d88cda11f9c2cd2353`  
		Last Modified: Tue, 07 Jun 2022 10:05:42 GMT  
		Size: 44.3 MB (44310293 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2bf2c13e52c2593322c06d9ed1d44076c9010b2db4829fff5a8c011ecccdc5c3`  
		Last Modified: Tue, 07 Jun 2022 10:05:13 GMT  
		Size: 161.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `eclipse-temurin:18-jre-focal` - linux; arm64 variant v8

```console
$ docker pull eclipse-temurin@sha256:ea17711f7d754f293ceec2718e0de494f880f3dd03c640432a57d91f4f1dc895
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **93.8 MB (93842318 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:77fc78d9163b33e2a76d2a91eab4e61b34b32d166007a74475ccc756a9438031`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 07 Jun 2022 01:25:15 GMT
ADD file:8bb0809a8ac8e978274cf731cff7529372088d22c5b0233a28f01ef414aefbca in / 
# Tue, 07 Jun 2022 01:25:16 GMT
CMD ["bash"]
# Tue, 07 Jun 2022 04:59:51 GMT
ENV LANG=en_US.UTF-8 LANGUAGE=en_US:en LC_ALL=en_US.UTF-8
# Tue, 07 Jun 2022 05:06:48 GMT
RUN apt-get update     && DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends tzdata curl ca-certificates fontconfig locales binutils     && echo "en_US.UTF-8 UTF-8" >> /etc/locale.gen     && locale-gen en_US.UTF-8     && rm -rf /var/lib/apt/lists/*
# Tue, 07 Jun 2022 06:38:11 GMT
ENV JAVA_VERSION=jdk-18.0.1+10
# Tue, 07 Jun 2022 06:39:08 GMT
RUN set -eux;     ARCH="$(dpkg --print-architecture)";     case "${ARCH}" in        aarch64|arm64)          ESUM='cacb261967585ccd3eefe9a44f277b23aaa0b60772589ac220f03941c2bcdad1';          BINARY_URL='https://github.com/adoptium/temurin18-binaries/releases/download/jdk-18.0.1%2B10/OpenJDK18U-jre_aarch64_linux_hotspot_18.0.1_10.tar.gz';          ;;        armhf|arm)          ESUM='24ec0eb692e30c7055cc863e4f47aa9cec2c069849f09b227adb14c87a70e8e7';          BINARY_URL='https://github.com/adoptium/temurin18-binaries/releases/download/jdk-18.0.1%2B10/OpenJDK18U-jre_arm_linux_hotspot_18.0.1_10.tar.gz';          ;;        ppc64el|powerpc:common64)          ESUM='3b43c2a662a88054886c7a89696248c0c99927fe97750c5e7690eddba4fb9645';          BINARY_URL='https://github.com/adoptium/temurin18-binaries/releases/download/jdk-18.0.1%2B10/OpenJDK18U-jre_ppc64le_linux_hotspot_18.0.1_10.tar.gz';          ;;        s390x|s390:64-bit)          ESUM='c9fb7c6fb110ad2e6ffaae9a8c3b8ea51098f98c60eaa1a0fcb0019c980227ab';          BINARY_URL='https://github.com/adoptium/temurin18-binaries/releases/download/jdk-18.0.1%2B10/OpenJDK18U-jre_s390x_linux_hotspot_18.0.1_10.tar.gz';          ;;        amd64|i386:x86-64)          ESUM='67c2cea6040b12c125bb1bea74b3eeb42c94072713b152b720e50c897b946ffa';          BINARY_URL='https://github.com/adoptium/temurin18-binaries/releases/download/jdk-18.0.1%2B10/OpenJDK18U-jre_x64_linux_hotspot_18.0.1_10.tar.gz';          ;;        *)          echo "Unsupported arch: ${ARCH}";          exit 1;          ;;     esac;     curl -LfsSo /tmp/openjdk.tar.gz ${BINARY_URL};     echo "${ESUM} */tmp/openjdk.tar.gz" | sha256sum -c -;     mkdir -p /opt/java/openjdk;     cd /opt/java/openjdk;     tar -xf /tmp/openjdk.tar.gz --strip-components=1;     rm -rf /tmp/openjdk.tar.gz;
# Tue, 07 Jun 2022 06:39:09 GMT
ENV JAVA_HOME=/opt/java/openjdk PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 07 Jun 2022 06:39:09 GMT
RUN echo Verifying install ...     && echo java --version && java --version     && echo Complete.
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
	-	`sha256:f517d07c09f27fbe66ce15644e8b677def6e6258735f82c24415fbb01274a349`  
		Last Modified: Tue, 07 Jun 2022 06:47:39 GMT  
		Size: 46.1 MB (46150000 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fff8915af63dd62ab928d690c1dfb1788c94104cb0abfeb3356d6816bddd4cca`  
		Last Modified: Tue, 07 Jun 2022 06:47:32 GMT  
		Size: 127.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `eclipse-temurin:18-jre-focal` - linux; ppc64le

```console
$ docker pull eclipse-temurin@sha256:e13a4d99e19c08696e4abb9ad63724a70475216225db83aefd269da423bb2f96
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **101.5 MB (101471588 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a0d6cfb87823b6b1437f5fc5dd283df1099901da8791adadf3e29642df9083df`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 07 Jun 2022 05:46:02 GMT
ADD file:86506a94b834ba2b6f10dc0d1955bee539be1cf565e4ccc2c4bc074e0375f115 in / 
# Tue, 07 Jun 2022 05:46:06 GMT
CMD ["bash"]
# Tue, 07 Jun 2022 07:16:49 GMT
ENV LANG=en_US.UTF-8 LANGUAGE=en_US:en LC_ALL=en_US.UTF-8
# Tue, 07 Jun 2022 07:24:06 GMT
RUN apt-get update     && DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends tzdata curl ca-certificates fontconfig locales binutils     && echo "en_US.UTF-8 UTF-8" >> /etc/locale.gen     && locale-gen en_US.UTF-8     && rm -rf /var/lib/apt/lists/*
# Tue, 07 Jun 2022 07:26:35 GMT
ENV JAVA_VERSION=jdk-18.0.1+10
# Tue, 07 Jun 2022 07:27:59 GMT
RUN set -eux;     ARCH="$(dpkg --print-architecture)";     case "${ARCH}" in        aarch64|arm64)          ESUM='cacb261967585ccd3eefe9a44f277b23aaa0b60772589ac220f03941c2bcdad1';          BINARY_URL='https://github.com/adoptium/temurin18-binaries/releases/download/jdk-18.0.1%2B10/OpenJDK18U-jre_aarch64_linux_hotspot_18.0.1_10.tar.gz';          ;;        armhf|arm)          ESUM='24ec0eb692e30c7055cc863e4f47aa9cec2c069849f09b227adb14c87a70e8e7';          BINARY_URL='https://github.com/adoptium/temurin18-binaries/releases/download/jdk-18.0.1%2B10/OpenJDK18U-jre_arm_linux_hotspot_18.0.1_10.tar.gz';          ;;        ppc64el|powerpc:common64)          ESUM='3b43c2a662a88054886c7a89696248c0c99927fe97750c5e7690eddba4fb9645';          BINARY_URL='https://github.com/adoptium/temurin18-binaries/releases/download/jdk-18.0.1%2B10/OpenJDK18U-jre_ppc64le_linux_hotspot_18.0.1_10.tar.gz';          ;;        s390x|s390:64-bit)          ESUM='c9fb7c6fb110ad2e6ffaae9a8c3b8ea51098f98c60eaa1a0fcb0019c980227ab';          BINARY_URL='https://github.com/adoptium/temurin18-binaries/releases/download/jdk-18.0.1%2B10/OpenJDK18U-jre_s390x_linux_hotspot_18.0.1_10.tar.gz';          ;;        amd64|i386:x86-64)          ESUM='67c2cea6040b12c125bb1bea74b3eeb42c94072713b152b720e50c897b946ffa';          BINARY_URL='https://github.com/adoptium/temurin18-binaries/releases/download/jdk-18.0.1%2B10/OpenJDK18U-jre_x64_linux_hotspot_18.0.1_10.tar.gz';          ;;        *)          echo "Unsupported arch: ${ARCH}";          exit 1;          ;;     esac;     curl -LfsSo /tmp/openjdk.tar.gz ${BINARY_URL};     echo "${ESUM} */tmp/openjdk.tar.gz" | sha256sum -c -;     mkdir -p /opt/java/openjdk;     cd /opt/java/openjdk;     tar -xf /tmp/openjdk.tar.gz --strip-components=1;     rm -rf /tmp/openjdk.tar.gz;
# Tue, 07 Jun 2022 07:28:01 GMT
ENV JAVA_HOME=/opt/java/openjdk PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 07 Jun 2022 07:28:07 GMT
RUN echo Verifying install ...     && echo java --version && java --version     && echo Complete.
```

-	Layers:
	-	`sha256:3f52d061d2d3fdde0d3a099bbeae64080476c9650e9f3ba05de898d5bb5f03e8`  
		Last Modified: Tue, 07 Jun 2022 05:49:10 GMT  
		Size: 33.3 MB (33294345 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:368221692b3b4fa9b7da472cb9db7d8f6b91844b0a5a8bef11b0b385c58763f2`  
		Last Modified: Tue, 07 Jun 2022 07:32:02 GMT  
		Size: 21.7 MB (21693610 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:eb3688ebc7f7298666501ffc055059029d198731fae85787f7a5e7cc299bcf67`  
		Last Modified: Tue, 07 Jun 2022 07:33:46 GMT  
		Size: 46.5 MB (46483474 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8b9eaaadd6cd1135e7600b09ec31d6803e18b26ead6f90c22689d9a01fca4dea`  
		Last Modified: Tue, 07 Jun 2022 07:33:37 GMT  
		Size: 159.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `eclipse-temurin:18-jre-focal` - linux; s390x

```console
$ docker pull eclipse-temurin@sha256:260922971b2f355c3876d2fe05980ea51449a0493556b4f859415304878540a2
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **89.7 MB (89734789 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:5aa2383e1d7387971f3d1c702dd58227bfcffb27dadf0ce36047d0ffd15dff8d`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 07 Jun 2022 04:05:02 GMT
ADD file:6250f895d7d6c591cfe1b9fc991313d21b02167d94c67991db7c5c1c6814c51e in / 
# Tue, 07 Jun 2022 04:05:06 GMT
CMD ["bash"]
# Tue, 07 Jun 2022 06:11:05 GMT
ENV LANG=en_US.UTF-8 LANGUAGE=en_US:en LC_ALL=en_US.UTF-8
# Tue, 07 Jun 2022 06:19:54 GMT
RUN apt-get update     && DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends tzdata curl ca-certificates fontconfig locales binutils     && echo "en_US.UTF-8 UTF-8" >> /etc/locale.gen     && locale-gen en_US.UTF-8     && rm -rf /var/lib/apt/lists/*
# Tue, 07 Jun 2022 06:39:23 GMT
ENV JAVA_VERSION=jdk-18.0.1+10
# Tue, 07 Jun 2022 06:40:36 GMT
RUN set -eux;     ARCH="$(dpkg --print-architecture)";     case "${ARCH}" in        aarch64|arm64)          ESUM='cacb261967585ccd3eefe9a44f277b23aaa0b60772589ac220f03941c2bcdad1';          BINARY_URL='https://github.com/adoptium/temurin18-binaries/releases/download/jdk-18.0.1%2B10/OpenJDK18U-jre_aarch64_linux_hotspot_18.0.1_10.tar.gz';          ;;        armhf|arm)          ESUM='24ec0eb692e30c7055cc863e4f47aa9cec2c069849f09b227adb14c87a70e8e7';          BINARY_URL='https://github.com/adoptium/temurin18-binaries/releases/download/jdk-18.0.1%2B10/OpenJDK18U-jre_arm_linux_hotspot_18.0.1_10.tar.gz';          ;;        ppc64el|powerpc:common64)          ESUM='3b43c2a662a88054886c7a89696248c0c99927fe97750c5e7690eddba4fb9645';          BINARY_URL='https://github.com/adoptium/temurin18-binaries/releases/download/jdk-18.0.1%2B10/OpenJDK18U-jre_ppc64le_linux_hotspot_18.0.1_10.tar.gz';          ;;        s390x|s390:64-bit)          ESUM='c9fb7c6fb110ad2e6ffaae9a8c3b8ea51098f98c60eaa1a0fcb0019c980227ab';          BINARY_URL='https://github.com/adoptium/temurin18-binaries/releases/download/jdk-18.0.1%2B10/OpenJDK18U-jre_s390x_linux_hotspot_18.0.1_10.tar.gz';          ;;        amd64|i386:x86-64)          ESUM='67c2cea6040b12c125bb1bea74b3eeb42c94072713b152b720e50c897b946ffa';          BINARY_URL='https://github.com/adoptium/temurin18-binaries/releases/download/jdk-18.0.1%2B10/OpenJDK18U-jre_x64_linux_hotspot_18.0.1_10.tar.gz';          ;;        *)          echo "Unsupported arch: ${ARCH}";          exit 1;          ;;     esac;     curl -LfsSo /tmp/openjdk.tar.gz ${BINARY_URL};     echo "${ESUM} */tmp/openjdk.tar.gz" | sha256sum -c -;     mkdir -p /opt/java/openjdk;     cd /opt/java/openjdk;     tar -xf /tmp/openjdk.tar.gz --strip-components=1;     rm -rf /tmp/openjdk.tar.gz;
# Tue, 07 Jun 2022 06:40:39 GMT
ENV JAVA_HOME=/opt/java/openjdk PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 07 Jun 2022 06:40:40 GMT
RUN echo Verifying install ...     && echo java --version && java --version     && echo Complete.
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
	-	`sha256:565c97a9a8c20a08d21de67a5fb17f10294cb0f0ecf0e5b41b15779af9ad17f6`  
		Last Modified: Tue, 07 Jun 2022 06:45:47 GMT  
		Size: 43.4 MB (43449059 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d7ef4b80ae4eb63487148201ee8b89f9ecea569c78aae09c1fa6b6411e907579`  
		Last Modified: Tue, 07 Jun 2022 06:45:41 GMT  
		Size: 161.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
