## `gradle:jdk8-jammy`

```console
$ docker pull gradle@sha256:9f18d14fafbdec7d915b9020e1b7e0f4aafb43255f242b9e52c407bb284f1fdc
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 4
	-	linux; amd64
	-	linux; arm variant v7
	-	linux; arm64 variant v8
	-	linux; ppc64le

### `gradle:jdk8-jammy` - linux; amd64

```console
$ docker pull gradle@sha256:3a99d198d6bd048734179e936a88f165a9454ed94989ca2806de9bea577e5823
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **318.3 MB (318307604 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:82c4751e1121d8260d591ebfeaab5df67c3f479cc745312d593d04367d8df197`
-	Default Command: `["gradle"]`

```dockerfile
# Tue, 02 Aug 2022 01:30:55 GMT
ADD file:396eeb65c8d737180cc1219713cf59efb214027b79d8ea0b7e58a08e7c8d7a21 in / 
# Tue, 02 Aug 2022 01:30:56 GMT
CMD ["bash"]
# Tue, 02 Aug 2022 19:05:11 GMT
ENV LANG=en_US.UTF-8 LANGUAGE=en_US:en LC_ALL=en_US.UTF-8
# Tue, 02 Aug 2022 19:06:14 GMT
RUN apt-get update     && DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends tzdata curl ca-certificates fontconfig locales     && echo "en_US.UTF-8 UTF-8" >> /etc/locale.gen     && locale-gen en_US.UTF-8     && rm -rf /var/lib/apt/lists/*
# Tue, 02 Aug 2022 19:06:14 GMT
ENV JAVA_VERSION=jdk8u342-b07
# Tue, 02 Aug 2022 19:06:20 GMT
RUN set -eux;     ARCH="$(dpkg --print-architecture)";     case "${ARCH}" in        aarch64|arm64)          ESUM='ebac40a9a126d1c5333106f9428c9a1d32593ad90b032c1cc147975fa554dfb7';          BINARY_URL='https://github.com/adoptium/temurin8-binaries/releases/download/jdk8u342-b07/OpenJDK8U-jdk_aarch64_linux_hotspot_8u342b07.tar.gz';          ;;        armhf|arm)          ESUM='a12987778eb1455ff5145ae4eda11025e21477c10b0c45e0db8ba96bf9ef20f1';          BINARY_URL='https://github.com/adoptium/temurin8-binaries/releases/download/jdk8u342-b07/OpenJDK8U-jdk_arm_linux_hotspot_8u342b07.tar.gz';          apt-get update          && DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends libatomic1          && rm -rf /var/lib/apt/lists/*          ;;        ppc64el|powerpc:common64)          ESUM='bc943c3e6bc1232ea4e7dd114831b609d83a79f271907941a18f1d7206f741b2';          BINARY_URL='https://github.com/adoptium/temurin8-binaries/releases/download/jdk8u342-b07/OpenJDK8U-jdk_ppc64le_linux_hotspot_8u342b07.tar.gz';          ;;        amd64|i386:x86-64)          ESUM='8252c0e11d542ea0f9ce6b8f147d1a2bea4a17e9fc299da270288f5a4f35b1f3';          BINARY_URL='https://github.com/adoptium/temurin8-binaries/releases/download/jdk8u342-b07/OpenJDK8U-jdk_x64_linux_hotspot_8u342b07.tar.gz';          ;;        *)          echo "Unsupported arch: ${ARCH}";          exit 1;          ;;     esac;     curl -LfsSo /tmp/openjdk.tar.gz ${BINARY_URL};     echo "${ESUM} */tmp/openjdk.tar.gz" | sha256sum -c -;     mkdir -p /opt/java/openjdk;     cd /opt/java/openjdk;     tar -xf /tmp/openjdk.tar.gz --strip-components=1;     rm -rf /tmp/openjdk.tar.gz;
# Tue, 02 Aug 2022 19:06:20 GMT
ENV JAVA_HOME=/opt/java/openjdk PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 02 Aug 2022 19:06:21 GMT
RUN echo Verifying install ...     && echo javac -version && javac -version     && echo java -version && java -version     && echo Complete.
# Wed, 03 Aug 2022 12:31:53 GMT
CMD ["gradle"]
# Wed, 03 Aug 2022 12:31:53 GMT
ENV GRADLE_HOME=/opt/gradle
# Wed, 03 Aug 2022 12:31:54 GMT
RUN set -o errexit -o nounset     && echo "Adding gradle user and group"     && groupadd --system --gid 1000 gradle     && useradd --system --gid gradle --uid 1000 --shell /bin/bash --create-home gradle     && mkdir /home/gradle/.gradle     && chown --recursive gradle:gradle /home/gradle         && echo "Symlinking root Gradle cache to gradle Gradle cache"     && ln --symbolic /home/gradle/.gradle /root/.gradle
# Wed, 03 Aug 2022 12:31:54 GMT
VOLUME [/home/gradle/.gradle]
# Wed, 03 Aug 2022 12:31:54 GMT
WORKDIR /home/gradle
# Wed, 03 Aug 2022 12:32:20 GMT
RUN set -o errexit -o nounset     && apt-get update     && apt-get install --yes --no-install-recommends         unzip         wget                 bzr         git         git-lfs         mercurial         openssh-client         subversion     && rm --recursive --force /var/lib/apt/lists/*         && echo "Testing VCSes"     && which bzr     && which git     && which git-lfs     && which hg     && which svn
# Wed, 03 Aug 2022 12:32:21 GMT
ENV GRADLE_VERSION=7.5
# Wed, 03 Aug 2022 12:32:21 GMT
ARG GRADLE_DOWNLOAD_SHA256=cb87f222c5585bd46838ad4db78463a5c5f3d336e5e2b98dc7c0c586527351c2
# Wed, 03 Aug 2022 12:32:26 GMT
# ARGS: GRADLE_DOWNLOAD_SHA256=cb87f222c5585bd46838ad4db78463a5c5f3d336e5e2b98dc7c0c586527351c2
RUN set -o errexit -o nounset     && echo "Downloading Gradle"     && wget --no-verbose --output-document=gradle.zip "https://services.gradle.org/distributions/gradle-${GRADLE_VERSION}-bin.zip"         && echo "Checking download hash"     && echo "${GRADLE_DOWNLOAD_SHA256} *gradle.zip" | sha256sum --check -         && echo "Installing Gradle"     && unzip gradle.zip     && rm gradle.zip     && mv "gradle-${GRADLE_VERSION}" "${GRADLE_HOME}/"     && ln --symbolic "${GRADLE_HOME}/bin/gradle" /usr/bin/gradle         && echo "Testing Gradle installation"     && gradle --version
```

-	Layers:
	-	`sha256:d19f32bd9e4106d487f1a703fc2f09c8edadd92db4405d477978e8e466ab290d`  
		Last Modified: Tue, 02 Aug 2022 01:32:15 GMT  
		Size: 30.4 MB (30426136 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:73d22c5dd126cf034b1cdacf9e5f6385608a4e026b4cb566a13dd165987a6d23`  
		Last Modified: Tue, 02 Aug 2022 19:13:40 GMT  
		Size: 12.1 MB (12117331 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5964ea20ac30ed02c9e86ac9b6251427121c74334e9f9a423602a73ebf799912`  
		Last Modified: Tue, 02 Aug 2022 19:13:48 GMT  
		Size: 103.5 MB (103515334 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:aced7aa08b023e096fc7eb79454ca1887a5319f992b247ac1ad5f76433272a9d`  
		Last Modified: Tue, 02 Aug 2022 19:13:38 GMT  
		Size: 160.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:15adfeaf132274618dd75b7b09d8e1a68194aca4223ef4b685cf1bc0d5e5b4e6`  
		Last Modified: Wed, 03 Aug 2022 12:39:35 GMT  
		Size: 4.4 KB (4364 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:abd5122494efad63c0963a0c813881713b2d61a28b34b4100e477daf9154295d`  
		Last Modified: Wed, 03 Aug 2022 12:39:44 GMT  
		Size: 51.6 MB (51588531 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2242c95e7935dc52c98cfc0cab5ad435428752e58b3fb8c428c528e4fd2ecd59`  
		Last Modified: Wed, 03 Aug 2022 12:39:41 GMT  
		Size: 120.7 MB (120655748 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `gradle:jdk8-jammy` - linux; arm variant v7

```console
$ docker pull gradle@sha256:584a7ff188871234249f8014c1ed6029db17a2a12e0a4cec35a3a646e834bbbe
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **312.1 MB (312145460 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:4276c1ee1f1550b96c8ec4d01ee31e2f1cdecf1a35d7e9e1d946769755f6f2e5`
-	Default Command: `["gradle"]`

```dockerfile
# Tue, 07 Jun 2022 05:51:35 GMT
ADD file:26c86cfcbc153addbca421974e648a7af07234cb3f741bfb030aa0db90b6a7c6 in / 
# Tue, 07 Jun 2022 05:51:36 GMT
CMD ["bash"]
# Sat, 30 Jul 2022 02:49:53 GMT
ENV LANG=en_US.UTF-8 LANGUAGE=en_US:en LC_ALL=en_US.UTF-8
# Sat, 30 Jul 2022 02:50:09 GMT
RUN apt-get update     && DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends tzdata curl ca-certificates fontconfig locales     && echo "en_US.UTF-8 UTF-8" >> /etc/locale.gen     && locale-gen en_US.UTF-8     && rm -rf /var/lib/apt/lists/*
# Sat, 30 Jul 2022 02:50:09 GMT
ENV JAVA_VERSION=jdk8u332-b09
# Sat, 30 Jul 2022 02:50:22 GMT
RUN set -eux;     ARCH="$(dpkg --print-architecture)";     case "${ARCH}" in        aarch64|arm64)          ESUM='d10efb2afad3ed3d7bac9d3249cea77928aca6acb973cac0f90a2dd3606a3533';          BINARY_URL='https://github.com/adoptium/temurin8-binaries/releases/download/jdk8u332-b09/OpenJDK8U-jdk_aarch64_linux_hotspot_8u332b09.tar.gz';          ;;        armhf|arm)          ESUM='c914250a736e620c12f9fe65fcd94ffa1acdacc5323e5aaff611a33a37cd158f';          BINARY_URL='https://github.com/adoptium/temurin8-binaries/releases/download/jdk8u332-b09/OpenJDK8U-jdk_arm_linux_hotspot_8u332b09.tar.gz';          apt-get update          && DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends libatomic1          && rm -rf /var/lib/apt/lists/*          ;;        ppc64el|powerpc:common64)          ESUM='1df8c12fd97e76c388d64e4df16893f4285e000e6ff837d1e39969e5428aafa0';          BINARY_URL='https://github.com/adoptium/temurin8-binaries/releases/download/jdk8u332-b09/OpenJDK8U-jdk_ppc64le_linux_hotspot_8u332b09.tar.gz';          ;;        amd64|i386:x86-64)          ESUM='adc13a0a0540d77f0a3481b48f10d61eb203e5ad4914507d489c2de3bd3d83da';          BINARY_URL='https://github.com/adoptium/temurin8-binaries/releases/download/jdk8u332-b09/OpenJDK8U-jdk_x64_linux_hotspot_8u332b09.tar.gz';          ;;        *)          echo "Unsupported arch: ${ARCH}";          exit 1;          ;;     esac;     curl -LfsSo /tmp/openjdk.tar.gz ${BINARY_URL};     echo "${ESUM} */tmp/openjdk.tar.gz" | sha256sum -c -;     mkdir -p /opt/java/openjdk;     cd /opt/java/openjdk;     tar -xf /tmp/openjdk.tar.gz --strip-components=1;     rm -rf /tmp/openjdk.tar.gz;
# Sat, 30 Jul 2022 02:50:22 GMT
ENV JAVA_HOME=/opt/java/openjdk PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Sat, 30 Jul 2022 02:50:23 GMT
RUN echo Verifying install ...     && echo javac -version && javac -version     && echo java -version && java -version     && echo Complete.
# Sat, 30 Jul 2022 12:21:02 GMT
CMD ["gradle"]
# Sat, 30 Jul 2022 12:21:02 GMT
ENV GRADLE_HOME=/opt/gradle
# Sat, 30 Jul 2022 12:21:03 GMT
RUN set -o errexit -o nounset     && echo "Adding gradle user and group"     && groupadd --system --gid 1000 gradle     && useradd --system --gid gradle --uid 1000 --shell /bin/bash --create-home gradle     && mkdir /home/gradle/.gradle     && chown --recursive gradle:gradle /home/gradle         && echo "Symlinking root Gradle cache to gradle Gradle cache"     && ln --symbolic /home/gradle/.gradle /root/.gradle
# Sat, 30 Jul 2022 12:21:03 GMT
VOLUME [/home/gradle/.gradle]
# Sat, 30 Jul 2022 12:21:03 GMT
WORKDIR /home/gradle
# Sat, 30 Jul 2022 12:21:25 GMT
RUN set -o errexit -o nounset     && apt-get update     && apt-get install --yes --no-install-recommends         unzip         wget                 bzr         git         git-lfs         mercurial         openssh-client         subversion     && rm --recursive --force /var/lib/apt/lists/*         && echo "Testing VCSes"     && which bzr     && which git     && which git-lfs     && which hg     && which svn
# Sat, 30 Jul 2022 12:21:26 GMT
ENV GRADLE_VERSION=7.5
# Sat, 30 Jul 2022 12:21:26 GMT
ARG GRADLE_DOWNLOAD_SHA256=cb87f222c5585bd46838ad4db78463a5c5f3d336e5e2b98dc7c0c586527351c2
# Sat, 30 Jul 2022 12:21:31 GMT
# ARGS: GRADLE_DOWNLOAD_SHA256=cb87f222c5585bd46838ad4db78463a5c5f3d336e5e2b98dc7c0c586527351c2
RUN set -o errexit -o nounset     && echo "Downloading Gradle"     && wget --no-verbose --output-document=gradle.zip "https://services.gradle.org/distributions/gradle-${GRADLE_VERSION}-bin.zip"         && echo "Checking download hash"     && echo "${GRADLE_DOWNLOAD_SHA256} *gradle.zip" | sha256sum --check -         && echo "Installing Gradle"     && unzip gradle.zip     && rm gradle.zip     && mv "gradle-${GRADLE_VERSION}" "${GRADLE_HOME}/"     && ln --symbolic "${GRADLE_HOME}/bin/gradle" /usr/bin/gradle         && echo "Testing Gradle installation"     && gradle --version
```

-	Layers:
	-	`sha256:5aeb313108e16ff98084efb2ae2830cbe915ea38b3e2fd1e32688dd9d8c11320`  
		Last Modified: Tue, 07 Jun 2022 05:56:03 GMT  
		Size: 27.0 MB (27017432 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d19fdce069a7dff1a637320e689a92f499bee9dae5c6492ede30168a6194ccd3`  
		Last Modified: Sat, 30 Jul 2022 02:57:14 GMT  
		Size: 11.7 MB (11712882 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:adf1e8743dc739a219121c8822bb067fc19049993e3e069f668ddfd472ea49b9`  
		Last Modified: Sat, 30 Jul 2022 02:57:21 GMT  
		Size: 99.2 MB (99168418 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:46c2957f0c39e18e932340c6a3108b2cd5990ba717659c18576e069caaebe48e`  
		Last Modified: Sat, 30 Jul 2022 02:57:11 GMT  
		Size: 160.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:da9fee596672bd06abda8b85a3c4f0f1e691265dc6952bfd8594cd179c31104a`  
		Last Modified: Sat, 30 Jul 2022 12:32:05 GMT  
		Size: 4.3 KB (4350 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:520f91b91274cf3005a204b78a7a302eaa86e83b9cebe4bb4dade734ffd0b705`  
		Last Modified: Sat, 30 Jul 2022 12:32:18 GMT  
		Size: 53.6 MB (53586468 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:38f1df2c539bdb10df28a0deadfdc431633bdfc0b8d1cccbeab154666736db79`  
		Last Modified: Sat, 30 Jul 2022 12:32:16 GMT  
		Size: 120.7 MB (120655750 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `gradle:jdk8-jammy` - linux; arm64 variant v8

```console
$ docker pull gradle@sha256:901a53871906e73e6ec5b7ff1e5231edfd55fa47515cbabcba390de83d1090d1
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **314.9 MB (314888820 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:9aaa3cdb95ed9bf8d64a1ca61da75ad0a22eba900f1031450883a29fbdde073c`
-	Default Command: `["gradle"]`

```dockerfile
# Tue, 02 Aug 2022 01:18:59 GMT
ADD file:3db67543ea64bf6723921d19cc5d0483db5c6658fc95834d8b2b5ed48a4cbacd in / 
# Tue, 02 Aug 2022 01:18:59 GMT
CMD ["bash"]
# Tue, 02 Aug 2022 17:51:30 GMT
ENV LANG=en_US.UTF-8 LANGUAGE=en_US:en LC_ALL=en_US.UTF-8
# Tue, 02 Aug 2022 17:51:46 GMT
RUN apt-get update     && DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends tzdata curl ca-certificates fontconfig locales     && echo "en_US.UTF-8 UTF-8" >> /etc/locale.gen     && locale-gen en_US.UTF-8     && rm -rf /var/lib/apt/lists/*
# Tue, 02 Aug 2022 17:51:46 GMT
ENV JAVA_VERSION=jdk8u342-b07
# Tue, 02 Aug 2022 17:51:52 GMT
RUN set -eux;     ARCH="$(dpkg --print-architecture)";     case "${ARCH}" in        aarch64|arm64)          ESUM='ebac40a9a126d1c5333106f9428c9a1d32593ad90b032c1cc147975fa554dfb7';          BINARY_URL='https://github.com/adoptium/temurin8-binaries/releases/download/jdk8u342-b07/OpenJDK8U-jdk_aarch64_linux_hotspot_8u342b07.tar.gz';          ;;        armhf|arm)          ESUM='a12987778eb1455ff5145ae4eda11025e21477c10b0c45e0db8ba96bf9ef20f1';          BINARY_URL='https://github.com/adoptium/temurin8-binaries/releases/download/jdk8u342-b07/OpenJDK8U-jdk_arm_linux_hotspot_8u342b07.tar.gz';          apt-get update          && DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends libatomic1          && rm -rf /var/lib/apt/lists/*          ;;        ppc64el|powerpc:common64)          ESUM='bc943c3e6bc1232ea4e7dd114831b609d83a79f271907941a18f1d7206f741b2';          BINARY_URL='https://github.com/adoptium/temurin8-binaries/releases/download/jdk8u342-b07/OpenJDK8U-jdk_ppc64le_linux_hotspot_8u342b07.tar.gz';          ;;        amd64|i386:x86-64)          ESUM='8252c0e11d542ea0f9ce6b8f147d1a2bea4a17e9fc299da270288f5a4f35b1f3';          BINARY_URL='https://github.com/adoptium/temurin8-binaries/releases/download/jdk8u342-b07/OpenJDK8U-jdk_x64_linux_hotspot_8u342b07.tar.gz';          ;;        *)          echo "Unsupported arch: ${ARCH}";          exit 1;          ;;     esac;     curl -LfsSo /tmp/openjdk.tar.gz ${BINARY_URL};     echo "${ESUM} */tmp/openjdk.tar.gz" | sha256sum -c -;     mkdir -p /opt/java/openjdk;     cd /opt/java/openjdk;     tar -xf /tmp/openjdk.tar.gz --strip-components=1;     rm -rf /tmp/openjdk.tar.gz;
# Tue, 02 Aug 2022 17:51:52 GMT
ENV JAVA_HOME=/opt/java/openjdk PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 02 Aug 2022 17:51:53 GMT
RUN echo Verifying install ...     && echo javac -version && javac -version     && echo java -version && java -version     && echo Complete.
# Wed, 03 Aug 2022 11:04:11 GMT
CMD ["gradle"]
# Wed, 03 Aug 2022 11:04:11 GMT
ENV GRADLE_HOME=/opt/gradle
# Wed, 03 Aug 2022 11:04:12 GMT
RUN set -o errexit -o nounset     && echo "Adding gradle user and group"     && groupadd --system --gid 1000 gradle     && useradd --system --gid gradle --uid 1000 --shell /bin/bash --create-home gradle     && mkdir /home/gradle/.gradle     && chown --recursive gradle:gradle /home/gradle         && echo "Symlinking root Gradle cache to gradle Gradle cache"     && ln --symbolic /home/gradle/.gradle /root/.gradle
# Wed, 03 Aug 2022 11:04:13 GMT
VOLUME [/home/gradle/.gradle]
# Wed, 03 Aug 2022 11:04:14 GMT
WORKDIR /home/gradle
# Wed, 03 Aug 2022 11:04:35 GMT
RUN set -o errexit -o nounset     && apt-get update     && apt-get install --yes --no-install-recommends         unzip         wget                 bzr         git         git-lfs         mercurial         openssh-client         subversion     && rm --recursive --force /var/lib/apt/lists/*         && echo "Testing VCSes"     && which bzr     && which git     && which git-lfs     && which hg     && which svn
# Wed, 03 Aug 2022 11:04:36 GMT
ENV GRADLE_VERSION=7.5
# Wed, 03 Aug 2022 11:04:37 GMT
ARG GRADLE_DOWNLOAD_SHA256=cb87f222c5585bd46838ad4db78463a5c5f3d336e5e2b98dc7c0c586527351c2
# Wed, 03 Aug 2022 11:04:43 GMT
# ARGS: GRADLE_DOWNLOAD_SHA256=cb87f222c5585bd46838ad4db78463a5c5f3d336e5e2b98dc7c0c586527351c2
RUN set -o errexit -o nounset     && echo "Downloading Gradle"     && wget --no-verbose --output-document=gradle.zip "https://services.gradle.org/distributions/gradle-${GRADLE_VERSION}-bin.zip"         && echo "Checking download hash"     && echo "${GRADLE_DOWNLOAD_SHA256} *gradle.zip" | sha256sum --check -         && echo "Installing Gradle"     && unzip gradle.zip     && rm gradle.zip     && mv "gradle-${GRADLE_VERSION}" "${GRADLE_HOME}/"     && ln --symbolic "${GRADLE_HOME}/bin/gradle" /usr/bin/gradle         && echo "Testing Gradle installation"     && gradle --version
```

-	Layers:
	-	`sha256:4a3049d340b7d3651a954fd25a32c42feb1086889d6287e2f15468aef865c5c4`  
		Last Modified: Tue, 02 Aug 2022 01:20:49 GMT  
		Size: 28.4 MB (28381155 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c1a97efc1a354ae767e234943d1f6e30a9985c45f60c828e9af06c2cd98ae470`  
		Last Modified: Tue, 02 Aug 2022 18:00:04 GMT  
		Size: 12.1 MB (12078076 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b0aa7dcb3949b825a76fc6ec8c7bafb3c76accb8daaa780dd120123b7becbe37`  
		Last Modified: Tue, 02 Aug 2022 18:00:12 GMT  
		Size: 102.6 MB (102614873 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:59d25261e65f0ba2bf50d522083d15fb968fa4dd6d1f0486c008cf296b44c296`  
		Last Modified: Tue, 02 Aug 2022 18:00:01 GMT  
		Size: 127.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:960dde7e9012f01b377f8977c26b2399313ce20a4295d9c2b42a02c8838fbaae`  
		Last Modified: Wed, 03 Aug 2022 11:14:40 GMT  
		Size: 4.3 KB (4313 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:55880b45cdb484e5a1e490f1c9b2de57b250ef4b4a679f72684d125492c2c104`  
		Last Modified: Wed, 03 Aug 2022 11:14:49 GMT  
		Size: 51.2 MB (51154662 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:730c7cc1068e6eb7cf65b0e2f14996a79d9aec9dc2827815fa3000baa03fa2dd`  
		Last Modified: Wed, 03 Aug 2022 11:14:49 GMT  
		Size: 120.7 MB (120655614 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `gradle:jdk8-jammy` - linux; ppc64le

```console
$ docker pull gradle@sha256:e7099ee65b8ef15416f24b776ef666d4a7fd7a85ad8b1bfc3d5fb134e8109381
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **326.2 MB (326162822 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:162559da94d7a70019c51b40227e19fb5bcc5654488dd2a1f891b9431c14690a`
-	Default Command: `["gradle"]`

```dockerfile
# Tue, 02 Aug 2022 01:31:12 GMT
ADD file:b6916c28c03568df4c2efc3da91ea6320f639cdbd2fa3f6741fcea7acad4fd5f in / 
# Tue, 02 Aug 2022 01:31:14 GMT
CMD ["bash"]
# Wed, 03 Aug 2022 03:20:49 GMT
ENV LANG=en_US.UTF-8 LANGUAGE=en_US:en LC_ALL=en_US.UTF-8
# Wed, 03 Aug 2022 03:21:52 GMT
RUN apt-get update     && DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends tzdata curl ca-certificates fontconfig locales     && echo "en_US.UTF-8 UTF-8" >> /etc/locale.gen     && locale-gen en_US.UTF-8     && rm -rf /var/lib/apt/lists/*
# Wed, 03 Aug 2022 03:21:53 GMT
ENV JAVA_VERSION=jdk8u342-b07
# Wed, 03 Aug 2022 03:22:06 GMT
RUN set -eux;     ARCH="$(dpkg --print-architecture)";     case "${ARCH}" in        aarch64|arm64)          ESUM='ebac40a9a126d1c5333106f9428c9a1d32593ad90b032c1cc147975fa554dfb7';          BINARY_URL='https://github.com/adoptium/temurin8-binaries/releases/download/jdk8u342-b07/OpenJDK8U-jdk_aarch64_linux_hotspot_8u342b07.tar.gz';          ;;        armhf|arm)          ESUM='a12987778eb1455ff5145ae4eda11025e21477c10b0c45e0db8ba96bf9ef20f1';          BINARY_URL='https://github.com/adoptium/temurin8-binaries/releases/download/jdk8u342-b07/OpenJDK8U-jdk_arm_linux_hotspot_8u342b07.tar.gz';          apt-get update          && DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends libatomic1          && rm -rf /var/lib/apt/lists/*          ;;        ppc64el|powerpc:common64)          ESUM='bc943c3e6bc1232ea4e7dd114831b609d83a79f271907941a18f1d7206f741b2';          BINARY_URL='https://github.com/adoptium/temurin8-binaries/releases/download/jdk8u342-b07/OpenJDK8U-jdk_ppc64le_linux_hotspot_8u342b07.tar.gz';          ;;        amd64|i386:x86-64)          ESUM='8252c0e11d542ea0f9ce6b8f147d1a2bea4a17e9fc299da270288f5a4f35b1f3';          BINARY_URL='https://github.com/adoptium/temurin8-binaries/releases/download/jdk8u342-b07/OpenJDK8U-jdk_x64_linux_hotspot_8u342b07.tar.gz';          ;;        *)          echo "Unsupported arch: ${ARCH}";          exit 1;          ;;     esac;     curl -LfsSo /tmp/openjdk.tar.gz ${BINARY_URL};     echo "${ESUM} */tmp/openjdk.tar.gz" | sha256sum -c -;     mkdir -p /opt/java/openjdk;     cd /opt/java/openjdk;     tar -xf /tmp/openjdk.tar.gz --strip-components=1;     rm -rf /tmp/openjdk.tar.gz;
# Wed, 03 Aug 2022 03:22:08 GMT
ENV JAVA_HOME=/opt/java/openjdk PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 03 Aug 2022 03:22:09 GMT
RUN echo Verifying install ...     && echo javac -version && javac -version     && echo java -version && java -version     && echo Complete.
# Wed, 03 Aug 2022 21:53:48 GMT
CMD ["gradle"]
# Wed, 03 Aug 2022 21:53:48 GMT
ENV GRADLE_HOME=/opt/gradle
# Wed, 03 Aug 2022 21:53:50 GMT
RUN set -o errexit -o nounset     && echo "Adding gradle user and group"     && groupadd --system --gid 1000 gradle     && useradd --system --gid gradle --uid 1000 --shell /bin/bash --create-home gradle     && mkdir /home/gradle/.gradle     && chown --recursive gradle:gradle /home/gradle         && echo "Symlinking root Gradle cache to gradle Gradle cache"     && ln --symbolic /home/gradle/.gradle /root/.gradle
# Wed, 03 Aug 2022 21:53:50 GMT
VOLUME [/home/gradle/.gradle]
# Wed, 03 Aug 2022 21:53:50 GMT
WORKDIR /home/gradle
# Wed, 03 Aug 2022 21:55:22 GMT
RUN set -o errexit -o nounset     && apt-get update     && apt-get install --yes --no-install-recommends         unzip         wget                 bzr         git         git-lfs         mercurial         openssh-client         subversion     && rm --recursive --force /var/lib/apt/lists/*         && echo "Testing VCSes"     && which bzr     && which git     && which git-lfs     && which hg     && which svn
# Wed, 03 Aug 2022 21:55:25 GMT
ENV GRADLE_VERSION=7.5
# Wed, 03 Aug 2022 21:55:26 GMT
ARG GRADLE_DOWNLOAD_SHA256=cb87f222c5585bd46838ad4db78463a5c5f3d336e5e2b98dc7c0c586527351c2
# Wed, 03 Aug 2022 21:55:37 GMT
# ARGS: GRADLE_DOWNLOAD_SHA256=cb87f222c5585bd46838ad4db78463a5c5f3d336e5e2b98dc7c0c586527351c2
RUN set -o errexit -o nounset     && echo "Downloading Gradle"     && wget --no-verbose --output-document=gradle.zip "https://services.gradle.org/distributions/gradle-${GRADLE_VERSION}-bin.zip"         && echo "Checking download hash"     && echo "${GRADLE_DOWNLOAD_SHA256} *gradle.zip" | sha256sum --check -         && echo "Installing Gradle"     && unzip gradle.zip     && rm gradle.zip     && mv "gradle-${GRADLE_VERSION}" "${GRADLE_HOME}/"     && ln --symbolic "${GRADLE_HOME}/bin/gradle" /usr/bin/gradle         && echo "Testing Gradle installation"     && gradle --version
```

-	Layers:
	-	`sha256:6f8c2fc0a4f976c1c0bd1c0e14022b3ed8b7c83cdb247c83016052c3678aaf28`  
		Last Modified: Tue, 02 Aug 2022 01:33:53 GMT  
		Size: 35.7 MB (35718004 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:12312efe1c15bed28c535aa9c41c1b820facd1b2a584f36ed7f7297df7eeac1c`  
		Last Modified: Wed, 03 Aug 2022 03:34:09 GMT  
		Size: 12.9 MB (12862334 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8bb3c821db749b67e68eed9a63a1ed6e908f4b69459c5a22144f800ae362c822`  
		Last Modified: Wed, 03 Aug 2022 03:34:20 GMT  
		Size: 101.0 MB (101016846 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ba6768b99a9350c8f10cdacf6c4e6c8241119e05249ff6489336884d89284259`  
		Last Modified: Wed, 03 Aug 2022 03:34:05 GMT  
		Size: 161.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d4308fcf27019bc86b51e90c8239783225a3c1ff87c425d58b3d00143bc43cee`  
		Last Modified: Wed, 03 Aug 2022 22:10:24 GMT  
		Size: 4.4 KB (4356 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:248db45ad88dcfcbbd600f85a00b28e556a095cf5590a5caa10f52fcbd394b5c`  
		Last Modified: Wed, 03 Aug 2022 22:10:40 GMT  
		Size: 55.9 MB (55905293 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3dcea9ebb8952efd70e91100b2c889302f2247b63098fdd0277ba610e5d3997a`  
		Last Modified: Wed, 03 Aug 2022 22:10:34 GMT  
		Size: 120.7 MB (120655828 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
