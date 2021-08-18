## `gradle:jre16`

```console
$ docker pull gradle@sha256:b26a25ceb3ee18f5e7cbd5bf5cee7b46e84e623f07be4c019c81c3be58fcdf84
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
$ docker pull gradle@sha256:98825ce9296d2ae3563f5c7d8e455da88d9ffcf8744bb0b3522b169322f203ae
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **272.1 MB (272092229 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:2b750261c9b286c285d30ac5a7873e59ecbe6c8ec43f938b3fb5b5f305c70175`
-	Default Command: `["gradle"]`

```dockerfile
# Thu, 17 Jun 2021 23:31:29 GMT
ADD file:920cf788d1ba88f76c97e41e03e4dc2f3005b08d65b5e9da9dd1cbe20a74459b in / 
# Thu, 17 Jun 2021 23:31:29 GMT
CMD ["bash"]
# Fri, 18 Jun 2021 00:28:46 GMT
ENV LANG=en_US.UTF-8 LANGUAGE=en_US:en LC_ALL=en_US.UTF-8
# Fri, 18 Jun 2021 00:29:23 GMT
RUN apt-get update     && apt-get install -y --no-install-recommends tzdata curl ca-certificates fontconfig locales     && echo "en_US.UTF-8 UTF-8" >> /etc/locale.gen     && locale-gen en_US.UTF-8     && rm -rf /var/lib/apt/lists/*
# Fri, 18 Jun 2021 00:30:35 GMT
ENV JAVA_VERSION=jdk-16.0.1+9
# Fri, 18 Jun 2021 00:30:56 GMT
RUN set -eux;     ARCH="$(dpkg --print-architecture)";     case "${ARCH}" in        aarch64|arm64)          ESUM='4e47f1cbf46190727be74cd73445ec2b693f5ba4a74542c554d6b3285811cab5';          BINARY_URL='https://github.com/AdoptOpenJDK/openjdk16-binaries/releases/download/jdk-16.0.1%2B9/OpenJDK16U-jre_aarch64_linux_hotspot_16.0.1_9.tar.gz';          ;;        armhf|armv7l)          ESUM='c1f88f3ce955cb2e9a4236a916cc6660ef55231d29c4390b1a4398ebbca358b7';          BINARY_URL='https://github.com/AdoptOpenJDK/openjdk16-binaries/releases/download/jdk-16.0.1%2B9/OpenJDK16U-jre_arm_linux_hotspot_16.0.1_9.tar.gz';          ;;        ppc64el|ppc64le)          ESUM='495805e2e9bcabeac0d8271623b6c92604440608286f4ce411ea48f582854930';          BINARY_URL='https://github.com/AdoptOpenJDK/openjdk16-binaries/releases/download/jdk-16.0.1%2B9/OpenJDK16U-jre_ppc64le_linux_hotspot_16.0.1_9.tar.gz';          ;;        s390x)          ESUM='780f10923df3230b6013c74482adcc6d8c1fef7b60aefe59a0b337183767d214';          BINARY_URL='https://github.com/AdoptOpenJDK/openjdk16-binaries/releases/download/jdk-16.0.1%2B9/OpenJDK16U-jre_s390x_linux_hotspot_16.0.1_9.tar.gz';          ;;        amd64|x86_64)          ESUM='5eca19d406c6d130e9c3a4b932b9cb0a6e9cd45932450668c3e911bded4bcf40';          BINARY_URL='https://github.com/AdoptOpenJDK/openjdk16-binaries/releases/download/jdk-16.0.1%2B9/OpenJDK16U-jre_x64_linux_hotspot_16.0.1_9.tar.gz';          ;;        *)          echo "Unsupported arch: ${ARCH}";          exit 1;          ;;     esac;     curl -LfsSo /tmp/openjdk.tar.gz ${BINARY_URL};     echo "${ESUM} */tmp/openjdk.tar.gz" | sha256sum -c -;     mkdir -p /opt/java/openjdk;     cd /opt/java/openjdk;     tar -xf /tmp/openjdk.tar.gz --strip-components=1;     rm -rf /tmp/openjdk.tar.gz;
# Fri, 18 Jun 2021 00:30:57 GMT
ENV JAVA_HOME=/opt/java/openjdk PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Fri, 02 Jul 2021 17:33:33 GMT
CMD ["gradle"]
# Fri, 02 Jul 2021 17:33:33 GMT
ENV GRADLE_HOME=/opt/gradle
# Fri, 02 Jul 2021 17:33:34 GMT
RUN set -o errexit -o nounset     && echo "Adding gradle user and group"     && groupadd --system --gid 1000 gradle     && useradd --system --gid gradle --uid 1000 --shell /bin/bash --create-home gradle     && mkdir /home/gradle/.gradle     && chown --recursive gradle:gradle /home/gradle         && echo "Symlinking root Gradle cache to gradle Gradle cache"     && ln -s /home/gradle/.gradle /root/.gradle
# Fri, 02 Jul 2021 17:33:34 GMT
VOLUME [/home/gradle/.gradle]
# Fri, 02 Jul 2021 17:33:35 GMT
WORKDIR /home/gradle
# Fri, 02 Jul 2021 17:33:53 GMT
RUN apt-get update     && apt-get install --yes --no-install-recommends         fontconfig         unzip         wget                 bzr         git         git-lfs         mercurial         openssh-client         subversion     && rm -rf /var/lib/apt/lists/*
# Fri, 02 Jul 2021 17:33:54 GMT
ENV GRADLE_VERSION=7.1.1
# Fri, 02 Jul 2021 17:33:54 GMT
ARG GRADLE_DOWNLOAD_SHA256=bf8b869948901d422e9bb7d1fa61da6a6e19411baa7ad6ee929073df85d6365d
# Fri, 02 Jul 2021 17:33:59 GMT
# ARGS: GRADLE_DOWNLOAD_SHA256=bf8b869948901d422e9bb7d1fa61da6a6e19411baa7ad6ee929073df85d6365d
RUN set -o errexit -o nounset     && echo "Downloading Gradle"     && wget --no-verbose --output-document=gradle.zip "https://services.gradle.org/distributions/gradle-${GRADLE_VERSION}-bin.zip"         && echo "Checking download hash"     && echo "${GRADLE_DOWNLOAD_SHA256} *gradle.zip" | sha256sum --check -         && echo "Installing Gradle"     && unzip gradle.zip     && rm gradle.zip     && mv "gradle-${GRADLE_VERSION}" "${GRADLE_HOME}/"     && ln --symbolic "${GRADLE_HOME}/bin/gradle" /usr/bin/gradle         && echo "Testing Gradle installation"     && gradle --version
```

