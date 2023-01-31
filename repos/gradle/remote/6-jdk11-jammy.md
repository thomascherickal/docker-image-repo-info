## `gradle:6-jdk11-jammy`

```console
$ docker pull gradle@sha256:e28290fa0c83a145d414808edf69706d65d159b53dd3456d43a0db44b5332b38
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 5
	-	linux; amd64
	-	linux; arm variant v7
	-	linux; arm64 variant v8
	-	linux; ppc64le
	-	linux; s390x

### `gradle:6-jdk11-jammy` - linux; amd64

```console
$ docker pull gradle@sha256:5162c8648b304424a378768f746fac3a78e02183679f845a8cd7c16678fffba7
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **400.3 MB (400296149 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:20d5a2dcbc935ae3c3df042af79e4de54a3ca6ac5c6720737fc7bd6196841b34`
-	Default Command: `["gradle"]`

```dockerfile
# Fri, 09 Dec 2022 01:20:30 GMT
ADD file:481dd2da6de71525248eba186feeeafcc73cc956ade0a196a4e8b0c2424e74b9 in / 
# Fri, 09 Dec 2022 01:20:31 GMT
CMD ["bash"]
# Fri, 09 Dec 2022 01:42:58 GMT
ENV JAVA_HOME=/opt/java/openjdk
# Fri, 09 Dec 2022 01:42:58 GMT
ENV PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Fri, 09 Dec 2022 01:42:58 GMT
ENV LANG=en_US.UTF-8 LANGUAGE=en_US:en LC_ALL=en_US.UTF-8
# Fri, 09 Dec 2022 01:43:29 GMT
RUN apt-get update     && DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends tzdata curl wget ca-certificates fontconfig locales     && echo "en_US.UTF-8 UTF-8" >> /etc/locale.gen     && locale-gen en_US.UTF-8     && rm -rf /var/lib/apt/lists/*
# Tue, 24 Jan 2023 18:43:59 GMT
ENV JAVA_VERSION=jdk-11.0.18+10
# Tue, 24 Jan 2023 18:44:07 GMT
RUN set -eux;     ARCH="$(dpkg --print-architecture)";     case "${ARCH}" in        aarch64|arm64)          ESUM='04d5eeff6a6449bcdca0f52cd97bafd43ce09d40ef1e73fa0e1add63bea4a9c8';          BINARY_URL='https://github.com/adoptium/temurin11-binaries/releases/download/jdk-11.0.18%2B10/OpenJDK11U-jdk_aarch64_linux_hotspot_11.0.18_10.tar.gz';          ;;        armhf|arm)          ESUM='b42840ef88621f87a4b49ae3a8db23dbf07cd9e7fb62823318709a592f597ea3';          BINARY_URL='https://github.com/adoptium/temurin11-binaries/releases/download/jdk-11.0.18%2B10/OpenJDK11U-jdk_arm_linux_hotspot_11.0.18_10.tar.gz';          ;;        ppc64el|powerpc:common64)          ESUM='459148d489b08ceec2d901e950ac36722b4c55e907e979291ddfc954ebdcea47';          BINARY_URL='https://github.com/adoptium/temurin11-binaries/releases/download/jdk-11.0.18%2B10/OpenJDK11U-jdk_ppc64le_linux_hotspot_11.0.18_10.tar.gz';          ;;        s390x|s390:64-bit)          ESUM='7a7193c8279dd889c0a39296bcbae8866d94cff7a6d1bdfe676ffe4ced018915';          BINARY_URL='https://github.com/adoptium/temurin11-binaries/releases/download/jdk-11.0.18%2B10/OpenJDK11U-jdk_s390x_linux_hotspot_11.0.18_10.tar.gz';          ;;        amd64|i386:x86-64)          ESUM='4a29efda1d702b8ff38e554cf932051f40ec70006caed5c4857a8cbc7a0b7db7';          BINARY_URL='https://github.com/adoptium/temurin11-binaries/releases/download/jdk-11.0.18%2B10/OpenJDK11U-jdk_x64_linux_hotspot_11.0.18_10.tar.gz';          ;;        *)          echo "Unsupported arch: ${ARCH}";          exit 1;          ;;     esac; 	  wget -O /tmp/openjdk.tar.gz ${BINARY_URL}; 	  echo "${ESUM} */tmp/openjdk.tar.gz" | sha256sum -c -; 	  mkdir -p "$JAVA_HOME"; 	  tar --extract 	      --file /tmp/openjdk.tar.gz 	      --directory "$JAVA_HOME" 	      --strip-components 1 	      --no-same-owner 	  ;     rm -f /tmp/openjdk.tar.gz ${JAVA_HOME}/src.zip;     find "$JAVA_HOME/lib" -name '*.so' -exec dirname '{}' ';' | sort -u > /etc/ld.so.conf.d/docker-openjdk.conf;     ldconfig;     java -Xshare:dump;
# Tue, 24 Jan 2023 18:44:10 GMT
RUN echo Verifying install ...     && fileEncoding="$(echo 'System.out.println(System.getProperty("file.encoding"))' | jshell -s -)"; [ "$fileEncoding" = 'UTF-8' ]; rm -rf ~/.java     && echo javac --version && javac --version     && echo java --version && java --version     && echo Complete.
# Tue, 24 Jan 2023 18:44:10 GMT
CMD ["jshell"]
# Tue, 24 Jan 2023 22:34:37 GMT
CMD ["gradle"]
# Tue, 24 Jan 2023 22:34:37 GMT
ENV GRADLE_HOME=/opt/gradle
# Tue, 24 Jan 2023 22:34:38 GMT
RUN set -o errexit -o nounset     && echo "Adding gradle user and group"     && groupadd --system --gid 1000 gradle     && useradd --system --gid gradle --uid 1000 --shell /bin/bash --create-home gradle     && mkdir /home/gradle/.gradle     && chown --recursive gradle:gradle /home/gradle         && echo "Symlinking root Gradle cache to gradle Gradle cache"     && ln --symbolic /home/gradle/.gradle /root/.gradle
# Tue, 24 Jan 2023 22:34:38 GMT
VOLUME [/home/gradle/.gradle]
# Tue, 24 Jan 2023 22:34:38 GMT
WORKDIR /home/gradle
# Tue, 24 Jan 2023 22:35:07 GMT
RUN set -o errexit -o nounset     && apt-get update     && apt-get install --yes --no-install-recommends         unzip         wget                 bzr         git         git-lfs         mercurial         openssh-client         subversion     && rm --recursive --force /var/lib/apt/lists/*         && echo "Testing VCSes"     && which bzr     && which git     && which git-lfs     && which hg     && which svn
# Tue, 24 Jan 2023 22:37:48 GMT
ENV GRADLE_VERSION=6.9.3
# Tue, 24 Jan 2023 22:37:48 GMT
ARG GRADLE_DOWNLOAD_SHA256=dcf350b8ae1aa192fc299aed6efc77b43825d4fedb224c94118ae7faf5fb035d
# Tue, 24 Jan 2023 22:37:52 GMT
# ARGS: GRADLE_DOWNLOAD_SHA256=dcf350b8ae1aa192fc299aed6efc77b43825d4fedb224c94118ae7faf5fb035d
RUN set -o errexit -o nounset     && echo "Downloading Gradle"     && wget --no-verbose --output-document=gradle.zip "https://services.gradle.org/distributions/gradle-${GRADLE_VERSION}-bin.zip"         && echo "Checking download hash"     && echo "${GRADLE_DOWNLOAD_SHA256} *gradle.zip" | sha256sum --check -         && echo "Installing Gradle"     && unzip gradle.zip     && rm gradle.zip     && mv "gradle-${GRADLE_VERSION}" "${GRADLE_HOME}/"     && ln --symbolic "${GRADLE_HOME}/bin/gradle" /usr/bin/gradle         && echo "Testing Gradle installation"     && gradle --version
```

-	Layers:
	-	`sha256:6e3729cf69e0ce2de9e779575a1fec8b7fb5efdfa822829290ab6d5d1bc3e797`  
		Last Modified: Thu, 08 Dec 2022 14:10:00 GMT  
		Size: 30.4 MB (30428708 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:96aa423488f0ed1e9bf6c6da11fa7fb53568d1ea4003892416b3adeccb47e3bf`  
		Last Modified: Fri, 09 Dec 2022 01:50:02 GMT  
		Size: 12.4 MB (12432218 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5231e9d0739b4e4d246bcb85210907656b461b7e455e8f94317955bf08c2d314`  
		Last Modified: Tue, 24 Jan 2023 18:50:50 GMT  
		Size: 198.5 MB (198487760 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:36a77878489014a05507aa57bbd74c4fa228b99b14f5d852ab4677ca302a4673`  
		Last Modified: Tue, 24 Jan 2023 18:50:35 GMT  
		Size: 173.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:754a1d9987fe190a84250b126e0ef10db7e5b9a89e08d33c7593c1d068df95d6`  
		Last Modified: Tue, 24 Jan 2023 22:40:41 GMT  
		Size: 4.4 KB (4364 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0d5f6d522908b70ab9fa4e8d0b391211dd042b335015b93eebb5d1abaa2b6a04`  
		Last Modified: Tue, 24 Jan 2023 22:40:50 GMT  
		Size: 51.3 MB (51251218 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:df04a4d50e0f089292e456e18603c713bfd6026ff58dc5ff16b2ed9f0d2fd62e`  
		Last Modified: Tue, 24 Jan 2023 22:44:37 GMT  
		Size: 107.7 MB (107691708 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `gradle:6-jdk11-jammy` - linux; arm variant v7

```console
$ docker pull gradle@sha256:3bee5b6015c2327680d46a53312788a45d936725e72f1e9b6f6cd9e0068bbb89
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **385.9 MB (385943011 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d8a8f5d0b3645bca71f5f3ce50ebdd448adf82b80dacdc6421b9b67a862e5853`
-	Default Command: `["gradle"]`

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
# Tue, 31 Jan 2023 18:57:11 GMT
ENV JAVA_VERSION=jdk-11.0.18+10
# Tue, 31 Jan 2023 18:57:21 GMT
RUN set -eux;     ARCH="$(dpkg --print-architecture)";     case "${ARCH}" in        aarch64|arm64)          ESUM='04d5eeff6a6449bcdca0f52cd97bafd43ce09d40ef1e73fa0e1add63bea4a9c8';          BINARY_URL='https://github.com/adoptium/temurin11-binaries/releases/download/jdk-11.0.18%2B10/OpenJDK11U-jdk_aarch64_linux_hotspot_11.0.18_10.tar.gz';          ;;        armhf|arm)          ESUM='b42840ef88621f87a4b49ae3a8db23dbf07cd9e7fb62823318709a592f597ea3';          BINARY_URL='https://github.com/adoptium/temurin11-binaries/releases/download/jdk-11.0.18%2B10/OpenJDK11U-jdk_arm_linux_hotspot_11.0.18_10.tar.gz';          ;;        ppc64el|powerpc:common64)          ESUM='459148d489b08ceec2d901e950ac36722b4c55e907e979291ddfc954ebdcea47';          BINARY_URL='https://github.com/adoptium/temurin11-binaries/releases/download/jdk-11.0.18%2B10/OpenJDK11U-jdk_ppc64le_linux_hotspot_11.0.18_10.tar.gz';          ;;        s390x|s390:64-bit)          ESUM='7a7193c8279dd889c0a39296bcbae8866d94cff7a6d1bdfe676ffe4ced018915';          BINARY_URL='https://github.com/adoptium/temurin11-binaries/releases/download/jdk-11.0.18%2B10/OpenJDK11U-jdk_s390x_linux_hotspot_11.0.18_10.tar.gz';          ;;        amd64|i386:x86-64)          ESUM='4a29efda1d702b8ff38e554cf932051f40ec70006caed5c4857a8cbc7a0b7db7';          BINARY_URL='https://github.com/adoptium/temurin11-binaries/releases/download/jdk-11.0.18%2B10/OpenJDK11U-jdk_x64_linux_hotspot_11.0.18_10.tar.gz';          ;;        *)          echo "Unsupported arch: ${ARCH}";          exit 1;          ;;     esac; 	  wget -O /tmp/openjdk.tar.gz ${BINARY_URL}; 	  echo "${ESUM} */tmp/openjdk.tar.gz" | sha256sum -c -; 	  mkdir -p "$JAVA_HOME"; 	  tar --extract 	      --file /tmp/openjdk.tar.gz 	      --directory "$JAVA_HOME" 	      --strip-components 1 	      --no-same-owner 	  ;     rm -f /tmp/openjdk.tar.gz ${JAVA_HOME}/src.zip;     find "$JAVA_HOME/lib" -name '*.so' -exec dirname '{}' ';' | sort -u > /etc/ld.so.conf.d/docker-openjdk.conf;     ldconfig;     java -Xshare:dump;
# Tue, 31 Jan 2023 18:57:24 GMT
RUN echo Verifying install ...     && fileEncoding="$(echo 'System.out.println(System.getProperty("file.encoding"))' | jshell -s -)"; [ "$fileEncoding" = 'UTF-8' ]; rm -rf ~/.java     && echo javac --version && javac --version     && echo java --version && java --version     && echo Complete.
# Tue, 31 Jan 2023 18:57:24 GMT
CMD ["jshell"]
# Tue, 31 Jan 2023 21:05:19 GMT
CMD ["gradle"]
# Tue, 31 Jan 2023 21:05:19 GMT
ENV GRADLE_HOME=/opt/gradle
# Tue, 31 Jan 2023 21:05:20 GMT
RUN set -o errexit -o nounset     && echo "Adding gradle user and group"     && groupadd --system --gid 1000 gradle     && useradd --system --gid gradle --uid 1000 --shell /bin/bash --create-home gradle     && mkdir /home/gradle/.gradle     && chown --recursive gradle:gradle /home/gradle         && echo "Symlinking root Gradle cache to gradle Gradle cache"     && ln --symbolic /home/gradle/.gradle /root/.gradle
# Tue, 31 Jan 2023 21:05:20 GMT
VOLUME [/home/gradle/.gradle]
# Tue, 31 Jan 2023 21:05:20 GMT
WORKDIR /home/gradle
# Tue, 31 Jan 2023 21:05:41 GMT
RUN set -o errexit -o nounset     && apt-get update     && apt-get install --yes --no-install-recommends         unzip         wget                 bzr         git         git-lfs         mercurial         openssh-client         subversion     && rm --recursive --force /var/lib/apt/lists/*         && echo "Testing VCSes"     && which bzr     && which git     && which git-lfs     && which hg     && which svn
# Tue, 31 Jan 2023 21:09:04 GMT
ENV GRADLE_VERSION=6.9.3
# Tue, 31 Jan 2023 21:09:04 GMT
ARG GRADLE_DOWNLOAD_SHA256=dcf350b8ae1aa192fc299aed6efc77b43825d4fedb224c94118ae7faf5fb035d
# Tue, 31 Jan 2023 21:09:09 GMT
# ARGS: GRADLE_DOWNLOAD_SHA256=dcf350b8ae1aa192fc299aed6efc77b43825d4fedb224c94118ae7faf5fb035d
RUN set -o errexit -o nounset     && echo "Downloading Gradle"     && wget --no-verbose --output-document=gradle.zip "https://services.gradle.org/distributions/gradle-${GRADLE_VERSION}-bin.zip"         && echo "Checking download hash"     && echo "${GRADLE_DOWNLOAD_SHA256} *gradle.zip" | sha256sum --check -         && echo "Installing Gradle"     && unzip gradle.zip     && rm gradle.zip     && mv "gradle-${GRADLE_VERSION}" "${GRADLE_HOME}/"     && ln --symbolic "${GRADLE_HOME}/bin/gradle" /usr/bin/gradle         && echo "Testing Gradle installation"     && gradle --version
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
	-	`sha256:21cb0acfa4b704fe9047e92e2943ab0300e1adddbc3d09bd67d402f5cf6cd1c4`  
		Last Modified: Tue, 31 Jan 2023 19:06:04 GMT  
		Size: 186.0 MB (185951107 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:be6ad9b3e53e03f1b1c3e6c940266f8909001529345259c3d57457d5e68e14f1`  
		Last Modified: Tue, 31 Jan 2023 19:05:44 GMT  
		Size: 177.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6afd20b2d4acc893531c0ae30d2b501eff5075571507d1eac8f354422f862adf`  
		Last Modified: Tue, 31 Jan 2023 21:15:45 GMT  
		Size: 4.3 KB (4320 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:104b1450acf0d22708ebbcbee4025b55ab445fb84c271884bb7e999b8220a67a`  
		Last Modified: Tue, 31 Jan 2023 21:15:56 GMT  
		Size: 53.3 MB (53280692 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9e29274149a840cdc8bd047899180791b6f57e22339fc877a0a562b6f6682b32`  
		Last Modified: Tue, 31 Jan 2023 21:21:55 GMT  
		Size: 107.7 MB (107691698 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `gradle:6-jdk11-jammy` - linux; arm64 variant v8

```console
$ docker pull gradle@sha256:09bbd6ae49a0dd250164ab903558e4efbfdb9077b13a417d8f3f86b6f7ebe2b8
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **394.5 MB (394547707 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:14b888e05e527180990eed94d2451776c61c9d6b571f0ad4e098a27fe7dec420`
-	Default Command: `["gradle"]`

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
# Tue, 31 Jan 2023 17:45:33 GMT
ENV JAVA_VERSION=jdk-11.0.18+10
# Tue, 31 Jan 2023 17:45:40 GMT
RUN set -eux;     ARCH="$(dpkg --print-architecture)";     case "${ARCH}" in        aarch64|arm64)          ESUM='04d5eeff6a6449bcdca0f52cd97bafd43ce09d40ef1e73fa0e1add63bea4a9c8';          BINARY_URL='https://github.com/adoptium/temurin11-binaries/releases/download/jdk-11.0.18%2B10/OpenJDK11U-jdk_aarch64_linux_hotspot_11.0.18_10.tar.gz';          ;;        armhf|arm)          ESUM='b42840ef88621f87a4b49ae3a8db23dbf07cd9e7fb62823318709a592f597ea3';          BINARY_URL='https://github.com/adoptium/temurin11-binaries/releases/download/jdk-11.0.18%2B10/OpenJDK11U-jdk_arm_linux_hotspot_11.0.18_10.tar.gz';          ;;        ppc64el|powerpc:common64)          ESUM='459148d489b08ceec2d901e950ac36722b4c55e907e979291ddfc954ebdcea47';          BINARY_URL='https://github.com/adoptium/temurin11-binaries/releases/download/jdk-11.0.18%2B10/OpenJDK11U-jdk_ppc64le_linux_hotspot_11.0.18_10.tar.gz';          ;;        s390x|s390:64-bit)          ESUM='7a7193c8279dd889c0a39296bcbae8866d94cff7a6d1bdfe676ffe4ced018915';          BINARY_URL='https://github.com/adoptium/temurin11-binaries/releases/download/jdk-11.0.18%2B10/OpenJDK11U-jdk_s390x_linux_hotspot_11.0.18_10.tar.gz';          ;;        amd64|i386:x86-64)          ESUM='4a29efda1d702b8ff38e554cf932051f40ec70006caed5c4857a8cbc7a0b7db7';          BINARY_URL='https://github.com/adoptium/temurin11-binaries/releases/download/jdk-11.0.18%2B10/OpenJDK11U-jdk_x64_linux_hotspot_11.0.18_10.tar.gz';          ;;        *)          echo "Unsupported arch: ${ARCH}";          exit 1;          ;;     esac; 	  wget -O /tmp/openjdk.tar.gz ${BINARY_URL}; 	  echo "${ESUM} */tmp/openjdk.tar.gz" | sha256sum -c -; 	  mkdir -p "$JAVA_HOME"; 	  tar --extract 	      --file /tmp/openjdk.tar.gz 	      --directory "$JAVA_HOME" 	      --strip-components 1 	      --no-same-owner 	  ;     rm -f /tmp/openjdk.tar.gz ${JAVA_HOME}/src.zip;     find "$JAVA_HOME/lib" -name '*.so' -exec dirname '{}' ';' | sort -u > /etc/ld.so.conf.d/docker-openjdk.conf;     ldconfig;     java -Xshare:dump;
# Tue, 31 Jan 2023 17:45:43 GMT
RUN echo Verifying install ...     && fileEncoding="$(echo 'System.out.println(System.getProperty("file.encoding"))' | jshell -s -)"; [ "$fileEncoding" = 'UTF-8' ]; rm -rf ~/.java     && echo javac --version && javac --version     && echo java --version && java --version     && echo Complete.
# Tue, 31 Jan 2023 17:45:43 GMT
CMD ["jshell"]
# Tue, 31 Jan 2023 21:26:46 GMT
CMD ["gradle"]
# Tue, 31 Jan 2023 21:26:46 GMT
ENV GRADLE_HOME=/opt/gradle
# Tue, 31 Jan 2023 21:26:46 GMT
RUN set -o errexit -o nounset     && echo "Adding gradle user and group"     && groupadd --system --gid 1000 gradle     && useradd --system --gid gradle --uid 1000 --shell /bin/bash --create-home gradle     && mkdir /home/gradle/.gradle     && chown --recursive gradle:gradle /home/gradle         && echo "Symlinking root Gradle cache to gradle Gradle cache"     && ln --symbolic /home/gradle/.gradle /root/.gradle
# Tue, 31 Jan 2023 21:26:46 GMT
VOLUME [/home/gradle/.gradle]
# Tue, 31 Jan 2023 21:26:46 GMT
WORKDIR /home/gradle
# Tue, 31 Jan 2023 21:26:58 GMT
RUN set -o errexit -o nounset     && apt-get update     && apt-get install --yes --no-install-recommends         unzip         wget                 bzr         git         git-lfs         mercurial         openssh-client         subversion     && rm --recursive --force /var/lib/apt/lists/*         && echo "Testing VCSes"     && which bzr     && which git     && which git-lfs     && which hg     && which svn
# Tue, 31 Jan 2023 21:29:23 GMT
ENV GRADLE_VERSION=6.9.3
# Tue, 31 Jan 2023 21:29:23 GMT
ARG GRADLE_DOWNLOAD_SHA256=dcf350b8ae1aa192fc299aed6efc77b43825d4fedb224c94118ae7faf5fb035d
# Tue, 31 Jan 2023 21:29:27 GMT
# ARGS: GRADLE_DOWNLOAD_SHA256=dcf350b8ae1aa192fc299aed6efc77b43825d4fedb224c94118ae7faf5fb035d
RUN set -o errexit -o nounset     && echo "Downloading Gradle"     && wget --no-verbose --output-document=gradle.zip "https://services.gradle.org/distributions/gradle-${GRADLE_VERSION}-bin.zip"         && echo "Checking download hash"     && echo "${GRADLE_DOWNLOAD_SHA256} *gradle.zip" | sha256sum --check -         && echo "Installing Gradle"     && unzip gradle.zip     && rm gradle.zip     && mv "gradle-${GRADLE_VERSION}" "${GRADLE_HOME}/"     && ln --symbolic "${GRADLE_HOME}/bin/gradle" /usr/bin/gradle         && echo "Testing Gradle installation"     && gradle --version
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
	-	`sha256:c8d8e0eedc83be474a9b2366f9c420c90e3f49c24003604b9fe63731bd03e0c8`  
		Last Modified: Tue, 31 Jan 2023 17:51:44 GMT  
		Size: 195.2 MB (195247627 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:80ce25351c32ab8a48e1e8cbfc834e00b148f1bb608f6f6c74432998feaaff91`  
		Last Modified: Tue, 31 Jan 2023 17:51:33 GMT  
		Size: 175.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8a6c98a617b67a3cb7a4d5d76aab84970634eef38381c0e15deb4804f57d7b4d`  
		Last Modified: Tue, 31 Jan 2023 21:32:29 GMT  
		Size: 4.4 KB (4370 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ef2e423a0ac54b33e858248d703f1f6480e1a3f0acf6ef0f4a47caac4ababcb7`  
		Last Modified: Tue, 31 Jan 2023 21:32:36 GMT  
		Size: 50.8 MB (50827598 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3ce7eea79fdcad019a417f394842b1d182cc4bce9b416551117a777052c90fee`  
		Last Modified: Tue, 31 Jan 2023 21:36:40 GMT  
		Size: 107.7 MB (107691699 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `gradle:6-jdk11-jammy` - linux; ppc64le

```console
$ docker pull gradle@sha256:b45797b40b5104166f174d2921423ff898e0146cdaf79644a20d020319c8d91f
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **392.6 MB (392597408 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:3bae38a284b2e4e1a763d01705a9aee972f1ba9c40164338546c9e4924360fff`
-	Default Command: `["gradle"]`

```dockerfile
# Fri, 09 Dec 2022 01:27:53 GMT
ADD file:1a2557b357a1dca8521ee846ec16c9b2bd8a53839b9d4fda21a28f9ceeecb4b7 in / 
# Fri, 09 Dec 2022 01:27:55 GMT
CMD ["bash"]
# Fri, 09 Dec 2022 02:39:34 GMT
ENV JAVA_HOME=/opt/java/openjdk
# Fri, 09 Dec 2022 02:39:34 GMT
ENV PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Fri, 09 Dec 2022 02:39:34 GMT
ENV LANG=en_US.UTF-8 LANGUAGE=en_US:en LC_ALL=en_US.UTF-8
# Fri, 09 Dec 2022 02:40:14 GMT
RUN apt-get update     && DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends tzdata curl wget ca-certificates fontconfig locales     && echo "en_US.UTF-8 UTF-8" >> /etc/locale.gen     && locale-gen en_US.UTF-8     && rm -rf /var/lib/apt/lists/*
# Tue, 24 Jan 2023 18:18:07 GMT
ENV JAVA_VERSION=jdk-11.0.18+10
# Tue, 24 Jan 2023 18:18:25 GMT
RUN set -eux;     ARCH="$(dpkg --print-architecture)";     case "${ARCH}" in        aarch64|arm64)          ESUM='04d5eeff6a6449bcdca0f52cd97bafd43ce09d40ef1e73fa0e1add63bea4a9c8';          BINARY_URL='https://github.com/adoptium/temurin11-binaries/releases/download/jdk-11.0.18%2B10/OpenJDK11U-jdk_aarch64_linux_hotspot_11.0.18_10.tar.gz';          ;;        armhf|arm)          ESUM='b42840ef88621f87a4b49ae3a8db23dbf07cd9e7fb62823318709a592f597ea3';          BINARY_URL='https://github.com/adoptium/temurin11-binaries/releases/download/jdk-11.0.18%2B10/OpenJDK11U-jdk_arm_linux_hotspot_11.0.18_10.tar.gz';          ;;        ppc64el|powerpc:common64)          ESUM='459148d489b08ceec2d901e950ac36722b4c55e907e979291ddfc954ebdcea47';          BINARY_URL='https://github.com/adoptium/temurin11-binaries/releases/download/jdk-11.0.18%2B10/OpenJDK11U-jdk_ppc64le_linux_hotspot_11.0.18_10.tar.gz';          ;;        s390x|s390:64-bit)          ESUM='7a7193c8279dd889c0a39296bcbae8866d94cff7a6d1bdfe676ffe4ced018915';          BINARY_URL='https://github.com/adoptium/temurin11-binaries/releases/download/jdk-11.0.18%2B10/OpenJDK11U-jdk_s390x_linux_hotspot_11.0.18_10.tar.gz';          ;;        amd64|i386:x86-64)          ESUM='4a29efda1d702b8ff38e554cf932051f40ec70006caed5c4857a8cbc7a0b7db7';          BINARY_URL='https://github.com/adoptium/temurin11-binaries/releases/download/jdk-11.0.18%2B10/OpenJDK11U-jdk_x64_linux_hotspot_11.0.18_10.tar.gz';          ;;        *)          echo "Unsupported arch: ${ARCH}";          exit 1;          ;;     esac; 	  wget -O /tmp/openjdk.tar.gz ${BINARY_URL}; 	  echo "${ESUM} */tmp/openjdk.tar.gz" | sha256sum -c -; 	  mkdir -p "$JAVA_HOME"; 	  tar --extract 	      --file /tmp/openjdk.tar.gz 	      --directory "$JAVA_HOME" 	      --strip-components 1 	      --no-same-owner 	  ;     rm -f /tmp/openjdk.tar.gz ${JAVA_HOME}/src.zip;     find "$JAVA_HOME/lib" -name '*.so' -exec dirname '{}' ';' | sort -u > /etc/ld.so.conf.d/docker-openjdk.conf;     ldconfig;     java -Xshare:dump;
# Tue, 24 Jan 2023 18:18:32 GMT
RUN echo Verifying install ...     && fileEncoding="$(echo 'System.out.println(System.getProperty("file.encoding"))' | jshell -s -)"; [ "$fileEncoding" = 'UTF-8' ]; rm -rf ~/.java     && echo javac --version && javac --version     && echo java --version && java --version     && echo Complete.
# Tue, 24 Jan 2023 18:18:32 GMT
CMD ["jshell"]
# Tue, 24 Jan 2023 21:33:38 GMT
CMD ["gradle"]
# Tue, 24 Jan 2023 21:33:39 GMT
ENV GRADLE_HOME=/opt/gradle
# Tue, 24 Jan 2023 21:33:40 GMT
RUN set -o errexit -o nounset     && echo "Adding gradle user and group"     && groupadd --system --gid 1000 gradle     && useradd --system --gid gradle --uid 1000 --shell /bin/bash --create-home gradle     && mkdir /home/gradle/.gradle     && chown --recursive gradle:gradle /home/gradle         && echo "Symlinking root Gradle cache to gradle Gradle cache"     && ln --symbolic /home/gradle/.gradle /root/.gradle
# Tue, 24 Jan 2023 21:33:40 GMT
VOLUME [/home/gradle/.gradle]
# Tue, 24 Jan 2023 21:33:41 GMT
WORKDIR /home/gradle
# Tue, 24 Jan 2023 21:34:47 GMT
RUN set -o errexit -o nounset     && apt-get update     && apt-get install --yes --no-install-recommends         unzip         wget                 bzr         git         git-lfs         mercurial         openssh-client         subversion     && rm --recursive --force /var/lib/apt/lists/*         && echo "Testing VCSes"     && which bzr     && which git     && which git-lfs     && which hg     && which svn
# Tue, 24 Jan 2023 21:39:27 GMT
ENV GRADLE_VERSION=6.9.3
# Tue, 24 Jan 2023 21:39:27 GMT
ARG GRADLE_DOWNLOAD_SHA256=dcf350b8ae1aa192fc299aed6efc77b43825d4fedb224c94118ae7faf5fb035d
# Tue, 24 Jan 2023 21:39:35 GMT
# ARGS: GRADLE_DOWNLOAD_SHA256=dcf350b8ae1aa192fc299aed6efc77b43825d4fedb224c94118ae7faf5fb035d
RUN set -o errexit -o nounset     && echo "Downloading Gradle"     && wget --no-verbose --output-document=gradle.zip "https://services.gradle.org/distributions/gradle-${GRADLE_VERSION}-bin.zip"         && echo "Checking download hash"     && echo "${GRADLE_DOWNLOAD_SHA256} *gradle.zip" | sha256sum --check -         && echo "Installing Gradle"     && unzip gradle.zip     && rm gradle.zip     && mv "gradle-${GRADLE_VERSION}" "${GRADLE_HOME}/"     && ln --symbolic "${GRADLE_HOME}/bin/gradle" /usr/bin/gradle         && echo "Testing Gradle installation"     && gradle --version
```

-	Layers:
	-	`sha256:ce75b47e476cd75b30dca46558ac79b39923aa94d7e4b0cc025e521404cdbab0`  
		Last Modified: Fri, 09 Dec 2022 01:30:32 GMT  
		Size: 35.7 MB (35708154 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a782dc6ae3d6a01674486598e1b3cdcfaa9696ad3e2125e712884667b1c2c37f`  
		Last Modified: Fri, 09 Dec 2022 02:53:02 GMT  
		Size: 13.2 MB (13245456 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:36efd19e6823a0528cad3f7285558f8f23f05aedddb6ccb00ce42e7443f33908`  
		Last Modified: Tue, 24 Jan 2023 18:28:55 GMT  
		Size: 180.5 MB (180464494 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0dd5ee379e41cb468c200b32969ed0642b16112384d4b5c1eb69a105af341536`  
		Last Modified: Tue, 24 Jan 2023 18:28:32 GMT  
		Size: 175.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:914c9eab063d480f312cafe92a16dcdcefde888491a91cb287f27a039269cc0f`  
		Last Modified: Tue, 24 Jan 2023 21:44:26 GMT  
		Size: 4.4 KB (4371 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:38c303b3aa63c299f8b1f3577e87903b9d04018c2098539eb2689f62f0fa0dff`  
		Last Modified: Tue, 24 Jan 2023 21:44:42 GMT  
		Size: 55.5 MB (55483065 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c799eb4f18f68de628571a96e03f4412249d1d361e052d2b2e6eacd40dd0366a`  
		Last Modified: Tue, 24 Jan 2023 21:48:55 GMT  
		Size: 107.7 MB (107691693 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `gradle:6-jdk11-jammy` - linux; s390x

```console
$ docker pull gradle@sha256:355501af9ba54afe8593b82501a81c129c1ca135b775926d062fe22be170f222
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **371.7 MB (371724081 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b774ece5e29081bbb3cd8ab7c29e076af56ebd71503d9457c1ad16f1dc2ce8ab`
-	Default Command: `["gradle"]`

```dockerfile
# Thu, 26 Jan 2023 05:08:35 GMT
ARG RELEASE
# Thu, 26 Jan 2023 05:08:35 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Thu, 26 Jan 2023 05:08:36 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Thu, 26 Jan 2023 05:08:36 GMT
LABEL org.opencontainers.image.version=22.04
# Thu, 26 Jan 2023 05:08:37 GMT
ADD file:a9794efc1a102ab6a7160e660a63f4b267797b8b7e0b0bfd9c04ed62846cfb36 in / 
# Thu, 26 Jan 2023 05:08:38 GMT
CMD ["/bin/bash"]
# Tue, 31 Jan 2023 17:59:04 GMT
ENV JAVA_HOME=/opt/java/openjdk
# Tue, 31 Jan 2023 17:59:04 GMT
ENV PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 31 Jan 2023 17:59:04 GMT
ENV LANG=en_US.UTF-8 LANGUAGE=en_US:en LC_ALL=en_US.UTF-8
# Tue, 31 Jan 2023 17:59:14 GMT
RUN apt-get update     && DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends tzdata curl wget ca-certificates fontconfig locales     && echo "en_US.UTF-8 UTF-8" >> /etc/locale.gen     && locale-gen en_US.UTF-8     && rm -rf /var/lib/apt/lists/*
# Tue, 31 Jan 2023 17:59:15 GMT
ENV JAVA_VERSION=jdk-11.0.18+10
# Tue, 31 Jan 2023 17:59:22 GMT
RUN set -eux;     ARCH="$(dpkg --print-architecture)";     case "${ARCH}" in        aarch64|arm64)          ESUM='04d5eeff6a6449bcdca0f52cd97bafd43ce09d40ef1e73fa0e1add63bea4a9c8';          BINARY_URL='https://github.com/adoptium/temurin11-binaries/releases/download/jdk-11.0.18%2B10/OpenJDK11U-jdk_aarch64_linux_hotspot_11.0.18_10.tar.gz';          ;;        armhf|arm)          ESUM='b42840ef88621f87a4b49ae3a8db23dbf07cd9e7fb62823318709a592f597ea3';          BINARY_URL='https://github.com/adoptium/temurin11-binaries/releases/download/jdk-11.0.18%2B10/OpenJDK11U-jdk_arm_linux_hotspot_11.0.18_10.tar.gz';          ;;        ppc64el|powerpc:common64)          ESUM='459148d489b08ceec2d901e950ac36722b4c55e907e979291ddfc954ebdcea47';          BINARY_URL='https://github.com/adoptium/temurin11-binaries/releases/download/jdk-11.0.18%2B10/OpenJDK11U-jdk_ppc64le_linux_hotspot_11.0.18_10.tar.gz';          ;;        s390x|s390:64-bit)          ESUM='7a7193c8279dd889c0a39296bcbae8866d94cff7a6d1bdfe676ffe4ced018915';          BINARY_URL='https://github.com/adoptium/temurin11-binaries/releases/download/jdk-11.0.18%2B10/OpenJDK11U-jdk_s390x_linux_hotspot_11.0.18_10.tar.gz';          ;;        amd64|i386:x86-64)          ESUM='4a29efda1d702b8ff38e554cf932051f40ec70006caed5c4857a8cbc7a0b7db7';          BINARY_URL='https://github.com/adoptium/temurin11-binaries/releases/download/jdk-11.0.18%2B10/OpenJDK11U-jdk_x64_linux_hotspot_11.0.18_10.tar.gz';          ;;        *)          echo "Unsupported arch: ${ARCH}";          exit 1;          ;;     esac; 	  wget -O /tmp/openjdk.tar.gz ${BINARY_URL}; 	  echo "${ESUM} */tmp/openjdk.tar.gz" | sha256sum -c -; 	  mkdir -p "$JAVA_HOME"; 	  tar --extract 	      --file /tmp/openjdk.tar.gz 	      --directory "$JAVA_HOME" 	      --strip-components 1 	      --no-same-owner 	  ;     rm -f /tmp/openjdk.tar.gz ${JAVA_HOME}/src.zip;     find "$JAVA_HOME/lib" -name '*.so' -exec dirname '{}' ';' | sort -u > /etc/ld.so.conf.d/docker-openjdk.conf;     ldconfig;     java -Xshare:dump;
# Tue, 31 Jan 2023 17:59:27 GMT
RUN echo Verifying install ...     && fileEncoding="$(echo 'System.out.println(System.getProperty("file.encoding"))' | jshell -s -)"; [ "$fileEncoding" = 'UTF-8' ]; rm -rf ~/.java     && echo javac --version && javac --version     && echo java --version && java --version     && echo Complete.
# Tue, 31 Jan 2023 17:59:27 GMT
CMD ["jshell"]
# Tue, 31 Jan 2023 19:24:34 GMT
CMD ["gradle"]
# Tue, 31 Jan 2023 19:24:35 GMT
ENV GRADLE_HOME=/opt/gradle
# Tue, 31 Jan 2023 19:24:35 GMT
RUN set -o errexit -o nounset     && echo "Adding gradle user and group"     && groupadd --system --gid 1000 gradle     && useradd --system --gid gradle --uid 1000 --shell /bin/bash --create-home gradle     && mkdir /home/gradle/.gradle     && chown --recursive gradle:gradle /home/gradle         && echo "Symlinking root Gradle cache to gradle Gradle cache"     && ln --symbolic /home/gradle/.gradle /root/.gradle
# Tue, 31 Jan 2023 19:24:35 GMT
VOLUME [/home/gradle/.gradle]
# Tue, 31 Jan 2023 19:24:35 GMT
WORKDIR /home/gradle
# Tue, 31 Jan 2023 19:24:55 GMT
RUN set -o errexit -o nounset     && apt-get update     && apt-get install --yes --no-install-recommends         unzip         wget                 bzr         git         git-lfs         mercurial         openssh-client         subversion     && rm --recursive --force /var/lib/apt/lists/*         && echo "Testing VCSes"     && which bzr     && which git     && which git-lfs     && which hg     && which svn
# Tue, 31 Jan 2023 19:28:08 GMT
ENV GRADLE_VERSION=6.9.3
# Tue, 31 Jan 2023 19:28:08 GMT
ARG GRADLE_DOWNLOAD_SHA256=dcf350b8ae1aa192fc299aed6efc77b43825d4fedb224c94118ae7faf5fb035d
# Tue, 31 Jan 2023 19:28:13 GMT
# ARGS: GRADLE_DOWNLOAD_SHA256=dcf350b8ae1aa192fc299aed6efc77b43825d4fedb224c94118ae7faf5fb035d
RUN set -o errexit -o nounset     && echo "Downloading Gradle"     && wget --no-verbose --output-document=gradle.zip "https://services.gradle.org/distributions/gradle-${GRADLE_VERSION}-bin.zip"         && echo "Checking download hash"     && echo "${GRADLE_DOWNLOAD_SHA256} *gradle.zip" | sha256sum --check -         && echo "Installing Gradle"     && unzip gradle.zip     && rm gradle.zip     && mv "gradle-${GRADLE_VERSION}" "${GRADLE_HOME}/"     && ln --symbolic "${GRADLE_HOME}/bin/gradle" /usr/bin/gradle         && echo "Testing Gradle installation"     && gradle --version
```

-	Layers:
	-	`sha256:dd969ed9de43018fe5442c859bf66eabf23145b966b9338392ea707aed18b26f`  
		Last Modified: Tue, 31 Jan 2023 17:55:34 GMT  
		Size: 28.6 MB (28641926 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:27e61b13b86195413895b2e2ae4499c0123469558bfd3409aeb3edaada381f0a`  
		Last Modified: Tue, 31 Jan 2023 18:05:26 GMT  
		Size: 12.5 MB (12479720 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0476560734c188e788b69787e35cdc0c1c4ecf5837b56e1d7e9df5974a406f50`  
		Last Modified: Tue, 31 Jan 2023 18:05:38 GMT  
		Size: 172.0 MB (171957418 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4417033c38235111aa45b7a81672b0998bb90210e139818b2e645da894af1a25`  
		Last Modified: Tue, 31 Jan 2023 18:05:25 GMT  
		Size: 173.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:19ac3bbe3bd1fc64fbadb1e63f6280fb3b199b1507250758454764f538c684ca`  
		Last Modified: Tue, 31 Jan 2023 19:31:57 GMT  
		Size: 4.4 KB (4365 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6f7775f55dd2449f2e95e1b1a9b705023d81e611043400545cc8058f5eb30f21`  
		Last Modified: Tue, 31 Jan 2023 19:32:05 GMT  
		Size: 50.9 MB (50948784 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:40c497283f59d9ceae6575f4b824d62895c8da5821a82cf60f86b2a07091c782`  
		Last Modified: Tue, 31 Jan 2023 19:35:13 GMT  
		Size: 107.7 MB (107691695 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
