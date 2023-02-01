## `gradle:6-jdk8-focal`

```console
$ docker pull gradle@sha256:a3f222b09761648be538dcbe2163bdb5ce66a63babcdbdd3c37a3ba9a94107d0
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 4
	-	linux; amd64
	-	linux; arm variant v7
	-	linux; arm64 variant v8
	-	linux; ppc64le

### `gradle:6-jdk8-focal` - linux; amd64

```console
$ docker pull gradle@sha256:dd824417caa24c7226b8547ff270549a9638bb7550fa1ee7a21679019d49372c
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **272.6 MB (272553217 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c29195d8a0d245e2207991d43d5d4a8b1cfada32f371010fca851c47bb73a6af`
-	Default Command: `["gradle"]`

```dockerfile
# Thu, 26 Jan 2023 13:19:55 GMT
ARG RELEASE
# Thu, 26 Jan 2023 13:19:55 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Thu, 26 Jan 2023 13:19:55 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Thu, 26 Jan 2023 13:19:55 GMT
LABEL org.opencontainers.image.version=20.04
# Thu, 26 Jan 2023 13:19:57 GMT
ADD file:8b180a9b4497de0c6e131d6b48cf5c69a885379e63033ab9639d1655991e626c in / 
# Thu, 26 Jan 2023 13:19:57 GMT
CMD ["/bin/bash"]
# Tue, 31 Jan 2023 20:26:24 GMT
ENV JAVA_HOME=/opt/java/openjdk
# Tue, 31 Jan 2023 20:26:24 GMT
ENV PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 31 Jan 2023 20:26:25 GMT
ENV LANG=en_US.UTF-8 LANGUAGE=en_US:en LC_ALL=en_US.UTF-8
# Tue, 31 Jan 2023 20:26:50 GMT
RUN apt-get update     && DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends tzdata curl wget ca-certificates fontconfig locales     && echo "en_US.UTF-8 UTF-8" >> /etc/locale.gen     && locale-gen en_US.UTF-8     && rm -rf /var/lib/apt/lists/*
# Tue, 31 Jan 2023 20:26:50 GMT
ENV JAVA_VERSION=jdk8u362-b09
# Tue, 31 Jan 2023 20:26:55 GMT
RUN set -eux;     ARCH="$(dpkg --print-architecture)";     case "${ARCH}" in        aarch64|arm64)          ESUM='9290a8beefd7a94f0eb030f62d402411a852100482b9c5b63714bacc57002c2a';          BINARY_URL='https://github.com/adoptium/temurin8-binaries/releases/download/jdk8u362-b09/OpenJDK8U-jdk_aarch64_linux_hotspot_8u362b09.tar.gz';          ;;        armhf|arm)          ESUM='039843c200d0773fe927fa07c368f23d1d74ae58edd09138c97aa1f5e2007b28';          BINARY_URL='https://github.com/adoptium/temurin8-binaries/releases/download/jdk8u362-b09/OpenJDK8U-jdk_arm_linux_hotspot_8u362b09.tar.gz';          apt-get update          && DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends libatomic1          && rm -rf /var/lib/apt/lists/*          ;;        ppc64el|powerpc:common64)          ESUM='69658dd316c6a160915655971573179766e19c6610ea03880c1e578a0e518f74';          BINARY_URL='https://github.com/adoptium/temurin8-binaries/releases/download/jdk8u362-b09/OpenJDK8U-jdk_ppc64le_linux_hotspot_8u362b09.tar.gz';          ;;        amd64|i386:x86-64)          ESUM='1486a792fb224611ce0cd0e83d4aacd3503b56698549f8e9a9f0a6ebb83bdba1';          BINARY_URL='https://github.com/adoptium/temurin8-binaries/releases/download/jdk8u362-b09/OpenJDK8U-jdk_x64_linux_hotspot_8u362b09.tar.gz';          ;;        *)          echo "Unsupported arch: ${ARCH}";          exit 1;          ;;     esac; 	  wget -O /tmp/openjdk.tar.gz ${BINARY_URL}; 	  echo "${ESUM} */tmp/openjdk.tar.gz" | sha256sum -c -; 	  mkdir -p "$JAVA_HOME"; 	  tar --extract 	      --file /tmp/openjdk.tar.gz 	      --directory "$JAVA_HOME" 	      --strip-components 1 	      --no-same-owner 	  ;     rm -f /tmp/openjdk.tar.gz ${JAVA_HOME}/src.zip;     find "$JAVA_HOME/lib" -name '*.so' -exec dirname '{}' ';' | sort -u > /etc/ld.so.conf.d/docker-openjdk.conf;     ldconfig;
# Tue, 31 Jan 2023 20:26:56 GMT
RUN echo Verifying install ...     && echo javac -version && javac -version     && echo java -version && java -version     && echo Complete.
# Wed, 01 Feb 2023 03:39:55 GMT
CMD ["gradle"]
# Wed, 01 Feb 2023 03:39:55 GMT
ENV GRADLE_HOME=/opt/gradle
# Wed, 01 Feb 2023 03:39:55 GMT
RUN set -o errexit -o nounset     && echo "Adding gradle user and group"     && groupadd --system --gid 1000 gradle     && useradd --system --gid gradle --uid 1000 --shell /bin/bash --create-home gradle     && mkdir /home/gradle/.gradle     && chown --recursive gradle:gradle /home/gradle         && echo "Symlinking root Gradle cache to gradle Gradle cache"     && ln --symbolic /home/gradle/.gradle /root/.gradle
# Wed, 01 Feb 2023 03:39:56 GMT
VOLUME [/home/gradle/.gradle]
# Wed, 01 Feb 2023 03:39:56 GMT
WORKDIR /home/gradle
# Wed, 01 Feb 2023 03:40:30 GMT
RUN set -o errexit -o nounset     && apt-get update     && apt-get install --yes --no-install-recommends         unzip         wget                 bzr         git         git-lfs         mercurial         openssh-client         subversion     && rm --recursive --force /var/lib/apt/lists/*         && echo "Testing VCSes"     && which bzr     && which git     && which git-lfs     && which hg     && which svn
# Wed, 01 Feb 2023 03:43:52 GMT
ENV GRADLE_VERSION=6.9.3
# Wed, 01 Feb 2023 03:43:52 GMT
ARG GRADLE_DOWNLOAD_SHA256=dcf350b8ae1aa192fc299aed6efc77b43825d4fedb224c94118ae7faf5fb035d
# Wed, 01 Feb 2023 03:43:56 GMT
# ARGS: GRADLE_DOWNLOAD_SHA256=dcf350b8ae1aa192fc299aed6efc77b43825d4fedb224c94118ae7faf5fb035d
RUN set -o errexit -o nounset     && echo "Downloading Gradle"     && wget --no-verbose --output-document=gradle.zip "https://services.gradle.org/distributions/gradle-${GRADLE_VERSION}-bin.zip"         && echo "Checking download hash"     && echo "${GRADLE_DOWNLOAD_SHA256} *gradle.zip" | sha256sum --check -         && echo "Installing Gradle"     && unzip gradle.zip     && rm gradle.zip     && mv "gradle-${GRADLE_VERSION}" "${GRADLE_HOME}/"     && ln --symbolic "${GRADLE_HOME}/bin/gradle" /usr/bin/gradle         && echo "Testing Gradle installation"     && gradle --version
```

-	Layers:
	-	`sha256:7608715873ec5c02d370e963aa9b19a149023ce218887221d93fe671b3abbf58`  
		Last Modified: Thu, 26 Jan 2023 17:04:53 GMT  
		Size: 28.6 MB (28577884 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0587d987c59813530b009ec9161a9b2baad8bda1c2a3634a8cd20458399e4aab`  
		Last Modified: Tue, 31 Jan 2023 20:33:27 GMT  
		Size: 16.3 MB (16335030 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e91d1a30eee0d214d1b40d1f21a168fc21abf29c4740bd483541ea278ed4d6f0`  
		Last Modified: Tue, 31 Jan 2023 20:33:32 GMT  
		Size: 54.6 MB (54635869 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b7e8e401d0cb917e928a3393461805fc9216b5c30beb5fa4c5a7438a026fc538`  
		Last Modified: Tue, 31 Jan 2023 20:33:25 GMT  
		Size: 161.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2a9f2e5d5f75bf0950cb1479611e07e226bb19ebaa3cb50d6eefd0b3487b43aa`  
		Last Modified: Wed, 01 Feb 2023 03:47:00 GMT  
		Size: 4.4 KB (4355 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:242d574f2f1da826dba7b865808f9a0d0b35874b6798b00e1504f8f92a70fe83`  
		Last Modified: Wed, 01 Feb 2023 03:47:12 GMT  
		Size: 65.3 MB (65308208 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:71da77c5d0cfe0e5fd4592b123732f991caa7893229d8931d9fe60102e603d96`  
		Last Modified: Wed, 01 Feb 2023 03:52:01 GMT  
		Size: 107.7 MB (107691710 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `gradle:6-jdk8-focal` - linux; arm variant v7

```console
$ docker pull gradle@sha256:f21cf5ae99372ba9cd67150a940125a65e9919fd50a2c08028cd20a42c67ba8e
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **257.5 MB (257472505 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e488385e1d95b59d448630067fbd4c3a5ba3c1f36170f9c9821ebdff88f70148`
-	Default Command: `["gradle"]`

```dockerfile
# Thu, 26 Jan 2023 13:35:44 GMT
ARG RELEASE
# Thu, 26 Jan 2023 13:35:44 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Thu, 26 Jan 2023 13:35:44 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Thu, 26 Jan 2023 13:35:44 GMT
LABEL org.opencontainers.image.version=20.04
# Thu, 26 Jan 2023 13:35:48 GMT
ADD file:6566d63937dd1808d3a4ea5591d4369b9083772d48fad60626fb91243a9f3f53 in / 
# Thu, 26 Jan 2023 13:35:49 GMT
CMD ["/bin/bash"]
# Tue, 31 Jan 2023 18:54:20 GMT
ENV JAVA_HOME=/opt/java/openjdk
# Tue, 31 Jan 2023 18:54:20 GMT
ENV PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 31 Jan 2023 18:54:21 GMT
ENV LANG=en_US.UTF-8 LANGUAGE=en_US:en LC_ALL=en_US.UTF-8
# Tue, 31 Jan 2023 18:54:40 GMT
RUN apt-get update     && DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends tzdata curl wget ca-certificates fontconfig locales     && echo "en_US.UTF-8 UTF-8" >> /etc/locale.gen     && locale-gen en_US.UTF-8     && rm -rf /var/lib/apt/lists/*
# Tue, 31 Jan 2023 18:54:40 GMT
ENV JAVA_VERSION=jdk8u362-b09
# Tue, 31 Jan 2023 18:54:49 GMT
RUN set -eux;     ARCH="$(dpkg --print-architecture)";     case "${ARCH}" in        aarch64|arm64)          ESUM='9290a8beefd7a94f0eb030f62d402411a852100482b9c5b63714bacc57002c2a';          BINARY_URL='https://github.com/adoptium/temurin8-binaries/releases/download/jdk8u362-b09/OpenJDK8U-jdk_aarch64_linux_hotspot_8u362b09.tar.gz';          ;;        armhf|arm)          ESUM='039843c200d0773fe927fa07c368f23d1d74ae58edd09138c97aa1f5e2007b28';          BINARY_URL='https://github.com/adoptium/temurin8-binaries/releases/download/jdk8u362-b09/OpenJDK8U-jdk_arm_linux_hotspot_8u362b09.tar.gz';          apt-get update          && DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends libatomic1          && rm -rf /var/lib/apt/lists/*          ;;        ppc64el|powerpc:common64)          ESUM='69658dd316c6a160915655971573179766e19c6610ea03880c1e578a0e518f74';          BINARY_URL='https://github.com/adoptium/temurin8-binaries/releases/download/jdk8u362-b09/OpenJDK8U-jdk_ppc64le_linux_hotspot_8u362b09.tar.gz';          ;;        amd64|i386:x86-64)          ESUM='1486a792fb224611ce0cd0e83d4aacd3503b56698549f8e9a9f0a6ebb83bdba1';          BINARY_URL='https://github.com/adoptium/temurin8-binaries/releases/download/jdk8u362-b09/OpenJDK8U-jdk_x64_linux_hotspot_8u362b09.tar.gz';          ;;        *)          echo "Unsupported arch: ${ARCH}";          exit 1;          ;;     esac; 	  wget -O /tmp/openjdk.tar.gz ${BINARY_URL}; 	  echo "${ESUM} */tmp/openjdk.tar.gz" | sha256sum -c -; 	  mkdir -p "$JAVA_HOME"; 	  tar --extract 	      --file /tmp/openjdk.tar.gz 	      --directory "$JAVA_HOME" 	      --strip-components 1 	      --no-same-owner 	  ;     rm -f /tmp/openjdk.tar.gz ${JAVA_HOME}/src.zip;     find "$JAVA_HOME/lib" -name '*.so' -exec dirname '{}' ';' | sort -u > /etc/ld.so.conf.d/docker-openjdk.conf;     ldconfig;
# Tue, 31 Jan 2023 18:54:50 GMT
RUN echo Verifying install ...     && echo javac -version && javac -version     && echo java -version && java -version     && echo Complete.
# Tue, 31 Jan 2023 21:04:17 GMT
CMD ["gradle"]
# Tue, 31 Jan 2023 21:04:17 GMT
ENV GRADLE_HOME=/opt/gradle
# Tue, 31 Jan 2023 21:04:18 GMT
RUN set -o errexit -o nounset     && echo "Adding gradle user and group"     && groupadd --system --gid 1000 gradle     && useradd --system --gid gradle --uid 1000 --shell /bin/bash --create-home gradle     && mkdir /home/gradle/.gradle     && chown --recursive gradle:gradle /home/gradle         && echo "Symlinking root Gradle cache to gradle Gradle cache"     && ln --symbolic /home/gradle/.gradle /root/.gradle
# Tue, 31 Jan 2023 21:04:18 GMT
VOLUME [/home/gradle/.gradle]
# Tue, 31 Jan 2023 21:04:18 GMT
WORKDIR /home/gradle
# Tue, 31 Jan 2023 21:05:04 GMT
RUN set -o errexit -o nounset     && apt-get update     && apt-get install --yes --no-install-recommends         unzip         wget                 bzr         git         git-lfs         mercurial         openssh-client         subversion     && rm --recursive --force /var/lib/apt/lists/*         && echo "Testing VCSes"     && which bzr     && which git     && which git-lfs     && which hg     && which svn
# Tue, 31 Jan 2023 21:08:53 GMT
ENV GRADLE_VERSION=6.9.3
# Tue, 31 Jan 2023 21:08:53 GMT
ARG GRADLE_DOWNLOAD_SHA256=dcf350b8ae1aa192fc299aed6efc77b43825d4fedb224c94118ae7faf5fb035d
# Tue, 31 Jan 2023 21:08:58 GMT
# ARGS: GRADLE_DOWNLOAD_SHA256=dcf350b8ae1aa192fc299aed6efc77b43825d4fedb224c94118ae7faf5fb035d
RUN set -o errexit -o nounset     && echo "Downloading Gradle"     && wget --no-verbose --output-document=gradle.zip "https://services.gradle.org/distributions/gradle-${GRADLE_VERSION}-bin.zip"         && echo "Checking download hash"     && echo "${GRADLE_DOWNLOAD_SHA256} *gradle.zip" | sha256sum --check -         && echo "Installing Gradle"     && unzip gradle.zip     && rm gradle.zip     && mv "gradle-${GRADLE_VERSION}" "${GRADLE_HOME}/"     && ln --symbolic "${GRADLE_HOME}/bin/gradle" /usr/bin/gradle         && echo "Testing Gradle installation"     && gradle --version
```

-	Layers:
	-	`sha256:316383d79e03258e1fee780854f6da78da364194ded4ace8bff50687070e1c8f`  
		Last Modified: Sat, 28 Jan 2023 04:40:09 GMT  
		Size: 24.6 MB (24586318 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:33ba80e2bd146e3878fc84a21e17e310b8a1a2b004207eb1e3db2b748f4c5936`  
		Last Modified: Tue, 31 Jan 2023 19:03:55 GMT  
		Size: 15.2 MB (15174763 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fea02d1ac732021141686cb59a4b988200b2bcf9d784d551292c4facf0d39232`  
		Last Modified: Tue, 31 Jan 2023 19:04:01 GMT  
		Size: 50.3 MB (50297247 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0c5a1f505f9098c0480e6a8e0c87139127e4d68da1d71e546152f1441b6fbc8c`  
		Last Modified: Tue, 31 Jan 2023 19:03:52 GMT  
		Size: 128.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d65f59a52fa49603359f9cb9825faecf2bc640ed1cca04e76e25e7b3bf77bd97`  
		Last Modified: Tue, 31 Jan 2023 21:15:15 GMT  
		Size: 4.3 KB (4314 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dfbd24c5552d1a58dbf3150330c37ca442afa94eff6b2c401723bc0c385cf7b2`  
		Last Modified: Tue, 31 Jan 2023 21:15:27 GMT  
		Size: 59.7 MB (59718036 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cbc3858c31fe9b25c855a362140b5f931eceacd48ed7c32558810fba9747b1d4`  
		Last Modified: Tue, 31 Jan 2023 21:21:32 GMT  
		Size: 107.7 MB (107691699 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `gradle:6-jdk8-focal` - linux; arm64 variant v8

```console
$ docker pull gradle@sha256:ed884b3b7d5d4431c9e06366dfa46f65c0acf17e66271c83841d81ab4e202a3a
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **269.9 MB (269876440 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:71d649bb9f536509486439a1b56aeeec4c01e930807dc3beb8083516d2151a57`
-	Default Command: `["gradle"]`

```dockerfile
# Thu, 26 Jan 2023 13:50:26 GMT
ARG RELEASE
# Thu, 26 Jan 2023 13:50:26 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Thu, 26 Jan 2023 13:50:26 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Thu, 26 Jan 2023 13:50:26 GMT
LABEL org.opencontainers.image.version=20.04
# Thu, 26 Jan 2023 13:50:33 GMT
ADD file:72ca0af0100de6591b59c44bd8856655c8441eb0fcbf7c32e427f6be5108a4a4 in / 
# Thu, 26 Jan 2023 13:50:33 GMT
CMD ["/bin/bash"]
# Tue, 31 Jan 2023 17:43:17 GMT
ENV JAVA_HOME=/opt/java/openjdk
# Tue, 31 Jan 2023 17:43:17 GMT
ENV PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 31 Jan 2023 17:43:17 GMT
ENV LANG=en_US.UTF-8 LANGUAGE=en_US:en LC_ALL=en_US.UTF-8
# Tue, 31 Jan 2023 17:43:47 GMT
RUN apt-get update     && DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends tzdata curl wget ca-certificates fontconfig locales     && echo "en_US.UTF-8 UTF-8" >> /etc/locale.gen     && locale-gen en_US.UTF-8     && rm -rf /var/lib/apt/lists/*
# Tue, 31 Jan 2023 17:43:47 GMT
ENV JAVA_VERSION=jdk8u362-b09
# Tue, 31 Jan 2023 17:43:53 GMT
RUN set -eux;     ARCH="$(dpkg --print-architecture)";     case "${ARCH}" in        aarch64|arm64)          ESUM='9290a8beefd7a94f0eb030f62d402411a852100482b9c5b63714bacc57002c2a';          BINARY_URL='https://github.com/adoptium/temurin8-binaries/releases/download/jdk8u362-b09/OpenJDK8U-jdk_aarch64_linux_hotspot_8u362b09.tar.gz';          ;;        armhf|arm)          ESUM='039843c200d0773fe927fa07c368f23d1d74ae58edd09138c97aa1f5e2007b28';          BINARY_URL='https://github.com/adoptium/temurin8-binaries/releases/download/jdk8u362-b09/OpenJDK8U-jdk_arm_linux_hotspot_8u362b09.tar.gz';          apt-get update          && DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends libatomic1          && rm -rf /var/lib/apt/lists/*          ;;        ppc64el|powerpc:common64)          ESUM='69658dd316c6a160915655971573179766e19c6610ea03880c1e578a0e518f74';          BINARY_URL='https://github.com/adoptium/temurin8-binaries/releases/download/jdk8u362-b09/OpenJDK8U-jdk_ppc64le_linux_hotspot_8u362b09.tar.gz';          ;;        amd64|i386:x86-64)          ESUM='1486a792fb224611ce0cd0e83d4aacd3503b56698549f8e9a9f0a6ebb83bdba1';          BINARY_URL='https://github.com/adoptium/temurin8-binaries/releases/download/jdk8u362-b09/OpenJDK8U-jdk_x64_linux_hotspot_8u362b09.tar.gz';          ;;        *)          echo "Unsupported arch: ${ARCH}";          exit 1;          ;;     esac; 	  wget -O /tmp/openjdk.tar.gz ${BINARY_URL}; 	  echo "${ESUM} */tmp/openjdk.tar.gz" | sha256sum -c -; 	  mkdir -p "$JAVA_HOME"; 	  tar --extract 	      --file /tmp/openjdk.tar.gz 	      --directory "$JAVA_HOME" 	      --strip-components 1 	      --no-same-owner 	  ;     rm -f /tmp/openjdk.tar.gz ${JAVA_HOME}/src.zip;     find "$JAVA_HOME/lib" -name '*.so' -exec dirname '{}' ';' | sort -u > /etc/ld.so.conf.d/docker-openjdk.conf;     ldconfig;
# Tue, 31 Jan 2023 17:43:54 GMT
RUN echo Verifying install ...     && echo javac -version && javac -version     && echo java -version && java -version     && echo Complete.
# Tue, 31 Jan 2023 21:25:58 GMT
CMD ["gradle"]
# Tue, 31 Jan 2023 21:25:58 GMT
ENV GRADLE_HOME=/opt/gradle
# Tue, 31 Jan 2023 21:25:58 GMT
RUN set -o errexit -o nounset     && echo "Adding gradle user and group"     && groupadd --system --gid 1000 gradle     && useradd --system --gid gradle --uid 1000 --shell /bin/bash --create-home gradle     && mkdir /home/gradle/.gradle     && chown --recursive gradle:gradle /home/gradle         && echo "Symlinking root Gradle cache to gradle Gradle cache"     && ln --symbolic /home/gradle/.gradle /root/.gradle
# Tue, 31 Jan 2023 21:25:58 GMT
VOLUME [/home/gradle/.gradle]
# Tue, 31 Jan 2023 21:25:58 GMT
WORKDIR /home/gradle
# Tue, 31 Jan 2023 21:26:35 GMT
RUN set -o errexit -o nounset     && apt-get update     && apt-get install --yes --no-install-recommends         unzip         wget                 bzr         git         git-lfs         mercurial         openssh-client         subversion     && rm --recursive --force /var/lib/apt/lists/*         && echo "Testing VCSes"     && which bzr     && which git     && which git-lfs     && which hg     && which svn
# Tue, 31 Jan 2023 21:29:17 GMT
ENV GRADLE_VERSION=6.9.3
# Tue, 31 Jan 2023 21:29:17 GMT
ARG GRADLE_DOWNLOAD_SHA256=dcf350b8ae1aa192fc299aed6efc77b43825d4fedb224c94118ae7faf5fb035d
# Tue, 31 Jan 2023 21:29:20 GMT
# ARGS: GRADLE_DOWNLOAD_SHA256=dcf350b8ae1aa192fc299aed6efc77b43825d4fedb224c94118ae7faf5fb035d
RUN set -o errexit -o nounset     && echo "Downloading Gradle"     && wget --no-verbose --output-document=gradle.zip "https://services.gradle.org/distributions/gradle-${GRADLE_VERSION}-bin.zip"         && echo "Checking download hash"     && echo "${GRADLE_DOWNLOAD_SHA256} *gradle.zip" | sha256sum --check -         && echo "Installing Gradle"     && unzip gradle.zip     && rm gradle.zip     && mv "gradle-${GRADLE_VERSION}" "${GRADLE_HOME}/"     && ln --symbolic "${GRADLE_HOME}/bin/gradle" /usr/bin/gradle         && echo "Testing Gradle installation"     && gradle --version
```

-	Layers:
	-	`sha256:70cf24b162395e1500d40f2b012f253bfd5d15f029ef9d636620fa2365ae503c`  
		Last Modified: Sat, 28 Jan 2023 04:42:53 GMT  
		Size: 27.2 MB (27193737 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3df2d776c5c5ff7acd285901b61b2f581c9497f13a32d1a49db14e3a2b7536be`  
		Last Modified: Tue, 31 Jan 2023 17:50:10 GMT  
		Size: 16.2 MB (16204764 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8d4103d41b1c8038835a70eb150c22630469a69dc0fbf4d2a145a66fd5933fa4`  
		Last Modified: Tue, 31 Jan 2023 17:50:14 GMT  
		Size: 53.7 MB (53731802 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:01405e9f1524563ba14196dbf4b895c52e338e811525843741ebfd476059064d`  
		Last Modified: Tue, 31 Jan 2023 17:50:08 GMT  
		Size: 162.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:426abf54b27179686c04f3c09f5c224600165ed6f065cc5401bcba365f2b8654`  
		Last Modified: Tue, 31 Jan 2023 21:32:07 GMT  
		Size: 4.4 KB (4363 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:437e89192e4744563904f8773583e5c9612022456ee20267673a4b85cf7dd81b`  
		Last Modified: Tue, 31 Jan 2023 21:32:16 GMT  
		Size: 65.0 MB (65049910 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0a4b74f1fd6479ca8a48c72070c79e2c3d9f3be2d938fe2c7197c26031f5b1dc`  
		Last Modified: Tue, 31 Jan 2023 21:36:24 GMT  
		Size: 107.7 MB (107691702 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `gradle:6-jdk8-focal` - linux; ppc64le

```console
$ docker pull gradle@sha256:2de39fa1064d124f21681c0bffcc828b2ffa409525b7c5ce111ea6057509b7b5
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **284.4 MB (284419726 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:7116d58ef2e22f37852a8b16459d4bb4b95430d011963efec415749409625097`
-	Default Command: `["gradle"]`

```dockerfile
# Thu, 26 Jan 2023 13:47:16 GMT
ARG RELEASE
# Thu, 26 Jan 2023 13:47:16 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Thu, 26 Jan 2023 13:47:17 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Thu, 26 Jan 2023 13:47:17 GMT
LABEL org.opencontainers.image.version=20.04
# Thu, 26 Jan 2023 13:47:20 GMT
ADD file:987b941a34ad98533c64e74a3d57b9c1b983ff16c8f36e21d29278a30a2403ee in / 
# Thu, 26 Jan 2023 13:47:20 GMT
CMD ["/bin/bash"]
# Tue, 31 Jan 2023 18:22:07 GMT
ENV JAVA_HOME=/opt/java/openjdk
# Tue, 31 Jan 2023 18:22:08 GMT
ENV PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 31 Jan 2023 18:22:08 GMT
ENV LANG=en_US.UTF-8 LANGUAGE=en_US:en LC_ALL=en_US.UTF-8
# Tue, 31 Jan 2023 18:22:35 GMT
RUN apt-get update     && DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends tzdata curl wget ca-certificates fontconfig locales     && echo "en_US.UTF-8 UTF-8" >> /etc/locale.gen     && locale-gen en_US.UTF-8     && rm -rf /var/lib/apt/lists/*
# Tue, 31 Jan 2023 18:22:36 GMT
ENV JAVA_VERSION=jdk8u362-b09
# Tue, 31 Jan 2023 18:22:46 GMT
RUN set -eux;     ARCH="$(dpkg --print-architecture)";     case "${ARCH}" in        aarch64|arm64)          ESUM='9290a8beefd7a94f0eb030f62d402411a852100482b9c5b63714bacc57002c2a';          BINARY_URL='https://github.com/adoptium/temurin8-binaries/releases/download/jdk8u362-b09/OpenJDK8U-jdk_aarch64_linux_hotspot_8u362b09.tar.gz';          ;;        armhf|arm)          ESUM='039843c200d0773fe927fa07c368f23d1d74ae58edd09138c97aa1f5e2007b28';          BINARY_URL='https://github.com/adoptium/temurin8-binaries/releases/download/jdk8u362-b09/OpenJDK8U-jdk_arm_linux_hotspot_8u362b09.tar.gz';          apt-get update          && DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends libatomic1          && rm -rf /var/lib/apt/lists/*          ;;        ppc64el|powerpc:common64)          ESUM='69658dd316c6a160915655971573179766e19c6610ea03880c1e578a0e518f74';          BINARY_URL='https://github.com/adoptium/temurin8-binaries/releases/download/jdk8u362-b09/OpenJDK8U-jdk_ppc64le_linux_hotspot_8u362b09.tar.gz';          ;;        amd64|i386:x86-64)          ESUM='1486a792fb224611ce0cd0e83d4aacd3503b56698549f8e9a9f0a6ebb83bdba1';          BINARY_URL='https://github.com/adoptium/temurin8-binaries/releases/download/jdk8u362-b09/OpenJDK8U-jdk_x64_linux_hotspot_8u362b09.tar.gz';          ;;        *)          echo "Unsupported arch: ${ARCH}";          exit 1;          ;;     esac; 	  wget -O /tmp/openjdk.tar.gz ${BINARY_URL}; 	  echo "${ESUM} */tmp/openjdk.tar.gz" | sha256sum -c -; 	  mkdir -p "$JAVA_HOME"; 	  tar --extract 	      --file /tmp/openjdk.tar.gz 	      --directory "$JAVA_HOME" 	      --strip-components 1 	      --no-same-owner 	  ;     rm -f /tmp/openjdk.tar.gz ${JAVA_HOME}/src.zip;     find "$JAVA_HOME/lib" -name '*.so' -exec dirname '{}' ';' | sort -u > /etc/ld.so.conf.d/docker-openjdk.conf;     ldconfig;
# Tue, 31 Jan 2023 18:22:49 GMT
RUN echo Verifying install ...     && echo javac -version && javac -version     && echo java -version && java -version     && echo Complete.
# Tue, 31 Jan 2023 22:06:16 GMT
CMD ["gradle"]
# Tue, 31 Jan 2023 22:06:17 GMT
ENV GRADLE_HOME=/opt/gradle
# Tue, 31 Jan 2023 22:06:18 GMT
RUN set -o errexit -o nounset     && echo "Adding gradle user and group"     && groupadd --system --gid 1000 gradle     && useradd --system --gid gradle --uid 1000 --shell /bin/bash --create-home gradle     && mkdir /home/gradle/.gradle     && chown --recursive gradle:gradle /home/gradle         && echo "Symlinking root Gradle cache to gradle Gradle cache"     && ln --symbolic /home/gradle/.gradle /root/.gradle
# Tue, 31 Jan 2023 22:06:19 GMT
VOLUME [/home/gradle/.gradle]
# Tue, 31 Jan 2023 22:06:19 GMT
WORKDIR /home/gradle
# Tue, 31 Jan 2023 22:07:18 GMT
RUN set -o errexit -o nounset     && apt-get update     && apt-get install --yes --no-install-recommends         unzip         wget                 bzr         git         git-lfs         mercurial         openssh-client         subversion     && rm --recursive --force /var/lib/apt/lists/*         && echo "Testing VCSes"     && which bzr     && which git     && which git-lfs     && which hg     && which svn
# Tue, 31 Jan 2023 22:14:36 GMT
ENV GRADLE_VERSION=6.9.3
# Tue, 31 Jan 2023 22:14:37 GMT
ARG GRADLE_DOWNLOAD_SHA256=dcf350b8ae1aa192fc299aed6efc77b43825d4fedb224c94118ae7faf5fb035d
# Tue, 31 Jan 2023 22:14:45 GMT
# ARGS: GRADLE_DOWNLOAD_SHA256=dcf350b8ae1aa192fc299aed6efc77b43825d4fedb224c94118ae7faf5fb035d
RUN set -o errexit -o nounset     && echo "Downloading Gradle"     && wget --no-verbose --output-document=gradle.zip "https://services.gradle.org/distributions/gradle-${GRADLE_VERSION}-bin.zip"         && echo "Checking download hash"     && echo "${GRADLE_DOWNLOAD_SHA256} *gradle.zip" | sha256sum --check -         && echo "Installing Gradle"     && unzip gradle.zip     && rm gradle.zip     && mv "gradle-${GRADLE_VERSION}" "${GRADLE_HOME}/"     && ln --symbolic "${GRADLE_HOME}/bin/gradle" /usr/bin/gradle         && echo "Testing Gradle installation"     && gradle --version
```

-	Layers:
	-	`sha256:0c2f997991bfe2ed920105bb595c3662038cc90a08c6db9888fffdfa8c673b16`  
		Last Modified: Tue, 31 Jan 2023 18:14:55 GMT  
		Size: 33.3 MB (33300341 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4b573c30570715eb291b5f8080eacf60d0995c5769e831ad724b215d3381bb36`  
		Last Modified: Tue, 31 Jan 2023 18:34:49 GMT  
		Size: 17.6 MB (17572772 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f0a7ccebde94db8fcdab4768c6b91e7380293bcb5f30b4a1fb979b127b1c639f`  
		Last Modified: Tue, 31 Jan 2023 18:34:55 GMT  
		Size: 52.1 MB (52113617 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:26c6eb87868ab07c57f819c1d428d609a8f402fdb972382918c12413a7732bfc`  
		Last Modified: Tue, 31 Jan 2023 18:34:44 GMT  
		Size: 162.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1bae331b522a9b2a6ad81ae7751f3eb40d6e37813bb40aecfcb7c9702bd27f50`  
		Last Modified: Tue, 31 Jan 2023 22:20:39 GMT  
		Size: 4.4 KB (4356 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:906003e9473b547be429fb8be077814ebefcdd83b9bd500e4402fc77c218b11b`  
		Last Modified: Tue, 31 Jan 2023 22:20:59 GMT  
		Size: 73.7 MB (73736816 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:86c458a689956df4cb69ecd4598eb7fd544e2441c67b3631f46b6eb2490c9b93`  
		Last Modified: Tue, 31 Jan 2023 22:27:29 GMT  
		Size: 107.7 MB (107691662 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
