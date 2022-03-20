## `gradle:jdk8`

```console
$ docker pull gradle@sha256:a26dd7882ebe964853db6317b1cb2be7af8a79e70ee0d776bb3504fabe43bc61
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 4
	-	linux; amd64
	-	linux; arm variant v7
	-	linux; arm64 variant v8
	-	linux; ppc64le

### `gradle:jdk8` - linux; amd64

```console
$ docker pull gradle@sha256:4afdec89bf5fe9494c2d8850a9e62b1c649a1f164cd747558264bd999eee7d55
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **329.7 MB (329748127 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e7a2845011ef86fb5c07fc3b1e3e220dcd7b3bb6a6e647f682402ba895cba88f`
-	Default Command: `["gradle"]`

```dockerfile
# Thu, 03 Mar 2022 20:19:33 GMT
ADD file:8a50ad78a668527e974b05a3dfbfd64760de3cb643ceb8a8805d21f6ceab3389 in / 
# Thu, 03 Mar 2022 20:19:33 GMT
CMD ["bash"]
# Thu, 03 Mar 2022 21:23:35 GMT
ENV LANG=en_US.UTF-8 LANGUAGE=en_US:en LC_ALL=en_US.UTF-8
# Thu, 03 Mar 2022 23:58:55 GMT
RUN apt-get update     && DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends tzdata curl ca-certificates fontconfig locales     && echo "en_US.UTF-8 UTF-8" >> /etc/locale.gen     && locale-gen en_US.UTF-8     && rm -rf /var/lib/apt/lists/*
# Mon, 07 Mar 2022 19:26:06 GMT
ENV JAVA_VERSION=jdk8u322-b06
# Mon, 07 Mar 2022 19:26:14 GMT
RUN set -eux;     ARCH="$(dpkg --print-architecture)";     case "${ARCH}" in        aarch64|arm64)          ESUM='42ed3ff5a859f9015a1362fb7e650026b913d688eab471714f795651120be173';          BINARY_URL='https://github.com/adoptium/temurin8-binaries/releases/download/jdk8u322-b06/OpenJDK8U-jdk_aarch64_linux_hotspot_8u322b06.tar.gz';          ;;        armhf|arm)          ESUM='0666c466b8aefcc66ab25aea9c0605f5c6eda3b174b1b817a4e4e74da0de0365';          BINARY_URL='https://github.com/adoptium/temurin8-binaries/releases/download/jdk8u322-b06/OpenJDK8U-jdk_arm_linux_hotspot_8u322b06.tar.gz';          apt-get update          && DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends libatomic1          && rm -rf /var/lib/apt/lists/*          ;;        ppc64el|powerpc:common64)          ESUM='c7cc9c5b237e9e1f1e3296593aba427375823592e4604fadf89a8c234c2574e1';          BINARY_URL='https://github.com/adoptium/temurin8-binaries/releases/download/jdk8u322-b06/OpenJDK8U-jdk_ppc64le_linux_hotspot_8u322b06.tar.gz';          ;;        amd64|i386:x86-64)          ESUM='3d62362a78c9412766471b05253507a4cfc212daea5cdf122860173ce902400e';          BINARY_URL='https://github.com/adoptium/temurin8-binaries/releases/download/jdk8u322-b06/OpenJDK8U-jdk_x64_linux_hotspot_8u322b06.tar.gz';          ;;        *)          echo "Unsupported arch: ${ARCH}";          exit 1;          ;;     esac;     curl -LfsSo /tmp/openjdk.tar.gz ${BINARY_URL};     echo "${ESUM} */tmp/openjdk.tar.gz" | sha256sum -c -;     mkdir -p /opt/java/openjdk;     cd /opt/java/openjdk;     tar -xf /tmp/openjdk.tar.gz --strip-components=1;     rm -rf /tmp/openjdk.tar.gz;
# Mon, 07 Mar 2022 19:26:14 GMT
ENV JAVA_HOME=/opt/java/openjdk PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Mon, 07 Mar 2022 19:26:15 GMT
RUN echo Verifying install ...     && echo javac -version && javac -version     && echo java -version && java -version     && echo Complete.
# Mon, 07 Mar 2022 19:53:27 GMT
CMD ["gradle"]
# Mon, 07 Mar 2022 19:53:27 GMT
ENV GRADLE_HOME=/opt/gradle
# Mon, 07 Mar 2022 19:53:28 GMT
RUN set -o errexit -o nounset     && echo "Adding gradle user and group"     && groupadd --system --gid 1000 gradle     && useradd --system --gid gradle --uid 1000 --shell /bin/bash --create-home gradle     && mkdir /home/gradle/.gradle     && chown --recursive gradle:gradle /home/gradle         && echo "Symlinking root Gradle cache to gradle Gradle cache"     && ln --symbolic /home/gradle/.gradle /root/.gradle
# Mon, 07 Mar 2022 19:53:28 GMT
VOLUME [/home/gradle/.gradle]
# Mon, 07 Mar 2022 19:53:28 GMT
WORKDIR /home/gradle
# Mon, 07 Mar 2022 19:54:04 GMT
RUN set -o errexit -o nounset     && apt-get update     && apt-get install --yes --no-install-recommends         unzip         wget                 bzr         git         git-lfs         mercurial         openssh-client         subversion     && rm --recursive --force /var/lib/apt/lists/*         && echo "Testing VCSes"     && which bzr     && which git     && which git-lfs     && which hg     && which svn
# Thu, 10 Mar 2022 18:19:39 GMT
ENV GRADLE_VERSION=7.4.1
# Thu, 10 Mar 2022 18:19:39 GMT
ARG GRADLE_DOWNLOAD_SHA256=e5444a57cda4a95f90b0c9446a9e1b47d3d7f69057765bfb54bd4f482542d548
# Thu, 10 Mar 2022 18:19:43 GMT
# ARGS: GRADLE_DOWNLOAD_SHA256=e5444a57cda4a95f90b0c9446a9e1b47d3d7f69057765bfb54bd4f482542d548
RUN set -o errexit -o nounset     && echo "Downloading Gradle"     && wget --no-verbose --output-document=gradle.zip "https://services.gradle.org/distributions/gradle-${GRADLE_VERSION}-bin.zip"         && echo "Checking download hash"     && echo "${GRADLE_DOWNLOAD_SHA256} *gradle.zip" | sha256sum --check -         && echo "Installing Gradle"     && unzip gradle.zip     && rm gradle.zip     && mv "gradle-${GRADLE_VERSION}" "${GRADLE_HOME}/"     && ln --symbolic "${GRADLE_HOME}/bin/gradle" /usr/bin/gradle         && echo "Testing Gradle installation"     && gradle --version
```

-	Layers:
	-	`sha256:7c3b88808835aa80f1ef7f03083c5ae781d0f44e644537cd72de4ce6c5e62e00`  
		Last Modified: Thu, 03 Mar 2022 20:20:44 GMT  
		Size: 28.6 MB (28565751 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8d66994d054da0091fad11fb497b2a23c0cfd350d897d78d57f78b3200b90fd6`  
		Last Modified: Fri, 04 Mar 2022 00:06:51 GMT  
		Size: 16.0 MB (16030868 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:55aac011d076c3e675482ec4760bbec59923e1e5eecd530063135e85de700798`  
		Last Modified: Mon, 07 Mar 2022 19:30:07 GMT  
		Size: 103.7 MB (103656365 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1b0c993e5c31ceb63e0849422a7ec8f63c02a0a38e8e9e3afc29985fcf7489d6`  
		Last Modified: Mon, 07 Mar 2022 19:29:57 GMT  
		Size: 162.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d2a1263d3f2dd8bbc4a6a6250099307a8aa6126e30b4e8c43b8c2020adfd076f`  
		Last Modified: Mon, 07 Mar 2022 19:56:57 GMT  
		Size: 4.4 KB (4359 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5273136416b1e28f7bf8144be33b1492937dc142bdacd813f75a536a57003af7`  
		Last Modified: Mon, 07 Mar 2022 19:57:08 GMT  
		Size: 65.6 MB (65625181 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e6bca66d51df29292a55cff8ed0be5986236aa12f58669fb84ac3bfeba1b4cee`  
		Last Modified: Thu, 10 Mar 2022 18:21:30 GMT  
		Size: 115.9 MB (115865441 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `gradle:jdk8` - linux; arm variant v7

```console
$ docker pull gradle@sha256:6d280547f7b1e6e0e42483f5faae25ca1812089ab1a1abec4f463041f8c5e79a
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **314.2 MB (314208291 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e8defe8a2bf9b7a2945abf34d52c1a7e209447b842ce4642cce46afdcca81f60`
-	Default Command: `["gradle"]`

```dockerfile
# Thu, 03 Mar 2022 21:21:31 GMT
ADD file:984d3d8b31abd025bb9be52f42d60245a76b1ee991f286db819ae204da45390c in / 
# Thu, 03 Mar 2022 21:21:32 GMT
CMD ["bash"]
# Fri, 04 Mar 2022 04:40:39 GMT
ENV LANG=en_US.UTF-8 LANGUAGE=en_US:en LC_ALL=en_US.UTF-8
# Mon, 07 Mar 2022 19:58:23 GMT
RUN apt-get update     && DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends tzdata curl ca-certificates fontconfig locales     && echo "en_US.UTF-8 UTF-8" >> /etc/locale.gen     && locale-gen en_US.UTF-8     && rm -rf /var/lib/apt/lists/*
# Mon, 07 Mar 2022 19:58:24 GMT
ENV JAVA_VERSION=jdk8u322-b06
# Mon, 07 Mar 2022 19:58:46 GMT
RUN set -eux;     ARCH="$(dpkg --print-architecture)";     case "${ARCH}" in        aarch64|arm64)          ESUM='42ed3ff5a859f9015a1362fb7e650026b913d688eab471714f795651120be173';          BINARY_URL='https://github.com/adoptium/temurin8-binaries/releases/download/jdk8u322-b06/OpenJDK8U-jdk_aarch64_linux_hotspot_8u322b06.tar.gz';          ;;        armhf|arm)          ESUM='0666c466b8aefcc66ab25aea9c0605f5c6eda3b174b1b817a4e4e74da0de0365';          BINARY_URL='https://github.com/adoptium/temurin8-binaries/releases/download/jdk8u322-b06/OpenJDK8U-jdk_arm_linux_hotspot_8u322b06.tar.gz';          apt-get update          && DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends libatomic1          && rm -rf /var/lib/apt/lists/*          ;;        ppc64el|powerpc:common64)          ESUM='c7cc9c5b237e9e1f1e3296593aba427375823592e4604fadf89a8c234c2574e1';          BINARY_URL='https://github.com/adoptium/temurin8-binaries/releases/download/jdk8u322-b06/OpenJDK8U-jdk_ppc64le_linux_hotspot_8u322b06.tar.gz';          ;;        amd64|i386:x86-64)          ESUM='3d62362a78c9412766471b05253507a4cfc212daea5cdf122860173ce902400e';          BINARY_URL='https://github.com/adoptium/temurin8-binaries/releases/download/jdk8u322-b06/OpenJDK8U-jdk_x64_linux_hotspot_8u322b06.tar.gz';          ;;        *)          echo "Unsupported arch: ${ARCH}";          exit 1;          ;;     esac;     curl -LfsSo /tmp/openjdk.tar.gz ${BINARY_URL};     echo "${ESUM} */tmp/openjdk.tar.gz" | sha256sum -c -;     mkdir -p /opt/java/openjdk;     cd /opt/java/openjdk;     tar -xf /tmp/openjdk.tar.gz --strip-components=1;     rm -rf /tmp/openjdk.tar.gz;
# Mon, 07 Mar 2022 19:58:47 GMT
ENV JAVA_HOME=/opt/java/openjdk PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Mon, 07 Mar 2022 19:58:49 GMT
RUN echo Verifying install ...     && echo javac -version && javac -version     && echo java -version && java -version     && echo Complete.
# Mon, 07 Mar 2022 21:54:42 GMT
CMD ["gradle"]
# Mon, 07 Mar 2022 21:54:43 GMT
ENV GRADLE_HOME=/opt/gradle
# Mon, 07 Mar 2022 21:54:45 GMT
RUN set -o errexit -o nounset     && echo "Adding gradle user and group"     && groupadd --system --gid 1000 gradle     && useradd --system --gid gradle --uid 1000 --shell /bin/bash --create-home gradle     && mkdir /home/gradle/.gradle     && chown --recursive gradle:gradle /home/gradle         && echo "Symlinking root Gradle cache to gradle Gradle cache"     && ln --symbolic /home/gradle/.gradle /root/.gradle
# Mon, 07 Mar 2022 21:54:45 GMT
VOLUME [/home/gradle/.gradle]
# Mon, 07 Mar 2022 21:54:45 GMT
WORKDIR /home/gradle
# Mon, 07 Mar 2022 21:55:36 GMT
RUN set -o errexit -o nounset     && apt-get update     && apt-get install --yes --no-install-recommends         unzip         wget                 bzr         git         git-lfs         mercurial         openssh-client         subversion     && rm --recursive --force /var/lib/apt/lists/*         && echo "Testing VCSes"     && which bzr     && which git     && which git-lfs     && which hg     && which svn
# Thu, 10 Mar 2022 19:42:31 GMT
ENV GRADLE_VERSION=7.4.1
# Thu, 10 Mar 2022 19:42:32 GMT
ARG GRADLE_DOWNLOAD_SHA256=e5444a57cda4a95f90b0c9446a9e1b47d3d7f69057765bfb54bd4f482542d548
# Thu, 10 Mar 2022 19:42:44 GMT
# ARGS: GRADLE_DOWNLOAD_SHA256=e5444a57cda4a95f90b0c9446a9e1b47d3d7f69057765bfb54bd4f482542d548
RUN set -o errexit -o nounset     && echo "Downloading Gradle"     && wget --no-verbose --output-document=gradle.zip "https://services.gradle.org/distributions/gradle-${GRADLE_VERSION}-bin.zip"         && echo "Checking download hash"     && echo "${GRADLE_DOWNLOAD_SHA256} *gradle.zip" | sha256sum --check -         && echo "Installing Gradle"     && unzip gradle.zip     && rm gradle.zip     && mv "gradle-${GRADLE_VERSION}" "${GRADLE_HOME}/"     && ln --symbolic "${GRADLE_HOME}/bin/gradle" /usr/bin/gradle         && echo "Testing Gradle installation"     && gradle --version
```

-	Layers:
	-	`sha256:12a77aaceb8aa1438ebb61cb4904d74fc225cfa20464a060980580674a0a31e9`  
		Last Modified: Thu, 03 Mar 2022 21:25:09 GMT  
		Size: 24.1 MB (24073718 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a3aaac75a0138a59e98810b993ebce72dbe24ae9f2b9ef694f4b9d0f7f2a63d1`  
		Last Modified: Mon, 07 Mar 2022 20:05:47 GMT  
		Size: 14.9 MB (14902332 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:26da233459ab6def22dae2a016690a4ea6d3c189ffb523fe21fb04365b7ad5df`  
		Last Modified: Mon, 07 Mar 2022 20:06:19 GMT  
		Size: 99.3 MB (99329244 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7ec7735019cc42927741d9ab56f4d70a7fd1f618de493a59bdd1434e5cccca4f`  
		Last Modified: Mon, 07 Mar 2022 20:05:37 GMT  
		Size: 160.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c74b9680f6cdfcff9d13756b9b1679627e8fac55517e03e8de06339807760c14`  
		Last Modified: Mon, 07 Mar 2022 22:02:44 GMT  
		Size: 4.3 KB (4347 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e8db927c51099e5593aa9ccab3fec7de771a03dc022e7f85a30f09a9e61dc190`  
		Last Modified: Mon, 07 Mar 2022 22:03:28 GMT  
		Size: 60.0 MB (60033134 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5cc73e07c30fc07b48fd2b5a2a00e466f89f029b35b54a1fa3e6840c6e7b52e6`  
		Last Modified: Thu, 10 Mar 2022 19:47:33 GMT  
		Size: 115.9 MB (115865356 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `gradle:jdk8` - linux; arm64 variant v8

```console
$ docker pull gradle@sha256:f469e6102c3b357cb91e06d78418ba976a4b6bd408bfc9e612d1891e300dd1db
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **327.0 MB (327018440 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b81eeaa0cbcb2bdcb0b91b0a5a3c8194adb5e2f1052789a4ceca413ea7c16947`
-	Default Command: `["gradle"]`

```dockerfile
# Fri, 18 Mar 2022 00:40:52 GMT
ADD file:39550cc6d55fc19ba68f94e7b3a21c3206bbd13264f26cf0a32ddd5ed0ad2782 in / 
# Fri, 18 Mar 2022 00:40:53 GMT
CMD ["bash"]
# Sat, 19 Mar 2022 15:28:12 GMT
ENV LANG=en_US.UTF-8 LANGUAGE=en_US:en LC_ALL=en_US.UTF-8
# Sat, 19 Mar 2022 15:28:31 GMT
RUN apt-get update     && DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends tzdata curl ca-certificates fontconfig locales     && echo "en_US.UTF-8 UTF-8" >> /etc/locale.gen     && locale-gen en_US.UTF-8     && rm -rf /var/lib/apt/lists/*
# Sat, 19 Mar 2022 15:28:31 GMT
ENV JAVA_VERSION=jdk8u322-b06
# Sat, 19 Mar 2022 15:28:39 GMT
RUN set -eux;     ARCH="$(dpkg --print-architecture)";     case "${ARCH}" in        aarch64|arm64)          ESUM='42ed3ff5a859f9015a1362fb7e650026b913d688eab471714f795651120be173';          BINARY_URL='https://github.com/adoptium/temurin8-binaries/releases/download/jdk8u322-b06/OpenJDK8U-jdk_aarch64_linux_hotspot_8u322b06.tar.gz';          ;;        armhf|arm)          ESUM='0666c466b8aefcc66ab25aea9c0605f5c6eda3b174b1b817a4e4e74da0de0365';          BINARY_URL='https://github.com/adoptium/temurin8-binaries/releases/download/jdk8u322-b06/OpenJDK8U-jdk_arm_linux_hotspot_8u322b06.tar.gz';          apt-get update          && DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends libatomic1          && rm -rf /var/lib/apt/lists/*          ;;        ppc64el|powerpc:common64)          ESUM='c7cc9c5b237e9e1f1e3296593aba427375823592e4604fadf89a8c234c2574e1';          BINARY_URL='https://github.com/adoptium/temurin8-binaries/releases/download/jdk8u322-b06/OpenJDK8U-jdk_ppc64le_linux_hotspot_8u322b06.tar.gz';          ;;        amd64|i386:x86-64)          ESUM='3d62362a78c9412766471b05253507a4cfc212daea5cdf122860173ce902400e';          BINARY_URL='https://github.com/adoptium/temurin8-binaries/releases/download/jdk8u322-b06/OpenJDK8U-jdk_x64_linux_hotspot_8u322b06.tar.gz';          ;;        *)          echo "Unsupported arch: ${ARCH}";          exit 1;          ;;     esac;     curl -LfsSo /tmp/openjdk.tar.gz ${BINARY_URL};     echo "${ESUM} */tmp/openjdk.tar.gz" | sha256sum -c -;     mkdir -p /opt/java/openjdk;     cd /opt/java/openjdk;     tar -xf /tmp/openjdk.tar.gz --strip-components=1;     rm -rf /tmp/openjdk.tar.gz;
# Sat, 19 Mar 2022 15:28:39 GMT
ENV JAVA_HOME=/opt/java/openjdk PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Sat, 19 Mar 2022 15:28:41 GMT
RUN echo Verifying install ...     && echo javac -version && javac -version     && echo java -version && java -version     && echo Complete.
# Sun, 20 Mar 2022 00:28:09 GMT
CMD ["gradle"]
# Sun, 20 Mar 2022 00:28:10 GMT
ENV GRADLE_HOME=/opt/gradle
# Sun, 20 Mar 2022 00:28:11 GMT
RUN set -o errexit -o nounset     && echo "Adding gradle user and group"     && groupadd --system --gid 1000 gradle     && useradd --system --gid gradle --uid 1000 --shell /bin/bash --create-home gradle     && mkdir /home/gradle/.gradle     && chown --recursive gradle:gradle /home/gradle         && echo "Symlinking root Gradle cache to gradle Gradle cache"     && ln --symbolic /home/gradle/.gradle /root/.gradle
# Sun, 20 Mar 2022 00:28:12 GMT
VOLUME [/home/gradle/.gradle]
# Sun, 20 Mar 2022 00:28:13 GMT
WORKDIR /home/gradle
# Sun, 20 Mar 2022 00:28:37 GMT
RUN set -o errexit -o nounset     && apt-get update     && apt-get install --yes --no-install-recommends         unzip         wget                 bzr         git         git-lfs         mercurial         openssh-client         subversion     && rm --recursive --force /var/lib/apt/lists/*         && echo "Testing VCSes"     && which bzr     && which git     && which git-lfs     && which hg     && which svn
# Sun, 20 Mar 2022 00:28:38 GMT
ENV GRADLE_VERSION=7.4.1
# Sun, 20 Mar 2022 00:28:38 GMT
ARG GRADLE_DOWNLOAD_SHA256=e5444a57cda4a95f90b0c9446a9e1b47d3d7f69057765bfb54bd4f482542d548
# Sun, 20 Mar 2022 00:28:43 GMT
# ARGS: GRADLE_DOWNLOAD_SHA256=e5444a57cda4a95f90b0c9446a9e1b47d3d7f69057765bfb54bd4f482542d548
RUN set -o errexit -o nounset     && echo "Downloading Gradle"     && wget --no-verbose --output-document=gradle.zip "https://services.gradle.org/distributions/gradle-${GRADLE_VERSION}-bin.zip"         && echo "Checking download hash"     && echo "${GRADLE_DOWNLOAD_SHA256} *gradle.zip" | sha256sum --check -         && echo "Installing Gradle"     && unzip gradle.zip     && rm gradle.zip     && mv "gradle-${GRADLE_VERSION}" "${GRADLE_HOME}/"     && ln --symbolic "${GRADLE_HOME}/bin/gradle" /usr/bin/gradle         && echo "Testing Gradle installation"     && gradle --version
```

-	Layers:
	-	`sha256:57d0418fe9dcc5262d8c4fcb06c852ad2d0407b541c64d0f5f2e6ec01fd411ba`  
		Last Modified: Fri, 18 Mar 2022 00:42:36 GMT  
		Size: 27.2 MB (27169617 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c236902da3463f4b33e5af2f3ff655994cbe47d5e8380294ee6d6a5957b77710`  
		Last Modified: Sat, 19 Mar 2022 15:32:57 GMT  
		Size: 15.9 MB (15897447 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d39d96fe6e260252d5646351de5271418f1d59ae7ba31a009db409bcf331416a`  
		Last Modified: Sat, 19 Mar 2022 15:33:09 GMT  
		Size: 102.7 MB (102746633 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:acb0b74e322b62e8d2b9db9a78da36b4d6992649b69bd01a35489375858a9572`  
		Last Modified: Sat, 19 Mar 2022 15:32:54 GMT  
		Size: 127.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:114e57f4f08cfefbb892abe5fe498730aeef83b17b018b7d4f37487b021e41fb`  
		Last Modified: Sun, 20 Mar 2022 00:32:03 GMT  
		Size: 4.3 KB (4311 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:eb68f543b42680dceaf0f10664b6e9645296038d739811491618f386cc828521`  
		Last Modified: Sun, 20 Mar 2022 00:32:14 GMT  
		Size: 65.3 MB (65334944 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f776c2a85951e784edb9b83fa7675c05495c99eabe3422beaa3ffa4640377d93`  
		Last Modified: Sun, 20 Mar 2022 00:32:14 GMT  
		Size: 115.9 MB (115865361 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `gradle:jdk8` - linux; ppc64le

```console
$ docker pull gradle@sha256:cb1a52abce47b58eed841b99946cdb2b48146bf897ce43af2ce38682792a804e
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **341.5 MB (341515102 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b177ee249176e014884e925567adf82e356e5a55235cf04f7976b21ef82c67e2`
-	Default Command: `["gradle"]`

```dockerfile
# Thu, 03 Mar 2022 20:28:30 GMT
ADD file:039f04ac6c5dbbe3fb0a5eee16945cf7c5fb7565751d6bdf8ec0c1102798c1de in / 
# Thu, 03 Mar 2022 20:28:38 GMT
CMD ["bash"]
# Thu, 03 Mar 2022 22:04:54 GMT
ENV LANG=en_US.UTF-8 LANGUAGE=en_US:en LC_ALL=en_US.UTF-8
# Thu, 03 Mar 2022 23:22:19 GMT
RUN apt-get update     && DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends tzdata curl ca-certificates fontconfig locales     && echo "en_US.UTF-8 UTF-8" >> /etc/locale.gen     && locale-gen en_US.UTF-8     && rm -rf /var/lib/apt/lists/*
# Mon, 07 Mar 2022 19:24:33 GMT
ENV JAVA_VERSION=jdk8u322-b06
# Mon, 07 Mar 2022 19:24:59 GMT
RUN set -eux;     ARCH="$(dpkg --print-architecture)";     case "${ARCH}" in        aarch64|arm64)          ESUM='42ed3ff5a859f9015a1362fb7e650026b913d688eab471714f795651120be173';          BINARY_URL='https://github.com/adoptium/temurin8-binaries/releases/download/jdk8u322-b06/OpenJDK8U-jdk_aarch64_linux_hotspot_8u322b06.tar.gz';          ;;        armhf|arm)          ESUM='0666c466b8aefcc66ab25aea9c0605f5c6eda3b174b1b817a4e4e74da0de0365';          BINARY_URL='https://github.com/adoptium/temurin8-binaries/releases/download/jdk8u322-b06/OpenJDK8U-jdk_arm_linux_hotspot_8u322b06.tar.gz';          apt-get update          && DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends libatomic1          && rm -rf /var/lib/apt/lists/*          ;;        ppc64el|powerpc:common64)          ESUM='c7cc9c5b237e9e1f1e3296593aba427375823592e4604fadf89a8c234c2574e1';          BINARY_URL='https://github.com/adoptium/temurin8-binaries/releases/download/jdk8u322-b06/OpenJDK8U-jdk_ppc64le_linux_hotspot_8u322b06.tar.gz';          ;;        amd64|i386:x86-64)          ESUM='3d62362a78c9412766471b05253507a4cfc212daea5cdf122860173ce902400e';          BINARY_URL='https://github.com/adoptium/temurin8-binaries/releases/download/jdk8u322-b06/OpenJDK8U-jdk_x64_linux_hotspot_8u322b06.tar.gz';          ;;        *)          echo "Unsupported arch: ${ARCH}";          exit 1;          ;;     esac;     curl -LfsSo /tmp/openjdk.tar.gz ${BINARY_URL};     echo "${ESUM} */tmp/openjdk.tar.gz" | sha256sum -c -;     mkdir -p /opt/java/openjdk;     cd /opt/java/openjdk;     tar -xf /tmp/openjdk.tar.gz --strip-components=1;     rm -rf /tmp/openjdk.tar.gz;
# Mon, 07 Mar 2022 19:25:07 GMT
ENV JAVA_HOME=/opt/java/openjdk PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Mon, 07 Mar 2022 19:25:19 GMT
RUN echo Verifying install ...     && echo javac -version && javac -version     && echo java -version && java -version     && echo Complete.
# Mon, 07 Mar 2022 19:56:12 GMT
CMD ["gradle"]
# Mon, 07 Mar 2022 19:56:16 GMT
ENV GRADLE_HOME=/opt/gradle
# Mon, 07 Mar 2022 19:56:23 GMT
RUN set -o errexit -o nounset     && echo "Adding gradle user and group"     && groupadd --system --gid 1000 gradle     && useradd --system --gid gradle --uid 1000 --shell /bin/bash --create-home gradle     && mkdir /home/gradle/.gradle     && chown --recursive gradle:gradle /home/gradle         && echo "Symlinking root Gradle cache to gradle Gradle cache"     && ln --symbolic /home/gradle/.gradle /root/.gradle
# Mon, 07 Mar 2022 19:56:25 GMT
VOLUME [/home/gradle/.gradle]
# Mon, 07 Mar 2022 19:56:28 GMT
WORKDIR /home/gradle
# Mon, 07 Mar 2022 19:58:41 GMT
RUN set -o errexit -o nounset     && apt-get update     && apt-get install --yes --no-install-recommends         unzip         wget                 bzr         git         git-lfs         mercurial         openssh-client         subversion     && rm --recursive --force /var/lib/apt/lists/*         && echo "Testing VCSes"     && which bzr     && which git     && which git-lfs     && which hg     && which svn
# Thu, 10 Mar 2022 18:16:47 GMT
ENV GRADLE_VERSION=7.4.1
# Thu, 10 Mar 2022 18:16:51 GMT
ARG GRADLE_DOWNLOAD_SHA256=e5444a57cda4a95f90b0c9446a9e1b47d3d7f69057765bfb54bd4f482542d548
# Thu, 10 Mar 2022 18:17:27 GMT
# ARGS: GRADLE_DOWNLOAD_SHA256=e5444a57cda4a95f90b0c9446a9e1b47d3d7f69057765bfb54bd4f482542d548
RUN set -o errexit -o nounset     && echo "Downloading Gradle"     && wget --no-verbose --output-document=gradle.zip "https://services.gradle.org/distributions/gradle-${GRADLE_VERSION}-bin.zip"         && echo "Checking download hash"     && echo "${GRADLE_DOWNLOAD_SHA256} *gradle.zip" | sha256sum --check -         && echo "Installing Gradle"     && unzip gradle.zip     && rm gradle.zip     && mv "gradle-${GRADLE_VERSION}" "${GRADLE_HOME}/"     && ln --symbolic "${GRADLE_HOME}/bin/gradle" /usr/bin/gradle         && echo "Testing Gradle installation"     && gradle --version
```

-	Layers:
	-	`sha256:a16b43de69d1e799ea2cb675e7e605db0ff3a8d692fd326fbde80a370e0676d5`  
		Last Modified: Thu, 03 Mar 2022 20:33:55 GMT  
		Size: 33.3 MB (33292195 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0daad88923e3aab34fc02032aaddf77f4caa3bd81fe7df9b280ef3fbd2796e10`  
		Last Modified: Thu, 03 Mar 2022 23:36:10 GMT  
		Size: 17.2 MB (17205102 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:72ad16679b810e4a3ef373d8c3be772cf312ca947fad3203750c66e1bc16b788`  
		Last Modified: Mon, 07 Mar 2022 19:36:39 GMT  
		Size: 101.1 MB (101145809 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8cd81dd04415db6772c228ccef9d14a8deace7bf73cb9ef4ddcecf4c619cecd5`  
		Last Modified: Mon, 07 Mar 2022 19:36:24 GMT  
		Size: 161.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bdb4fd90200e77e80e7210af4a2441fe77fb09645f293e7487cea3ef3d063074`  
		Last Modified: Mon, 07 Mar 2022 20:11:16 GMT  
		Size: 4.4 KB (4372 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:56726572e333fccd639e24e38dc7a5b3c7e53620d54b4ef849cc052b8522209c`  
		Last Modified: Mon, 07 Mar 2022 20:11:31 GMT  
		Size: 74.0 MB (74002037 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:12383064d9056cc7f94ef8ed3be700e4842883367a82bc970b59d2a89800cb8e`  
		Last Modified: Thu, 10 Mar 2022 18:21:17 GMT  
		Size: 115.9 MB (115865426 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
