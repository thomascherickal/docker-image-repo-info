## `gradle:jre16`

```console
$ docker pull gradle@sha256:f1e6011531e82c0782c009c056fe05314aa7be425ea0dde9df4b858e90628be0
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 5
	-	linux; amd64
	-	linux; arm variant v7
	-	linux; arm64 variant v8
	-	linux; ppc64le
	-	linux; s390x

### `gradle:jre16` - linux; amd64

```console
$ docker pull gradle@sha256:d78771281a12b744195c319b56a24210ca7960a4eaefb8faf02fb88213e2d899
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **274.2 MB (274227188 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:fce952174c18beac720737240f61f70c4870b790e5d7c7788ad8e57c757bb795`
-	Default Command: `["gradle"]`

```dockerfile
# Fri, 01 Oct 2021 02:23:40 GMT
ADD file:8d2f4a45a58b3f5426c89e2ef57164824fbf0e4d17b8a90fffa0d5ff3b4e5114 in / 
# Fri, 01 Oct 2021 02:23:40 GMT
CMD ["bash"]
# Fri, 01 Oct 2021 03:25:06 GMT
ENV LANG=en_US.UTF-8 LANGUAGE=en_US:en LC_ALL=en_US.UTF-8
# Fri, 01 Oct 2021 03:25:22 GMT
RUN apt-get update     && apt-get install -y --no-install-recommends tzdata curl ca-certificates fontconfig locales     && echo "en_US.UTF-8 UTF-8" >> /etc/locale.gen     && locale-gen en_US.UTF-8     && rm -rf /var/lib/apt/lists/*
# Fri, 01 Oct 2021 03:26:35 GMT
ENV JAVA_VERSION=jdk-16.0.1+9
# Fri, 01 Oct 2021 03:26:57 GMT
RUN set -eux;     ARCH="$(dpkg --print-architecture)";     case "${ARCH}" in        aarch64|arm64)          ESUM='4e47f1cbf46190727be74cd73445ec2b693f5ba4a74542c554d6b3285811cab5';          BINARY_URL='https://github.com/AdoptOpenJDK/openjdk16-binaries/releases/download/jdk-16.0.1%2B9/OpenJDK16U-jre_aarch64_linux_hotspot_16.0.1_9.tar.gz';          ;;        armhf|armv7l)          ESUM='c1f88f3ce955cb2e9a4236a916cc6660ef55231d29c4390b1a4398ebbca358b7';          BINARY_URL='https://github.com/AdoptOpenJDK/openjdk16-binaries/releases/download/jdk-16.0.1%2B9/OpenJDK16U-jre_arm_linux_hotspot_16.0.1_9.tar.gz';          ;;        ppc64el|ppc64le)          ESUM='495805e2e9bcabeac0d8271623b6c92604440608286f4ce411ea48f582854930';          BINARY_URL='https://github.com/AdoptOpenJDK/openjdk16-binaries/releases/download/jdk-16.0.1%2B9/OpenJDK16U-jre_ppc64le_linux_hotspot_16.0.1_9.tar.gz';          ;;        s390x)          ESUM='780f10923df3230b6013c74482adcc6d8c1fef7b60aefe59a0b337183767d214';          BINARY_URL='https://github.com/AdoptOpenJDK/openjdk16-binaries/releases/download/jdk-16.0.1%2B9/OpenJDK16U-jre_s390x_linux_hotspot_16.0.1_9.tar.gz';          ;;        amd64|x86_64)          ESUM='5eca19d406c6d130e9c3a4b932b9cb0a6e9cd45932450668c3e911bded4bcf40';          BINARY_URL='https://github.com/AdoptOpenJDK/openjdk16-binaries/releases/download/jdk-16.0.1%2B9/OpenJDK16U-jre_x64_linux_hotspot_16.0.1_9.tar.gz';          ;;        *)          echo "Unsupported arch: ${ARCH}";          exit 1;          ;;     esac;     curl -LfsSo /tmp/openjdk.tar.gz ${BINARY_URL};     echo "${ESUM} */tmp/openjdk.tar.gz" | sha256sum -c -;     mkdir -p /opt/java/openjdk;     cd /opt/java/openjdk;     tar -xf /tmp/openjdk.tar.gz --strip-components=1;     rm -rf /tmp/openjdk.tar.gz;
# Fri, 01 Oct 2021 03:26:58 GMT
ENV JAVA_HOME=/opt/java/openjdk PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Fri, 01 Oct 2021 08:09:38 GMT
CMD ["gradle"]
# Fri, 01 Oct 2021 08:09:38 GMT
ENV GRADLE_HOME=/opt/gradle
# Fri, 01 Oct 2021 08:09:39 GMT
RUN set -o errexit -o nounset     && echo "Adding gradle user and group"     && groupadd --system --gid 1000 gradle     && useradd --system --gid gradle --uid 1000 --shell /bin/bash --create-home gradle     && mkdir /home/gradle/.gradle     && chown --recursive gradle:gradle /home/gradle         && echo "Symlinking root Gradle cache to gradle Gradle cache"     && ln -s /home/gradle/.gradle /root/.gradle
# Fri, 01 Oct 2021 08:09:40 GMT
VOLUME [/home/gradle/.gradle]
# Fri, 01 Oct 2021 08:09:40 GMT
WORKDIR /home/gradle
# Fri, 01 Oct 2021 08:09:58 GMT
RUN apt-get update     && apt-get install --yes --no-install-recommends         fontconfig         unzip         wget                 bzr         git         git-lfs         mercurial         openssh-client         subversion     && rm -rf /var/lib/apt/lists/*
# Fri, 01 Oct 2021 08:09:59 GMT
ENV GRADLE_VERSION=7.2
# Fri, 01 Oct 2021 08:09:59 GMT
ARG GRADLE_DOWNLOAD_SHA256=f581709a9c35e9cb92e16f585d2c4bc99b2b1a5f85d2badbd3dc6bff59e1e6dd
# Fri, 01 Oct 2021 08:10:04 GMT
# ARGS: GRADLE_DOWNLOAD_SHA256=f581709a9c35e9cb92e16f585d2c4bc99b2b1a5f85d2badbd3dc6bff59e1e6dd
RUN set -o errexit -o nounset     && echo "Downloading Gradle"     && wget --no-verbose --output-document=gradle.zip "https://services.gradle.org/distributions/gradle-${GRADLE_VERSION}-bin.zip"         && echo "Checking download hash"     && echo "${GRADLE_DOWNLOAD_SHA256} *gradle.zip" | sha256sum --check -         && echo "Installing Gradle"     && unzip gradle.zip     && rm gradle.zip     && mv "gradle-${GRADLE_VERSION}" "${GRADLE_HOME}/"     && ln --symbolic "${GRADLE_HOME}/bin/gradle" /usr/bin/gradle         && echo "Testing Gradle installation"     && gradle --version
```

-	Layers:
	-	`sha256:f3ef4ff62e0da0ef761ec1c8a578f3035bef51043e53ae1b13a20b3e03726d17`  
		Last Modified: Thu, 23 Sep 2021 03:03:26 GMT  
		Size: 28.6 MB (28568914 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:706b9b9c1c443d1cd3d83fa6ecf9e3a4ae13b711dcc6b3aa34e9603c1cb8a930`  
		Last Modified: Fri, 01 Oct 2021 03:35:45 GMT  
		Size: 16.0 MB (16033975 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:47b6345bdb0d99bdd58f07cac7fbe1cae1ebe99265b9d88c082e1e5ad9fd4085`  
		Last Modified: Fri, 01 Oct 2021 03:38:32 GMT  
		Size: 49.6 MB (49621497 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6b6719c0695ddde7201427d3c60a67728da594062a26b0e6c802437572eb8c07`  
		Last Modified: Fri, 01 Oct 2021 08:21:11 GMT  
		Size: 4.4 KB (4360 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:49c402e332c6bb030b820519445ed7c36d9e293c985dd81aec8b8e4966ed39f1`  
		Last Modified: Fri, 01 Oct 2021 08:21:22 GMT  
		Size: 65.6 MB (65624594 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:da4cd448d8296201b708cdd64f2fb455a18825b4b6943e4ae11a6f1338dc486b`  
		Last Modified: Fri, 01 Oct 2021 08:21:17 GMT  
		Size: 114.4 MB (114373848 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `gradle:jre16` - linux; arm variant v7

```console
$ docker pull gradle@sha256:21348bb1ce7f382f2e3a138833c863d7dee757fda6cf843ca2ae8dde7b6bafc6
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **258.0 MB (258030105 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:25940d2ad87eed5b2b2c3e888b77ac6c37fbf060e4bc828187214265a5428f72`
-	Default Command: `["gradle"]`

```dockerfile
# Sat, 02 Oct 2021 05:58:58 GMT
ADD file:17b7faea72ce285877ae2e83ecc15fc88de184361899edfcb561531ea121090b in / 
# Sat, 02 Oct 2021 05:58:59 GMT
CMD ["bash"]
# Sat, 02 Oct 2021 23:26:18 GMT
ENV LANG=en_US.UTF-8 LANGUAGE=en_US:en LC_ALL=en_US.UTF-8
# Sat, 02 Oct 2021 23:37:39 GMT
RUN apt-get update     && apt-get install -y --no-install-recommends tzdata curl ca-certificates fontconfig locales     && echo "en_US.UTF-8 UTF-8" >> /etc/locale.gen     && locale-gen en_US.UTF-8     && rm -rf /var/lib/apt/lists/*
# Sat, 02 Oct 2021 23:40:47 GMT
ENV JAVA_VERSION=jdk-16.0.1+9
# Sat, 02 Oct 2021 23:41:43 GMT
RUN set -eux;     ARCH="$(dpkg --print-architecture)";     case "${ARCH}" in        aarch64|arm64)          ESUM='4e47f1cbf46190727be74cd73445ec2b693f5ba4a74542c554d6b3285811cab5';          BINARY_URL='https://github.com/AdoptOpenJDK/openjdk16-binaries/releases/download/jdk-16.0.1%2B9/OpenJDK16U-jre_aarch64_linux_hotspot_16.0.1_9.tar.gz';          ;;        armhf|armv7l)          ESUM='c1f88f3ce955cb2e9a4236a916cc6660ef55231d29c4390b1a4398ebbca358b7';          BINARY_URL='https://github.com/AdoptOpenJDK/openjdk16-binaries/releases/download/jdk-16.0.1%2B9/OpenJDK16U-jre_arm_linux_hotspot_16.0.1_9.tar.gz';          ;;        ppc64el|ppc64le)          ESUM='495805e2e9bcabeac0d8271623b6c92604440608286f4ce411ea48f582854930';          BINARY_URL='https://github.com/AdoptOpenJDK/openjdk16-binaries/releases/download/jdk-16.0.1%2B9/OpenJDK16U-jre_ppc64le_linux_hotspot_16.0.1_9.tar.gz';          ;;        s390x)          ESUM='780f10923df3230b6013c74482adcc6d8c1fef7b60aefe59a0b337183767d214';          BINARY_URL='https://github.com/AdoptOpenJDK/openjdk16-binaries/releases/download/jdk-16.0.1%2B9/OpenJDK16U-jre_s390x_linux_hotspot_16.0.1_9.tar.gz';          ;;        amd64|x86_64)          ESUM='5eca19d406c6d130e9c3a4b932b9cb0a6e9cd45932450668c3e911bded4bcf40';          BINARY_URL='https://github.com/AdoptOpenJDK/openjdk16-binaries/releases/download/jdk-16.0.1%2B9/OpenJDK16U-jre_x64_linux_hotspot_16.0.1_9.tar.gz';          ;;        *)          echo "Unsupported arch: ${ARCH}";          exit 1;          ;;     esac;     curl -LfsSo /tmp/openjdk.tar.gz ${BINARY_URL};     echo "${ESUM} */tmp/openjdk.tar.gz" | sha256sum -c -;     mkdir -p /opt/java/openjdk;     cd /opt/java/openjdk;     tar -xf /tmp/openjdk.tar.gz --strip-components=1;     rm -rf /tmp/openjdk.tar.gz;
# Sat, 02 Oct 2021 23:41:44 GMT
ENV JAVA_HOME=/opt/java/openjdk PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Sun, 03 Oct 2021 04:28:00 GMT
CMD ["gradle"]
# Sun, 03 Oct 2021 04:28:00 GMT
ENV GRADLE_HOME=/opt/gradle
# Sun, 03 Oct 2021 04:28:02 GMT
RUN set -o errexit -o nounset     && echo "Adding gradle user and group"     && groupadd --system --gid 1000 gradle     && useradd --system --gid gradle --uid 1000 --shell /bin/bash --create-home gradle     && mkdir /home/gradle/.gradle     && chown --recursive gradle:gradle /home/gradle         && echo "Symlinking root Gradle cache to gradle Gradle cache"     && ln -s /home/gradle/.gradle /root/.gradle
# Sun, 03 Oct 2021 04:28:03 GMT
VOLUME [/home/gradle/.gradle]
# Sun, 03 Oct 2021 04:28:03 GMT
WORKDIR /home/gradle
# Sun, 03 Oct 2021 04:28:52 GMT
RUN apt-get update     && apt-get install --yes --no-install-recommends         fontconfig         unzip         wget                 bzr         git         git-lfs         mercurial         openssh-client         subversion     && rm -rf /var/lib/apt/lists/*
# Sun, 03 Oct 2021 04:28:53 GMT
ENV GRADLE_VERSION=7.2
# Sun, 03 Oct 2021 04:28:53 GMT
ARG GRADLE_DOWNLOAD_SHA256=f581709a9c35e9cb92e16f585d2c4bc99b2b1a5f85d2badbd3dc6bff59e1e6dd
# Sun, 03 Oct 2021 04:29:06 GMT
# ARGS: GRADLE_DOWNLOAD_SHA256=f581709a9c35e9cb92e16f585d2c4bc99b2b1a5f85d2badbd3dc6bff59e1e6dd
RUN set -o errexit -o nounset     && echo "Downloading Gradle"     && wget --no-verbose --output-document=gradle.zip "https://services.gradle.org/distributions/gradle-${GRADLE_VERSION}-bin.zip"         && echo "Checking download hash"     && echo "${GRADLE_DOWNLOAD_SHA256} *gradle.zip" | sha256sum --check -         && echo "Installing Gradle"     && unzip gradle.zip     && rm gradle.zip     && mv "gradle-${GRADLE_VERSION}" "${GRADLE_HOME}/"     && ln --symbolic "${GRADLE_HOME}/bin/gradle" /usr/bin/gradle         && echo "Testing Gradle installation"     && gradle --version
```

-	Layers:
	-	`sha256:29a0bfee4452af9c258710b3049350eec1ed6ee85e33634a638e982934e59d83`  
		Last Modified: Sat, 02 Oct 2021 06:03:00 GMT  
		Size: 24.1 MB (24067218 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:18110d4575fb4d6fc0f882483d001f57cf4cc83a308eacce1e903c788025fd10`  
		Last Modified: Sat, 02 Oct 2021 23:45:17 GMT  
		Size: 14.9 MB (14898568 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:99c864c36f22d19808745e368f082b1800b9c1556b49bae2fdd3f957517f80ee`  
		Last Modified: Sat, 02 Oct 2021 23:52:56 GMT  
		Size: 44.7 MB (44663184 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bae4dbee003c02c8f1a2f1cd2703ab261fa84760498c17be8b100bddea65509d`  
		Last Modified: Sun, 03 Oct 2021 04:38:39 GMT  
		Size: 4.4 KB (4351 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:72f80c29a381f5a223e6a56ea073b256193862751271f011e143cf3338dea924`  
		Last Modified: Sun, 03 Oct 2021 04:39:21 GMT  
		Size: 60.0 MB (60023009 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:12bc552c40bcf5a7948281f8e437685ab3c2ce5d493bc94ba6edc1c69a106cc8`  
		Last Modified: Sun, 03 Oct 2021 04:39:12 GMT  
		Size: 114.4 MB (114373775 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `gradle:jre16` - linux; arm64 variant v8

```console
$ docker pull gradle@sha256:046380fc97f9743869f5455ef20e05d882feabbead49c7eed9d45434618684ee
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **271.2 MB (271197233 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a4e23ac1a91b00ab650210811cc5be5c32db66298a5ce4befc491afd5c84e215`
-	Default Command: `["gradle"]`

```dockerfile
# Fri, 01 Oct 2021 02:43:52 GMT
ADD file:e297c32269d46d9846129f357af15b231eb977271968f7f63e65fff73934824b in / 
# Fri, 01 Oct 2021 02:43:52 GMT
CMD ["bash"]
# Fri, 01 Oct 2021 03:02:08 GMT
ENV LANG=en_US.UTF-8 LANGUAGE=en_US:en LC_ALL=en_US.UTF-8
# Fri, 01 Oct 2021 03:02:25 GMT
RUN apt-get update     && apt-get install -y --no-install-recommends tzdata curl ca-certificates fontconfig locales     && echo "en_US.UTF-8 UTF-8" >> /etc/locale.gen     && locale-gen en_US.UTF-8     && rm -rf /var/lib/apt/lists/*
# Fri, 01 Oct 2021 03:03:48 GMT
ENV JAVA_VERSION=jdk-16.0.1+9
# Fri, 01 Oct 2021 03:04:14 GMT
RUN set -eux;     ARCH="$(dpkg --print-architecture)";     case "${ARCH}" in        aarch64|arm64)          ESUM='4e47f1cbf46190727be74cd73445ec2b693f5ba4a74542c554d6b3285811cab5';          BINARY_URL='https://github.com/AdoptOpenJDK/openjdk16-binaries/releases/download/jdk-16.0.1%2B9/OpenJDK16U-jre_aarch64_linux_hotspot_16.0.1_9.tar.gz';          ;;        armhf|armv7l)          ESUM='c1f88f3ce955cb2e9a4236a916cc6660ef55231d29c4390b1a4398ebbca358b7';          BINARY_URL='https://github.com/AdoptOpenJDK/openjdk16-binaries/releases/download/jdk-16.0.1%2B9/OpenJDK16U-jre_arm_linux_hotspot_16.0.1_9.tar.gz';          ;;        ppc64el|ppc64le)          ESUM='495805e2e9bcabeac0d8271623b6c92604440608286f4ce411ea48f582854930';          BINARY_URL='https://github.com/AdoptOpenJDK/openjdk16-binaries/releases/download/jdk-16.0.1%2B9/OpenJDK16U-jre_ppc64le_linux_hotspot_16.0.1_9.tar.gz';          ;;        s390x)          ESUM='780f10923df3230b6013c74482adcc6d8c1fef7b60aefe59a0b337183767d214';          BINARY_URL='https://github.com/AdoptOpenJDK/openjdk16-binaries/releases/download/jdk-16.0.1%2B9/OpenJDK16U-jre_s390x_linux_hotspot_16.0.1_9.tar.gz';          ;;        amd64|x86_64)          ESUM='5eca19d406c6d130e9c3a4b932b9cb0a6e9cd45932450668c3e911bded4bcf40';          BINARY_URL='https://github.com/AdoptOpenJDK/openjdk16-binaries/releases/download/jdk-16.0.1%2B9/OpenJDK16U-jre_x64_linux_hotspot_16.0.1_9.tar.gz';          ;;        *)          echo "Unsupported arch: ${ARCH}";          exit 1;          ;;     esac;     curl -LfsSo /tmp/openjdk.tar.gz ${BINARY_URL};     echo "${ESUM} */tmp/openjdk.tar.gz" | sha256sum -c -;     mkdir -p /opt/java/openjdk;     cd /opt/java/openjdk;     tar -xf /tmp/openjdk.tar.gz --strip-components=1;     rm -rf /tmp/openjdk.tar.gz;
# Fri, 01 Oct 2021 03:04:15 GMT
ENV JAVA_HOME=/opt/java/openjdk PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Fri, 01 Oct 2021 04:31:08 GMT
CMD ["gradle"]
# Fri, 01 Oct 2021 04:31:08 GMT
ENV GRADLE_HOME=/opt/gradle
# Fri, 01 Oct 2021 04:31:09 GMT
RUN set -o errexit -o nounset     && echo "Adding gradle user and group"     && groupadd --system --gid 1000 gradle     && useradd --system --gid gradle --uid 1000 --shell /bin/bash --create-home gradle     && mkdir /home/gradle/.gradle     && chown --recursive gradle:gradle /home/gradle         && echo "Symlinking root Gradle cache to gradle Gradle cache"     && ln -s /home/gradle/.gradle /root/.gradle
# Fri, 01 Oct 2021 04:31:09 GMT
VOLUME [/home/gradle/.gradle]
# Fri, 01 Oct 2021 04:31:10 GMT
WORKDIR /home/gradle
# Fri, 01 Oct 2021 04:31:30 GMT
RUN apt-get update     && apt-get install --yes --no-install-recommends         fontconfig         unzip         wget                 bzr         git         git-lfs         mercurial         openssh-client         subversion     && rm -rf /var/lib/apt/lists/*
# Fri, 01 Oct 2021 04:31:31 GMT
ENV GRADLE_VERSION=7.2
# Fri, 01 Oct 2021 04:31:31 GMT
ARG GRADLE_DOWNLOAD_SHA256=f581709a9c35e9cb92e16f585d2c4bc99b2b1a5f85d2badbd3dc6bff59e1e6dd
# Fri, 01 Oct 2021 04:31:36 GMT
# ARGS: GRADLE_DOWNLOAD_SHA256=f581709a9c35e9cb92e16f585d2c4bc99b2b1a5f85d2badbd3dc6bff59e1e6dd
RUN set -o errexit -o nounset     && echo "Downloading Gradle"     && wget --no-verbose --output-document=gradle.zip "https://services.gradle.org/distributions/gradle-${GRADLE_VERSION}-bin.zip"         && echo "Checking download hash"     && echo "${GRADLE_DOWNLOAD_SHA256} *gradle.zip" | sha256sum --check -         && echo "Installing Gradle"     && unzip gradle.zip     && rm gradle.zip     && mv "gradle-${GRADLE_VERSION}" "${GRADLE_HOME}/"     && ln --symbolic "${GRADLE_HOME}/bin/gradle" /usr/bin/gradle         && echo "Testing Gradle installation"     && gradle --version
```

-	Layers:
	-	`sha256:a2e448ef5a4dfc8e290db319d98910aa96a3abfcf38ae90bbac21672b8438d9e`  
		Last Modified: Fri, 01 Oct 2021 02:45:48 GMT  
		Size: 27.2 MB (27172405 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:965f9c84d32763760a8a95b798239bf2dd8423aeb8fb56015ddd90196d483d9f`  
		Last Modified: Fri, 01 Oct 2021 03:06:06 GMT  
		Size: 15.9 MB (15895939 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:22d94c05262d780295dd8214b29db520cbaead56c618f3bf2531dbb268af5d84`  
		Last Modified: Fri, 01 Oct 2021 03:09:11 GMT  
		Size: 48.4 MB (48422624 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4753c953c011b0b265e3580968df83351d969655a76f2b6ce936880412740697`  
		Last Modified: Fri, 01 Oct 2021 04:44:16 GMT  
		Size: 4.4 KB (4365 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e872bd19233a58831135ef5cec3e22c473cbf4bbd0bd7d5a9646975c7219323d`  
		Last Modified: Fri, 01 Oct 2021 04:44:28 GMT  
		Size: 65.3 MB (65328130 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ed1db0756b51b4e2053b8ab7928375a457b77147033cf677aa68633a6ffe2d71`  
		Last Modified: Fri, 01 Oct 2021 04:44:24 GMT  
		Size: 114.4 MB (114373770 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `gradle:jre16` - linux; ppc64le

```console
$ docker pull gradle@sha256:0f8e2f7973a6b7438de2b20d7c3b811983c6830ac3a1ad282396d231c017c5d6
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **283.7 MB (283735323 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:1bb64edc8a279e02472778717166d7f16a8f0f8e1df4fad3ef1243fac4dc76bb`
-	Default Command: `["gradle"]`

```dockerfile
# Tue, 31 Aug 2021 02:10:40 GMT
ADD file:7e5ee5560faaa801aa10a76122190026f8c1da00c809f4fb6ff441751ba0c90f in / 
# Tue, 31 Aug 2021 02:10:45 GMT
CMD ["bash"]
# Tue, 31 Aug 2021 02:31:18 GMT
ENV LANG=en_US.UTF-8 LANGUAGE=en_US:en LC_ALL=en_US.UTF-8
# Tue, 31 Aug 2021 02:33:24 GMT
RUN apt-get update     && apt-get install -y --no-install-recommends tzdata curl ca-certificates fontconfig locales     && echo "en_US.UTF-8 UTF-8" >> /etc/locale.gen     && locale-gen en_US.UTF-8     && rm -rf /var/lib/apt/lists/*
# Tue, 31 Aug 2021 02:37:45 GMT
ENV JAVA_VERSION=jdk-16.0.1+9
# Tue, 31 Aug 2021 02:39:04 GMT
RUN set -eux;     ARCH="$(dpkg --print-architecture)";     case "${ARCH}" in        aarch64|arm64)          ESUM='4e47f1cbf46190727be74cd73445ec2b693f5ba4a74542c554d6b3285811cab5';          BINARY_URL='https://github.com/AdoptOpenJDK/openjdk16-binaries/releases/download/jdk-16.0.1%2B9/OpenJDK16U-jre_aarch64_linux_hotspot_16.0.1_9.tar.gz';          ;;        armhf|armv7l)          ESUM='c1f88f3ce955cb2e9a4236a916cc6660ef55231d29c4390b1a4398ebbca358b7';          BINARY_URL='https://github.com/AdoptOpenJDK/openjdk16-binaries/releases/download/jdk-16.0.1%2B9/OpenJDK16U-jre_arm_linux_hotspot_16.0.1_9.tar.gz';          ;;        ppc64el|ppc64le)          ESUM='495805e2e9bcabeac0d8271623b6c92604440608286f4ce411ea48f582854930';          BINARY_URL='https://github.com/AdoptOpenJDK/openjdk16-binaries/releases/download/jdk-16.0.1%2B9/OpenJDK16U-jre_ppc64le_linux_hotspot_16.0.1_9.tar.gz';          ;;        s390x)          ESUM='780f10923df3230b6013c74482adcc6d8c1fef7b60aefe59a0b337183767d214';          BINARY_URL='https://github.com/AdoptOpenJDK/openjdk16-binaries/releases/download/jdk-16.0.1%2B9/OpenJDK16U-jre_s390x_linux_hotspot_16.0.1_9.tar.gz';          ;;        amd64|x86_64)          ESUM='5eca19d406c6d130e9c3a4b932b9cb0a6e9cd45932450668c3e911bded4bcf40';          BINARY_URL='https://github.com/AdoptOpenJDK/openjdk16-binaries/releases/download/jdk-16.0.1%2B9/OpenJDK16U-jre_x64_linux_hotspot_16.0.1_9.tar.gz';          ;;        *)          echo "Unsupported arch: ${ARCH}";          exit 1;          ;;     esac;     curl -LfsSo /tmp/openjdk.tar.gz ${BINARY_URL};     echo "${ESUM} */tmp/openjdk.tar.gz" | sha256sum -c -;     mkdir -p /opt/java/openjdk;     cd /opt/java/openjdk;     tar -xf /tmp/openjdk.tar.gz --strip-components=1;     rm -rf /tmp/openjdk.tar.gz;
# Tue, 31 Aug 2021 02:39:11 GMT
ENV JAVA_HOME=/opt/java/openjdk PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 31 Aug 2021 07:56:07 GMT
CMD ["gradle"]
# Tue, 31 Aug 2021 07:56:14 GMT
ENV GRADLE_HOME=/opt/gradle
# Tue, 31 Aug 2021 07:56:27 GMT
RUN set -o errexit -o nounset     && echo "Adding gradle user and group"     && groupadd --system --gid 1000 gradle     && useradd --system --gid gradle --uid 1000 --shell /bin/bash --create-home gradle     && mkdir /home/gradle/.gradle     && chown --recursive gradle:gradle /home/gradle         && echo "Symlinking root Gradle cache to gradle Gradle cache"     && ln -s /home/gradle/.gradle /root/.gradle
# Tue, 31 Aug 2021 07:56:30 GMT
VOLUME [/home/gradle/.gradle]
# Tue, 31 Aug 2021 07:56:36 GMT
WORKDIR /home/gradle
# Tue, 31 Aug 2021 08:02:22 GMT
RUN apt-get update     && apt-get install --yes --no-install-recommends         fontconfig         unzip         wget                 bzr         git         git-lfs         mercurial         openssh-client         subversion     && rm -rf /var/lib/apt/lists/*
# Tue, 31 Aug 2021 08:02:28 GMT
ENV GRADLE_VERSION=7.2
# Tue, 31 Aug 2021 08:02:35 GMT
ARG GRADLE_DOWNLOAD_SHA256=f581709a9c35e9cb92e16f585d2c4bc99b2b1a5f85d2badbd3dc6bff59e1e6dd
# Tue, 31 Aug 2021 08:03:00 GMT
# ARGS: GRADLE_DOWNLOAD_SHA256=f581709a9c35e9cb92e16f585d2c4bc99b2b1a5f85d2badbd3dc6bff59e1e6dd
RUN set -o errexit -o nounset     && echo "Downloading Gradle"     && wget --no-verbose --output-document=gradle.zip "https://services.gradle.org/distributions/gradle-${GRADLE_VERSION}-bin.zip"         && echo "Checking download hash"     && echo "${GRADLE_DOWNLOAD_SHA256} *gradle.zip" | sha256sum --check -         && echo "Installing Gradle"     && unzip gradle.zip     && rm gradle.zip     && mv "gradle-${GRADLE_VERSION}" "${GRADLE_HOME}/"     && ln --symbolic "${GRADLE_HOME}/bin/gradle" /usr/bin/gradle         && echo "Testing Gradle installation"     && gradle --version
```

-	Layers:
	-	`sha256:59390c695558464c51dc1fced64934b549770630192a1639ac6a90f59bd63b13`  
		Last Modified: Tue, 31 Aug 2021 02:14:21 GMT  
		Size: 33.3 MB (33291791 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:df6df1a3e21a26bf9e0775ad823e1762b00bf8c2a0650a891b7860b7fe18741a`  
		Last Modified: Tue, 31 Aug 2021 02:54:54 GMT  
		Size: 17.2 MB (17208636 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8b6914bc910b228b8ef6d99dfdb4ea1b290b8e76ece716b73ebd8a67fda256d4`  
		Last Modified: Tue, 31 Aug 2021 02:58:15 GMT  
		Size: 44.9 MB (44852180 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d48535f41deeaa2a15d7606849773ec588758edb81f7ea11035f6bed5a895554`  
		Last Modified: Tue, 31 Aug 2021 09:04:01 GMT  
		Size: 4.4 KB (4361 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e556d0dd61a1a01c124ea0be784ecb6a50ddfda7b06ccfcb2b5159a2d77b352b`  
		Last Modified: Tue, 31 Aug 2021 09:05:12 GMT  
		Size: 74.0 MB (74004485 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b3e8746551fe1c7668d4ccc1453f8cbefacc3398e276e89670fc540873b66f07`  
		Last Modified: Tue, 31 Aug 2021 09:04:23 GMT  
		Size: 114.4 MB (114373870 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `gradle:jre16` - linux; s390x

```console
$ docker pull gradle@sha256:d9c4f1a468df0ff36c6c3d11eb277b43a337b5bf5f8f82d00dd781d483a19ee2
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **266.1 MB (266112210 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:731073c8520549ca22f1595c6571f61f7cbba5457ee3b668fce403b72ceea1e6`
-	Default Command: `["gradle"]`

```dockerfile
# Fri, 01 Oct 2021 01:42:28 GMT
ADD file:28b3d1959812d7666f9f73b52562cdaaaf84ff25ce6331995e21c66bb31b0cc2 in / 
# Fri, 01 Oct 2021 01:42:30 GMT
CMD ["bash"]
# Fri, 01 Oct 2021 02:00:06 GMT
ENV LANG=en_US.UTF-8 LANGUAGE=en_US:en LC_ALL=en_US.UTF-8
# Fri, 01 Oct 2021 02:00:17 GMT
RUN apt-get update     && apt-get install -y --no-install-recommends tzdata curl ca-certificates fontconfig locales     && echo "en_US.UTF-8 UTF-8" >> /etc/locale.gen     && locale-gen en_US.UTF-8     && rm -rf /var/lib/apt/lists/*
# Fri, 01 Oct 2021 02:01:57 GMT
ENV JAVA_VERSION=jdk-16.0.1+9
# Fri, 01 Oct 2021 02:02:26 GMT
RUN set -eux;     ARCH="$(dpkg --print-architecture)";     case "${ARCH}" in        aarch64|arm64)          ESUM='4e47f1cbf46190727be74cd73445ec2b693f5ba4a74542c554d6b3285811cab5';          BINARY_URL='https://github.com/AdoptOpenJDK/openjdk16-binaries/releases/download/jdk-16.0.1%2B9/OpenJDK16U-jre_aarch64_linux_hotspot_16.0.1_9.tar.gz';          ;;        armhf|armv7l)          ESUM='c1f88f3ce955cb2e9a4236a916cc6660ef55231d29c4390b1a4398ebbca358b7';          BINARY_URL='https://github.com/AdoptOpenJDK/openjdk16-binaries/releases/download/jdk-16.0.1%2B9/OpenJDK16U-jre_arm_linux_hotspot_16.0.1_9.tar.gz';          ;;        ppc64el|ppc64le)          ESUM='495805e2e9bcabeac0d8271623b6c92604440608286f4ce411ea48f582854930';          BINARY_URL='https://github.com/AdoptOpenJDK/openjdk16-binaries/releases/download/jdk-16.0.1%2B9/OpenJDK16U-jre_ppc64le_linux_hotspot_16.0.1_9.tar.gz';          ;;        s390x)          ESUM='780f10923df3230b6013c74482adcc6d8c1fef7b60aefe59a0b337183767d214';          BINARY_URL='https://github.com/AdoptOpenJDK/openjdk16-binaries/releases/download/jdk-16.0.1%2B9/OpenJDK16U-jre_s390x_linux_hotspot_16.0.1_9.tar.gz';          ;;        amd64|x86_64)          ESUM='5eca19d406c6d130e9c3a4b932b9cb0a6e9cd45932450668c3e911bded4bcf40';          BINARY_URL='https://github.com/AdoptOpenJDK/openjdk16-binaries/releases/download/jdk-16.0.1%2B9/OpenJDK16U-jre_x64_linux_hotspot_16.0.1_9.tar.gz';          ;;        *)          echo "Unsupported arch: ${ARCH}";          exit 1;          ;;     esac;     curl -LfsSo /tmp/openjdk.tar.gz ${BINARY_URL};     echo "${ESUM} */tmp/openjdk.tar.gz" | sha256sum -c -;     mkdir -p /opt/java/openjdk;     cd /opt/java/openjdk;     tar -xf /tmp/openjdk.tar.gz --strip-components=1;     rm -rf /tmp/openjdk.tar.gz;
# Fri, 01 Oct 2021 02:02:27 GMT
ENV JAVA_HOME=/opt/java/openjdk PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Fri, 01 Oct 2021 02:52:25 GMT
CMD ["gradle"]
# Fri, 01 Oct 2021 02:52:25 GMT
ENV GRADLE_HOME=/opt/gradle
# Fri, 01 Oct 2021 02:52:26 GMT
RUN set -o errexit -o nounset     && echo "Adding gradle user and group"     && groupadd --system --gid 1000 gradle     && useradd --system --gid gradle --uid 1000 --shell /bin/bash --create-home gradle     && mkdir /home/gradle/.gradle     && chown --recursive gradle:gradle /home/gradle         && echo "Symlinking root Gradle cache to gradle Gradle cache"     && ln -s /home/gradle/.gradle /root/.gradle
# Fri, 01 Oct 2021 02:52:26 GMT
VOLUME [/home/gradle/.gradle]
# Fri, 01 Oct 2021 02:52:26 GMT
WORKDIR /home/gradle
# Fri, 01 Oct 2021 02:52:42 GMT
RUN apt-get update     && apt-get install --yes --no-install-recommends         fontconfig         unzip         wget                 bzr         git         git-lfs         mercurial         openssh-client         subversion     && rm -rf /var/lib/apt/lists/*
# Fri, 01 Oct 2021 02:52:45 GMT
ENV GRADLE_VERSION=7.2
# Fri, 01 Oct 2021 02:52:46 GMT
ARG GRADLE_DOWNLOAD_SHA256=f581709a9c35e9cb92e16f585d2c4bc99b2b1a5f85d2badbd3dc6bff59e1e6dd
# Fri, 01 Oct 2021 02:52:51 GMT
# ARGS: GRADLE_DOWNLOAD_SHA256=f581709a9c35e9cb92e16f585d2c4bc99b2b1a5f85d2badbd3dc6bff59e1e6dd
RUN set -o errexit -o nounset     && echo "Downloading Gradle"     && wget --no-verbose --output-document=gradle.zip "https://services.gradle.org/distributions/gradle-${GRADLE_VERSION}-bin.zip"         && echo "Checking download hash"     && echo "${GRADLE_DOWNLOAD_SHA256} *gradle.zip" | sha256sum --check -         && echo "Installing Gradle"     && unzip gradle.zip     && rm gradle.zip     && mv "gradle-${GRADLE_VERSION}" "${GRADLE_HOME}/"     && ln --symbolic "${GRADLE_HOME}/bin/gradle" /usr/bin/gradle         && echo "Testing Gradle installation"     && gradle --version
```

-	Layers:
	-	`sha256:21245da3aae0a4172d9a415c8ba92069601c8a55fc39b783bce7981e97de1b4d`  
		Last Modified: Fri, 01 Oct 2021 01:44:02 GMT  
		Size: 27.1 MB (27122910 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c1b23a8bdcc3c25fc238593c281d2480b42fe86d322be5a1580ea62c30b309a9`  
		Last Modified: Fri, 01 Oct 2021 02:12:12 GMT  
		Size: 15.7 MB (15739781 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d38ca3efaae54312e26c738e57017707c109b255caececf6c3c06fe66cc117eb`  
		Last Modified: Fri, 01 Oct 2021 02:14:13 GMT  
		Size: 44.0 MB (44034537 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6b706c181d7bb0f75b5559ec5f979c5f17b184a2378097736df6c4316983a54c`  
		Last Modified: Fri, 01 Oct 2021 03:07:11 GMT  
		Size: 4.4 KB (4365 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f32eca31abd99927f3585fea57628a542822f2b6b793d22088edd1a6ee051d99`  
		Last Modified: Fri, 01 Oct 2021 03:07:21 GMT  
		Size: 64.8 MB (64836773 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c0ac7464fa95c468007e4a8426cd9d1c9e95256f7e5c3a392d04bd5e5eacdc88`  
		Last Modified: Fri, 01 Oct 2021 03:07:16 GMT  
		Size: 114.4 MB (114373844 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
