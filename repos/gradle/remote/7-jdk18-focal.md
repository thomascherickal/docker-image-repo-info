## `gradle:7-jdk18-focal`

```console
$ docker pull gradle@sha256:732ddc021050bc7e91218b10c351a190f7d6136b6bc851ed36e6e22a5a3ccb3b
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 5
	-	linux; amd64
	-	linux; arm variant v7
	-	linux; arm64 variant v8
	-	linux; ppc64le
	-	linux; s390x

### `gradle:7-jdk18-focal` - linux; amd64

```console
$ docker pull gradle@sha256:ab6e43d55fcac761feb5326eac8732e77af4a242d5c258022d7f5ffe0c385cf2
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **428.2 MB (428230007 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:224bfb4c97125e677e8e813e99c58c25431b344c2f1f33b70f2cd19153605def`
-	Default Command: `["gradle"]`

```dockerfile
# Tue, 02 Aug 2022 01:30:49 GMT
ADD file:af4cf77e6818016b697a1491101b40c71d06529ced65f36107749f099d6d4bdc in / 
# Tue, 02 Aug 2022 01:30:49 GMT
CMD ["bash"]
# Tue, 02 Aug 2022 19:04:22 GMT
ENV LANG=en_US.UTF-8 LANGUAGE=en_US:en LC_ALL=en_US.UTF-8
# Tue, 02 Aug 2022 19:08:27 GMT
RUN apt-get update     && DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends tzdata curl ca-certificates fontconfig locales binutils     && echo "en_US.UTF-8 UTF-8" >> /etc/locale.gen     && locale-gen en_US.UTF-8     && rm -rf /var/lib/apt/lists/*
# Tue, 02 Aug 2022 19:09:58 GMT
ENV JAVA_VERSION=jdk-18.0.2+9
# Tue, 02 Aug 2022 19:10:15 GMT
RUN set -eux;     ARCH="$(dpkg --print-architecture)";     case "${ARCH}" in        aarch64|arm64)          ESUM='f4aca720bfcea4df7f02b59de1f68648632070c492f210b9e41e69170ee5e48f';          BINARY_URL='https://github.com/adoptium/temurin18-binaries/releases/download/jdk-18.0.2%2B9/OpenJDK18U-jdk_aarch64_linux_hotspot_18.0.2_9.tar.gz';          ;;        armhf|arm)          ESUM='52ec0ddee9ff16397de2c9f614ff6b5464220bd5c3d705e8b89d28fd478feb60';          BINARY_URL='https://github.com/adoptium/temurin18-binaries/releases/download/jdk-18.0.2%2B9/OpenJDK18U-jdk_arm_linux_hotspot_18.0.2_9.tar.gz';          ;;        ppc64el|powerpc:common64)          ESUM='4262677f8b6054d26f1c0042ac47dfbaab6a18d7dc73fa807b15ee03cdcbdece';          BINARY_URL='https://github.com/adoptium/temurin18-binaries/releases/download/jdk-18.0.2%2B9/OpenJDK18U-jdk_ppc64le_linux_hotspot_18.0.2_9.tar.gz';          ;;        s390x|s390:64-bit)          ESUM='d916cfa15552ae2ad2f2c96ebc72aaaea4c844af9842f5ca9724fcbbdc08d25c';          BINARY_URL='https://github.com/adoptium/temurin18-binaries/releases/download/jdk-18.0.2%2B9/OpenJDK18U-jdk_s390x_linux_hotspot_18.0.2_9.tar.gz';          ;;        amd64|i386:x86-64)          ESUM='5e5dbf6f1308829528778e00631ec83e252d90fc444503091e71a66465e88941';          BINARY_URL='https://github.com/adoptium/temurin18-binaries/releases/download/jdk-18.0.2%2B9/OpenJDK18U-jdk_x64_linux_hotspot_18.0.2_9.tar.gz';          ;;        *)          echo "Unsupported arch: ${ARCH}";          exit 1;          ;;     esac;     curl -LfsSo /tmp/openjdk.tar.gz ${BINARY_URL};     echo "${ESUM} */tmp/openjdk.tar.gz" | sha256sum -c -;     mkdir -p /opt/java/openjdk;     cd /opt/java/openjdk;     tar -xf /tmp/openjdk.tar.gz --strip-components=1;     rm -rf /tmp/openjdk.tar.gz;
# Tue, 02 Aug 2022 19:10:16 GMT
ENV JAVA_HOME=/opt/java/openjdk PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 02 Aug 2022 19:10:17 GMT
RUN echo Verifying install ...     && echo javac --version && javac --version     && echo java --version && java --version     && echo Complete.
# Tue, 02 Aug 2022 19:10:17 GMT
CMD ["jshell"]
# Wed, 03 Aug 2022 12:35:51 GMT
CMD ["gradle"]
# Wed, 03 Aug 2022 12:35:51 GMT
ENV GRADLE_HOME=/opt/gradle
# Wed, 03 Aug 2022 12:35:52 GMT
RUN set -o errexit -o nounset     && echo "Adding gradle user and group"     && groupadd --system --gid 1000 gradle     && useradd --system --gid gradle --uid 1000 --shell /bin/bash --create-home gradle     && mkdir /home/gradle/.gradle     && chown --recursive gradle:gradle /home/gradle         && echo "Symlinking root Gradle cache to gradle Gradle cache"     && ln --symbolic /home/gradle/.gradle /root/.gradle
# Wed, 03 Aug 2022 12:35:52 GMT
VOLUME [/home/gradle/.gradle]
# Wed, 03 Aug 2022 12:35:52 GMT
WORKDIR /home/gradle
# Wed, 03 Aug 2022 12:36:11 GMT
RUN set -o errexit -o nounset     && apt-get update     && apt-get install --yes --no-install-recommends         unzip         wget                 bzr         git         git-lfs         mercurial         openssh-client         subversion     && rm --recursive --force /var/lib/apt/lists/*         && echo "Testing VCSes"     && which bzr     && which git     && which git-lfs     && which hg     && which svn
# Wed, 03 Aug 2022 12:36:12 GMT
ENV GRADLE_VERSION=7.5
# Wed, 03 Aug 2022 12:36:12 GMT
ARG GRADLE_DOWNLOAD_SHA256=cb87f222c5585bd46838ad4db78463a5c5f3d336e5e2b98dc7c0c586527351c2
# Wed, 03 Aug 2022 12:36:17 GMT
# ARGS: GRADLE_DOWNLOAD_SHA256=cb87f222c5585bd46838ad4db78463a5c5f3d336e5e2b98dc7c0c586527351c2
RUN set -o errexit -o nounset     && echo "Downloading Gradle"     && wget --no-verbose --output-document=gradle.zip "https://services.gradle.org/distributions/gradle-${GRADLE_VERSION}-bin.zip"         && echo "Checking download hash"     && echo "${GRADLE_DOWNLOAD_SHA256} *gradle.zip" | sha256sum --check -         && echo "Installing Gradle"     && unzip gradle.zip     && rm gradle.zip     && mv "gradle-${GRADLE_VERSION}" "${GRADLE_HOME}/"     && ln --symbolic "${GRADLE_HOME}/bin/gradle" /usr/bin/gradle         && echo "Testing Gradle installation"     && gradle --version
```

-	Layers:
	-	`sha256:3b65ec22a9e96affe680712973e88355927506aa3f792ff03330f3a3eb601a98`  
		Last Modified: Tue, 02 Aug 2022 01:31:59 GMT  
		Size: 28.6 MB (28572596 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:884d368865943a6ccba3c240161c72a7574ea8c91ec858d4fc4e0513d1b584bf`  
		Last Modified: Tue, 02 Aug 2022 19:16:51 GMT  
		Size: 19.8 MB (19773356 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1d4aa8f807ef0f1da934d7bba1935a55ccfb263283391f9b5b44acbdad1f9028`  
		Last Modified: Tue, 02 Aug 2022 19:18:58 GMT  
		Size: 193.6 MB (193574331 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e0cbe7e6ff114775d194df3b4efa427883a816c883ad960825c95375665baac3`  
		Last Modified: Tue, 02 Aug 2022 19:18:43 GMT  
		Size: 162.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5ac0e3c4661721dca2eeb9ea0b3ef8091d22ae7c5caa4bb6bd9bef47654ce09b`  
		Last Modified: Wed, 03 Aug 2022 12:44:24 GMT  
		Size: 4.4 KB (4360 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:75f4b8389bfb431a6bbc0069fc169e2c5c38f229f51c92b0fb07bd1245e56cab`  
		Last Modified: Wed, 03 Aug 2022 12:44:35 GMT  
		Size: 65.6 MB (65649440 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7f59c5fe0c05a26098bdae729664de453822aee567760f0d8ef4a534516e5e6b`  
		Last Modified: Wed, 03 Aug 2022 12:44:31 GMT  
		Size: 120.7 MB (120655762 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `gradle:7-jdk18-focal` - linux; arm variant v7

```console
$ docker pull gradle@sha256:3db356798cf06589dc72a3a73b073a55a1a8c907be2eb503ddeae11b838dcd65
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **415.1 MB (415126196 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:3b1ee79f5bbf53a8a073889cf54a7463b27633f96279cc6473eb5037e71f5b3e`
-	Default Command: `["gradle"]`

```dockerfile
# Tue, 07 Jun 2022 05:50:50 GMT
ADD file:c95d34737ba1f11ac8b92be0125aad2baae46448f0d8ebd85ad69076006a3254 in / 
# Tue, 07 Jun 2022 05:50:51 GMT
CMD ["bash"]
# Sat, 30 Jul 2022 02:49:11 GMT
ENV LANG=en_US.UTF-8 LANGUAGE=en_US:en LC_ALL=en_US.UTF-8
# Sat, 30 Jul 2022 02:52:16 GMT
RUN apt-get update     && DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends tzdata curl ca-certificates fontconfig locales binutils     && echo "en_US.UTF-8 UTF-8" >> /etc/locale.gen     && locale-gen en_US.UTF-8     && rm -rf /var/lib/apt/lists/*
# Sat, 30 Jul 2022 02:53:39 GMT
ENV JAVA_VERSION=jdk-18.0.1+10
# Sat, 30 Jul 2022 02:53:52 GMT
RUN set -eux;     ARCH="$(dpkg --print-architecture)";     case "${ARCH}" in        aarch64|arm64)          ESUM='37ceaf232a85cce46bcccfd71839854e8b14bf3160e7ef72a676b9cae45ee8af';          BINARY_URL='https://github.com/adoptium/temurin18-binaries/releases/download/jdk-18.0.1%2B10/OpenJDK18U-jdk_aarch64_linux_hotspot_18.0.1_10.tar.gz';          ;;        armhf|arm)          ESUM='0ddec3c165ab0b662a57a845db3fdaeb840660b493f164696b03df76aadf61c8';          BINARY_URL='https://github.com/adoptium/temurin18-binaries/releases/download/jdk-18.0.1%2B10/OpenJDK18U-jdk_arm_linux_hotspot_18.0.1_10.tar.gz';          ;;        ppc64el|powerpc:common64)          ESUM='7c3376b4eb14a58d27816776e965f1b214c17c4c2e918dc9e996a0f30e76550e';          BINARY_URL='https://github.com/adoptium/temurin18-binaries/releases/download/jdk-18.0.1%2B10/OpenJDK18U-jdk_ppc64le_linux_hotspot_18.0.1_10.tar.gz';          ;;        s390x|s390:64-bit)          ESUM='236dc78e698c21f258078661ab5c74b8cc7d38a1febb7aa7a6598bd3b999c0dc';          BINARY_URL='https://github.com/adoptium/temurin18-binaries/releases/download/jdk-18.0.1%2B10/OpenJDK18U-jdk_s390x_linux_hotspot_18.0.1_10.tar.gz';          ;;        amd64|i386:x86-64)          ESUM='16b1d9d75f22c157af04a1fd9c664324c7f4b5163c022b382a2f2e8897c1b0a2';          BINARY_URL='https://github.com/adoptium/temurin18-binaries/releases/download/jdk-18.0.1%2B10/OpenJDK18U-jdk_x64_linux_hotspot_18.0.1_10.tar.gz';          ;;        *)          echo "Unsupported arch: ${ARCH}";          exit 1;          ;;     esac;     curl -LfsSo /tmp/openjdk.tar.gz ${BINARY_URL};     echo "${ESUM} */tmp/openjdk.tar.gz" | sha256sum -c -;     mkdir -p /opt/java/openjdk;     cd /opt/java/openjdk;     tar -xf /tmp/openjdk.tar.gz --strip-components=1;     rm -rf /tmp/openjdk.tar.gz;
# Sat, 30 Jul 2022 02:53:53 GMT
ENV JAVA_HOME=/opt/java/openjdk PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Sat, 30 Jul 2022 02:53:53 GMT
RUN echo Verifying install ...     && echo javac --version && javac --version     && echo java --version && java --version     && echo Complete.
# Sat, 30 Jul 2022 02:53:53 GMT
CMD ["jshell"]
# Sat, 30 Jul 2022 12:25:42 GMT
CMD ["gradle"]
# Sat, 30 Jul 2022 12:25:42 GMT
ENV GRADLE_HOME=/opt/gradle
# Sat, 30 Jul 2022 12:25:42 GMT
RUN set -o errexit -o nounset     && echo "Adding gradle user and group"     && groupadd --system --gid 1000 gradle     && useradd --system --gid gradle --uid 1000 --shell /bin/bash --create-home gradle     && mkdir /home/gradle/.gradle     && chown --recursive gradle:gradle /home/gradle         && echo "Symlinking root Gradle cache to gradle Gradle cache"     && ln --symbolic /home/gradle/.gradle /root/.gradle
# Sat, 30 Jul 2022 12:25:42 GMT
VOLUME [/home/gradle/.gradle]
# Sat, 30 Jul 2022 12:25:42 GMT
WORKDIR /home/gradle
# Sat, 30 Jul 2022 12:26:06 GMT
RUN set -o errexit -o nounset     && apt-get update     && apt-get install --yes --no-install-recommends         unzip         wget                 bzr         git         git-lfs         mercurial         openssh-client         subversion     && rm --recursive --force /var/lib/apt/lists/*         && echo "Testing VCSes"     && which bzr     && which git     && which git-lfs     && which hg     && which svn
# Sat, 30 Jul 2022 12:26:06 GMT
ENV GRADLE_VERSION=7.5
# Sat, 30 Jul 2022 12:26:06 GMT
ARG GRADLE_DOWNLOAD_SHA256=cb87f222c5585bd46838ad4db78463a5c5f3d336e5e2b98dc7c0c586527351c2
# Sat, 30 Jul 2022 12:26:11 GMT
# ARGS: GRADLE_DOWNLOAD_SHA256=cb87f222c5585bd46838ad4db78463a5c5f3d336e5e2b98dc7c0c586527351c2
RUN set -o errexit -o nounset     && echo "Downloading Gradle"     && wget --no-verbose --output-document=gradle.zip "https://services.gradle.org/distributions/gradle-${GRADLE_VERSION}-bin.zip"         && echo "Checking download hash"     && echo "${GRADLE_DOWNLOAD_SHA256} *gradle.zip" | sha256sum --check -         && echo "Installing Gradle"     && unzip gradle.zip     && rm gradle.zip     && mv "gradle-${GRADLE_VERSION}" "${GRADLE_HOME}/"     && ln --symbolic "${GRADLE_HOME}/bin/gradle" /usr/bin/gradle         && echo "Testing Gradle installation"     && gradle --version
```

-	Layers:
	-	`sha256:36754881d0ec0d456ee49776d62f6f0df47d29956ac7b2231b797e05780c6744`  
		Last Modified: Tue, 07 Jun 2022 05:55:05 GMT  
		Size: 24.6 MB (24592639 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:916985a90d5d9c5f2a2e834acb83d3a31a527d90f6140d699201612fc01376a1`  
		Last Modified: Sat, 30 Jul 2022 02:59:50 GMT  
		Size: 19.2 MB (19191327 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:327f31f061032dc4c925a0d1d33ef3b8e8e18658ff59a5145e0698d676361226`  
		Last Modified: Sat, 30 Jul 2022 03:01:48 GMT  
		Size: 190.7 MB (190657726 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a37456abe16fba290dbda690e34ef148645998550a6aa066ba23f2079b4c1ddc`  
		Last Modified: Sat, 30 Jul 2022 03:01:31 GMT  
		Size: 160.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4c006ffa39d44de238d18ce91cd6a3f33fbee0106a12f5b1fe8e8f8392d563ca`  
		Last Modified: Sat, 30 Jul 2022 12:38:15 GMT  
		Size: 4.3 KB (4349 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:969a6939911cc92aae59e51f8a2e2f20e6222a3b62c6d795d75da4f7d4ef2eaa`  
		Last Modified: Sat, 30 Jul 2022 12:38:30 GMT  
		Size: 60.0 MB (60024264 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:186f4924678e87b988411e9524b5920210cced33cc6466b8b7f83c4a29ffa08f`  
		Last Modified: Sat, 30 Jul 2022 12:38:26 GMT  
		Size: 120.7 MB (120655731 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `gradle:7-jdk18-focal` - linux; arm64 variant v8

```console
$ docker pull gradle@sha256:af804d7a71db5f007d736a154eeae3a7cb36b232ef464d31be819172ae996167
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **426.2 MB (426150807 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:5db6d470477aaf9444a2592bf408d60587337a3bede408714b2d16a8e981454c`
-	Default Command: `["gradle"]`

```dockerfile
# Tue, 02 Aug 2022 01:18:51 GMT
ADD file:151548d1bfac57d762f2c0b18b2378c363ffd1568da9fecd4be611db4832e8e2 in / 
# Tue, 02 Aug 2022 01:18:51 GMT
CMD ["bash"]
# Tue, 02 Aug 2022 17:50:53 GMT
ENV LANG=en_US.UTF-8 LANGUAGE=en_US:en LC_ALL=en_US.UTF-8
# Tue, 02 Aug 2022 17:54:11 GMT
RUN apt-get update     && DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends tzdata curl ca-certificates fontconfig locales binutils     && echo "en_US.UTF-8 UTF-8" >> /etc/locale.gen     && locale-gen en_US.UTF-8     && rm -rf /var/lib/apt/lists/*
# Tue, 02 Aug 2022 17:55:38 GMT
ENV JAVA_VERSION=jdk-18.0.2+9
# Tue, 02 Aug 2022 17:55:53 GMT
RUN set -eux;     ARCH="$(dpkg --print-architecture)";     case "${ARCH}" in        aarch64|arm64)          ESUM='f4aca720bfcea4df7f02b59de1f68648632070c492f210b9e41e69170ee5e48f';          BINARY_URL='https://github.com/adoptium/temurin18-binaries/releases/download/jdk-18.0.2%2B9/OpenJDK18U-jdk_aarch64_linux_hotspot_18.0.2_9.tar.gz';          ;;        armhf|arm)          ESUM='52ec0ddee9ff16397de2c9f614ff6b5464220bd5c3d705e8b89d28fd478feb60';          BINARY_URL='https://github.com/adoptium/temurin18-binaries/releases/download/jdk-18.0.2%2B9/OpenJDK18U-jdk_arm_linux_hotspot_18.0.2_9.tar.gz';          ;;        ppc64el|powerpc:common64)          ESUM='4262677f8b6054d26f1c0042ac47dfbaab6a18d7dc73fa807b15ee03cdcbdece';          BINARY_URL='https://github.com/adoptium/temurin18-binaries/releases/download/jdk-18.0.2%2B9/OpenJDK18U-jdk_ppc64le_linux_hotspot_18.0.2_9.tar.gz';          ;;        s390x|s390:64-bit)          ESUM='d916cfa15552ae2ad2f2c96ebc72aaaea4c844af9842f5ca9724fcbbdc08d25c';          BINARY_URL='https://github.com/adoptium/temurin18-binaries/releases/download/jdk-18.0.2%2B9/OpenJDK18U-jdk_s390x_linux_hotspot_18.0.2_9.tar.gz';          ;;        amd64|i386:x86-64)          ESUM='5e5dbf6f1308829528778e00631ec83e252d90fc444503091e71a66465e88941';          BINARY_URL='https://github.com/adoptium/temurin18-binaries/releases/download/jdk-18.0.2%2B9/OpenJDK18U-jdk_x64_linux_hotspot_18.0.2_9.tar.gz';          ;;        *)          echo "Unsupported arch: ${ARCH}";          exit 1;          ;;     esac;     curl -LfsSo /tmp/openjdk.tar.gz ${BINARY_URL};     echo "${ESUM} */tmp/openjdk.tar.gz" | sha256sum -c -;     mkdir -p /opt/java/openjdk;     cd /opt/java/openjdk;     tar -xf /tmp/openjdk.tar.gz --strip-components=1;     rm -rf /tmp/openjdk.tar.gz;
# Tue, 02 Aug 2022 17:55:54 GMT
ENV JAVA_HOME=/opt/java/openjdk PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 02 Aug 2022 17:55:55 GMT
RUN echo Verifying install ...     && echo javac --version && javac --version     && echo java --version && java --version     && echo Complete.
# Tue, 02 Aug 2022 17:55:55 GMT
CMD ["jshell"]
# Wed, 03 Aug 2022 11:09:16 GMT
CMD ["gradle"]
# Wed, 03 Aug 2022 11:09:17 GMT
ENV GRADLE_HOME=/opt/gradle
# Wed, 03 Aug 2022 11:09:18 GMT
RUN set -o errexit -o nounset     && echo "Adding gradle user and group"     && groupadd --system --gid 1000 gradle     && useradd --system --gid gradle --uid 1000 --shell /bin/bash --create-home gradle     && mkdir /home/gradle/.gradle     && chown --recursive gradle:gradle /home/gradle         && echo "Symlinking root Gradle cache to gradle Gradle cache"     && ln --symbolic /home/gradle/.gradle /root/.gradle
# Wed, 03 Aug 2022 11:09:19 GMT
VOLUME [/home/gradle/.gradle]
# Wed, 03 Aug 2022 11:09:20 GMT
WORKDIR /home/gradle
# Wed, 03 Aug 2022 11:09:43 GMT
RUN set -o errexit -o nounset     && apt-get update     && apt-get install --yes --no-install-recommends         unzip         wget                 bzr         git         git-lfs         mercurial         openssh-client         subversion     && rm --recursive --force /var/lib/apt/lists/*         && echo "Testing VCSes"     && which bzr     && which git     && which git-lfs     && which hg     && which svn
# Wed, 03 Aug 2022 11:09:44 GMT
ENV GRADLE_VERSION=7.5
# Wed, 03 Aug 2022 11:09:45 GMT
ARG GRADLE_DOWNLOAD_SHA256=cb87f222c5585bd46838ad4db78463a5c5f3d336e5e2b98dc7c0c586527351c2
# Wed, 03 Aug 2022 11:09:51 GMT
# ARGS: GRADLE_DOWNLOAD_SHA256=cb87f222c5585bd46838ad4db78463a5c5f3d336e5e2b98dc7c0c586527351c2
RUN set -o errexit -o nounset     && echo "Downloading Gradle"     && wget --no-verbose --output-document=gradle.zip "https://services.gradle.org/distributions/gradle-${GRADLE_VERSION}-bin.zip"         && echo "Checking download hash"     && echo "${GRADLE_DOWNLOAD_SHA256} *gradle.zip" | sha256sum --check -         && echo "Installing Gradle"     && unzip gradle.zip     && rm gradle.zip     && mv "gradle-${GRADLE_VERSION}" "${GRADLE_HOME}/"     && ln --symbolic "${GRADLE_HOME}/bin/gradle" /usr/bin/gradle         && echo "Testing Gradle installation"     && gradle --version
```

-	Layers:
	-	`sha256:a749a280e3e905de447c3d95a39e8aa1ede5835a6eadeb0c11596051592b675b`  
		Last Modified: Tue, 02 Aug 2022 01:20:32 GMT  
		Size: 27.2 MB (27191804 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8ae4b399269fa184aac3bbe66763d5b373c71d601c49266b8828e09b7fdd6789`  
		Last Modified: Tue, 02 Aug 2022 18:03:22 GMT  
		Size: 20.5 MB (20491864 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b229932ee14f3a95a3f18ef43efdda9f131cea961acc685be93686c7fea3f22f`  
		Last Modified: Tue, 02 Aug 2022 18:05:24 GMT  
		Size: 192.4 MB (192425956 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bb972f16157bf25735443794500d753294ab548aea5b95d0fdac143072e1615e`  
		Last Modified: Tue, 02 Aug 2022 18:05:07 GMT  
		Size: 128.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:28386f693d651fa3ef5554fb35651b9e02065e5fe971a1c0b973a902b61cf721`  
		Last Modified: Wed, 03 Aug 2022 11:20:03 GMT  
		Size: 4.3 KB (4310 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ba597ec4c2782087a3fbeea5a93be682050ffd1bf245d73cf97fe6d594e6bcd6`  
		Last Modified: Wed, 03 Aug 2022 11:20:14 GMT  
		Size: 65.4 MB (65381132 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:370d5213dc1b582d55466f54e974410422409ee0170f87f5e47925957b5c7013`  
		Last Modified: Wed, 03 Aug 2022 11:20:10 GMT  
		Size: 120.7 MB (120655613 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `gradle:7-jdk18-focal` - linux; ppc64le

```console
$ docker pull gradle@sha256:cfc270742cfe283e11877f538cde7daa3e202dc675d1f33c7dd081cecdb0a071
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **442.7 MB (442681023 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:eae0bdbf0026e6bc4b71e6ee21e2083f1cd9d9910fd5391832ccf2f45c250341`
-	Default Command: `["gradle"]`

```dockerfile
# Tue, 07 Jun 2022 05:46:02 GMT
ADD file:86506a94b834ba2b6f10dc0d1955bee539be1cf565e4ccc2c4bc074e0375f115 in / 
# Tue, 07 Jun 2022 05:46:06 GMT
CMD ["bash"]
# Wed, 27 Jul 2022 00:33:57 GMT
ENV LANG=en_US.UTF-8 LANGUAGE=en_US:en LC_ALL=en_US.UTF-8
# Wed, 27 Jul 2022 00:41:17 GMT
RUN apt-get update     && DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends tzdata curl ca-certificates fontconfig locales binutils     && echo "en_US.UTF-8 UTF-8" >> /etc/locale.gen     && locale-gen en_US.UTF-8     && rm -rf /var/lib/apt/lists/*
# Wed, 27 Jul 2022 00:45:18 GMT
ENV JAVA_VERSION=jdk-18.0.1+10
# Wed, 27 Jul 2022 00:45:38 GMT
RUN set -eux;     ARCH="$(dpkg --print-architecture)";     case "${ARCH}" in        aarch64|arm64)          ESUM='37ceaf232a85cce46bcccfd71839854e8b14bf3160e7ef72a676b9cae45ee8af';          BINARY_URL='https://github.com/adoptium/temurin18-binaries/releases/download/jdk-18.0.1%2B10/OpenJDK18U-jdk_aarch64_linux_hotspot_18.0.1_10.tar.gz';          ;;        armhf|arm)          ESUM='0ddec3c165ab0b662a57a845db3fdaeb840660b493f164696b03df76aadf61c8';          BINARY_URL='https://github.com/adoptium/temurin18-binaries/releases/download/jdk-18.0.1%2B10/OpenJDK18U-jdk_arm_linux_hotspot_18.0.1_10.tar.gz';          ;;        ppc64el|powerpc:common64)          ESUM='7c3376b4eb14a58d27816776e965f1b214c17c4c2e918dc9e996a0f30e76550e';          BINARY_URL='https://github.com/adoptium/temurin18-binaries/releases/download/jdk-18.0.1%2B10/OpenJDK18U-jdk_ppc64le_linux_hotspot_18.0.1_10.tar.gz';          ;;        s390x|s390:64-bit)          ESUM='236dc78e698c21f258078661ab5c74b8cc7d38a1febb7aa7a6598bd3b999c0dc';          BINARY_URL='https://github.com/adoptium/temurin18-binaries/releases/download/jdk-18.0.1%2B10/OpenJDK18U-jdk_s390x_linux_hotspot_18.0.1_10.tar.gz';          ;;        amd64|i386:x86-64)          ESUM='16b1d9d75f22c157af04a1fd9c664324c7f4b5163c022b382a2f2e8897c1b0a2';          BINARY_URL='https://github.com/adoptium/temurin18-binaries/releases/download/jdk-18.0.1%2B10/OpenJDK18U-jdk_x64_linux_hotspot_18.0.1_10.tar.gz';          ;;        *)          echo "Unsupported arch: ${ARCH}";          exit 1;          ;;     esac;     curl -LfsSo /tmp/openjdk.tar.gz ${BINARY_URL};     echo "${ESUM} */tmp/openjdk.tar.gz" | sha256sum -c -;     mkdir -p /opt/java/openjdk;     cd /opt/java/openjdk;     tar -xf /tmp/openjdk.tar.gz --strip-components=1;     rm -rf /tmp/openjdk.tar.gz;
# Wed, 27 Jul 2022 00:45:41 GMT
ENV JAVA_HOME=/opt/java/openjdk PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 27 Jul 2022 00:45:42 GMT
RUN echo Verifying install ...     && echo javac --version && javac --version     && echo java --version && java --version     && echo Complete.
# Wed, 27 Jul 2022 00:45:43 GMT
CMD ["jshell"]
# Thu, 28 Jul 2022 07:07:09 GMT
CMD ["gradle"]
# Thu, 28 Jul 2022 07:07:09 GMT
ENV GRADLE_HOME=/opt/gradle
# Thu, 28 Jul 2022 07:07:11 GMT
RUN set -o errexit -o nounset     && echo "Adding gradle user and group"     && groupadd --system --gid 1000 gradle     && useradd --system --gid gradle --uid 1000 --shell /bin/bash --create-home gradle     && mkdir /home/gradle/.gradle     && chown --recursive gradle:gradle /home/gradle         && echo "Symlinking root Gradle cache to gradle Gradle cache"     && ln --symbolic /home/gradle/.gradle /root/.gradle
# Thu, 28 Jul 2022 07:07:11 GMT
VOLUME [/home/gradle/.gradle]
# Thu, 28 Jul 2022 07:07:11 GMT
WORKDIR /home/gradle
# Thu, 28 Jul 2022 07:07:50 GMT
RUN set -o errexit -o nounset     && apt-get update     && apt-get install --yes --no-install-recommends         unzip         wget                 bzr         git         git-lfs         mercurial         openssh-client         subversion     && rm --recursive --force /var/lib/apt/lists/*         && echo "Testing VCSes"     && which bzr     && which git     && which git-lfs     && which hg     && which svn
# Thu, 28 Jul 2022 07:07:54 GMT
ENV GRADLE_VERSION=7.5
# Thu, 28 Jul 2022 07:07:54 GMT
ARG GRADLE_DOWNLOAD_SHA256=cb87f222c5585bd46838ad4db78463a5c5f3d336e5e2b98dc7c0c586527351c2
# Thu, 28 Jul 2022 07:08:05 GMT
# ARGS: GRADLE_DOWNLOAD_SHA256=cb87f222c5585bd46838ad4db78463a5c5f3d336e5e2b98dc7c0c586527351c2
RUN set -o errexit -o nounset     && echo "Downloading Gradle"     && wget --no-verbose --output-document=gradle.zip "https://services.gradle.org/distributions/gradle-${GRADLE_VERSION}-bin.zip"         && echo "Checking download hash"     && echo "${GRADLE_DOWNLOAD_SHA256} *gradle.zip" | sha256sum --check -         && echo "Installing Gradle"     && unzip gradle.zip     && rm gradle.zip     && mv "gradle-${GRADLE_VERSION}" "${GRADLE_HOME}/"     && ln --symbolic "${GRADLE_HOME}/bin/gradle" /usr/bin/gradle         && echo "Testing Gradle installation"     && gradle --version
```

-	Layers:
	-	`sha256:3f52d061d2d3fdde0d3a099bbeae64080476c9650e9f3ba05de898d5bb5f03e8`  
		Last Modified: Tue, 07 Jun 2022 05:49:10 GMT  
		Size: 33.3 MB (33294345 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:abff6ca525e26e65e4f33725ff2f731fb66f9fa21452fe1cff1f1d65d9860921`  
		Last Modified: Wed, 27 Jul 2022 00:55:32 GMT  
		Size: 21.7 MB (21686416 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4df7eb7cd5ec16e042b0a9247d6745c5aaf1271227acc11159e7763897cd01ac`  
		Last Modified: Wed, 27 Jul 2022 00:59:05 GMT  
		Size: 192.9 MB (192911578 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:abcd961cc5a44f01bdc20a7a2ade7c8c231e377c4c9d26cbc1b632edc5d86952`  
		Last Modified: Wed, 27 Jul 2022 00:58:40 GMT  
		Size: 160.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c04bd92ad0be418bdebd27fc7207955f31db57b7dfa5562caad7d7dfe025b1f9`  
		Last Modified: Thu, 28 Jul 2022 07:21:03 GMT  
		Size: 4.4 KB (4359 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f2fd7eb1da876659ad6f86db7d3a5908c65ff11084f8349a9118bc9f7fcdbd46`  
		Last Modified: Thu, 28 Jul 2022 07:21:24 GMT  
		Size: 74.1 MB (74128413 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e22947b65f699474f6e7a070aaa6d590c457cfd13aeb9c267b6885af92ecadc5`  
		Last Modified: Thu, 28 Jul 2022 07:21:13 GMT  
		Size: 120.7 MB (120655752 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `gradle:7-jdk18-focal` - linux; s390x

```console
$ docker pull gradle@sha256:9fc96a791068129812d7bfe2e51a39b8fdad34d6994f424d8a74840b895db056
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **413.3 MB (413271407 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:614d33a6d87e8134d280394e0342ddaa20d84521e44cbd3ed936f935069c9bb8`
-	Default Command: `["gradle"]`

```dockerfile
# Tue, 02 Aug 2022 01:02:06 GMT
ADD file:409a01624b482522ab1ba2da28ff57bceb3bf89ff2f3cae5c9ea6068f6993355 in / 
# Tue, 02 Aug 2022 01:02:08 GMT
CMD ["bash"]
# Tue, 02 Aug 2022 12:41:20 GMT
ENV LANG=en_US.UTF-8 LANGUAGE=en_US:en LC_ALL=en_US.UTF-8
# Tue, 02 Aug 2022 12:49:17 GMT
RUN apt-get update     && DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends tzdata curl ca-certificates fontconfig locales binutils     && echo "en_US.UTF-8 UTF-8" >> /etc/locale.gen     && locale-gen en_US.UTF-8     && rm -rf /var/lib/apt/lists/*
# Wed, 03 Aug 2022 02:19:13 GMT
ENV JAVA_VERSION=jdk-18.0.2+9
# Wed, 03 Aug 2022 02:19:22 GMT
RUN set -eux;     ARCH="$(dpkg --print-architecture)";     case "${ARCH}" in        aarch64|arm64)          ESUM='f4aca720bfcea4df7f02b59de1f68648632070c492f210b9e41e69170ee5e48f';          BINARY_URL='https://github.com/adoptium/temurin18-binaries/releases/download/jdk-18.0.2%2B9/OpenJDK18U-jdk_aarch64_linux_hotspot_18.0.2_9.tar.gz';          ;;        armhf|arm)          ESUM='52ec0ddee9ff16397de2c9f614ff6b5464220bd5c3d705e8b89d28fd478feb60';          BINARY_URL='https://github.com/adoptium/temurin18-binaries/releases/download/jdk-18.0.2%2B9/OpenJDK18U-jdk_arm_linux_hotspot_18.0.2_9.tar.gz';          ;;        ppc64el|powerpc:common64)          ESUM='4262677f8b6054d26f1c0042ac47dfbaab6a18d7dc73fa807b15ee03cdcbdece';          BINARY_URL='https://github.com/adoptium/temurin18-binaries/releases/download/jdk-18.0.2%2B9/OpenJDK18U-jdk_ppc64le_linux_hotspot_18.0.2_9.tar.gz';          ;;        s390x|s390:64-bit)          ESUM='d916cfa15552ae2ad2f2c96ebc72aaaea4c844af9842f5ca9724fcbbdc08d25c';          BINARY_URL='https://github.com/adoptium/temurin18-binaries/releases/download/jdk-18.0.2%2B9/OpenJDK18U-jdk_s390x_linux_hotspot_18.0.2_9.tar.gz';          ;;        amd64|i386:x86-64)          ESUM='5e5dbf6f1308829528778e00631ec83e252d90fc444503091e71a66465e88941';          BINARY_URL='https://github.com/adoptium/temurin18-binaries/releases/download/jdk-18.0.2%2B9/OpenJDK18U-jdk_x64_linux_hotspot_18.0.2_9.tar.gz';          ;;        *)          echo "Unsupported arch: ${ARCH}";          exit 1;          ;;     esac;     curl -LfsSo /tmp/openjdk.tar.gz ${BINARY_URL};     echo "${ESUM} */tmp/openjdk.tar.gz" | sha256sum -c -;     mkdir -p /opt/java/openjdk;     cd /opt/java/openjdk;     tar -xf /tmp/openjdk.tar.gz --strip-components=1;     rm -rf /tmp/openjdk.tar.gz;
# Wed, 03 Aug 2022 02:19:26 GMT
ENV JAVA_HOME=/opt/java/openjdk PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 03 Aug 2022 02:19:26 GMT
RUN echo Verifying install ...     && echo javac --version && javac --version     && echo java --version && java --version     && echo Complete.
# Wed, 03 Aug 2022 02:19:26 GMT
CMD ["jshell"]
# Wed, 03 Aug 2022 03:14:04 GMT
CMD ["gradle"]
# Wed, 03 Aug 2022 03:14:04 GMT
ENV GRADLE_HOME=/opt/gradle
# Wed, 03 Aug 2022 03:14:04 GMT
RUN set -o errexit -o nounset     && echo "Adding gradle user and group"     && groupadd --system --gid 1000 gradle     && useradd --system --gid gradle --uid 1000 --shell /bin/bash --create-home gradle     && mkdir /home/gradle/.gradle     && chown --recursive gradle:gradle /home/gradle         && echo "Symlinking root Gradle cache to gradle Gradle cache"     && ln --symbolic /home/gradle/.gradle /root/.gradle
# Wed, 03 Aug 2022 03:14:05 GMT
VOLUME [/home/gradle/.gradle]
# Wed, 03 Aug 2022 03:14:05 GMT
WORKDIR /home/gradle
# Wed, 03 Aug 2022 03:14:37 GMT
RUN set -o errexit -o nounset     && apt-get update     && apt-get install --yes --no-install-recommends         unzip         wget                 bzr         git         git-lfs         mercurial         openssh-client         subversion     && rm --recursive --force /var/lib/apt/lists/*         && echo "Testing VCSes"     && which bzr     && which git     && which git-lfs     && which hg     && which svn
# Wed, 03 Aug 2022 03:14:42 GMT
ENV GRADLE_VERSION=7.5
# Wed, 03 Aug 2022 03:14:42 GMT
ARG GRADLE_DOWNLOAD_SHA256=cb87f222c5585bd46838ad4db78463a5c5f3d336e5e2b98dc7c0c586527351c2
# Wed, 03 Aug 2022 03:14:47 GMT
# ARGS: GRADLE_DOWNLOAD_SHA256=cb87f222c5585bd46838ad4db78463a5c5f3d336e5e2b98dc7c0c586527351c2
RUN set -o errexit -o nounset     && echo "Downloading Gradle"     && wget --no-verbose --output-document=gradle.zip "https://services.gradle.org/distributions/gradle-${GRADLE_VERSION}-bin.zip"         && echo "Checking download hash"     && echo "${GRADLE_DOWNLOAD_SHA256} *gradle.zip" | sha256sum --check -         && echo "Installing Gradle"     && unzip gradle.zip     && rm gradle.zip     && mv "gradle-${GRADLE_VERSION}" "${GRADLE_HOME}/"     && ln --symbolic "${GRADLE_HOME}/bin/gradle" /usr/bin/gradle         && echo "Testing Gradle installation"     && gradle --version
```

-	Layers:
	-	`sha256:d522b75fb69271e75617d2e7bbeede1210f48bffdc57121ee39534eea94e2815`  
		Last Modified: Tue, 02 Aug 2022 01:03:38 GMT  
		Size: 27.0 MB (27045363 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:79b48d17296789cbed49100fd665aec2330de5c27d57190835247afb1fa0799b`  
		Last Modified: Tue, 02 Aug 2022 12:54:34 GMT  
		Size: 19.2 MB (19224154 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c20fda1986f50637f712fe50c461310545001dfb1a1974bcbae5f0e7867c6c31`  
		Last Modified: Wed, 03 Aug 2022 02:22:15 GMT  
		Size: 181.5 MB (181504097 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5376c1759a9c6a0ebcdda364eaeb21b62ce3ba5c393fbe594c9c14384de53640`  
		Last Modified: Wed, 03 Aug 2022 02:22:03 GMT  
		Size: 160.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f52e5faa1d47f89efa9cc3bf684bbce0699eaddfc797babe92cfe4fa276ff03d`  
		Last Modified: Wed, 03 Aug 2022 03:19:36 GMT  
		Size: 4.4 KB (4363 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ba84c9b4ad8a3c9b99df42994649723f4733277bd74bc608c6c0892523219bfa`  
		Last Modified: Wed, 03 Aug 2022 03:19:46 GMT  
		Size: 64.8 MB (64837544 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:311ade88a383339bb1640254a9dd2fc07bb107f92a28ca1fb35e3d57007d9d8f`  
		Last Modified: Wed, 03 Aug 2022 03:19:42 GMT  
		Size: 120.7 MB (120655726 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
