## `gradle:jdk11`

```console
$ docker pull gradle@sha256:c4550288e6c3e9723b0d086e25e1efd04c8c8728b09eaf668803442a99f7992b
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 5
	-	linux; amd64
	-	linux; arm variant v7
	-	linux; arm64 variant v8
	-	linux; ppc64le
	-	linux; s390x

### `gradle:jdk11` - linux; amd64

```console
$ docker pull gradle@sha256:5c84c8e8f088135c68c660fe54d4623608a13de8c20d5304dc6e7a3b677103d7
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **420.1 MB (420068230 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:1c946b286bfef3162950afebefa0158424c27117bc90b0ce844322a6cdf7ac5a`
-	Default Command: `["gradle"]`

```dockerfile
# Wed, 02 Feb 2022 02:14:45 GMT
ADD file:3ccf747d646089ed7fbb43c40c45dd43e86f0674115f856efada93c7e4a63624 in / 
# Wed, 02 Feb 2022 02:14:46 GMT
CMD ["bash"]
# Wed, 02 Feb 2022 02:57:26 GMT
ENV LANG=en_US.UTF-8 LANGUAGE=en_US:en LC_ALL=en_US.UTF-8
# Wed, 02 Feb 2022 02:58:19 GMT
RUN apt-get update     && DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends tzdata curl ca-certificates fontconfig locales python-is-python3     && echo "en_US.UTF-8 UTF-8" >> /etc/locale.gen     && locale-gen en_US.UTF-8     && rm -rf /var/lib/apt/lists/*
# Thu, 10 Feb 2022 20:19:53 GMT
ENV JAVA_VERSION=jdk-11.0.14.1+1
# Thu, 10 Feb 2022 20:20:02 GMT
RUN set -eux;     ARCH="$(dpkg --print-architecture)";     case "${ARCH}" in        aarch64|arm64)          ESUM='79572f5172c6a040591d34632f98a20ed148702bbce2f57649e8ac01c0d2e3db';          BINARY_URL='https://github.com/adoptium/temurin11-binaries/releases/download/jdk-11.0.14.1%2B1/OpenJDK11U-jdk_aarch64_linux_hotspot_11.0.14.1_1.tar.gz';          ;;        armhf|arm)          ESUM='f4d53a1753cdde830d7872c6a1279df441f3f9aeb5d5037a568b3a392ebce9c2';          BINARY_URL='https://github.com/adoptium/temurin11-binaries/releases/download/jdk-11.0.14.1%2B1/OpenJDK11U-jdk_arm_linux_hotspot_11.0.14.1_1.tar.gz';          ;;        ppc64el|powerpc:common64)          ESUM='9750e11721282a9afd18a07743f19c699b2b71ce20d02f3f0a906088b9ae6d9a';          BINARY_URL='https://github.com/adoptium/temurin11-binaries/releases/download/jdk-11.0.14.1%2B1/OpenJDK11U-jdk_ppc64le_linux_hotspot_11.0.14.1_1.tar.gz';          ;;        s390x|s390:64-bit)          ESUM='79a27a4dc23dff38a5c21e5ba9b7efcf0aa5e14ace1a3b19bec53e255c487521';          BINARY_URL='https://github.com/adoptium/temurin11-binaries/releases/download/jdk-11.0.14.1%2B1/OpenJDK11U-jdk_s390x_linux_hotspot_11.0.14.1_1.tar.gz';          ;;        amd64|i386:x86-64)          ESUM='43fb84f8063ad9bf6b6d694a67b8f64c8827552b920ec5ce794dfe5602edffe7';          BINARY_URL='https://github.com/adoptium/temurin11-binaries/releases/download/jdk-11.0.14.1%2B1/OpenJDK11U-jdk_x64_linux_hotspot_11.0.14.1_1.tar.gz';          ;;        *)          echo "Unsupported arch: ${ARCH}";          exit 1;          ;;     esac;     curl -LfsSo /tmp/openjdk.tar.gz ${BINARY_URL};     echo "${ESUM} */tmp/openjdk.tar.gz" | sha256sum -c -;     mkdir -p /opt/java/openjdk;     cd /opt/java/openjdk;     tar -xf /tmp/openjdk.tar.gz --strip-components=1;     rm -rf /tmp/openjdk.tar.gz;
# Thu, 10 Feb 2022 20:20:03 GMT
ENV JAVA_HOME=/opt/java/openjdk PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 10 Feb 2022 20:20:04 GMT
RUN echo Verifying install ...     && echo javac --version && javac --version     && echo java --version && java --version     && echo Complete.
# Thu, 10 Feb 2022 20:20:04 GMT
CMD ["jshell"]
# Thu, 10 Feb 2022 21:00:37 GMT
CMD ["gradle"]
# Thu, 10 Feb 2022 21:00:37 GMT
ENV GRADLE_HOME=/opt/gradle
# Thu, 10 Feb 2022 21:00:38 GMT
RUN set -o errexit -o nounset     && echo "Adding gradle user and group"     && groupadd --system --gid 1000 gradle     && useradd --system --gid gradle --uid 1000 --shell /bin/bash --create-home gradle     && mkdir /home/gradle/.gradle     && chown --recursive gradle:gradle /home/gradle         && echo "Symlinking root Gradle cache to gradle Gradle cache"     && ln --symbolic /home/gradle/.gradle /root/.gradle
# Thu, 10 Feb 2022 21:00:39 GMT
VOLUME [/home/gradle/.gradle]
# Thu, 10 Feb 2022 21:00:39 GMT
WORKDIR /home/gradle
# Thu, 10 Feb 2022 21:00:55 GMT
RUN set -o errexit -o nounset     && apt-get update     && apt-get install --yes --no-install-recommends         unzip         wget                 bzr         git         git-lfs         mercurial         openssh-client         subversion     && rm --recursive --force /var/lib/apt/lists/*         && echo "Testing VCSes"     && which bzr     && which git     && which git-lfs     && which hg     && which svn
# Fri, 11 Feb 2022 01:19:42 GMT
ENV GRADLE_VERSION=7.4
# Fri, 11 Feb 2022 01:19:42 GMT
ARG GRADLE_DOWNLOAD_SHA256=8cc27038d5dbd815759851ba53e70cf62e481b87494cc97cfd97982ada5ba634
# Fri, 11 Feb 2022 01:19:47 GMT
# ARGS: GRADLE_DOWNLOAD_SHA256=8cc27038d5dbd815759851ba53e70cf62e481b87494cc97cfd97982ada5ba634
RUN set -o errexit -o nounset     && echo "Downloading Gradle"     && wget --no-verbose --output-document=gradle.zip "https://services.gradle.org/distributions/gradle-${GRADLE_VERSION}-bin.zip"         && echo "Checking download hash"     && echo "${GRADLE_DOWNLOAD_SHA256} *gradle.zip" | sha256sum --check -         && echo "Installing Gradle"     && unzip gradle.zip     && rm gradle.zip     && mv "gradle-${GRADLE_VERSION}" "${GRADLE_HOME}/"     && ln --symbolic "${GRADLE_HOME}/bin/gradle" /usr/bin/gradle         && echo "Testing Gradle installation"     && gradle --version
```

-	Layers:
	-	`sha256:08c01a0ec47e82ebe2bec112f373d160983a6d1e9e66627f66a3322bc403221b`  
		Last Modified: Wed, 02 Feb 2022 02:16:20 GMT  
		Size: 28.6 MB (28564099 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cd22f8f9007b7341ddccd906a9f476337b871592380b8c0c2cc5f7c8e4b16928`  
		Last Modified: Wed, 02 Feb 2022 03:02:00 GMT  
		Size: 24.8 MB (24814660 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:962258e67b65f2a3b28ee0b30a39ffa3d06862bb2df87d488dd1a464182c5888`  
		Last Modified: Thu, 10 Feb 2022 20:23:06 GMT  
		Size: 193.9 MB (193949693 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e1c05ef18c521e9bf4032d689231b8d6bf152444efbdb9f082e5a99c4de38b28`  
		Last Modified: Thu, 10 Feb 2022 20:22:53 GMT  
		Size: 160.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7d8ef99f43613a495124d2990330ca46000c01d4859b94da0ecb666dc1da5670`  
		Last Modified: Thu, 10 Feb 2022 21:03:02 GMT  
		Size: 4.4 KB (4358 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:22009ad048742315cca30a35ec6a09f30220162f49bc3ddc869e0cacf474929f`  
		Last Modified: Thu, 10 Feb 2022 21:03:13 GMT  
		Size: 56.9 MB (56870497 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:35fc79ca510d8aa807c02319a90b27d4de63b4ad7bebdef0fbdc566c3f36d84f`  
		Last Modified: Fri, 11 Feb 2022 01:21:52 GMT  
		Size: 115.9 MB (115864763 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `gradle:jdk11` - linux; arm variant v7

```console
$ docker pull gradle@sha256:cc2fdebae0e005135f560420a1b6edb7cff0df94d57861a9f33f7e330ccab3d0
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **396.7 MB (396729664 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:1dad6762ebb92676c2ccf37fa8af684d903667e7f0f348f9932502b2e9951779`
-	Default Command: `["gradle"]`

```dockerfile
# Wed, 02 Feb 2022 02:25:11 GMT
ADD file:0adc3f597b5ba8c31a9a4d67126166cf067749754e269fe2c3ed43f03457b53c in / 
# Wed, 02 Feb 2022 02:25:12 GMT
CMD ["bash"]
# Wed, 02 Feb 2022 02:47:09 GMT
ENV LANG=en_US.UTF-8 LANGUAGE=en_US:en LC_ALL=en_US.UTF-8
# Wed, 02 Feb 2022 02:48:03 GMT
RUN apt-get update     && DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends tzdata curl ca-certificates fontconfig locales python-is-python3     && echo "en_US.UTF-8 UTF-8" >> /etc/locale.gen     && locale-gen en_US.UTF-8     && rm -rf /var/lib/apt/lists/*
# Thu, 10 Feb 2022 19:59:07 GMT
ENV JAVA_VERSION=jdk-11.0.14.1+1
# Thu, 10 Feb 2022 19:59:33 GMT
RUN set -eux;     ARCH="$(dpkg --print-architecture)";     case "${ARCH}" in        aarch64|arm64)          ESUM='79572f5172c6a040591d34632f98a20ed148702bbce2f57649e8ac01c0d2e3db';          BINARY_URL='https://github.com/adoptium/temurin11-binaries/releases/download/jdk-11.0.14.1%2B1/OpenJDK11U-jdk_aarch64_linux_hotspot_11.0.14.1_1.tar.gz';          ;;        armhf|arm)          ESUM='f4d53a1753cdde830d7872c6a1279df441f3f9aeb5d5037a568b3a392ebce9c2';          BINARY_URL='https://github.com/adoptium/temurin11-binaries/releases/download/jdk-11.0.14.1%2B1/OpenJDK11U-jdk_arm_linux_hotspot_11.0.14.1_1.tar.gz';          ;;        ppc64el|powerpc:common64)          ESUM='9750e11721282a9afd18a07743f19c699b2b71ce20d02f3f0a906088b9ae6d9a';          BINARY_URL='https://github.com/adoptium/temurin11-binaries/releases/download/jdk-11.0.14.1%2B1/OpenJDK11U-jdk_ppc64le_linux_hotspot_11.0.14.1_1.tar.gz';          ;;        s390x|s390:64-bit)          ESUM='79a27a4dc23dff38a5c21e5ba9b7efcf0aa5e14ace1a3b19bec53e255c487521';          BINARY_URL='https://github.com/adoptium/temurin11-binaries/releases/download/jdk-11.0.14.1%2B1/OpenJDK11U-jdk_s390x_linux_hotspot_11.0.14.1_1.tar.gz';          ;;        amd64|i386:x86-64)          ESUM='43fb84f8063ad9bf6b6d694a67b8f64c8827552b920ec5ce794dfe5602edffe7';          BINARY_URL='https://github.com/adoptium/temurin11-binaries/releases/download/jdk-11.0.14.1%2B1/OpenJDK11U-jdk_x64_linux_hotspot_11.0.14.1_1.tar.gz';          ;;        *)          echo "Unsupported arch: ${ARCH}";          exit 1;          ;;     esac;     curl -LfsSo /tmp/openjdk.tar.gz ${BINARY_URL};     echo "${ESUM} */tmp/openjdk.tar.gz" | sha256sum -c -;     mkdir -p /opt/java/openjdk;     cd /opt/java/openjdk;     tar -xf /tmp/openjdk.tar.gz --strip-components=1;     rm -rf /tmp/openjdk.tar.gz;
# Thu, 10 Feb 2022 19:59:35 GMT
ENV JAVA_HOME=/opt/java/openjdk PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 10 Feb 2022 19:59:37 GMT
RUN echo Verifying install ...     && echo javac --version && javac --version     && echo java --version && java --version     && echo Complete.
# Thu, 10 Feb 2022 19:59:38 GMT
CMD ["jshell"]
# Thu, 10 Feb 2022 20:24:11 GMT
CMD ["gradle"]
# Thu, 10 Feb 2022 20:24:11 GMT
ENV GRADLE_HOME=/opt/gradle
# Thu, 10 Feb 2022 20:24:13 GMT
RUN set -o errexit -o nounset     && echo "Adding gradle user and group"     && groupadd --system --gid 1000 gradle     && useradd --system --gid gradle --uid 1000 --shell /bin/bash --create-home gradle     && mkdir /home/gradle/.gradle     && chown --recursive gradle:gradle /home/gradle         && echo "Symlinking root Gradle cache to gradle Gradle cache"     && ln --symbolic /home/gradle/.gradle /root/.gradle
# Thu, 10 Feb 2022 20:24:13 GMT
VOLUME [/home/gradle/.gradle]
# Thu, 10 Feb 2022 20:24:14 GMT
WORKDIR /home/gradle
# Thu, 10 Feb 2022 20:25:00 GMT
RUN set -o errexit -o nounset     && apt-get update     && apt-get install --yes --no-install-recommends         unzip         wget                 bzr         git         git-lfs         mercurial         openssh-client         subversion     && rm --recursive --force /var/lib/apt/lists/*         && echo "Testing VCSes"     && which bzr     && which git     && which git-lfs     && which hg     && which svn
# Fri, 11 Feb 2022 01:59:09 GMT
ENV GRADLE_VERSION=7.4
# Fri, 11 Feb 2022 01:59:10 GMT
ARG GRADLE_DOWNLOAD_SHA256=8cc27038d5dbd815759851ba53e70cf62e481b87494cc97cfd97982ada5ba634
# Fri, 11 Feb 2022 01:59:24 GMT
# ARGS: GRADLE_DOWNLOAD_SHA256=8cc27038d5dbd815759851ba53e70cf62e481b87494cc97cfd97982ada5ba634
RUN set -o errexit -o nounset     && echo "Downloading Gradle"     && wget --no-verbose --output-document=gradle.zip "https://services.gradle.org/distributions/gradle-${GRADLE_VERSION}-bin.zip"         && echo "Checking download hash"     && echo "${GRADLE_DOWNLOAD_SHA256} *gradle.zip" | sha256sum --check -         && echo "Installing Gradle"     && unzip gradle.zip     && rm gradle.zip     && mv "gradle-${GRADLE_VERSION}" "${GRADLE_HOME}/"     && ln --symbolic "${GRADLE_HOME}/bin/gradle" /usr/bin/gradle         && echo "Testing Gradle installation"     && gradle --version
```

-	Layers:
	-	`sha256:42bcffb5d2901aadaedc35f036cf725a537494a5869ae378ec427d313ff41fa6`  
		Last Modified: Wed, 02 Feb 2022 02:29:41 GMT  
		Size: 24.1 MB (24062751 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ca45b223849013a5db7d5850e0832f4aac669b33c69f09d9d74f6d6ae56a91d8`  
		Last Modified: Wed, 02 Feb 2022 02:54:22 GMT  
		Size: 23.1 MB (23072061 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6affff1ad1f3a5476156b49961430ea27fb50b89ceee1b8ca8807407149e685d`  
		Last Modified: Thu, 10 Feb 2022 20:05:56 GMT  
		Size: 181.8 MB (181831083 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b6f6db64d8d2efe6a6a9c22bd293c56633a10caf7dcd120fd5b9a5de4bb4d5db`  
		Last Modified: Thu, 10 Feb 2022 20:04:47 GMT  
		Size: 160.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ec351c58955c21aa178ad7ecd91e656288059be216ca70ea1187f1fd49778706`  
		Last Modified: Thu, 10 Feb 2022 20:30:17 GMT  
		Size: 4.3 KB (4348 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4104dce350adb3a7237377d7a255e2953e8e7d09b6bac40260bca0e260950156`  
		Last Modified: Thu, 10 Feb 2022 20:30:53 GMT  
		Size: 51.9 MB (51894467 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8dbbfeed7ac33ca8b315a4031118f340be12cede12cfc0413fbff5d78858c4ba`  
		Last Modified: Fri, 11 Feb 2022 02:04:51 GMT  
		Size: 115.9 MB (115864794 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `gradle:jdk11` - linux; arm64 variant v8

```console
$ docker pull gradle@sha256:c170cd47984efd3468866b8569b00bd91e1b31c44dd8e1cc62b3671253c30dff
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **415.0 MB (414978175 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d3ded3a213ab9ce18e2cfd386a03843ca890d133917efc8a8a48577e1a06f5d3`
-	Default Command: `["gradle"]`

```dockerfile
# Wed, 02 Feb 2022 03:19:27 GMT
ADD file:3acc741be29b0b58e44d7302ab5ce65bf65ea1b35922be58a2cee9cb708d006a in / 
# Wed, 02 Feb 2022 03:19:27 GMT
CMD ["bash"]
# Wed, 02 Feb 2022 05:01:31 GMT
ENV LANG=en_US.UTF-8 LANGUAGE=en_US:en LC_ALL=en_US.UTF-8
# Wed, 02 Feb 2022 05:01:53 GMT
RUN apt-get update     && DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends tzdata curl ca-certificates fontconfig locales python-is-python3     && echo "en_US.UTF-8 UTF-8" >> /etc/locale.gen     && locale-gen en_US.UTF-8     && rm -rf /var/lib/apt/lists/*
# Thu, 10 Feb 2022 19:40:27 GMT
ENV JAVA_VERSION=jdk-11.0.14.1+1
# Thu, 10 Feb 2022 19:40:40 GMT
RUN set -eux;     ARCH="$(dpkg --print-architecture)";     case "${ARCH}" in        aarch64|arm64)          ESUM='79572f5172c6a040591d34632f98a20ed148702bbce2f57649e8ac01c0d2e3db';          BINARY_URL='https://github.com/adoptium/temurin11-binaries/releases/download/jdk-11.0.14.1%2B1/OpenJDK11U-jdk_aarch64_linux_hotspot_11.0.14.1_1.tar.gz';          ;;        armhf|arm)          ESUM='f4d53a1753cdde830d7872c6a1279df441f3f9aeb5d5037a568b3a392ebce9c2';          BINARY_URL='https://github.com/adoptium/temurin11-binaries/releases/download/jdk-11.0.14.1%2B1/OpenJDK11U-jdk_arm_linux_hotspot_11.0.14.1_1.tar.gz';          ;;        ppc64el|powerpc:common64)          ESUM='9750e11721282a9afd18a07743f19c699b2b71ce20d02f3f0a906088b9ae6d9a';          BINARY_URL='https://github.com/adoptium/temurin11-binaries/releases/download/jdk-11.0.14.1%2B1/OpenJDK11U-jdk_ppc64le_linux_hotspot_11.0.14.1_1.tar.gz';          ;;        s390x|s390:64-bit)          ESUM='79a27a4dc23dff38a5c21e5ba9b7efcf0aa5e14ace1a3b19bec53e255c487521';          BINARY_URL='https://github.com/adoptium/temurin11-binaries/releases/download/jdk-11.0.14.1%2B1/OpenJDK11U-jdk_s390x_linux_hotspot_11.0.14.1_1.tar.gz';          ;;        amd64|i386:x86-64)          ESUM='43fb84f8063ad9bf6b6d694a67b8f64c8827552b920ec5ce794dfe5602edffe7';          BINARY_URL='https://github.com/adoptium/temurin11-binaries/releases/download/jdk-11.0.14.1%2B1/OpenJDK11U-jdk_x64_linux_hotspot_11.0.14.1_1.tar.gz';          ;;        *)          echo "Unsupported arch: ${ARCH}";          exit 1;          ;;     esac;     curl -LfsSo /tmp/openjdk.tar.gz ${BINARY_URL};     echo "${ESUM} */tmp/openjdk.tar.gz" | sha256sum -c -;     mkdir -p /opt/java/openjdk;     cd /opt/java/openjdk;     tar -xf /tmp/openjdk.tar.gz --strip-components=1;     rm -rf /tmp/openjdk.tar.gz;
# Thu, 10 Feb 2022 19:40:40 GMT
ENV JAVA_HOME=/opt/java/openjdk PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 10 Feb 2022 19:40:42 GMT
RUN echo Verifying install ...     && echo javac --version && javac --version     && echo java --version && java --version     && echo Complete.
# Thu, 10 Feb 2022 19:40:42 GMT
CMD ["jshell"]
# Thu, 10 Feb 2022 21:21:29 GMT
CMD ["gradle"]
# Thu, 10 Feb 2022 21:21:30 GMT
ENV GRADLE_HOME=/opt/gradle
# Thu, 10 Feb 2022 21:21:31 GMT
RUN set -o errexit -o nounset     && echo "Adding gradle user and group"     && groupadd --system --gid 1000 gradle     && useradd --system --gid gradle --uid 1000 --shell /bin/bash --create-home gradle     && mkdir /home/gradle/.gradle     && chown --recursive gradle:gradle /home/gradle         && echo "Symlinking root Gradle cache to gradle Gradle cache"     && ln --symbolic /home/gradle/.gradle /root/.gradle
# Thu, 10 Feb 2022 21:21:32 GMT
VOLUME [/home/gradle/.gradle]
# Thu, 10 Feb 2022 21:21:33 GMT
WORKDIR /home/gradle
# Thu, 10 Feb 2022 21:21:54 GMT
RUN set -o errexit -o nounset     && apt-get update     && apt-get install --yes --no-install-recommends         unzip         wget                 bzr         git         git-lfs         mercurial         openssh-client         subversion     && rm --recursive --force /var/lib/apt/lists/*         && echo "Testing VCSes"     && which bzr     && which git     && which git-lfs     && which hg     && which svn
# Fri, 11 Feb 2022 01:39:59 GMT
ENV GRADLE_VERSION=7.4
# Fri, 11 Feb 2022 01:40:00 GMT
ARG GRADLE_DOWNLOAD_SHA256=8cc27038d5dbd815759851ba53e70cf62e481b87494cc97cfd97982ada5ba634
# Fri, 11 Feb 2022 01:40:07 GMT
# ARGS: GRADLE_DOWNLOAD_SHA256=8cc27038d5dbd815759851ba53e70cf62e481b87494cc97cfd97982ada5ba634
RUN set -o errexit -o nounset     && echo "Downloading Gradle"     && wget --no-verbose --output-document=gradle.zip "https://services.gradle.org/distributions/gradle-${GRADLE_VERSION}-bin.zip"         && echo "Checking download hash"     && echo "${GRADLE_DOWNLOAD_SHA256} *gradle.zip" | sha256sum --check -         && echo "Installing Gradle"     && unzip gradle.zip     && rm gradle.zip     && mv "gradle-${GRADLE_VERSION}" "${GRADLE_HOME}/"     && ln --symbolic "${GRADLE_HOME}/bin/gradle" /usr/bin/gradle         && echo "Testing Gradle installation"     && gradle --version
```

-	Layers:
	-	`sha256:bbf2fb66fa6e06dd46eb26f518f93171ee7c48be68aafb213aa7c2c12f4018ca`  
		Last Modified: Wed, 02 Feb 2022 03:21:24 GMT  
		Size: 27.2 MB (27169640 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:20305b79e1520f1abaac4873914620f971be40e552579ba5d7dae3be52dd4f68`  
		Last Modified: Wed, 02 Feb 2022 05:06:28 GMT  
		Size: 24.8 MB (24762728 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:967bd311c8921141563ced612bba0752a4b00e3cf70ffd9a7da94c923ffc159e`  
		Last Modified: Thu, 10 Feb 2022 19:44:46 GMT  
		Size: 190.7 MB (190684890 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b62c3d758ff40f96613e6b018b922bbe1a21d9bcf59c1e8088a64ef9313a422b`  
		Last Modified: Thu, 10 Feb 2022 19:44:26 GMT  
		Size: 127.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f283b3b5916d34a72f4a2bd9425ab54f7195f0bbd755302026df11a145f607c2`  
		Last Modified: Thu, 10 Feb 2022 21:24:15 GMT  
		Size: 4.3 KB (4315 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:829024693e1baa4e9ea3de35c9c489e1eaaded6d45346a9a2c160fe591b5795f`  
		Last Modified: Thu, 10 Feb 2022 21:24:25 GMT  
		Size: 56.5 MB (56491834 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:11cf51ae05052e0d39503e90e83b62670f53b1522675726a7b35a32c8b33c5be`  
		Last Modified: Fri, 11 Feb 2022 01:42:18 GMT  
		Size: 115.9 MB (115864641 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `gradle:jdk11` - linux; ppc64le

```console
$ docker pull gradle@sha256:d465e3526b83f0489bbada3c3c5ee009e1c67a90aac5b7d564bc6f4b099178e2
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **416.2 MB (416214269 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:17c9282cfc96d874849e8efadbd2d4b57bfe715b1624c0933d93ee11ca35e56e`
-	Default Command: `["gradle"]`

```dockerfile
# Wed, 02 Feb 2022 03:50:21 GMT
ADD file:e27da75ca1655de0ac82ef9879f868863388ea992e031aeace61195495bc21bc in / 
# Wed, 02 Feb 2022 03:50:25 GMT
CMD ["bash"]
# Wed, 02 Feb 2022 05:45:23 GMT
ENV LANG=en_US.UTF-8 LANGUAGE=en_US:en LC_ALL=en_US.UTF-8
# Wed, 02 Feb 2022 05:48:39 GMT
RUN apt-get update     && DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends tzdata curl ca-certificates fontconfig locales python-is-python3     && echo "en_US.UTF-8 UTF-8" >> /etc/locale.gen     && locale-gen en_US.UTF-8     && rm -rf /var/lib/apt/lists/*
# Thu, 10 Feb 2022 20:18:23 GMT
ENV JAVA_VERSION=jdk-11.0.14.1+1
# Thu, 10 Feb 2022 20:18:50 GMT
RUN set -eux;     ARCH="$(dpkg --print-architecture)";     case "${ARCH}" in        aarch64|arm64)          ESUM='79572f5172c6a040591d34632f98a20ed148702bbce2f57649e8ac01c0d2e3db';          BINARY_URL='https://github.com/adoptium/temurin11-binaries/releases/download/jdk-11.0.14.1%2B1/OpenJDK11U-jdk_aarch64_linux_hotspot_11.0.14.1_1.tar.gz';          ;;        armhf|arm)          ESUM='f4d53a1753cdde830d7872c6a1279df441f3f9aeb5d5037a568b3a392ebce9c2';          BINARY_URL='https://github.com/adoptium/temurin11-binaries/releases/download/jdk-11.0.14.1%2B1/OpenJDK11U-jdk_arm_linux_hotspot_11.0.14.1_1.tar.gz';          ;;        ppc64el|powerpc:common64)          ESUM='9750e11721282a9afd18a07743f19c699b2b71ce20d02f3f0a906088b9ae6d9a';          BINARY_URL='https://github.com/adoptium/temurin11-binaries/releases/download/jdk-11.0.14.1%2B1/OpenJDK11U-jdk_ppc64le_linux_hotspot_11.0.14.1_1.tar.gz';          ;;        s390x|s390:64-bit)          ESUM='79a27a4dc23dff38a5c21e5ba9b7efcf0aa5e14ace1a3b19bec53e255c487521';          BINARY_URL='https://github.com/adoptium/temurin11-binaries/releases/download/jdk-11.0.14.1%2B1/OpenJDK11U-jdk_s390x_linux_hotspot_11.0.14.1_1.tar.gz';          ;;        amd64|i386:x86-64)          ESUM='43fb84f8063ad9bf6b6d694a67b8f64c8827552b920ec5ce794dfe5602edffe7';          BINARY_URL='https://github.com/adoptium/temurin11-binaries/releases/download/jdk-11.0.14.1%2B1/OpenJDK11U-jdk_x64_linux_hotspot_11.0.14.1_1.tar.gz';          ;;        *)          echo "Unsupported arch: ${ARCH}";          exit 1;          ;;     esac;     curl -LfsSo /tmp/openjdk.tar.gz ${BINARY_URL};     echo "${ESUM} */tmp/openjdk.tar.gz" | sha256sum -c -;     mkdir -p /opt/java/openjdk;     cd /opt/java/openjdk;     tar -xf /tmp/openjdk.tar.gz --strip-components=1;     rm -rf /tmp/openjdk.tar.gz;
# Thu, 10 Feb 2022 20:18:57 GMT
ENV JAVA_HOME=/opt/java/openjdk PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 10 Feb 2022 20:19:03 GMT
RUN echo Verifying install ...     && echo javac --version && javac --version     && echo java --version && java --version     && echo Complete.
# Thu, 10 Feb 2022 20:19:06 GMT
CMD ["jshell"]
# Thu, 10 Feb 2022 20:44:15 GMT
CMD ["gradle"]
# Thu, 10 Feb 2022 20:44:18 GMT
ENV GRADLE_HOME=/opt/gradle
# Thu, 10 Feb 2022 20:44:26 GMT
RUN set -o errexit -o nounset     && echo "Adding gradle user and group"     && groupadd --system --gid 1000 gradle     && useradd --system --gid gradle --uid 1000 --shell /bin/bash --create-home gradle     && mkdir /home/gradle/.gradle     && chown --recursive gradle:gradle /home/gradle         && echo "Symlinking root Gradle cache to gradle Gradle cache"     && ln --symbolic /home/gradle/.gradle /root/.gradle
# Thu, 10 Feb 2022 20:44:30 GMT
VOLUME [/home/gradle/.gradle]
# Thu, 10 Feb 2022 20:44:35 GMT
WORKDIR /home/gradle
# Thu, 10 Feb 2022 20:46:01 GMT
RUN set -o errexit -o nounset     && apt-get update     && apt-get install --yes --no-install-recommends         unzip         wget                 bzr         git         git-lfs         mercurial         openssh-client         subversion     && rm --recursive --force /var/lib/apt/lists/*         && echo "Testing VCSes"     && which bzr     && which git     && which git-lfs     && which hg     && which svn
# Fri, 11 Feb 2022 01:36:39 GMT
ENV GRADLE_VERSION=7.4
# Fri, 11 Feb 2022 01:36:42 GMT
ARG GRADLE_DOWNLOAD_SHA256=8cc27038d5dbd815759851ba53e70cf62e481b87494cc97cfd97982ada5ba634
# Fri, 11 Feb 2022 01:37:08 GMT
# ARGS: GRADLE_DOWNLOAD_SHA256=8cc27038d5dbd815759851ba53e70cf62e481b87494cc97cfd97982ada5ba634
RUN set -o errexit -o nounset     && echo "Downloading Gradle"     && wget --no-verbose --output-document=gradle.zip "https://services.gradle.org/distributions/gradle-${GRADLE_VERSION}-bin.zip"         && echo "Checking download hash"     && echo "${GRADLE_DOWNLOAD_SHA256} *gradle.zip" | sha256sum --check -         && echo "Installing Gradle"     && unzip gradle.zip     && rm gradle.zip     && mv "gradle-${GRADLE_VERSION}" "${GRADLE_HOME}/"     && ln --symbolic "${GRADLE_HOME}/bin/gradle" /usr/bin/gradle         && echo "Testing Gradle installation"     && gradle --version
```

-	Layers:
	-	`sha256:e4ad98202983f0b602991305f807e9b8460bb3fdb617889c276ccbd4b92c69b4`  
		Last Modified: Wed, 02 Feb 2022 03:53:11 GMT  
		Size: 33.3 MB (33284717 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b628b171f10e336a4f91bbf963a6d636a2d90773ed7eef1ecafde5d9939c3c11`  
		Last Modified: Wed, 02 Feb 2022 05:57:19 GMT  
		Size: 26.6 MB (26643271 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b63b955c60d8f56b89215605e99752a2fef17c56b03c77fa2d755ec4f3cf9117`  
		Last Modified: Thu, 10 Feb 2022 20:24:24 GMT  
		Size: 175.8 MB (175842548 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:47c0bdac2d2688977b775f7d60bb1834751bbbfc3d3a7b23c763ed770f879f02`  
		Last Modified: Thu, 10 Feb 2022 20:24:05 GMT  
		Size: 160.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dd0e8815fcb42aa93cd860f5a38e2b44cbc75ec3f64fada8efff6a633b645a7e`  
		Last Modified: Thu, 10 Feb 2022 20:50:08 GMT  
		Size: 4.4 KB (4372 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2d1df885d2fef4f9215ba9278a7920d78088a811dd5291115eb64c41ba157d6e`  
		Last Modified: Thu, 10 Feb 2022 20:50:22 GMT  
		Size: 64.6 MB (64574438 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1dae24e7fc746619baaee4827e3359dfb0e09f29892838c55951689b5408fd48`  
		Last Modified: Fri, 11 Feb 2022 01:40:08 GMT  
		Size: 115.9 MB (115864763 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `gradle:jdk11` - linux; s390x

```console
$ docker pull gradle@sha256:a0fb4b22c8c85a642f2df67e00fc6c793886004014212b32271858ca05991a40
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **391.9 MB (391945162 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:1a540d07b1c1f4df1ed3fa6661bd99524de352274d9923b57fc9c395583132dd`
-	Default Command: `["gradle"]`

```dockerfile
# Wed, 02 Feb 2022 01:42:16 GMT
ADD file:f35a5307585c918b783420eea01f5947181ac58f8eeb855a8f73f38f1477700f in / 
# Wed, 02 Feb 2022 01:42:17 GMT
CMD ["bash"]
# Wed, 02 Feb 2022 02:22:59 GMT
ENV LANG=en_US.UTF-8 LANGUAGE=en_US:en LC_ALL=en_US.UTF-8
# Wed, 02 Feb 2022 02:23:15 GMT
RUN apt-get update     && DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends tzdata curl ca-certificates fontconfig locales python-is-python3     && echo "en_US.UTF-8 UTF-8" >> /etc/locale.gen     && locale-gen en_US.UTF-8     && rm -rf /var/lib/apt/lists/*
# Thu, 10 Feb 2022 19:41:41 GMT
ENV JAVA_VERSION=jdk-11.0.14.1+1
# Thu, 10 Feb 2022 19:41:54 GMT
RUN set -eux;     ARCH="$(dpkg --print-architecture)";     case "${ARCH}" in        aarch64|arm64)          ESUM='79572f5172c6a040591d34632f98a20ed148702bbce2f57649e8ac01c0d2e3db';          BINARY_URL='https://github.com/adoptium/temurin11-binaries/releases/download/jdk-11.0.14.1%2B1/OpenJDK11U-jdk_aarch64_linux_hotspot_11.0.14.1_1.tar.gz';          ;;        armhf|arm)          ESUM='f4d53a1753cdde830d7872c6a1279df441f3f9aeb5d5037a568b3a392ebce9c2';          BINARY_URL='https://github.com/adoptium/temurin11-binaries/releases/download/jdk-11.0.14.1%2B1/OpenJDK11U-jdk_arm_linux_hotspot_11.0.14.1_1.tar.gz';          ;;        ppc64el|powerpc:common64)          ESUM='9750e11721282a9afd18a07743f19c699b2b71ce20d02f3f0a906088b9ae6d9a';          BINARY_URL='https://github.com/adoptium/temurin11-binaries/releases/download/jdk-11.0.14.1%2B1/OpenJDK11U-jdk_ppc64le_linux_hotspot_11.0.14.1_1.tar.gz';          ;;        s390x|s390:64-bit)          ESUM='79a27a4dc23dff38a5c21e5ba9b7efcf0aa5e14ace1a3b19bec53e255c487521';          BINARY_URL='https://github.com/adoptium/temurin11-binaries/releases/download/jdk-11.0.14.1%2B1/OpenJDK11U-jdk_s390x_linux_hotspot_11.0.14.1_1.tar.gz';          ;;        amd64|i386:x86-64)          ESUM='43fb84f8063ad9bf6b6d694a67b8f64c8827552b920ec5ce794dfe5602edffe7';          BINARY_URL='https://github.com/adoptium/temurin11-binaries/releases/download/jdk-11.0.14.1%2B1/OpenJDK11U-jdk_x64_linux_hotspot_11.0.14.1_1.tar.gz';          ;;        *)          echo "Unsupported arch: ${ARCH}";          exit 1;          ;;     esac;     curl -LfsSo /tmp/openjdk.tar.gz ${BINARY_URL};     echo "${ESUM} */tmp/openjdk.tar.gz" | sha256sum -c -;     mkdir -p /opt/java/openjdk;     cd /opt/java/openjdk;     tar -xf /tmp/openjdk.tar.gz --strip-components=1;     rm -rf /tmp/openjdk.tar.gz;
# Thu, 10 Feb 2022 19:41:58 GMT
ENV JAVA_HOME=/opt/java/openjdk PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 10 Feb 2022 19:41:58 GMT
RUN echo Verifying install ...     && echo javac --version && javac --version     && echo java --version && java --version     && echo Complete.
# Thu, 10 Feb 2022 19:41:59 GMT
CMD ["jshell"]
# Thu, 10 Feb 2022 21:40:14 GMT
CMD ["gradle"]
# Thu, 10 Feb 2022 21:40:14 GMT
ENV GRADLE_HOME=/opt/gradle
# Thu, 10 Feb 2022 21:40:15 GMT
RUN set -o errexit -o nounset     && echo "Adding gradle user and group"     && groupadd --system --gid 1000 gradle     && useradd --system --gid gradle --uid 1000 --shell /bin/bash --create-home gradle     && mkdir /home/gradle/.gradle     && chown --recursive gradle:gradle /home/gradle         && echo "Symlinking root Gradle cache to gradle Gradle cache"     && ln --symbolic /home/gradle/.gradle /root/.gradle
# Thu, 10 Feb 2022 21:40:15 GMT
VOLUME [/home/gradle/.gradle]
# Thu, 10 Feb 2022 21:40:15 GMT
WORKDIR /home/gradle
# Thu, 10 Feb 2022 21:40:38 GMT
RUN set -o errexit -o nounset     && apt-get update     && apt-get install --yes --no-install-recommends         unzip         wget                 bzr         git         git-lfs         mercurial         openssh-client         subversion     && rm --recursive --force /var/lib/apt/lists/*         && echo "Testing VCSes"     && which bzr     && which git     && which git-lfs     && which hg     && which svn
# Fri, 11 Feb 2022 01:41:29 GMT
ENV GRADLE_VERSION=7.4
# Fri, 11 Feb 2022 01:41:29 GMT
ARG GRADLE_DOWNLOAD_SHA256=8cc27038d5dbd815759851ba53e70cf62e481b87494cc97cfd97982ada5ba634
# Fri, 11 Feb 2022 01:41:34 GMT
# ARGS: GRADLE_DOWNLOAD_SHA256=8cc27038d5dbd815759851ba53e70cf62e481b87494cc97cfd97982ada5ba634
RUN set -o errexit -o nounset     && echo "Downloading Gradle"     && wget --no-verbose --output-document=gradle.zip "https://services.gradle.org/distributions/gradle-${GRADLE_VERSION}-bin.zip"         && echo "Checking download hash"     && echo "${GRADLE_DOWNLOAD_SHA256} *gradle.zip" | sha256sum --check -         && echo "Installing Gradle"     && unzip gradle.zip     && rm gradle.zip     && mv "gradle-${GRADLE_VERSION}" "${GRADLE_HOME}/"     && ln --symbolic "${GRADLE_HOME}/bin/gradle" /usr/bin/gradle         && echo "Testing Gradle installation"     && gradle --version
```

-	Layers:
	-	`sha256:723da7fec7371c2b30effc8da0790968bef9dd221f5e34b5c8f7d2eff90fbd5e`  
		Last Modified: Wed, 02 Feb 2022 01:44:01 GMT  
		Size: 27.1 MB (27118737 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3e6f03368f8ab26f1db664cfc3332680df5d0a5a30115c89be2b6a6a1205c806`  
		Last Modified: Wed, 02 Feb 2022 02:26:22 GMT  
		Size: 24.4 MB (24446542 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ecf0d343cb4a79b47e6f38151d9d8eb8830adee4b447c67db3506867cd67a94b`  
		Last Modified: Thu, 10 Feb 2022 19:43:45 GMT  
		Size: 168.4 MB (168352457 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b0709131a125058d4bf57cde6fc770d8a5aa578fef14d03365fe98d098966f83`  
		Last Modified: Thu, 10 Feb 2022 19:43:33 GMT  
		Size: 160.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d18b623435ce413f42ae2c89d8a9e71cfffca286b7d2ac264973c83db81b62d3`  
		Last Modified: Thu, 10 Feb 2022 21:42:22 GMT  
		Size: 4.4 KB (4366 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5c5e0e68c92decf5ad0a123774824cc041236f33c690bafea6a319a424c69d51`  
		Last Modified: Thu, 10 Feb 2022 21:42:30 GMT  
		Size: 56.2 MB (56158100 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2087a6239e8e91bf51467491a4ef1f1895f8aaf21fe42f31456d3ae9127253c9`  
		Last Modified: Fri, 11 Feb 2022 01:43:13 GMT  
		Size: 115.9 MB (115864800 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
