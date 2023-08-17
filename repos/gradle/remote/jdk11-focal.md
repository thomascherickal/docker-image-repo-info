## `gradle:jdk11-focal`

```console
$ docker pull gradle@sha256:52e716bae437c62c5ff020cfeb2ee1f5a889f69ef3b78811c8c99e19cb9a9cf5
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 5
	-	linux; amd64
	-	linux; arm variant v7
	-	linux; arm64 variant v8
	-	linux; ppc64le
	-	linux; s390x

### `gradle:jdk11-focal` - linux; amd64

```console
$ docker pull gradle@sha256:485600bf9a97ea9caed99b1698a32dbcd5b8fa69833035acea39c923b85fd464
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **384.6 MB (384558325 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:143727d01de9b8fa2f33eff58b3f7270c98692e5d41f4d54e6810314da19675c`
-	Entrypoint: `["\/__cacert_entrypoint.sh"]`
-	Default Command: `["gradle"]`

```dockerfile
# Tue, 01 Aug 2023 06:16:43 GMT
ARG RELEASE
# Tue, 01 Aug 2023 06:16:44 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Tue, 01 Aug 2023 06:16:44 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Tue, 01 Aug 2023 06:16:44 GMT
LABEL org.opencontainers.image.version=20.04
# Tue, 01 Aug 2023 06:16:45 GMT
ADD file:233702cd816c07bc9fed02881b11fb3bdcaee41f3ce3ec1c9f0c4a060b155d5b in / 
# Tue, 01 Aug 2023 06:16:46 GMT
CMD ["/bin/bash"]
# Thu, 03 Aug 2023 02:34:40 GMT
ENV JAVA_HOME=/opt/java/openjdk
# Thu, 03 Aug 2023 02:34:40 GMT
ENV PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 03 Aug 2023 02:34:40 GMT
ENV LANG=en_US.UTF-8 LANGUAGE=en_US:en LC_ALL=en_US.UTF-8
# Tue, 08 Aug 2023 19:20:25 GMT
RUN apt-get update     && DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends tzdata curl wget ca-certificates fontconfig locales p11-kit     && echo "en_US.UTF-8 UTF-8" >> /etc/locale.gen     && locale-gen en_US.UTF-8     && rm -rf /var/lib/apt/lists/*
# Tue, 08 Aug 2023 19:22:00 GMT
ENV JAVA_VERSION=jdk-11.0.20+8
# Tue, 08 Aug 2023 19:22:08 GMT
RUN set -eux;     ARCH="$(dpkg --print-architecture)";     case "${ARCH}" in        aarch64|arm64)          ESUM='eb821c049c2d2f7c3fbf8ddcce2d608d3aa7d488700e76bfbbebabba93021748';          BINARY_URL='https://github.com/adoptium/temurin11-binaries/releases/download/jdk-11.0.20%2B8/OpenJDK11U-jdk_aarch64_linux_hotspot_11.0.20_8.tar.gz';          ;;        armhf|arm)          ESUM='fdf98d94ac3fd49a73a534fd88cf60e757e885c04791d15f76ccfcecb43a25e0';          BINARY_URL='https://github.com/adoptium/temurin11-binaries/releases/download/jdk-11.0.20%2B8/OpenJDK11U-jdk_arm_linux_hotspot_11.0.20_8.tar.gz';          ;;        ppc64el|powerpc:common64)          ESUM='1125931b3a38e6e305a1932fc6cfd0b023a0fbec2cab10e835a2ee2c50848b42';          BINARY_URL='https://github.com/adoptium/temurin11-binaries/releases/download/jdk-11.0.20%2B8/OpenJDK11U-jdk_ppc64le_linux_hotspot_11.0.20_8.tar.gz';          ;;        s390x|s390:64-bit)          ESUM='688c83d9edf2204220df94ce5bab4a6d19f3d91bc0e500f31dda41e16d9a383f';          BINARY_URL='https://github.com/adoptium/temurin11-binaries/releases/download/jdk-11.0.20%2B8/OpenJDK11U-jdk_s390x_linux_hotspot_11.0.20_8.tar.gz';          ;;        amd64|i386:x86-64)          ESUM='7a99258af2e3ee9047e90f1c0c1775fd6285085759501295358d934d662e01f9';          BINARY_URL='https://github.com/adoptium/temurin11-binaries/releases/download/jdk-11.0.20%2B8/OpenJDK11U-jdk_x64_linux_hotspot_11.0.20_8.tar.gz';          ;;        *)          echo "Unsupported arch: ${ARCH}";          exit 1;          ;;     esac; 	  wget -O /tmp/openjdk.tar.gz ${BINARY_URL}; 	  echo "${ESUM} */tmp/openjdk.tar.gz" | sha256sum -c -; 	  mkdir -p "$JAVA_HOME"; 	  tar --extract 	      --file /tmp/openjdk.tar.gz 	      --directory "$JAVA_HOME" 	      --strip-components 1 	      --no-same-owner 	  ;     rm -f /tmp/openjdk.tar.gz ${JAVA_HOME}/lib/src.zip;     find "$JAVA_HOME/lib" -name '*.so' -exec dirname '{}' ';' | sort -u > /etc/ld.so.conf.d/docker-openjdk.conf;     ldconfig;     java -Xshare:dump;
# Tue, 08 Aug 2023 19:22:10 GMT
RUN echo Verifying install ...     && fileEncoding="$(echo 'System.out.println(System.getProperty("file.encoding"))' | jshell -s -)"; [ "$fileEncoding" = 'UTF-8' ]; rm -rf ~/.java     && echo javac --version && javac --version     && echo java --version && java --version     && echo Complete.
# Mon, 14 Aug 2023 18:10:05 GMT
COPY file:8b8864b3e02a33a579dc216fd51b28a6047bc8eeaa03045b258980fe0cf7fcb3 in /__cacert_entrypoint.sh 
# Mon, 14 Aug 2023 18:10:05 GMT
ENTRYPOINT ["/__cacert_entrypoint.sh"]
# Mon, 14 Aug 2023 18:10:05 GMT
CMD ["jshell"]
# Mon, 14 Aug 2023 19:14:17 GMT
CMD ["gradle"]
# Mon, 14 Aug 2023 19:14:17 GMT
ENV GRADLE_HOME=/opt/gradle
# Mon, 14 Aug 2023 19:14:18 GMT
RUN set -o errexit -o nounset     && echo "Adding gradle user and group"     && groupadd --system --gid 1000 gradle     && useradd --system --gid gradle --uid 1000 --shell /bin/bash --create-home gradle     && mkdir /home/gradle/.gradle     && chown --recursive gradle:gradle /home/gradle         && echo "Symlinking root Gradle cache to gradle Gradle cache"     && ln --symbolic /home/gradle/.gradle /root/.gradle
# Mon, 14 Aug 2023 19:14:18 GMT
VOLUME [/home/gradle/.gradle]
# Mon, 14 Aug 2023 19:14:18 GMT
WORKDIR /home/gradle
# Mon, 14 Aug 2023 19:14:36 GMT
RUN set -o errexit -o nounset     && apt-get update     && apt-get install --yes --no-install-recommends         unzip         wget                 bzr         git         git-lfs         mercurial         openssh-client         subversion     && rm --recursive --force /var/lib/apt/lists/*         && echo "Testing VCSes"     && which bzr     && which git     && which git-lfs     && which hg     && which svn
# Mon, 14 Aug 2023 19:14:37 GMT
ENV GRADLE_VERSION=8.2.1
# Mon, 14 Aug 2023 19:14:37 GMT
ARG GRADLE_DOWNLOAD_SHA256=03ec176d388f2aa99defcadc3ac6adf8dd2bce5145a129659537c0874dea5ad1
# Tue, 15 Aug 2023 23:20:17 GMT
# ARGS: GRADLE_DOWNLOAD_SHA256=03ec176d388f2aa99defcadc3ac6adf8dd2bce5145a129659537c0874dea5ad1
RUN set -o errexit -o nounset     && echo "Downloading Gradle"     && wget --no-verbose --output-document=gradle.zip "https://services.gradle.org/distributions/gradle-${GRADLE_VERSION}-bin.zip"         && echo "Checking Gradle download hash"     && echo "${GRADLE_DOWNLOAD_SHA256} *gradle.zip" | sha256sum --check -         && echo "Installing Gradle"     && unzip gradle.zip     && rm gradle.zip     && mv "gradle-${GRADLE_VERSION}" "${GRADLE_HOME}/"     && ln --symbolic "${GRADLE_HOME}/bin/gradle" /usr/bin/gradle         && echo "Testing Gradle installation"     && gradle --version
```

-	Layers:
	-	`sha256:7007490126efaae58924972668256aaeb4858e6c4537eb4257e1978719b958c7`  
		Last Modified: Tue, 01 Aug 2023 08:35:40 GMT  
		Size: 28.6 MB (28580671 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6f32e041863d53bbb7f9f65ba31f023a9f344dd4105bf5345c6e748e3cc3e71a`  
		Last Modified: Tue, 08 Aug 2023 19:26:48 GMT  
		Size: 16.9 MB (16919807 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0ed845eba6ff77c64654082d3598052901e73b088c0193d8f913a3f70986ba4d`  
		Last Modified: Tue, 08 Aug 2023 19:29:19 GMT  
		Size: 144.8 MB (144837891 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9fec33b4efce19118e13918719dc8749fb388bca9f90b03f2dc3b6b88e3c862c`  
		Last Modified: Tue, 08 Aug 2023 19:29:08 GMT  
		Size: 173.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e05b1ae642a382a478084f56e78084ccf25b814fcad7687d5416d52b4c2992ad`  
		Last Modified: Mon, 14 Aug 2023 18:15:08 GMT  
		Size: 731.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e22f1aabc4447a638afff9b481737c66abcaf1a4f0363cb486b34e50234a30c6`  
		Last Modified: Mon, 14 Aug 2023 19:21:06 GMT  
		Size: 4.4 KB (4359 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d99c66c4beefa3a0fdf500b1ca2673798409af5ec5e0873b7eddb5e529b5fe6d`  
		Last Modified: Mon, 14 Aug 2023 19:21:16 GMT  
		Size: 65.5 MB (65487603 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9c3ba2692e426247152b78238bc1240157af03a8f13eebf783c90ff6c066301e`  
		Last Modified: Tue, 15 Aug 2023 23:26:13 GMT  
		Size: 128.7 MB (128727090 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `gradle:jdk11-focal` - linux; arm variant v7

```console
$ docker pull gradle@sha256:ef1e28129ec5f723de31f117ddb0bf0f0805b8f1db1a5b1f7b4dadffb3d8c970
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **366.5 MB (366485336 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:2ef0d00faaa95ec6269a44bbd4c356b3b0a259f995ee64f0677a51e49c8b752d`
-	Entrypoint: `["\/__cacert_entrypoint.sh"]`
-	Default Command: `["gradle"]`

```dockerfile
# Tue, 01 Aug 2023 06:16:45 GMT
ARG RELEASE
# Tue, 01 Aug 2023 06:16:45 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Tue, 01 Aug 2023 06:16:46 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Tue, 01 Aug 2023 06:16:46 GMT
LABEL org.opencontainers.image.version=20.04
# Tue, 01 Aug 2023 06:16:49 GMT
ADD file:60aa8465a6ba5538decc41365cc9b78ae86131e8c2cfc9177b4a336354ead988 in / 
# Tue, 01 Aug 2023 06:16:50 GMT
CMD ["/bin/bash"]
# Thu, 03 Aug 2023 01:27:39 GMT
ENV JAVA_HOME=/opt/java/openjdk
# Thu, 03 Aug 2023 01:27:39 GMT
ENV PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 03 Aug 2023 01:27:39 GMT
ENV LANG=en_US.UTF-8 LANGUAGE=en_US:en LC_ALL=en_US.UTF-8
# Tue, 08 Aug 2023 18:57:54 GMT
RUN apt-get update     && DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends tzdata curl wget ca-certificates fontconfig locales p11-kit     && echo "en_US.UTF-8 UTF-8" >> /etc/locale.gen     && locale-gen en_US.UTF-8     && rm -rf /var/lib/apt/lists/*
# Tue, 08 Aug 2023 18:59:47 GMT
ENV JAVA_VERSION=jdk-11.0.20+8
# Tue, 08 Aug 2023 18:59:58 GMT
RUN set -eux;     ARCH="$(dpkg --print-architecture)";     case "${ARCH}" in        aarch64|arm64)          ESUM='eb821c049c2d2f7c3fbf8ddcce2d608d3aa7d488700e76bfbbebabba93021748';          BINARY_URL='https://github.com/adoptium/temurin11-binaries/releases/download/jdk-11.0.20%2B8/OpenJDK11U-jdk_aarch64_linux_hotspot_11.0.20_8.tar.gz';          ;;        armhf|arm)          ESUM='fdf98d94ac3fd49a73a534fd88cf60e757e885c04791d15f76ccfcecb43a25e0';          BINARY_URL='https://github.com/adoptium/temurin11-binaries/releases/download/jdk-11.0.20%2B8/OpenJDK11U-jdk_arm_linux_hotspot_11.0.20_8.tar.gz';          ;;        ppc64el|powerpc:common64)          ESUM='1125931b3a38e6e305a1932fc6cfd0b023a0fbec2cab10e835a2ee2c50848b42';          BINARY_URL='https://github.com/adoptium/temurin11-binaries/releases/download/jdk-11.0.20%2B8/OpenJDK11U-jdk_ppc64le_linux_hotspot_11.0.20_8.tar.gz';          ;;        s390x|s390:64-bit)          ESUM='688c83d9edf2204220df94ce5bab4a6d19f3d91bc0e500f31dda41e16d9a383f';          BINARY_URL='https://github.com/adoptium/temurin11-binaries/releases/download/jdk-11.0.20%2B8/OpenJDK11U-jdk_s390x_linux_hotspot_11.0.20_8.tar.gz';          ;;        amd64|i386:x86-64)          ESUM='7a99258af2e3ee9047e90f1c0c1775fd6285085759501295358d934d662e01f9';          BINARY_URL='https://github.com/adoptium/temurin11-binaries/releases/download/jdk-11.0.20%2B8/OpenJDK11U-jdk_x64_linux_hotspot_11.0.20_8.tar.gz';          ;;        *)          echo "Unsupported arch: ${ARCH}";          exit 1;          ;;     esac; 	  wget -O /tmp/openjdk.tar.gz ${BINARY_URL}; 	  echo "${ESUM} */tmp/openjdk.tar.gz" | sha256sum -c -; 	  mkdir -p "$JAVA_HOME"; 	  tar --extract 	      --file /tmp/openjdk.tar.gz 	      --directory "$JAVA_HOME" 	      --strip-components 1 	      --no-same-owner 	  ;     rm -f /tmp/openjdk.tar.gz ${JAVA_HOME}/lib/src.zip;     find "$JAVA_HOME/lib" -name '*.so' -exec dirname '{}' ';' | sort -u > /etc/ld.so.conf.d/docker-openjdk.conf;     ldconfig;     java -Xshare:dump;
# Tue, 08 Aug 2023 19:00:01 GMT
RUN echo Verifying install ...     && fileEncoding="$(echo 'System.out.println(System.getProperty("file.encoding"))' | jshell -s -)"; [ "$fileEncoding" = 'UTF-8' ]; rm -rf ~/.java     && echo javac --version && javac --version     && echo java --version && java --version     && echo Complete.
# Mon, 14 Aug 2023 18:09:41 GMT
COPY file:8b8864b3e02a33a579dc216fd51b28a6047bc8eeaa03045b258980fe0cf7fcb3 in /__cacert_entrypoint.sh 
# Mon, 14 Aug 2023 18:09:41 GMT
ENTRYPOINT ["/__cacert_entrypoint.sh"]
# Mon, 14 Aug 2023 18:09:41 GMT
CMD ["jshell"]
# Mon, 14 Aug 2023 18:34:01 GMT
CMD ["gradle"]
# Mon, 14 Aug 2023 18:34:01 GMT
ENV GRADLE_HOME=/opt/gradle
# Mon, 14 Aug 2023 18:34:02 GMT
RUN set -o errexit -o nounset     && echo "Adding gradle user and group"     && groupadd --system --gid 1000 gradle     && useradd --system --gid gradle --uid 1000 --shell /bin/bash --create-home gradle     && mkdir /home/gradle/.gradle     && chown --recursive gradle:gradle /home/gradle         && echo "Symlinking root Gradle cache to gradle Gradle cache"     && ln --symbolic /home/gradle/.gradle /root/.gradle
# Mon, 14 Aug 2023 18:34:02 GMT
VOLUME [/home/gradle/.gradle]
# Mon, 14 Aug 2023 18:34:02 GMT
WORKDIR /home/gradle
# Mon, 14 Aug 2023 18:34:20 GMT
RUN set -o errexit -o nounset     && apt-get update     && apt-get install --yes --no-install-recommends         unzip         wget                 bzr         git         git-lfs         mercurial         openssh-client         subversion     && rm --recursive --force /var/lib/apt/lists/*         && echo "Testing VCSes"     && which bzr     && which git     && which git-lfs     && which hg     && which svn
# Mon, 14 Aug 2023 18:34:21 GMT
ENV GRADLE_VERSION=8.2.1
# Mon, 14 Aug 2023 18:34:21 GMT
ARG GRADLE_DOWNLOAD_SHA256=03ec176d388f2aa99defcadc3ac6adf8dd2bce5145a129659537c0874dea5ad1
# Tue, 15 Aug 2023 22:57:55 GMT
# ARGS: GRADLE_DOWNLOAD_SHA256=03ec176d388f2aa99defcadc3ac6adf8dd2bce5145a129659537c0874dea5ad1
RUN set -o errexit -o nounset     && echo "Downloading Gradle"     && wget --no-verbose --output-document=gradle.zip "https://services.gradle.org/distributions/gradle-${GRADLE_VERSION}-bin.zip"         && echo "Checking Gradle download hash"     && echo "${GRADLE_DOWNLOAD_SHA256} *gradle.zip" | sha256sum --check -         && echo "Installing Gradle"     && unzip gradle.zip     && rm gradle.zip     && mv "gradle-${GRADLE_VERSION}" "${GRADLE_HOME}/"     && ln --symbolic "${GRADLE_HOME}/bin/gradle" /usr/bin/gradle         && echo "Testing Gradle installation"     && gradle --version
```

-	Layers:
	-	`sha256:c429b4536d4b2ab209b0a779f71ba68570f10acf9dd806c7e2011fce49bd5c97`  
		Last Modified: Wed, 02 Aug 2023 04:28:29 GMT  
		Size: 24.6 MB (24591882 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:91cd3a8f320fb2da0d9f7694604e369817023cd4b7b62173714bbff7cad25aae`  
		Last Modified: Tue, 08 Aug 2023 19:02:31 GMT  
		Size: 15.7 MB (15659457 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4ad1990e27ade14531ec7150a6a4cf3ed0ed676255c771a68a092e6eb89fe4ba`  
		Last Modified: Tue, 08 Aug 2023 19:03:57 GMT  
		Size: 137.4 MB (137406168 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c8920371c7c345e4d7c82ddf5775c110c0a98814e6666555b43ad5f939d3532d`  
		Last Modified: Tue, 08 Aug 2023 19:03:44 GMT  
		Size: 176.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8d9d4013242c9260910ba7dab1e82b91413849eed4679db25eea050d374c7381`  
		Last Modified: Mon, 14 Aug 2023 18:11:00 GMT  
		Size: 734.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bc2fae29b932bd3f21a54a4372e25e0c8e393fca87c01a8dd33be5be0500f0ea`  
		Last Modified: Mon, 14 Aug 2023 18:39:36 GMT  
		Size: 4.3 KB (4341 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e0cd1f6c82053dae1ca9772a58d44689134a28e2933e1edcf2265b18c49db867`  
		Last Modified: Mon, 14 Aug 2023 18:39:47 GMT  
		Size: 60.1 MB (60095490 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7c9164a8e630e0c691d7e64ea7b82abbd11d9b7bc9bb780afbb4ff29e5853d7f`  
		Last Modified: Tue, 15 Aug 2023 23:01:01 GMT  
		Size: 128.7 MB (128727088 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `gradle:jdk11-focal` - linux; arm64 variant v8

```console
$ docker pull gradle@sha256:be136029f4782649586fe9135fd131b71854a1bab2f4d3e0a62dd0ee7c83bd31
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **379.5 MB (379509866 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:5c35606b1fe3523a781a4f4f0ac69f50c02d95daad673f9454c3a018b6d5b29c`
-	Entrypoint: `["\/__cacert_entrypoint.sh"]`
-	Default Command: `["gradle"]`

```dockerfile
# Tue, 01 Aug 2023 06:20:56 GMT
ARG RELEASE
# Tue, 01 Aug 2023 06:20:56 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Tue, 01 Aug 2023 06:20:56 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Tue, 01 Aug 2023 06:20:57 GMT
LABEL org.opencontainers.image.version=20.04
# Tue, 01 Aug 2023 06:21:03 GMT
ADD file:ef6e767091d76c1461d099d5bc7a18c526ec80834cf87280803ab6480192f766 in / 
# Tue, 01 Aug 2023 06:21:03 GMT
CMD ["/bin/bash"]
# Thu, 03 Aug 2023 01:05:44 GMT
ENV JAVA_HOME=/opt/java/openjdk
# Thu, 03 Aug 2023 01:05:44 GMT
ENV PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 03 Aug 2023 01:05:44 GMT
ENV LANG=en_US.UTF-8 LANGUAGE=en_US:en LC_ALL=en_US.UTF-8
# Tue, 08 Aug 2023 19:40:01 GMT
RUN apt-get update     && DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends tzdata curl wget ca-certificates fontconfig locales p11-kit     && echo "en_US.UTF-8 UTF-8" >> /etc/locale.gen     && locale-gen en_US.UTF-8     && rm -rf /var/lib/apt/lists/*
# Tue, 08 Aug 2023 19:41:09 GMT
ENV JAVA_VERSION=jdk-11.0.20+8
# Tue, 08 Aug 2023 19:41:20 GMT
RUN set -eux;     ARCH="$(dpkg --print-architecture)";     case "${ARCH}" in        aarch64|arm64)          ESUM='eb821c049c2d2f7c3fbf8ddcce2d608d3aa7d488700e76bfbbebabba93021748';          BINARY_URL='https://github.com/adoptium/temurin11-binaries/releases/download/jdk-11.0.20%2B8/OpenJDK11U-jdk_aarch64_linux_hotspot_11.0.20_8.tar.gz';          ;;        armhf|arm)          ESUM='fdf98d94ac3fd49a73a534fd88cf60e757e885c04791d15f76ccfcecb43a25e0';          BINARY_URL='https://github.com/adoptium/temurin11-binaries/releases/download/jdk-11.0.20%2B8/OpenJDK11U-jdk_arm_linux_hotspot_11.0.20_8.tar.gz';          ;;        ppc64el|powerpc:common64)          ESUM='1125931b3a38e6e305a1932fc6cfd0b023a0fbec2cab10e835a2ee2c50848b42';          BINARY_URL='https://github.com/adoptium/temurin11-binaries/releases/download/jdk-11.0.20%2B8/OpenJDK11U-jdk_ppc64le_linux_hotspot_11.0.20_8.tar.gz';          ;;        s390x|s390:64-bit)          ESUM='688c83d9edf2204220df94ce5bab4a6d19f3d91bc0e500f31dda41e16d9a383f';          BINARY_URL='https://github.com/adoptium/temurin11-binaries/releases/download/jdk-11.0.20%2B8/OpenJDK11U-jdk_s390x_linux_hotspot_11.0.20_8.tar.gz';          ;;        amd64|i386:x86-64)          ESUM='7a99258af2e3ee9047e90f1c0c1775fd6285085759501295358d934d662e01f9';          BINARY_URL='https://github.com/adoptium/temurin11-binaries/releases/download/jdk-11.0.20%2B8/OpenJDK11U-jdk_x64_linux_hotspot_11.0.20_8.tar.gz';          ;;        *)          echo "Unsupported arch: ${ARCH}";          exit 1;          ;;     esac; 	  wget -O /tmp/openjdk.tar.gz ${BINARY_URL}; 	  echo "${ESUM} */tmp/openjdk.tar.gz" | sha256sum -c -; 	  mkdir -p "$JAVA_HOME"; 	  tar --extract 	      --file /tmp/openjdk.tar.gz 	      --directory "$JAVA_HOME" 	      --strip-components 1 	      --no-same-owner 	  ;     rm -f /tmp/openjdk.tar.gz ${JAVA_HOME}/lib/src.zip;     find "$JAVA_HOME/lib" -name '*.so' -exec dirname '{}' ';' | sort -u > /etc/ld.so.conf.d/docker-openjdk.conf;     ldconfig;     java -Xshare:dump;
# Tue, 08 Aug 2023 19:41:23 GMT
RUN echo Verifying install ...     && fileEncoding="$(echo 'System.out.println(System.getProperty("file.encoding"))' | jshell -s -)"; [ "$fileEncoding" = 'UTF-8' ]; rm -rf ~/.java     && echo javac --version && javac --version     && echo java --version && java --version     && echo Complete.
# Mon, 14 Aug 2023 18:09:07 GMT
COPY file:8b8864b3e02a33a579dc216fd51b28a6047bc8eeaa03045b258980fe0cf7fcb3 in /__cacert_entrypoint.sh 
# Mon, 14 Aug 2023 18:09:07 GMT
ENTRYPOINT ["/__cacert_entrypoint.sh"]
# Mon, 14 Aug 2023 18:09:07 GMT
CMD ["jshell"]
# Mon, 14 Aug 2023 18:47:00 GMT
CMD ["gradle"]
# Mon, 14 Aug 2023 18:47:00 GMT
ENV GRADLE_HOME=/opt/gradle
# Mon, 14 Aug 2023 18:47:00 GMT
RUN set -o errexit -o nounset     && echo "Adding gradle user and group"     && groupadd --system --gid 1000 gradle     && useradd --system --gid gradle --uid 1000 --shell /bin/bash --create-home gradle     && mkdir /home/gradle/.gradle     && chown --recursive gradle:gradle /home/gradle         && echo "Symlinking root Gradle cache to gradle Gradle cache"     && ln --symbolic /home/gradle/.gradle /root/.gradle
# Mon, 14 Aug 2023 18:47:00 GMT
VOLUME [/home/gradle/.gradle]
# Mon, 14 Aug 2023 18:47:00 GMT
WORKDIR /home/gradle
# Mon, 14 Aug 2023 18:47:15 GMT
RUN set -o errexit -o nounset     && apt-get update     && apt-get install --yes --no-install-recommends         unzip         wget                 bzr         git         git-lfs         mercurial         openssh-client         subversion     && rm --recursive --force /var/lib/apt/lists/*         && echo "Testing VCSes"     && which bzr     && which git     && which git-lfs     && which hg     && which svn
# Mon, 14 Aug 2023 18:47:16 GMT
ENV GRADLE_VERSION=8.2.1
# Mon, 14 Aug 2023 18:47:16 GMT
ARG GRADLE_DOWNLOAD_SHA256=03ec176d388f2aa99defcadc3ac6adf8dd2bce5145a129659537c0874dea5ad1
# Thu, 17 Aug 2023 01:12:52 GMT
# ARGS: GRADLE_DOWNLOAD_SHA256=03ec176d388f2aa99defcadc3ac6adf8dd2bce5145a129659537c0874dea5ad1
RUN set -o errexit -o nounset     && echo "Downloading Gradle"     && wget --no-verbose --output-document=gradle.zip "https://services.gradle.org/distributions/gradle-${GRADLE_VERSION}-bin.zip"         && echo "Checking Gradle download hash"     && echo "${GRADLE_DOWNLOAD_SHA256} *gradle.zip" | sha256sum --check -         && echo "Installing Gradle"     && unzip gradle.zip     && rm gradle.zip     && mv "gradle-${GRADLE_VERSION}" "${GRADLE_HOME}/"     && ln --symbolic "${GRADLE_HOME}/bin/gradle" /usr/bin/gradle
# Thu, 17 Aug 2023 01:12:53 GMT
USER gradle
# Thu, 17 Aug 2023 01:12:54 GMT
# ARGS: GRADLE_DOWNLOAD_SHA256=03ec176d388f2aa99defcadc3ac6adf8dd2bce5145a129659537c0874dea5ad1
RUN set -o errexit -o nounset     && echo "Testing Gradle installation"     && gradle --version
# Thu, 17 Aug 2023 01:12:54 GMT
USER root
```

-	Layers:
	-	`sha256:edab87ea811e56041127f5e9eb4115fb62cb96d0e6a14056e0d2dbf51a945a22`  
		Last Modified: Wed, 02 Aug 2023 04:28:23 GMT  
		Size: 27.2 MB (27200587 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:36d3de389f9fd6a81c60e4d6444266df2002734ab5660161fa9bf374cd8cd473`  
		Last Modified: Tue, 08 Aug 2023 19:44:02 GMT  
		Size: 16.8 MB (16770361 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:88c803c27d2200fb247385a0666816111596b67ef7d7e28595dc4384ee80a1ff`  
		Last Modified: Tue, 08 Aug 2023 19:45:50 GMT  
		Size: 141.6 MB (141571550 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:679890a142403ff758bd49535f3960d17ab7aeff31c1fcbe0c8631c876b66302`  
		Last Modified: Tue, 08 Aug 2023 19:45:40 GMT  
		Size: 171.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bab742585620ec5115efc61d71ec32b57cea1e5b6a6faa5ae752df4da8285f25`  
		Last Modified: Mon, 14 Aug 2023 18:11:58 GMT  
		Size: 733.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fdd19afa08c74871c3260e50bcae9de65c15b1086e64f1a9d972dd5e3e9515f7`  
		Last Modified: Mon, 14 Aug 2023 18:51:50 GMT  
		Size: 4.4 KB (4365 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:88d4b3e349639dec73815e0ea6134a127dd9a5392ce2738a853f656f5ccba9e8`  
		Last Modified: Mon, 14 Aug 2023 18:51:58 GMT  
		Size: 65.2 MB (65234898 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c1a151a18b47bb6f03d61999425ee26b3381a0867fc197bb14871639d8d5c9a5`  
		Last Modified: Thu, 17 Aug 2023 01:18:41 GMT  
		Size: 128.7 MB (128727029 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ff88b18d22588322b852e461e2a4afbeb1197ec18f55a6ab1b768f1988f608af`  
		Last Modified: Thu, 17 Aug 2023 01:18:35 GMT  
		Size: 172.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `gradle:jdk11-focal` - linux; ppc64le

```console
$ docker pull gradle@sha256:b0846517ffc960bee4799abafa6964a304e62a610e2fd1370de8c7d0c7118a60
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **386.1 MB (386095555 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:3dfb2c05de6c093647e6f96df00e1aebd03614307eaad2523cb5b1b136ed637d`
-	Entrypoint: `["\/__cacert_entrypoint.sh"]`
-	Default Command: `["gradle"]`

```dockerfile
# Tue, 01 Aug 2023 06:20:36 GMT
ARG RELEASE
# Tue, 01 Aug 2023 06:20:36 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Tue, 01 Aug 2023 06:20:37 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Tue, 01 Aug 2023 06:20:37 GMT
LABEL org.opencontainers.image.version=20.04
# Tue, 01 Aug 2023 06:20:40 GMT
ADD file:822df76493d1d533c1a283ab7bb20ce81309f57279422a0eebb2ffb9fab55963 in / 
# Tue, 01 Aug 2023 06:20:40 GMT
CMD ["/bin/bash"]
# Thu, 03 Aug 2023 02:44:09 GMT
ENV JAVA_HOME=/opt/java/openjdk
# Thu, 03 Aug 2023 02:44:10 GMT
ENV PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 03 Aug 2023 02:44:10 GMT
ENV LANG=en_US.UTF-8 LANGUAGE=en_US:en LC_ALL=en_US.UTF-8
# Tue, 08 Aug 2023 19:18:01 GMT
RUN apt-get update     && DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends tzdata curl wget ca-certificates fontconfig locales p11-kit     && echo "en_US.UTF-8 UTF-8" >> /etc/locale.gen     && locale-gen en_US.UTF-8     && rm -rf /var/lib/apt/lists/*
# Tue, 08 Aug 2023 19:20:50 GMT
ENV JAVA_VERSION=jdk-11.0.20+8
# Tue, 08 Aug 2023 19:21:08 GMT
RUN set -eux;     ARCH="$(dpkg --print-architecture)";     case "${ARCH}" in        aarch64|arm64)          ESUM='eb821c049c2d2f7c3fbf8ddcce2d608d3aa7d488700e76bfbbebabba93021748';          BINARY_URL='https://github.com/adoptium/temurin11-binaries/releases/download/jdk-11.0.20%2B8/OpenJDK11U-jdk_aarch64_linux_hotspot_11.0.20_8.tar.gz';          ;;        armhf|arm)          ESUM='fdf98d94ac3fd49a73a534fd88cf60e757e885c04791d15f76ccfcecb43a25e0';          BINARY_URL='https://github.com/adoptium/temurin11-binaries/releases/download/jdk-11.0.20%2B8/OpenJDK11U-jdk_arm_linux_hotspot_11.0.20_8.tar.gz';          ;;        ppc64el|powerpc:common64)          ESUM='1125931b3a38e6e305a1932fc6cfd0b023a0fbec2cab10e835a2ee2c50848b42';          BINARY_URL='https://github.com/adoptium/temurin11-binaries/releases/download/jdk-11.0.20%2B8/OpenJDK11U-jdk_ppc64le_linux_hotspot_11.0.20_8.tar.gz';          ;;        s390x|s390:64-bit)          ESUM='688c83d9edf2204220df94ce5bab4a6d19f3d91bc0e500f31dda41e16d9a383f';          BINARY_URL='https://github.com/adoptium/temurin11-binaries/releases/download/jdk-11.0.20%2B8/OpenJDK11U-jdk_s390x_linux_hotspot_11.0.20_8.tar.gz';          ;;        amd64|i386:x86-64)          ESUM='7a99258af2e3ee9047e90f1c0c1775fd6285085759501295358d934d662e01f9';          BINARY_URL='https://github.com/adoptium/temurin11-binaries/releases/download/jdk-11.0.20%2B8/OpenJDK11U-jdk_x64_linux_hotspot_11.0.20_8.tar.gz';          ;;        *)          echo "Unsupported arch: ${ARCH}";          exit 1;          ;;     esac; 	  wget -O /tmp/openjdk.tar.gz ${BINARY_URL}; 	  echo "${ESUM} */tmp/openjdk.tar.gz" | sha256sum -c -; 	  mkdir -p "$JAVA_HOME"; 	  tar --extract 	      --file /tmp/openjdk.tar.gz 	      --directory "$JAVA_HOME" 	      --strip-components 1 	      --no-same-owner 	  ;     rm -f /tmp/openjdk.tar.gz ${JAVA_HOME}/lib/src.zip;     find "$JAVA_HOME/lib" -name '*.so' -exec dirname '{}' ';' | sort -u > /etc/ld.so.conf.d/docker-openjdk.conf;     ldconfig;     java -Xshare:dump;
# Tue, 08 Aug 2023 19:21:17 GMT
RUN echo Verifying install ...     && fileEncoding="$(echo 'System.out.println(System.getProperty("file.encoding"))' | jshell -s -)"; [ "$fileEncoding" = 'UTF-8' ]; rm -rf ~/.java     && echo javac --version && javac --version     && echo java --version && java --version     && echo Complete.
# Mon, 14 Aug 2023 18:09:33 GMT
COPY file:8b8864b3e02a33a579dc216fd51b28a6047bc8eeaa03045b258980fe0cf7fcb3 in /__cacert_entrypoint.sh 
# Mon, 14 Aug 2023 18:09:33 GMT
ENTRYPOINT ["/__cacert_entrypoint.sh"]
# Mon, 14 Aug 2023 18:09:33 GMT
CMD ["jshell"]
# Mon, 14 Aug 2023 19:10:19 GMT
CMD ["gradle"]
# Mon, 14 Aug 2023 19:10:20 GMT
ENV GRADLE_HOME=/opt/gradle
# Mon, 14 Aug 2023 19:10:22 GMT
RUN set -o errexit -o nounset     && echo "Adding gradle user and group"     && groupadd --system --gid 1000 gradle     && useradd --system --gid gradle --uid 1000 --shell /bin/bash --create-home gradle     && mkdir /home/gradle/.gradle     && chown --recursive gradle:gradle /home/gradle         && echo "Symlinking root Gradle cache to gradle Gradle cache"     && ln --symbolic /home/gradle/.gradle /root/.gradle
# Mon, 14 Aug 2023 19:10:23 GMT
VOLUME [/home/gradle/.gradle]
# Mon, 14 Aug 2023 19:10:23 GMT
WORKDIR /home/gradle
# Mon, 14 Aug 2023 19:11:28 GMT
RUN set -o errexit -o nounset     && apt-get update     && apt-get install --yes --no-install-recommends         unzip         wget                 bzr         git         git-lfs         mercurial         openssh-client         subversion     && rm --recursive --force /var/lib/apt/lists/*         && echo "Testing VCSes"     && which bzr     && which git     && which git-lfs     && which hg     && which svn
# Mon, 14 Aug 2023 19:11:32 GMT
ENV GRADLE_VERSION=8.2.1
# Mon, 14 Aug 2023 19:11:33 GMT
ARG GRADLE_DOWNLOAD_SHA256=03ec176d388f2aa99defcadc3ac6adf8dd2bce5145a129659537c0874dea5ad1
# Tue, 15 Aug 2023 23:17:52 GMT
# ARGS: GRADLE_DOWNLOAD_SHA256=03ec176d388f2aa99defcadc3ac6adf8dd2bce5145a129659537c0874dea5ad1
RUN set -o errexit -o nounset     && echo "Downloading Gradle"     && wget --no-verbose --output-document=gradle.zip "https://services.gradle.org/distributions/gradle-${GRADLE_VERSION}-bin.zip"         && echo "Checking Gradle download hash"     && echo "${GRADLE_DOWNLOAD_SHA256} *gradle.zip" | sha256sum --check -         && echo "Installing Gradle"     && unzip gradle.zip     && rm gradle.zip     && mv "gradle-${GRADLE_VERSION}" "${GRADLE_HOME}/"     && ln --symbolic "${GRADLE_HOME}/bin/gradle" /usr/bin/gradle         && echo "Testing Gradle installation"     && gradle --version
```

-	Layers:
	-	`sha256:be0253994e7bea97e6b44cdeec04bf996c8dd3380e70409de3783a1d1971e747`  
		Last Modified: Thu, 03 Aug 2023 02:50:24 GMT  
		Size: 33.3 MB (33306772 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:af03d96af036322b1cf090be8f29d0a3931c623558764bccaca2826ee7b9af6b`  
		Last Modified: Tue, 08 Aug 2023 19:28:27 GMT  
		Size: 18.2 MB (18215568 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:940753c995cfcec994576831e89ce855433c66dd41114ed4594bbfaf42b32bd5`  
		Last Modified: Tue, 08 Aug 2023 19:31:19 GMT  
		Size: 132.0 MB (132002777 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3d6ae2db5a2cb42af386a1a7f7c50f847cd83d4a64faf780497968140b8bcc30`  
		Last Modified: Tue, 08 Aug 2023 19:31:01 GMT  
		Size: 175.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9792a1c0ec22cff6e43676641c40a568b8fca7fee9b1e81327619466b2f2a695`  
		Last Modified: Mon, 14 Aug 2023 18:13:46 GMT  
		Size: 734.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:63a8105fd46bd181bf29191638fabc331f8a992e601437de1bec915c54a4f785`  
		Last Modified: Mon, 14 Aug 2023 19:23:42 GMT  
		Size: 4.4 KB (4360 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1a653efdc537a5e900cec6c6c94b9ff47c2961198fceec722205c9b3a76bd081`  
		Last Modified: Mon, 14 Aug 2023 19:24:03 GMT  
		Size: 73.8 MB (73838109 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:128ce1998e1b6c3226b106d4b4c58471b0bad0dffd40803a0f9b4f944ec45b41`  
		Last Modified: Tue, 15 Aug 2023 23:22:59 GMT  
		Size: 128.7 MB (128727060 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `gradle:jdk11-focal` - linux; s390x

```console
$ docker pull gradle@sha256:72db494570bbea88a2efa6d9fda667f5730e005c258cd46e0a78efaf85b0a8d4
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **362.3 MB (362321720 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:36d49b1c55bd5c378d823a1f7ccec2344602d8040ee0696808c0439ad330768b`
-	Entrypoint: `["\/__cacert_entrypoint.sh"]`
-	Default Command: `["gradle"]`

```dockerfile
# Tue, 01 Aug 2023 06:17:39 GMT
ARG RELEASE
# Tue, 01 Aug 2023 06:17:39 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Tue, 01 Aug 2023 06:17:39 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Tue, 01 Aug 2023 06:17:39 GMT
LABEL org.opencontainers.image.version=20.04
# Tue, 01 Aug 2023 06:17:41 GMT
ADD file:36efc3ec29bb54e0987fe91be1aa7cc849909b3cd2534af3de2d3d07a03804cf in / 
# Tue, 01 Aug 2023 06:17:41 GMT
CMD ["/bin/bash"]
# Thu, 03 Aug 2023 00:24:09 GMT
ENV JAVA_HOME=/opt/java/openjdk
# Thu, 03 Aug 2023 00:24:09 GMT
ENV PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 03 Aug 2023 00:24:09 GMT
ENV LANG=en_US.UTF-8 LANGUAGE=en_US:en LC_ALL=en_US.UTF-8
# Tue, 08 Aug 2023 19:42:12 GMT
RUN apt-get update     && DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends tzdata curl wget ca-certificates fontconfig locales p11-kit     && echo "en_US.UTF-8 UTF-8" >> /etc/locale.gen     && locale-gen en_US.UTF-8     && rm -rf /var/lib/apt/lists/*
# Tue, 08 Aug 2023 19:42:13 GMT
ENV JAVA_VERSION=jdk-11.0.20+8
# Tue, 08 Aug 2023 19:42:20 GMT
RUN set -eux;     ARCH="$(dpkg --print-architecture)";     case "${ARCH}" in        aarch64|arm64)          ESUM='eb821c049c2d2f7c3fbf8ddcce2d608d3aa7d488700e76bfbbebabba93021748';          BINARY_URL='https://github.com/adoptium/temurin11-binaries/releases/download/jdk-11.0.20%2B8/OpenJDK11U-jdk_aarch64_linux_hotspot_11.0.20_8.tar.gz';          ;;        armhf|arm)          ESUM='fdf98d94ac3fd49a73a534fd88cf60e757e885c04791d15f76ccfcecb43a25e0';          BINARY_URL='https://github.com/adoptium/temurin11-binaries/releases/download/jdk-11.0.20%2B8/OpenJDK11U-jdk_arm_linux_hotspot_11.0.20_8.tar.gz';          ;;        ppc64el|powerpc:common64)          ESUM='1125931b3a38e6e305a1932fc6cfd0b023a0fbec2cab10e835a2ee2c50848b42';          BINARY_URL='https://github.com/adoptium/temurin11-binaries/releases/download/jdk-11.0.20%2B8/OpenJDK11U-jdk_ppc64le_linux_hotspot_11.0.20_8.tar.gz';          ;;        s390x|s390:64-bit)          ESUM='688c83d9edf2204220df94ce5bab4a6d19f3d91bc0e500f31dda41e16d9a383f';          BINARY_URL='https://github.com/adoptium/temurin11-binaries/releases/download/jdk-11.0.20%2B8/OpenJDK11U-jdk_s390x_linux_hotspot_11.0.20_8.tar.gz';          ;;        amd64|i386:x86-64)          ESUM='7a99258af2e3ee9047e90f1c0c1775fd6285085759501295358d934d662e01f9';          BINARY_URL='https://github.com/adoptium/temurin11-binaries/releases/download/jdk-11.0.20%2B8/OpenJDK11U-jdk_x64_linux_hotspot_11.0.20_8.tar.gz';          ;;        *)          echo "Unsupported arch: ${ARCH}";          exit 1;          ;;     esac; 	  wget -O /tmp/openjdk.tar.gz ${BINARY_URL}; 	  echo "${ESUM} */tmp/openjdk.tar.gz" | sha256sum -c -; 	  mkdir -p "$JAVA_HOME"; 	  tar --extract 	      --file /tmp/openjdk.tar.gz 	      --directory "$JAVA_HOME" 	      --strip-components 1 	      --no-same-owner 	  ;     rm -f /tmp/openjdk.tar.gz ${JAVA_HOME}/lib/src.zip;     find "$JAVA_HOME/lib" -name '*.so' -exec dirname '{}' ';' | sort -u > /etc/ld.so.conf.d/docker-openjdk.conf;     ldconfig;     java -Xshare:dump;
# Tue, 08 Aug 2023 19:42:24 GMT
RUN echo Verifying install ...     && fileEncoding="$(echo 'System.out.println(System.getProperty("file.encoding"))' | jshell -s -)"; [ "$fileEncoding" = 'UTF-8' ]; rm -rf ~/.java     && echo javac --version && javac --version     && echo java --version && java --version     && echo Complete.
# Mon, 14 Aug 2023 18:09:05 GMT
COPY file:8b8864b3e02a33a579dc216fd51b28a6047bc8eeaa03045b258980fe0cf7fcb3 in /__cacert_entrypoint.sh 
# Mon, 14 Aug 2023 18:09:05 GMT
ENTRYPOINT ["/__cacert_entrypoint.sh"]
# Mon, 14 Aug 2023 18:09:05 GMT
CMD ["jshell"]
# Mon, 14 Aug 2023 18:31:22 GMT
CMD ["gradle"]
# Mon, 14 Aug 2023 18:31:22 GMT
ENV GRADLE_HOME=/opt/gradle
# Mon, 14 Aug 2023 18:31:23 GMT
RUN set -o errexit -o nounset     && echo "Adding gradle user and group"     && groupadd --system --gid 1000 gradle     && useradd --system --gid gradle --uid 1000 --shell /bin/bash --create-home gradle     && mkdir /home/gradle/.gradle     && chown --recursive gradle:gradle /home/gradle         && echo "Symlinking root Gradle cache to gradle Gradle cache"     && ln --symbolic /home/gradle/.gradle /root/.gradle
# Mon, 14 Aug 2023 18:31:23 GMT
VOLUME [/home/gradle/.gradle]
# Mon, 14 Aug 2023 18:31:23 GMT
WORKDIR /home/gradle
# Mon, 14 Aug 2023 18:32:11 GMT
RUN set -o errexit -o nounset     && apt-get update     && apt-get install --yes --no-install-recommends         unzip         wget                 bzr         git         git-lfs         mercurial         openssh-client         subversion     && rm --recursive --force /var/lib/apt/lists/*         && echo "Testing VCSes"     && which bzr     && which git     && which git-lfs     && which hg     && which svn
# Mon, 14 Aug 2023 18:32:16 GMT
ENV GRADLE_VERSION=8.2.1
# Mon, 14 Aug 2023 18:32:16 GMT
ARG GRADLE_DOWNLOAD_SHA256=03ec176d388f2aa99defcadc3ac6adf8dd2bce5145a129659537c0874dea5ad1
# Thu, 17 Aug 2023 00:43:02 GMT
# ARGS: GRADLE_DOWNLOAD_SHA256=03ec176d388f2aa99defcadc3ac6adf8dd2bce5145a129659537c0874dea5ad1
RUN set -o errexit -o nounset     && echo "Downloading Gradle"     && wget --no-verbose --output-document=gradle.zip "https://services.gradle.org/distributions/gradle-${GRADLE_VERSION}-bin.zip"         && echo "Checking Gradle download hash"     && echo "${GRADLE_DOWNLOAD_SHA256} *gradle.zip" | sha256sum --check -         && echo "Installing Gradle"     && unzip gradle.zip     && rm gradle.zip     && mv "gradle-${GRADLE_VERSION}" "${GRADLE_HOME}/"     && ln --symbolic "${GRADLE_HOME}/bin/gradle" /usr/bin/gradle
# Thu, 17 Aug 2023 00:43:06 GMT
USER gradle
# Thu, 17 Aug 2023 00:43:08 GMT
# ARGS: GRADLE_DOWNLOAD_SHA256=03ec176d388f2aa99defcadc3ac6adf8dd2bce5145a129659537c0874dea5ad1
RUN set -o errexit -o nounset     && echo "Testing Gradle installation"     && gradle --version
# Thu, 17 Aug 2023 00:43:08 GMT
USER root
```

-	Layers:
	-	`sha256:365fa2124eb5f6f369204f3fe0210d9965952628707dfacd4194a8e15caf0420`  
		Last Modified: Thu, 03 Aug 2023 00:03:37 GMT  
		Size: 27.0 MB (27014233 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ff4bb71ff7cf2cdfba432549f8f118e2394ed9d63653317801c650fc5cdf556b`  
		Last Modified: Tue, 08 Aug 2023 19:46:12 GMT  
		Size: 16.6 MB (16643421 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:91b9f1937d0278d3991f9dc15a84261af1bc814f27411e6aa5774265b0158d24`  
		Last Modified: Tue, 08 Aug 2023 19:46:19 GMT  
		Size: 125.1 MB (125135954 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5510761437258e07ebcc6619f18216e87c0006d5421400b3adbf0739b76a4729`  
		Last Modified: Tue, 08 Aug 2023 19:46:09 GMT  
		Size: 172.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8afcf44c91de3d3c4b246cdde53e5b08eb01574eeb9bbaf1e927c00e547fd969`  
		Last Modified: Mon, 14 Aug 2023 18:11:03 GMT  
		Size: 733.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:93354c2142bbe36e62a638cdafc5e805d0a9730e12beea9fd90b5b14f3413e96`  
		Last Modified: Mon, 14 Aug 2023 18:38:06 GMT  
		Size: 4.4 KB (4363 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:84ad92c2fd0d6747de454f9253eb649f21b7fd8be1926e5c5ed8a03378d35d40`  
		Last Modified: Mon, 14 Aug 2023 18:38:16 GMT  
		Size: 64.8 MB (64795644 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f074070369985b9212d3cee69bb795c5404ee00462dd0b79a6c00002e6898a7c`  
		Last Modified: Thu, 17 Aug 2023 00:47:59 GMT  
		Size: 128.7 MB (128727029 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:44e9731d518ed1a481d87b52aa5537d577c9e284c019b0ac285959907077ad7f`  
		Last Modified: Thu, 17 Aug 2023 00:47:52 GMT  
		Size: 171.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