-	Layers:
	-	`sha256:c549ccf8d472c3bce9ce02e49c62b8f6cbc736ea2b8ba812a1ae9390c69d0b71`  
		Last Modified: Thu, 17 Jun 2021 23:32:58 GMT  
		Size: 28.6 MB (28553692 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bd7766c75e8fade5c21578ec8566d2929e7238f9ac1dbe88551bf2f147b76c65`  
		Last Modified: Fri, 18 Jun 2021 00:39:29 GMT  
		Size: 16.0 MB (16033037 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:23bb7f46497dde5a532f0125f2397431feab57bd390b0f032faad94d5c7472e0`  
		Last Modified: Fri, 18 Jun 2021 00:42:26 GMT  
		Size: 49.6 MB (49621512 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3c706a4396220bf4d46209d5cf5c370e5b1c668008a051ffd526252d0b4fd0d0`  
		Last Modified: Fri, 02 Jul 2021 17:45:49 GMT  
		Size: 4.4 KB (4361 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e59e776adda92412346449ca95dc1784717ed5e7f6df64c173379819b3255c0c`  
		Last Modified: Fri, 02 Jul 2021 17:46:03 GMT  
		Size: 65.6 MB (65626411 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5fe0b0521f11069bb68e77c89ecb5fcfb76814830c74bc776c5efec0e07569c4`  
		Last Modified: Fri, 02 Jul 2021 17:45:57 GMT  
		Size: 112.3 MB (112253216 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `gradle:jre16` - linux; arm variant v7

```console
$ docker pull gradle@sha256:5c17d4288fe28eecdfd9a6783ff56a4c7c6f057144a03b90eb600ee6f1a95909
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **255.9 MB (255891781 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:3a64feaaf45dd41711f11648a5211dd6a88a6dd436db77d31c9d48abdd5a7581`
-	Default Command: `["gradle"]`

```dockerfile
# Thu, 17 Jun 2021 23:32:07 GMT
ADD file:80eca60b823985c38c6de6b89041c5b4c6c668371ec1651af2252d3e29802b48 in / 
# Thu, 17 Jun 2021 23:32:08 GMT
CMD ["bash"]
# Fri, 18 Jun 2021 00:19:21 GMT
ENV LANG=en_US.UTF-8 LANGUAGE=en_US:en LC_ALL=en_US.UTF-8
# Fri, 18 Jun 2021 00:19:37 GMT
RUN apt-get update     && apt-get install -y --no-install-recommends tzdata curl ca-certificates fontconfig locales     && echo "en_US.UTF-8 UTF-8" >> /etc/locale.gen     && locale-gen en_US.UTF-8     && rm -rf /var/lib/apt/lists/*
# Fri, 18 Jun 2021 00:21:40 GMT
ENV JAVA_VERSION=jdk-16.0.1+9
# Fri, 18 Jun 2021 00:22:14 GMT
RUN set -eux;     ARCH="$(dpkg --print-architecture)";     case "${ARCH}" in        aarch64|arm64)          ESUM='4e47f1cbf46190727be74cd73445ec2b693f5ba4a74542c554d6b3285811cab5';          BINARY_URL='https://github.com/AdoptOpenJDK/openjdk16-binaries/releases/download/jdk-16.0.1%2B9/OpenJDK16U-jre_aarch64_linux_hotspot_16.0.1_9.tar.gz';          ;;        armhf|armv7l)          ESUM='c1f88f3ce955cb2e9a4236a916cc6660ef55231d29c4390b1a4398ebbca358b7';          BINARY_URL='https://github.com/AdoptOpenJDK/openjdk16-binaries/releases/download/jdk-16.0.1%2B9/OpenJDK16U-jre_arm_linux_hotspot_16.0.1_9.tar.gz';          ;;        ppc64el|ppc64le)          ESUM='495805e2e9bcabeac0d8271623b6c92604440608286f4ce411ea48f582854930';          BINARY_URL='https://github.com/AdoptOpenJDK/openjdk16-binaries/releases/download/jdk-16.0.1%2B9/OpenJDK16U-jre_ppc64le_linux_hotspot_16.0.1_9.tar.gz';          ;;        s390x)          ESUM='780f10923df3230b6013c74482adcc6d8c1fef7b60aefe59a0b337183767d214';          BINARY_URL='https://github.com/AdoptOpenJDK/openjdk16-binaries/releases/download/jdk-16.0.1%2B9/OpenJDK16U-jre_s390x_linux_hotspot_16.0.1_9.tar.gz';          ;;        amd64|x86_64)          ESUM='5eca19d406c6d130e9c3a4b932b9cb0a6e9cd45932450668c3e911bded4bcf40';          BINARY_URL='https://github.com/AdoptOpenJDK/openjdk16-binaries/releases/download/jdk-16.0.1%2B9/OpenJDK16U-jre_x64_linux_hotspot_16.0.1_9.tar.gz';          ;;        *)          echo "Unsupported arch: ${ARCH}";          exit 1;          ;;     esac;     curl -LfsSo /tmp/openjdk.tar.gz ${BINARY_URL};     echo "${ESUM} */tmp/openjdk.tar.gz" | sha256sum -c -;     mkdir -p /opt/java/openjdk;     cd /opt/java/openjdk;     tar -xf /tmp/openjdk.tar.gz --strip-components=1;     rm -rf /tmp/openjdk.tar.gz;
# Fri, 18 Jun 2021 00:22:14 GMT
ENV JAVA_HOME=/opt/java/openjdk PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Fri, 25 Jun 2021 22:36:24 GMT
CMD ["gradle"]
# Fri, 25 Jun 2021 22:36:24 GMT
ENV GRADLE_HOME=/opt/gradle
# Fri, 25 Jun 2021 22:36:27 GMT
RUN set -o errexit -o nounset     && echo "Adding gradle user and group"     && groupadd --system --gid 1000 gradle     && useradd --system --gid gradle --uid 1000 --shell /bin/bash --create-home gradle     && mkdir /home/gradle/.gradle     && chown --recursive gradle:gradle /home/gradle         && echo "Symlinking root Gradle cache to gradle Gradle cache"     && ln -s /home/gradle/.gradle /root/.gradle
# Fri, 25 Jun 2021 22:36:27 GMT
VOLUME [/home/gradle/.gradle]
# Fri, 25 Jun 2021 22:36:28 GMT
WORKDIR /home/gradle
# Fri, 25 Jun 2021 22:37:16 GMT
RUN apt-get update     && apt-get install --yes --no-install-recommends         fontconfig         unzip         wget                 bzr         git         git-lfs         mercurial         openssh-client         subversion     && rm -rf /var/lib/apt/lists/*
# Fri, 02 Jul 2021 19:13:16 GMT
ENV GRADLE_VERSION=7.1.1
# Fri, 02 Jul 2021 19:13:16 GMT
ARG GRADLE_DOWNLOAD_SHA256=bf8b869948901d422e9bb7d1fa61da6a6e19411baa7ad6ee929073df85d6365d
# Fri, 02 Jul 2021 19:13:29 GMT
# ARGS: GRADLE_DOWNLOAD_SHA256=bf8b869948901d422e9bb7d1fa61da6a6e19411baa7ad6ee929073df85d6365d
RUN set -o errexit -o nounset     && echo "Downloading Gradle"     && wget --no-verbose --output-document=gradle.zip "https://services.gradle.org/distributions/gradle-${GRADLE_VERSION}-bin.zip"         && echo "Checking download hash"     && echo "${GRADLE_DOWNLOAD_SHA256} *gradle.zip" | sha256sum --check -         && echo "Installing Gradle"     && unzip gradle.zip     && rm gradle.zip     && mv "gradle-${GRADLE_VERSION}" "${GRADLE_HOME}/"     && ln --symbolic "${GRADLE_HOME}/bin/gradle" /usr/bin/gradle         && echo "Testing Gradle installation"     && gradle --version
```

-	Layers:
	-	`sha256:10ded72e3c7fd53116a7f233f140c1e56753fdee4f5cbd888b9e62f3b6684a5f`  
		Last Modified: Thu, 17 Jun 2021 23:34:59 GMT  
		Size: 24.1 MB (24051742 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a86a63ece73e003c3e90921fca83be84403e1adf5cbe48609ee1937a5270a1c3`  
		Last Modified: Fri, 18 Jun 2021 00:24:43 GMT  
		Size: 14.9 MB (14898847 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:24fcc8711c549a13367d176f88ceb8bf0c2ff20cd458281462c6da4eebc3eb3d`  
		Last Modified: Fri, 18 Jun 2021 00:28:29 GMT  
		Size: 44.7 MB (44663246 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e6b59f0c936aad59d70e1bca2ea3dbfaedfacf7bb1b731abca7f188f4af9fd38`  
		Last Modified: Fri, 25 Jun 2021 22:47:09 GMT  
		Size: 4.3 KB (4345 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f45e954c14418e820ff6a16968fd1d516c2ce4957387250a91537462ebeb6131`  
		Last Modified: Fri, 25 Jun 2021 22:47:54 GMT  
		Size: 60.0 MB (60020388 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ee04f7634e367b92ff562872c315f2aa1bb3f9aec363fde12683dc27e691ac4b`  
		Last Modified: Fri, 02 Jul 2021 19:22:33 GMT  
		Size: 112.3 MB (112253213 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `gradle:jre16` - linux; arm64 variant v8

```console
$ docker pull gradle@sha256:a1fdd3151e80723682c44184275e31f55e05d9db7c0f1fe78241d6f184a82927
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **271.2 MB (271196730 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c14df3382b08166dc78911d47539a9646095912191804e037673119d1c8bf1e3`
-	Default Command: `["gradle"]`

```dockerfile
# Mon, 26 Jul 2021 21:48:57 GMT
ADD file:10d7c5e7290ff5627132fb35c51a2143351e184b02e3fb6d9c1c06815ae803ae in / 
# Mon, 26 Jul 2021 21:48:57 GMT
CMD ["bash"]
# Mon, 26 Jul 2021 22:15:02 GMT
ENV LANG=en_US.UTF-8 LANGUAGE=en_US:en LC_ALL=en_US.UTF-8
# Mon, 26 Jul 2021 22:15:18 GMT
RUN apt-get update     && apt-get install -y --no-install-recommends tzdata curl ca-certificates fontconfig locales     && echo "en_US.UTF-8 UTF-8" >> /etc/locale.gen     && locale-gen en_US.UTF-8     && rm -rf /var/lib/apt/lists/*
# Mon, 26 Jul 2021 22:16:41 GMT
ENV JAVA_VERSION=jdk-16.0.1+9
# Mon, 26 Jul 2021 22:17:05 GMT
RUN set -eux;     ARCH="$(dpkg --print-architecture)";     case "${ARCH}" in        aarch64|arm64)          ESUM='4e47f1cbf46190727be74cd73445ec2b693f5ba4a74542c554d6b3285811cab5';          BINARY_URL='https://github.com/AdoptOpenJDK/openjdk16-binaries/releases/download/jdk-16.0.1%2B9/OpenJDK16U-jre_aarch64_linux_hotspot_16.0.1_9.tar.gz';          ;;        armhf|armv7l)          ESUM='c1f88f3ce955cb2e9a4236a916cc6660ef55231d29c4390b1a4398ebbca358b7';          BINARY_URL='https://github.com/AdoptOpenJDK/openjdk16-binaries/releases/download/jdk-16.0.1%2B9/OpenJDK16U-jre_arm_linux_hotspot_16.0.1_9.tar.gz';          ;;        ppc64el|ppc64le)          ESUM='495805e2e9bcabeac0d8271623b6c92604440608286f4ce411ea48f582854930';          BINARY_URL='https://github.com/AdoptOpenJDK/openjdk16-binaries/releases/download/jdk-16.0.1%2B9/OpenJDK16U-jre_ppc64le_linux_hotspot_16.0.1_9.tar.gz';          ;;        s390x)          ESUM='780f10923df3230b6013c74482adcc6d8c1fef7b60aefe59a0b337183767d214';          BINARY_URL='https://github.com/AdoptOpenJDK/openjdk16-binaries/releases/download/jdk-16.0.1%2B9/OpenJDK16U-jre_s390x_linux_hotspot_16.0.1_9.tar.gz';          ;;        amd64|x86_64)          ESUM='5eca19d406c6d130e9c3a4b932b9cb0a6e9cd45932450668c3e911bded4bcf40';          BINARY_URL='https://github.com/AdoptOpenJDK/openjdk16-binaries/releases/download/jdk-16.0.1%2B9/OpenJDK16U-jre_x64_linux_hotspot_16.0.1_9.tar.gz';          ;;        *)          echo "Unsupported arch: ${ARCH}";          exit 1;          ;;     esac;     curl -LfsSo /tmp/openjdk.tar.gz ${BINARY_URL};     echo "${ESUM} */tmp/openjdk.tar.gz" | sha256sum -c -;     mkdir -p /opt/java/openjdk;     cd /opt/java/openjdk;     tar -xf /tmp/openjdk.tar.gz --strip-components=1;     rm -rf /tmp/openjdk.tar.gz;
# Mon, 26 Jul 2021 22:17:06 GMT
ENV JAVA_HOME=/opt/java/openjdk PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 18 Aug 2021 18:42:02 GMT
CMD ["gradle"]
# Wed, 18 Aug 2021 18:42:02 GMT
ENV GRADLE_HOME=/opt/gradle
# Wed, 18 Aug 2021 18:42:03 GMT
RUN set -o errexit -o nounset     && echo "Adding gradle user and group"     && groupadd --system --gid 1000 gradle     && useradd --system --gid gradle --uid 1000 --shell /bin/bash --create-home gradle     && mkdir /home/gradle/.gradle     && chown --recursive gradle:gradle /home/gradle         && echo "Symlinking root Gradle cache to gradle Gradle cache"     && ln -s /home/gradle/.gradle /root/.gradle
# Wed, 18 Aug 2021 18:42:03 GMT
VOLUME [/home/gradle/.gradle]
# Wed, 18 Aug 2021 18:42:03 GMT
WORKDIR /home/gradle
# Wed, 18 Aug 2021 18:42:23 GMT
RUN apt-get update     && apt-get install --yes --no-install-recommends         fontconfig         unzip         wget                 bzr         git         git-lfs         mercurial         openssh-client         subversion     && rm -rf /var/lib/apt/lists/*
# Wed, 18 Aug 2021 18:42:24 GMT
ENV GRADLE_VERSION=7.2
# Wed, 18 Aug 2021 18:42:24 GMT
ARG GRADLE_DOWNLOAD_SHA256=f581709a9c35e9cb92e16f585d2c4bc99b2b1a5f85d2badbd3dc6bff59e1e6dd
# Wed, 18 Aug 2021 18:42:29 GMT
# ARGS: GRADLE_DOWNLOAD_SHA256=f581709a9c35e9cb92e16f585d2c4bc99b2b1a5f85d2badbd3dc6bff59e1e6dd
RUN set -o errexit -o nounset     && echo "Downloading Gradle"     && wget --no-verbose --output-document=gradle.zip "https://services.gradle.org/distributions/gradle-${GRADLE_VERSION}-bin.zip"         && echo "Checking download hash"     && echo "${GRADLE_DOWNLOAD_SHA256} *gradle.zip" | sha256sum --check -         && echo "Installing Gradle"     && unzip gradle.zip     && rm gradle.zip     && mv "gradle-${GRADLE_VERSION}" "${GRADLE_HOME}/"     && ln --symbolic "${GRADLE_HOME}/bin/gradle" /usr/bin/gradle         && echo "Testing Gradle installation"     && gradle --version
```

-	Layers:
	-	`sha256:be0de17fe24f767ec21bec97d0e8ea8f0d907fe05238a0bf9cce0995f529f7ea`  
		Last Modified: Mon, 26 Jul 2021 21:50:59 GMT  
		Size: 27.2 MB (27170255 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a3fcc4ceb51ac08370be105d7f328e8fe57475e20b0b894a485dbdbfa93e0fbc`  
		Last Modified: Mon, 26 Jul 2021 22:18:58 GMT  
		Size: 15.9 MB (15894651 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:92d56cff2a067496566397d00e7be80fb217cbac95573c3e0c9d72490a3bffbb`  
		Last Modified: Mon, 26 Jul 2021 22:22:27 GMT  
		Size: 48.4 MB (48422623 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9d74c890d1260ad5cabbd130999acd3b090057847899b212c60b87e0e76e4612`  
		Last Modified: Wed, 18 Aug 2021 18:55:54 GMT  
		Size: 4.4 KB (4366 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f2c17e6fbcc0ac9d18b8fd930aeb3a8f187a5390f09f503a240e37cbc5f5f466`  
		Last Modified: Wed, 18 Aug 2021 18:56:06 GMT  
		Size: 65.3 MB (65330968 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0860491e4067f205624ca95846212554a1ad1a7581670e1898c497585b147c08`  
		Last Modified: Wed, 18 Aug 2021 18:56:02 GMT  
		Size: 114.4 MB (114373867 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `gradle:jre16` - linux; ppc64le

```console
$ docker pull gradle@sha256:dd99c4844be38d8423ebeff50bc2c9073189eac7de2522c076a0bf252ef965b6
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **281.6 MB (281597078 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:549ae45042d0a333c41e94a27f3d8b6afbb7ce5049d4aa9bdb986f72ab736adf`
-	Default Command: `["gradle"]`

```dockerfile
# Thu, 17 Jun 2021 23:25:15 GMT
ADD file:8bcc5606b1ba5ed52b8c7ede7afc0f1a2303865b9f9c1a268f8893b2772d227b in / 
# Thu, 17 Jun 2021 23:25:21 GMT
CMD ["bash"]
# Fri, 18 Jun 2021 01:29:17 GMT
ENV LANG=en_US.UTF-8 LANGUAGE=en_US:en LC_ALL=en_US.UTF-8
# Fri, 18 Jun 2021 01:31:53 GMT
RUN apt-get update     && apt-get install -y --no-install-recommends tzdata curl ca-certificates fontconfig locales     && echo "en_US.UTF-8 UTF-8" >> /etc/locale.gen     && locale-gen en_US.UTF-8     && rm -rf /var/lib/apt/lists/*
# Fri, 18 Jun 2021 01:36:36 GMT
ENV JAVA_VERSION=jdk-16.0.1+9
# Fri, 18 Jun 2021 01:37:33 GMT
RUN set -eux;     ARCH="$(dpkg --print-architecture)";     case "${ARCH}" in        aarch64|arm64)          ESUM='4e47f1cbf46190727be74cd73445ec2b693f5ba4a74542c554d6b3285811cab5';          BINARY_URL='https://github.com/AdoptOpenJDK/openjdk16-binaries/releases/download/jdk-16.0.1%2B9/OpenJDK16U-jre_aarch64_linux_hotspot_16.0.1_9.tar.gz';          ;;        armhf|armv7l)          ESUM='c1f88f3ce955cb2e9a4236a916cc6660ef55231d29c4390b1a4398ebbca358b7';          BINARY_URL='https://github.com/AdoptOpenJDK/openjdk16-binaries/releases/download/jdk-16.0.1%2B9/OpenJDK16U-jre_arm_linux_hotspot_16.0.1_9.tar.gz';          ;;        ppc64el|ppc64le)          ESUM='495805e2e9bcabeac0d8271623b6c92604440608286f4ce411ea48f582854930';          BINARY_URL='https://github.com/AdoptOpenJDK/openjdk16-binaries/releases/download/jdk-16.0.1%2B9/OpenJDK16U-jre_ppc64le_linux_hotspot_16.0.1_9.tar.gz';          ;;        s390x)          ESUM='780f10923df3230b6013c74482adcc6d8c1fef7b60aefe59a0b337183767d214';          BINARY_URL='https://github.com/AdoptOpenJDK/openjdk16-binaries/releases/download/jdk-16.0.1%2B9/OpenJDK16U-jre_s390x_linux_hotspot_16.0.1_9.tar.gz';          ;;        amd64|x86_64)          ESUM='5eca19d406c6d130e9c3a4b932b9cb0a6e9cd45932450668c3e911bded4bcf40';          BINARY_URL='https://github.com/AdoptOpenJDK/openjdk16-binaries/releases/download/jdk-16.0.1%2B9/OpenJDK16U-jre_x64_linux_hotspot_16.0.1_9.tar.gz';          ;;        *)          echo "Unsupported arch: ${ARCH}";          exit 1;          ;;     esac;     curl -LfsSo /tmp/openjdk.tar.gz ${BINARY_URL};     echo "${ESUM} */tmp/openjdk.tar.gz" | sha256sum -c -;     mkdir -p /opt/java/openjdk;     cd /opt/java/openjdk;     tar -xf /tmp/openjdk.tar.gz --strip-components=1;     rm -rf /tmp/openjdk.tar.gz;
# Fri, 18 Jun 2021 01:37:39 GMT
ENV JAVA_HOME=/opt/java/openjdk PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 08 Jul 2021 04:41:33 GMT
CMD ["gradle"]
# Thu, 08 Jul 2021 04:41:36 GMT
ENV GRADLE_HOME=/opt/gradle
# Thu, 08 Jul 2021 04:41:45 GMT
RUN set -o errexit -o nounset     && echo "Adding gradle user and group"     && groupadd --system --gid 1000 gradle     && useradd --system --gid gradle --uid 1000 --shell /bin/bash --create-home gradle     && mkdir /home/gradle/.gradle     && chown --recursive gradle:gradle /home/gradle         && echo "Symlinking root Gradle cache to gradle Gradle cache"     && ln -s /home/gradle/.gradle /root/.gradle
# Thu, 08 Jul 2021 04:41:48 GMT
VOLUME [/home/gradle/.gradle]
# Thu, 08 Jul 2021 04:41:52 GMT
WORKDIR /home/gradle
# Thu, 08 Jul 2021 04:44:30 GMT
RUN apt-get update     && apt-get install --yes --no-install-recommends         fontconfig         unzip         wget                 bzr         git         git-lfs         mercurial         openssh-client         subversion     && rm -rf /var/lib/apt/lists/*
# Thu, 08 Jul 2021 04:44:39 GMT
ENV GRADLE_VERSION=7.1.1
# Thu, 08 Jul 2021 04:44:42 GMT
ARG GRADLE_DOWNLOAD_SHA256=bf8b869948901d422e9bb7d1fa61da6a6e19411baa7ad6ee929073df85d6365d
# Thu, 08 Jul 2021 04:45:42 GMT
# ARGS: GRADLE_DOWNLOAD_SHA256=bf8b869948901d422e9bb7d1fa61da6a6e19411baa7ad6ee929073df85d6365d
RUN set -o errexit -o nounset     && echo "Downloading Gradle"     && wget --no-verbose --output-document=gradle.zip "https://services.gradle.org/distributions/gradle-${GRADLE_VERSION}-bin.zip"         && echo "Checking download hash"     && echo "${GRADLE_DOWNLOAD_SHA256} *gradle.zip" | sha256sum --check -         && echo "Installing Gradle"     && unzip gradle.zip     && rm gradle.zip     && mv "gradle-${GRADLE_VERSION}" "${GRADLE_HOME}/"     && ln --symbolic "${GRADLE_HOME}/bin/gradle" /usr/bin/gradle         && echo "Testing Gradle installation"     && gradle --version
```

-	Layers:
	-	`sha256:830138a32e2b9cb850f077b06d89ea5d26428556430bf886f193115b2527779a`  
		Last Modified: Thu, 17 Jun 2021 23:28:41 GMT  
		Size: 33.3 MB (33278245 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:83b268950217e490e209e0491ae6fbd3af12b4642aefad9c0039daf7b3ea0371`  
		Last Modified: Fri, 18 Jun 2021 01:52:43 GMT  
		Size: 17.2 MB (17208433 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4ac3fc4e00afed6f9b8054ca4817d47cc47551ff322803839545c3ab484305cd`  
		Last Modified: Fri, 18 Jun 2021 01:55:57 GMT  
		Size: 44.9 MB (44852176 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2aec91680bf358d4d6c8200aa8913824d441731d723069c165f1fb49ea513f37`  
		Last Modified: Thu, 08 Jul 2021 05:41:57 GMT  
		Size: 4.4 KB (4364 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d7c6bc9c9e9316a7f417d360bc395c8590bb1b1f618e7b26097cf7087a7eadd9`  
		Last Modified: Thu, 08 Jul 2021 05:42:13 GMT  
		Size: 74.0 MB (74000609 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:51c68eb977fc846284fe93b6d33b467c5acfa6c924d7fb5b8f725203e0558462`  
		Last Modified: Thu, 08 Jul 2021 05:42:09 GMT  
		Size: 112.3 MB (112253251 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `gradle:jre16` - linux; s390x

```console
$ docker pull gradle@sha256:e3e6668cd972b80737aed92c90bb679143d48be89b96a0f6615c31c5f7178edd
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **266.1 MB (266136853 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:456b3f5488a6ddf672b4c839b66fd28df47b2e50f29928689030bcb14a521e37`
-	Default Command: `["gradle"]`

```dockerfile
# Mon, 26 Jul 2021 20:55:12 GMT
ADD file:b8731edfdacfade2ec96757342f216962f3971b24077a9144da3f80003e6893e in / 
# Mon, 26 Jul 2021 20:55:14 GMT
CMD ["bash"]
# Mon, 26 Jul 2021 21:19:34 GMT
ENV LANG=en_US.UTF-8 LANGUAGE=en_US:en LC_ALL=en_US.UTF-8
# Mon, 26 Jul 2021 21:19:45 GMT
RUN apt-get update     && apt-get install -y --no-install-recommends tzdata curl ca-certificates fontconfig locales     && echo "en_US.UTF-8 UTF-8" >> /etc/locale.gen     && locale-gen en_US.UTF-8     && rm -rf /var/lib/apt/lists/*
# Mon, 26 Jul 2021 21:21:31 GMT
ENV JAVA_VERSION=jdk-16.0.1+9
# Mon, 26 Jul 2021 21:22:00 GMT
RUN set -eux;     ARCH="$(dpkg --print-architecture)";     case "${ARCH}" in        aarch64|arm64)          ESUM='4e47f1cbf46190727be74cd73445ec2b693f5ba4a74542c554d6b3285811cab5';          BINARY_URL='https://github.com/AdoptOpenJDK/openjdk16-binaries/releases/download/jdk-16.0.1%2B9/OpenJDK16U-jre_aarch64_linux_hotspot_16.0.1_9.tar.gz';          ;;        armhf|armv7l)          ESUM='c1f88f3ce955cb2e9a4236a916cc6660ef55231d29c4390b1a4398ebbca358b7';          BINARY_URL='https://github.com/AdoptOpenJDK/openjdk16-binaries/releases/download/jdk-16.0.1%2B9/OpenJDK16U-jre_arm_linux_hotspot_16.0.1_9.tar.gz';          ;;        ppc64el|ppc64le)          ESUM='495805e2e9bcabeac0d8271623b6c92604440608286f4ce411ea48f582854930';          BINARY_URL='https://github.com/AdoptOpenJDK/openjdk16-binaries/releases/download/jdk-16.0.1%2B9/OpenJDK16U-jre_ppc64le_linux_hotspot_16.0.1_9.tar.gz';          ;;        s390x)          ESUM='780f10923df3230b6013c74482adcc6d8c1fef7b60aefe59a0b337183767d214';          BINARY_URL='https://github.com/AdoptOpenJDK/openjdk16-binaries/releases/download/jdk-16.0.1%2B9/OpenJDK16U-jre_s390x_linux_hotspot_16.0.1_9.tar.gz';          ;;        amd64|x86_64)          ESUM='5eca19d406c6d130e9c3a4b932b9cb0a6e9cd45932450668c3e911bded4bcf40';          BINARY_URL='https://github.com/AdoptOpenJDK/openjdk16-binaries/releases/download/jdk-16.0.1%2B9/OpenJDK16U-jre_x64_linux_hotspot_16.0.1_9.tar.gz';          ;;        *)          echo "Unsupported arch: ${ARCH}";          exit 1;          ;;     esac;     curl -LfsSo /tmp/openjdk.tar.gz ${BINARY_URL};     echo "${ESUM} */tmp/openjdk.tar.gz" | sha256sum -c -;     mkdir -p /opt/java/openjdk;     cd /opt/java/openjdk;     tar -xf /tmp/openjdk.tar.gz --strip-components=1;     rm -rf /tmp/openjdk.tar.gz;
# Mon, 26 Jul 2021 21:22:03 GMT
ENV JAVA_HOME=/opt/java/openjdk PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 18 Aug 2021 14:49:22 GMT
CMD ["gradle"]
# Wed, 18 Aug 2021 14:49:23 GMT
ENV GRADLE_HOME=/opt/gradle
# Wed, 18 Aug 2021 14:49:24 GMT
RUN set -o errexit -o nounset     && echo "Adding gradle user and group"     && groupadd --system --gid 1000 gradle     && useradd --system --gid gradle --uid 1000 --shell /bin/bash --create-home gradle     && mkdir /home/gradle/.gradle     && chown --recursive gradle:gradle /home/gradle         && echo "Symlinking root Gradle cache to gradle Gradle cache"     && ln -s /home/gradle/.gradle /root/.gradle
# Wed, 18 Aug 2021 14:49:24 GMT
VOLUME [/home/gradle/.gradle]
# Wed, 18 Aug 2021 14:49:25 GMT
WORKDIR /home/gradle
# Wed, 18 Aug 2021 14:50:01 GMT
RUN apt-get update     && apt-get install --yes --no-install-recommends         fontconfig         unzip         wget                 bzr         git         git-lfs         mercurial         openssh-client         subversion     && rm -rf /var/lib/apt/lists/*
# Wed, 18 Aug 2021 14:50:10 GMT
ENV GRADLE_VERSION=7.2
# Wed, 18 Aug 2021 14:50:11 GMT
ARG GRADLE_DOWNLOAD_SHA256=f581709a9c35e9cb92e16f585d2c4bc99b2b1a5f85d2badbd3dc6bff59e1e6dd
# Wed, 18 Aug 2021 14:50:22 GMT
# ARGS: GRADLE_DOWNLOAD_SHA256=f581709a9c35e9cb92e16f585d2c4bc99b2b1a5f85d2badbd3dc6bff59e1e6dd
RUN set -o errexit -o nounset     && echo "Downloading Gradle"     && wget --no-verbose --output-document=gradle.zip "https://services.gradle.org/distributions/gradle-${GRADLE_VERSION}-bin.zip"         && echo "Checking download hash"     && echo "${GRADLE_DOWNLOAD_SHA256} *gradle.zip" | sha256sum --check -         && echo "Installing Gradle"     && unzip gradle.zip     && rm gradle.zip     && mv "gradle-${GRADLE_VERSION}" "${GRADLE_HOME}/"     && ln --symbolic "${GRADLE_HOME}/bin/gradle" /usr/bin/gradle         && echo "Testing Gradle installation"     && gradle --version
```

-	Layers:
	-	`sha256:38800a0044dea146ca3c3a08bc2c9c956396ad3241a3c343010775650298c379`  
		Last Modified: Mon, 26 Jul 2021 20:57:03 GMT  
		Size: 27.1 MB (27149898 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c2859ea56dafeb61512cbd72a03b7e2b1e762e9a60e7ca4d0bda5d8d7433dc6e`  
		Last Modified: Mon, 26 Jul 2021 21:32:13 GMT  
		Size: 15.7 MB (15741671 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6ad339e26b8f311f2134260cb560f9b1404b3e7cd25eb076724924a768a93fe0`  
		Last Modified: Mon, 26 Jul 2021 21:34:24 GMT  
		Size: 44.0 MB (44034533 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a9743fa58b6a2fbcb7bac89074f94a0c63ac3c679069060c8d18cc8b7cf0b6f3`  
		Last Modified: Wed, 18 Aug 2021 15:10:04 GMT  
		Size: 4.4 KB (4367 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3bf7430194416c2c027c53573d2cf9785e327ecd529c5c026c521bbc28250e76`  
		Last Modified: Wed, 18 Aug 2021 15:10:14 GMT  
		Size: 64.8 MB (64832530 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:95ffd830d27c8400ba620538befe0e9714fc33f75cb02fa6c2c52375b1488caf`  
		Last Modified: Wed, 18 Aug 2021 15:10:11 GMT  
		Size: 114.4 MB (114373854 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
