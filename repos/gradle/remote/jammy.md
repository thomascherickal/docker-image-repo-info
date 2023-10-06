## `gradle:jammy`

```console
$ docker pull gradle@sha256:099eb6f6c2050264d29a8e433a8554753b77936ba983445a00ba5485970d9b40
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 5
	-	linux; amd64
	-	linux; arm variant v7
	-	linux; arm64 variant v8
	-	linux; ppc64le
	-	linux; s390x

### `gradle:jammy` - linux; amd64

```console
$ docker pull gradle@sha256:05084968493d4cda45759ba15dde424f0c1f14d680524a9a4479c4880fe02532
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **374.9 MB (374903917 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:bab2a91004a34b2556a65f65bcd90e320283d067d1470d63bf706f3527efef2f`
-	Entrypoint: `["\/__cacert_entrypoint.sh"]`
-	Default Command: `["gradle"]`

```dockerfile
# Mon, 25 Sep 2023 10:17:05 GMT
ARG RELEASE
# Mon, 25 Sep 2023 10:17:05 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Mon, 25 Sep 2023 10:17:05 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Mon, 25 Sep 2023 10:17:05 GMT
LABEL org.opencontainers.image.version=22.04
# Mon, 25 Sep 2023 10:17:07 GMT
ADD file:194c886b88876c1804cc5f80719669653c16a388b664147b7f22402105f533c4 in / 
# Mon, 25 Sep 2023 10:17:08 GMT
CMD ["/bin/bash"]
# Tue, 03 Oct 2023 05:11:45 GMT
ENV JAVA_HOME=/opt/java/openjdk
# Tue, 03 Oct 2023 05:11:45 GMT
ENV PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 03 Oct 2023 05:11:45 GMT
ENV LANG=en_US.UTF-8 LANGUAGE=en_US:en LC_ALL=en_US.UTF-8
# Tue, 03 Oct 2023 05:13:30 GMT
RUN apt-get update     && DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends tzdata curl wget ca-certificates fontconfig locales p11-kit binutils     && echo "en_US.UTF-8 UTF-8" >> /etc/locale.gen     && locale-gen en_US.UTF-8     && rm -rf /var/lib/apt/lists/*
# Tue, 03 Oct 2023 05:13:30 GMT
ENV JAVA_VERSION=jdk-17.0.8.1+1
# Tue, 03 Oct 2023 05:13:39 GMT
RUN set -eux;     ARCH="$(dpkg --print-architecture)";     case "${ARCH}" in        aarch64|arm64)          ESUM='eefd3cf3b3dd47ff269fa5b5c10b5e096b163f4e9c1810023abdbc00dc6cc304';          BINARY_URL='https://github.com/adoptium/temurin17-binaries/releases/download/jdk-17.0.8.1%2B1/OpenJDK17U-jdk_aarch64_linux_hotspot_17.0.8.1_1.tar.gz';          ;;        armhf|arm)          ESUM='b1f1d8b7fcb159a0a8029b6c3106d1d16207cecbb2047f9a4be2a64d29897da5';          BINARY_URL='https://github.com/adoptium/temurin17-binaries/releases/download/jdk-17.0.8.1%2B1/OpenJDK17U-jdk_arm_linux_hotspot_17.0.8.1_1.tar.gz';          ;;        ppc64el|powerpc:common64)          ESUM='00a4c07603d0218cd678461b5b3b7e25b3253102da4022d31fc35907f21a2efd';          BINARY_URL='https://github.com/adoptium/temurin17-binaries/releases/download/jdk-17.0.8.1%2B1/OpenJDK17U-jdk_ppc64le_linux_hotspot_17.0.8.1_1.tar.gz';          ;;        s390x|s390:64-bit)          ESUM='ffacba69c6843d7ca70d572489d6cc7ab7ae52c60f0852cedf4cf0d248b6fc37';          BINARY_URL='https://github.com/adoptium/temurin17-binaries/releases/download/jdk-17.0.8.1%2B1/OpenJDK17U-jdk_s390x_linux_hotspot_17.0.8.1_1.tar.gz';          ;;        amd64|i386:x86-64)          ESUM='c25dfbc334068a48c19c44ce39ad4b8427e309ae1cfa83f23c102e78b8a6dcc0';          BINARY_URL='https://github.com/adoptium/temurin17-binaries/releases/download/jdk-17.0.8.1%2B1/OpenJDK17U-jdk_x64_linux_hotspot_17.0.8.1_1.tar.gz';          ;;        *)          echo "Unsupported arch: ${ARCH}";          exit 1;          ;;     esac; 	  wget -O /tmp/openjdk.tar.gz ${BINARY_URL}; 	  echo "${ESUM} */tmp/openjdk.tar.gz" | sha256sum -c -; 	  mkdir -p "$JAVA_HOME"; 	  tar --extract 	      --file /tmp/openjdk.tar.gz 	      --directory "$JAVA_HOME" 	      --strip-components 1 	      --no-same-owner 	  ;     rm -f /tmp/openjdk.tar.gz ${JAVA_HOME}/lib/src.zip;     find "$JAVA_HOME/lib" -name '*.so' -exec dirname '{}' ';' | sort -u > /etc/ld.so.conf.d/docker-openjdk.conf;     ldconfig;     java -Xshare:dump;
# Tue, 03 Oct 2023 05:13:41 GMT
RUN echo Verifying install ...     && fileEncoding="$(echo 'System.out.println(System.getProperty("file.encoding"))' | jshell -s -)"; [ "$fileEncoding" = 'UTF-8' ]; rm -rf ~/.java     && echo javac --version && javac --version     && echo java --version && java --version     && echo Complete.
# Tue, 03 Oct 2023 05:13:41 GMT
COPY file:8b8864b3e02a33a579dc216fd51b28a6047bc8eeaa03045b258980fe0cf7fcb3 in /__cacert_entrypoint.sh 
# Tue, 03 Oct 2023 05:13:41 GMT
ENTRYPOINT ["/__cacert_entrypoint.sh"]
# Tue, 03 Oct 2023 05:13:41 GMT
CMD ["jshell"]
# Tue, 03 Oct 2023 07:00:02 GMT
CMD ["gradle"]
# Tue, 03 Oct 2023 07:00:02 GMT
ENV GRADLE_HOME=/opt/gradle
# Tue, 03 Oct 2023 07:00:03 GMT
RUN set -o errexit -o nounset     && echo "Adding gradle user and group"     && groupadd --system --gid 1000 gradle     && useradd --system --gid gradle --uid 1000 --shell /bin/bash --create-home gradle     && mkdir /home/gradle/.gradle     && chown --recursive gradle:gradle /home/gradle         && echo "Symlinking root Gradle cache to gradle Gradle cache"     && ln --symbolic /home/gradle/.gradle /root/.gradle
# Tue, 03 Oct 2023 07:00:03 GMT
VOLUME [/home/gradle/.gradle]
# Tue, 03 Oct 2023 07:00:03 GMT
WORKDIR /home/gradle
# Tue, 03 Oct 2023 07:00:18 GMT
RUN set -o errexit -o nounset     && apt-get update     && apt-get install --yes --no-install-recommends         unzip         wget                 bzr         git         git-lfs         mercurial         openssh-client         subversion     && rm --recursive --force /var/lib/apt/lists/*         && echo "Testing VCSes"     && which bzr     && which git     && which git-lfs     && which hg     && which svn
# Tue, 03 Oct 2023 07:00:19 GMT
ENV GRADLE_VERSION=8.3
# Tue, 03 Oct 2023 07:00:19 GMT
ARG GRADLE_DOWNLOAD_SHA256=591855b517fc635b9e04de1d05d5e76ada3f89f5fc76f87978d1b245b4f69225
# Tue, 03 Oct 2023 07:00:23 GMT
# ARGS: GRADLE_DOWNLOAD_SHA256=591855b517fc635b9e04de1d05d5e76ada3f89f5fc76f87978d1b245b4f69225
RUN set -o errexit -o nounset     && echo "Downloading Gradle"     && wget --no-verbose --output-document=gradle.zip "https://services.gradle.org/distributions/gradle-${GRADLE_VERSION}-bin.zip"         && echo "Checking Gradle download hash"     && echo "${GRADLE_DOWNLOAD_SHA256} *gradle.zip" | sha256sum --check -         && echo "Installing Gradle"     && unzip gradle.zip     && rm gradle.zip     && mv "gradle-${GRADLE_VERSION}" "${GRADLE_HOME}/"     && ln --symbolic "${GRADLE_HOME}/bin/gradle" /usr/bin/gradle
# Tue, 03 Oct 2023 07:00:23 GMT
USER gradle
# Tue, 03 Oct 2023 07:00:25 GMT
# ARGS: GRADLE_DOWNLOAD_SHA256=591855b517fc635b9e04de1d05d5e76ada3f89f5fc76f87978d1b245b4f69225
RUN set -o errexit -o nounset     && echo "Testing Gradle installation"     && gradle --version
# Tue, 03 Oct 2023 07:00:25 GMT
USER root
```

-	Layers:
	-	`sha256:707e32e9fc569fee476af9e92ae3d1df8b8e6dca47f9cb31db9d2c922a6de952`  
		Last Modified: Mon, 25 Sep 2023 12:54:05 GMT  
		Size: 30.4 MB (30440869 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8e560b9ae2a605cbabd174647e334b0807409ab4cdb14e3ffa28655f8e033811`  
		Last Modified: Tue, 03 Oct 2023 05:17:36 GMT  
		Size: 17.5 MB (17455429 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2a200e428b29b17c8b134286a64173f5831f00680858051961b5ca7505306d59`  
		Last Modified: Tue, 03 Oct 2023 05:17:45 GMT  
		Size: 144.8 MB (144778433 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3cc43ecfdc127e5008009135350763c92b0750409668ab2304125d4e657891ef`  
		Last Modified: Tue, 03 Oct 2023 05:17:34 GMT  
		Size: 173.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8ef680a12b1abdae0115a150b78eb9007d4d676c8bd48ddd8a63b50a1f58df57`  
		Last Modified: Tue, 03 Oct 2023 05:17:34 GMT  
		Size: 734.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3336aac7641834ee464fc1ca10f25df598ef659aae0c5ac51f3f96073417160a`  
		Last Modified: Tue, 03 Oct 2023 07:06:50 GMT  
		Size: 4.4 KB (4364 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:92385c6b273f24d2ce04246a4dbb09c587583c035371050091452c917ab6087b`  
		Last Modified: Tue, 03 Oct 2023 07:06:59 GMT  
		Size: 51.6 MB (51556476 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:20a23d1d68c60b5001082bd7a6ca59e57fbf323f7148e14a456ff5e89bf4988f`  
		Last Modified: Tue, 03 Oct 2023 07:06:57 GMT  
		Size: 130.7 MB (130667270 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:42900feea052f01ec479fd863cfeb97423c535e19e4e22d6be8c2cdfbb669515`  
		Last Modified: Tue, 03 Oct 2023 07:06:50 GMT  
		Size: 169.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `gradle:jammy` - linux; arm variant v7

```console
$ docker pull gradle@sha256:83dfb493096ab4b2ac9b716373412a46f1caa04237f2fb8141476f0bd01f43c8
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **372.1 MB (372071733 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:780efeab965295e376494dd1da6df90eba6828d2ab238dc95a46b9786467ab5e`
-	Entrypoint: `["\/__cacert_entrypoint.sh"]`
-	Default Command: `["gradle"]`

```dockerfile
# Mon, 25 Sep 2023 10:19:15 GMT
ARG RELEASE
# Mon, 25 Sep 2023 10:19:15 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Mon, 25 Sep 2023 10:19:16 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Mon, 25 Sep 2023 10:19:16 GMT
LABEL org.opencontainers.image.version=22.04
# Mon, 25 Sep 2023 10:19:18 GMT
ADD file:0008d56422c09f73afbcd40ace46d311e36ba0d60eef05198ea3665172ba3433 in / 
# Mon, 25 Sep 2023 10:19:18 GMT
CMD ["/bin/bash"]
# Tue, 03 Oct 2023 06:00:53 GMT
ENV JAVA_HOME=/opt/java/openjdk
# Tue, 03 Oct 2023 06:00:54 GMT
ENV PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 03 Oct 2023 06:00:54 GMT
ENV LANG=en_US.UTF-8 LANGUAGE=en_US:en LC_ALL=en_US.UTF-8
# Tue, 03 Oct 2023 06:02:49 GMT
RUN apt-get update     && DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends tzdata curl wget ca-certificates fontconfig locales p11-kit binutils     && echo "en_US.UTF-8 UTF-8" >> /etc/locale.gen     && locale-gen en_US.UTF-8     && rm -rf /var/lib/apt/lists/*
# Tue, 03 Oct 2023 06:02:50 GMT
ENV JAVA_VERSION=jdk-17.0.8.1+1
# Tue, 03 Oct 2023 06:03:01 GMT
RUN set -eux;     ARCH="$(dpkg --print-architecture)";     case "${ARCH}" in        aarch64|arm64)          ESUM='eefd3cf3b3dd47ff269fa5b5c10b5e096b163f4e9c1810023abdbc00dc6cc304';          BINARY_URL='https://github.com/adoptium/temurin17-binaries/releases/download/jdk-17.0.8.1%2B1/OpenJDK17U-jdk_aarch64_linux_hotspot_17.0.8.1_1.tar.gz';          ;;        armhf|arm)          ESUM='b1f1d8b7fcb159a0a8029b6c3106d1d16207cecbb2047f9a4be2a64d29897da5';          BINARY_URL='https://github.com/adoptium/temurin17-binaries/releases/download/jdk-17.0.8.1%2B1/OpenJDK17U-jdk_arm_linux_hotspot_17.0.8.1_1.tar.gz';          ;;        ppc64el|powerpc:common64)          ESUM='00a4c07603d0218cd678461b5b3b7e25b3253102da4022d31fc35907f21a2efd';          BINARY_URL='https://github.com/adoptium/temurin17-binaries/releases/download/jdk-17.0.8.1%2B1/OpenJDK17U-jdk_ppc64le_linux_hotspot_17.0.8.1_1.tar.gz';          ;;        s390x|s390:64-bit)          ESUM='ffacba69c6843d7ca70d572489d6cc7ab7ae52c60f0852cedf4cf0d248b6fc37';          BINARY_URL='https://github.com/adoptium/temurin17-binaries/releases/download/jdk-17.0.8.1%2B1/OpenJDK17U-jdk_s390x_linux_hotspot_17.0.8.1_1.tar.gz';          ;;        amd64|i386:x86-64)          ESUM='c25dfbc334068a48c19c44ce39ad4b8427e309ae1cfa83f23c102e78b8a6dcc0';          BINARY_URL='https://github.com/adoptium/temurin17-binaries/releases/download/jdk-17.0.8.1%2B1/OpenJDK17U-jdk_x64_linux_hotspot_17.0.8.1_1.tar.gz';          ;;        *)          echo "Unsupported arch: ${ARCH}";          exit 1;          ;;     esac; 	  wget -O /tmp/openjdk.tar.gz ${BINARY_URL}; 	  echo "${ESUM} */tmp/openjdk.tar.gz" | sha256sum -c -; 	  mkdir -p "$JAVA_HOME"; 	  tar --extract 	      --file /tmp/openjdk.tar.gz 	      --directory "$JAVA_HOME" 	      --strip-components 1 	      --no-same-owner 	  ;     rm -f /tmp/openjdk.tar.gz ${JAVA_HOME}/lib/src.zip;     find "$JAVA_HOME/lib" -name '*.so' -exec dirname '{}' ';' | sort -u > /etc/ld.so.conf.d/docker-openjdk.conf;     ldconfig;     java -Xshare:dump;
# Tue, 03 Oct 2023 06:03:04 GMT
RUN echo Verifying install ...     && fileEncoding="$(echo 'System.out.println(System.getProperty("file.encoding"))' | jshell -s -)"; [ "$fileEncoding" = 'UTF-8' ]; rm -rf ~/.java     && echo javac --version && javac --version     && echo java --version && java --version     && echo Complete.
# Tue, 03 Oct 2023 06:03:04 GMT
COPY file:8b8864b3e02a33a579dc216fd51b28a6047bc8eeaa03045b258980fe0cf7fcb3 in /__cacert_entrypoint.sh 
# Tue, 03 Oct 2023 06:03:04 GMT
ENTRYPOINT ["/__cacert_entrypoint.sh"]
# Tue, 03 Oct 2023 06:03:04 GMT
CMD ["jshell"]
# Tue, 03 Oct 2023 06:44:40 GMT
CMD ["gradle"]
# Tue, 03 Oct 2023 06:44:40 GMT
ENV GRADLE_HOME=/opt/gradle
# Tue, 03 Oct 2023 06:44:40 GMT
RUN set -o errexit -o nounset     && echo "Adding gradle user and group"     && groupadd --system --gid 1000 gradle     && useradd --system --gid gradle --uid 1000 --shell /bin/bash --create-home gradle     && mkdir /home/gradle/.gradle     && chown --recursive gradle:gradle /home/gradle         && echo "Symlinking root Gradle cache to gradle Gradle cache"     && ln --symbolic /home/gradle/.gradle /root/.gradle
# Tue, 03 Oct 2023 06:44:41 GMT
VOLUME [/home/gradle/.gradle]
# Tue, 03 Oct 2023 06:44:41 GMT
WORKDIR /home/gradle
# Tue, 03 Oct 2023 06:44:56 GMT
RUN set -o errexit -o nounset     && apt-get update     && apt-get install --yes --no-install-recommends         unzip         wget                 bzr         git         git-lfs         mercurial         openssh-client         subversion     && rm --recursive --force /var/lib/apt/lists/*         && echo "Testing VCSes"     && which bzr     && which git     && which git-lfs     && which hg     && which svn
# Fri, 06 Oct 2023 00:01:24 GMT
ENV GRADLE_VERSION=8.4
# Fri, 06 Oct 2023 00:01:24 GMT
ARG GRADLE_DOWNLOAD_SHA256=3e1af3ae886920c3ac87f7a91f816c0c7c436f276a6eefdb3da152100fef72ae
# Fri, 06 Oct 2023 00:01:29 GMT
# ARGS: GRADLE_DOWNLOAD_SHA256=3e1af3ae886920c3ac87f7a91f816c0c7c436f276a6eefdb3da152100fef72ae
RUN set -o errexit -o nounset     && echo "Downloading Gradle"     && wget --no-verbose --output-document=gradle.zip "https://services.gradle.org/distributions/gradle-${GRADLE_VERSION}-bin.zip"         && echo "Checking Gradle download hash"     && echo "${GRADLE_DOWNLOAD_SHA256} *gradle.zip" | sha256sum --check -         && echo "Installing Gradle"     && unzip gradle.zip     && rm gradle.zip     && mv "gradle-${GRADLE_VERSION}" "${GRADLE_HOME}/"     && ln --symbolic "${GRADLE_HOME}/bin/gradle" /usr/bin/gradle
# Fri, 06 Oct 2023 00:01:29 GMT
USER gradle
# Fri, 06 Oct 2023 00:01:31 GMT
# ARGS: GRADLE_DOWNLOAD_SHA256=3e1af3ae886920c3ac87f7a91f816c0c7c436f276a6eefdb3da152100fef72ae
RUN set -o errexit -o nounset     && echo "Testing Gradle installation"     && gradle --version
# Fri, 06 Oct 2023 00:01:31 GMT
USER root
```

-	Layers:
	-	`sha256:7271b2c80df6c73d794550b50f57d78c6fd5b85da7934c6506c76ea706087280`  
		Last Modified: Tue, 26 Sep 2023 02:07:56 GMT  
		Size: 27.5 MB (27515498 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1a42f949007cfbde4e09ba505ced26b019abd8a7ea5591c2ee0c80fe213191ee`  
		Last Modified: Tue, 03 Oct 2023 06:05:16 GMT  
		Size: 17.6 MB (17587273 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0cc8cb2c36aabb6e51e5cb39d9ab060ca54e69d03596ee2fb3f3a2013aa6949b`  
		Last Modified: Tue, 03 Oct 2023 06:05:26 GMT  
		Size: 142.1 MB (142064196 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f283f5a680dae88eb915b9ed36820132a65dd6d02068dec9c2217211bf3600a0`  
		Last Modified: Tue, 03 Oct 2023 06:05:13 GMT  
		Size: 176.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dbdb39d0c5347dc505dfd2a2b89a3972c4c610328559f92df055be0d6d90b5ef`  
		Last Modified: Tue, 03 Oct 2023 06:05:13 GMT  
		Size: 734.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1645a9ffce50ab06cc69c152cbf85005bba59e5e7423d6aa7922d4e25afe398e`  
		Last Modified: Tue, 03 Oct 2023 06:48:42 GMT  
		Size: 4.4 KB (4351 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:99f317e0b1ccbca72b6bbbdfc307d4570c5091ed2450e005b467f4141e9b2425`  
		Last Modified: Tue, 03 Oct 2023 06:48:52 GMT  
		Size: 53.9 MB (53889606 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:64b056d79c280e65eef99a56e0564a33fe97501f83606030b8cecb5bea7b16a3`  
		Last Modified: Fri, 06 Oct 2023 00:06:12 GMT  
		Size: 131.0 MB (131009729 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:06d48ec722ec427d55c26dfd03cb9567433c2d2fcc38c87da5136c0f848685d3`  
		Last Modified: Fri, 06 Oct 2023 00:06:04 GMT  
		Size: 170.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `gradle:jammy` - linux; arm64 variant v8

```console
$ docker pull gradle@sha256:910273c2a4f558444c3675e808364e7537cbb54921dd0d88f3f5a18bd0079a59
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **372.9 MB (372943220 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:7b8ce0aa0c58e23233fef406071a90db25b033d6ddb3db0e196323dbaebb0284`
-	Entrypoint: `["\/__cacert_entrypoint.sh"]`
-	Default Command: `["gradle"]`

```dockerfile
# Mon, 25 Sep 2023 10:17:41 GMT
ARG RELEASE
# Mon, 25 Sep 2023 10:17:41 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Mon, 25 Sep 2023 10:17:41 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Mon, 25 Sep 2023 10:17:41 GMT
LABEL org.opencontainers.image.version=22.04
# Mon, 25 Sep 2023 10:17:44 GMT
ADD file:8540670760767f19eaf101fbce1da1881a2f24a7d65da6abdedc644b8fb00463 in / 
# Mon, 25 Sep 2023 10:17:45 GMT
CMD ["/bin/bash"]
# Tue, 03 Oct 2023 06:06:59 GMT
ENV JAVA_HOME=/opt/java/openjdk
# Tue, 03 Oct 2023 06:06:59 GMT
ENV PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 03 Oct 2023 06:06:59 GMT
ENV LANG=en_US.UTF-8 LANGUAGE=en_US:en LC_ALL=en_US.UTF-8
# Tue, 03 Oct 2023 06:08:16 GMT
RUN apt-get update     && DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends tzdata curl wget ca-certificates fontconfig locales p11-kit binutils     && echo "en_US.UTF-8 UTF-8" >> /etc/locale.gen     && locale-gen en_US.UTF-8     && rm -rf /var/lib/apt/lists/*
# Tue, 03 Oct 2023 06:08:17 GMT
ENV JAVA_VERSION=jdk-17.0.8.1+1
# Tue, 03 Oct 2023 06:08:26 GMT
RUN set -eux;     ARCH="$(dpkg --print-architecture)";     case "${ARCH}" in        aarch64|arm64)          ESUM='eefd3cf3b3dd47ff269fa5b5c10b5e096b163f4e9c1810023abdbc00dc6cc304';          BINARY_URL='https://github.com/adoptium/temurin17-binaries/releases/download/jdk-17.0.8.1%2B1/OpenJDK17U-jdk_aarch64_linux_hotspot_17.0.8.1_1.tar.gz';          ;;        armhf|arm)          ESUM='b1f1d8b7fcb159a0a8029b6c3106d1d16207cecbb2047f9a4be2a64d29897da5';          BINARY_URL='https://github.com/adoptium/temurin17-binaries/releases/download/jdk-17.0.8.1%2B1/OpenJDK17U-jdk_arm_linux_hotspot_17.0.8.1_1.tar.gz';          ;;        ppc64el|powerpc:common64)          ESUM='00a4c07603d0218cd678461b5b3b7e25b3253102da4022d31fc35907f21a2efd';          BINARY_URL='https://github.com/adoptium/temurin17-binaries/releases/download/jdk-17.0.8.1%2B1/OpenJDK17U-jdk_ppc64le_linux_hotspot_17.0.8.1_1.tar.gz';          ;;        s390x|s390:64-bit)          ESUM='ffacba69c6843d7ca70d572489d6cc7ab7ae52c60f0852cedf4cf0d248b6fc37';          BINARY_URL='https://github.com/adoptium/temurin17-binaries/releases/download/jdk-17.0.8.1%2B1/OpenJDK17U-jdk_s390x_linux_hotspot_17.0.8.1_1.tar.gz';          ;;        amd64|i386:x86-64)          ESUM='c25dfbc334068a48c19c44ce39ad4b8427e309ae1cfa83f23c102e78b8a6dcc0';          BINARY_URL='https://github.com/adoptium/temurin17-binaries/releases/download/jdk-17.0.8.1%2B1/OpenJDK17U-jdk_x64_linux_hotspot_17.0.8.1_1.tar.gz';          ;;        *)          echo "Unsupported arch: ${ARCH}";          exit 1;          ;;     esac; 	  wget -O /tmp/openjdk.tar.gz ${BINARY_URL}; 	  echo "${ESUM} */tmp/openjdk.tar.gz" | sha256sum -c -; 	  mkdir -p "$JAVA_HOME"; 	  tar --extract 	      --file /tmp/openjdk.tar.gz 	      --directory "$JAVA_HOME" 	      --strip-components 1 	      --no-same-owner 	  ;     rm -f /tmp/openjdk.tar.gz ${JAVA_HOME}/lib/src.zip;     find "$JAVA_HOME/lib" -name '*.so' -exec dirname '{}' ';' | sort -u > /etc/ld.so.conf.d/docker-openjdk.conf;     ldconfig;     java -Xshare:dump;
# Tue, 03 Oct 2023 06:08:29 GMT
RUN echo Verifying install ...     && fileEncoding="$(echo 'System.out.println(System.getProperty("file.encoding"))' | jshell -s -)"; [ "$fileEncoding" = 'UTF-8' ]; rm -rf ~/.java     && echo javac --version && javac --version     && echo java --version && java --version     && echo Complete.
# Tue, 03 Oct 2023 06:08:29 GMT
COPY file:8b8864b3e02a33a579dc216fd51b28a6047bc8eeaa03045b258980fe0cf7fcb3 in /__cacert_entrypoint.sh 
# Tue, 03 Oct 2023 06:08:29 GMT
ENTRYPOINT ["/__cacert_entrypoint.sh"]
# Tue, 03 Oct 2023 06:08:29 GMT
CMD ["jshell"]
# Tue, 03 Oct 2023 06:57:38 GMT
CMD ["gradle"]
# Tue, 03 Oct 2023 06:57:38 GMT
ENV GRADLE_HOME=/opt/gradle
# Tue, 03 Oct 2023 06:57:38 GMT
RUN set -o errexit -o nounset     && echo "Adding gradle user and group"     && groupadd --system --gid 1000 gradle     && useradd --system --gid gradle --uid 1000 --shell /bin/bash --create-home gradle     && mkdir /home/gradle/.gradle     && chown --recursive gradle:gradle /home/gradle         && echo "Symlinking root Gradle cache to gradle Gradle cache"     && ln --symbolic /home/gradle/.gradle /root/.gradle
# Tue, 03 Oct 2023 06:57:38 GMT
VOLUME [/home/gradle/.gradle]
# Tue, 03 Oct 2023 06:57:38 GMT
WORKDIR /home/gradle
# Tue, 03 Oct 2023 06:57:51 GMT
RUN set -o errexit -o nounset     && apt-get update     && apt-get install --yes --no-install-recommends         unzip         wget                 bzr         git         git-lfs         mercurial         openssh-client         subversion     && rm --recursive --force /var/lib/apt/lists/*         && echo "Testing VCSes"     && which bzr     && which git     && which git-lfs     && which hg     && which svn
# Thu, 05 Oct 2023 23:40:05 GMT
ENV GRADLE_VERSION=8.4
# Thu, 05 Oct 2023 23:40:05 GMT
ARG GRADLE_DOWNLOAD_SHA256=3e1af3ae886920c3ac87f7a91f816c0c7c436f276a6eefdb3da152100fef72ae
# Thu, 05 Oct 2023 23:40:09 GMT
# ARGS: GRADLE_DOWNLOAD_SHA256=3e1af3ae886920c3ac87f7a91f816c0c7c436f276a6eefdb3da152100fef72ae
RUN set -o errexit -o nounset     && echo "Downloading Gradle"     && wget --no-verbose --output-document=gradle.zip "https://services.gradle.org/distributions/gradle-${GRADLE_VERSION}-bin.zip"         && echo "Checking Gradle download hash"     && echo "${GRADLE_DOWNLOAD_SHA256} *gradle.zip" | sha256sum --check -         && echo "Installing Gradle"     && unzip gradle.zip     && rm gradle.zip     && mv "gradle-${GRADLE_VERSION}" "${GRADLE_HOME}/"     && ln --symbolic "${GRADLE_HOME}/bin/gradle" /usr/bin/gradle
# Thu, 05 Oct 2023 23:40:10 GMT
USER gradle
# Thu, 05 Oct 2023 23:40:11 GMT
# ARGS: GRADLE_DOWNLOAD_SHA256=3e1af3ae886920c3ac87f7a91f816c0c7c436f276a6eefdb3da152100fef72ae
RUN set -o errexit -o nounset     && echo "Testing Gradle installation"     && gradle --version
# Thu, 05 Oct 2023 23:40:11 GMT
USER root
```

-	Layers:
	-	`sha256:6ea603f1df5e3d23206761eca19fba4cdf4e22d773256cb65b71b730aa5acced`  
		Last Modified: Mon, 25 Sep 2023 17:30:11 GMT  
		Size: 28.4 MB (28392073 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5ba2aefbab3334adfc4bfa89dd448c89bc452ab89a02053172fb42a8e5288ba3`  
		Last Modified: Tue, 03 Oct 2023 06:11:30 GMT  
		Size: 18.9 MB (18859718 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:753b98fc35cd82fe89ecc7d11b833688e92102be27567d036bb1ead5eec98ed5`  
		Last Modified: Tue, 03 Oct 2023 06:11:37 GMT  
		Size: 143.6 MB (143553841 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ce8e5167f5e56a4dc905a342ae65372a5b2d6d6947e1d47086302582aa91263e`  
		Last Modified: Tue, 03 Oct 2023 06:11:27 GMT  
		Size: 169.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:580f4b189461fdb8b41219e07a2c3ea5531b35d7e2b6e4768a911c12cff95029`  
		Last Modified: Tue, 03 Oct 2023 06:11:27 GMT  
		Size: 733.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:356253a20dfe92ea3e4a1d86673d16def45e5e207485b8a2e3142384f71fb645`  
		Last Modified: Tue, 03 Oct 2023 07:02:20 GMT  
		Size: 4.4 KB (4370 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2ef15e1f76aeeaf74fc5b079ac7892d2bf51d8e3d54e583dda66379b1ce071c2`  
		Last Modified: Tue, 03 Oct 2023 07:02:26 GMT  
		Size: 51.1 MB (51122415 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7db56bd72ab7259eee165e450586eebc1fa9a2b2ae2f7941bfb931694605a9bf`  
		Last Modified: Thu, 05 Oct 2023 23:45:19 GMT  
		Size: 131.0 MB (131009731 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:310f349f385e4bf2820eb5799466e5d13a5e5bf782bf737e71ce126b8bda7385`  
		Last Modified: Thu, 05 Oct 2023 23:45:13 GMT  
		Size: 170.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `gradle:jammy` - linux; ppc64le

```console
$ docker pull gradle@sha256:c7471110ada44830e87519667db31062e31b70fd0ef731cdfacc6fb5caf6b43c
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **385.3 MB (385298197 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:43b7cd3819226606eb0dc195db3e2e9a2d6a4eae22ac45b4b945e8ebca9a25a7`
-	Entrypoint: `["\/__cacert_entrypoint.sh"]`
-	Default Command: `["gradle"]`

```dockerfile
# Mon, 25 Sep 2023 10:20:46 GMT
ARG RELEASE
# Mon, 25 Sep 2023 10:20:46 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Mon, 25 Sep 2023 10:20:46 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Mon, 25 Sep 2023 10:20:46 GMT
LABEL org.opencontainers.image.version=22.04
# Mon, 25 Sep 2023 10:20:49 GMT
ADD file:4e52928c778d7e98d90ccfcaacd039ae1fdde494dfa310adbe229d7051c30918 in / 
# Mon, 25 Sep 2023 10:20:49 GMT
CMD ["/bin/bash"]
# Tue, 03 Oct 2023 08:16:45 GMT
ENV JAVA_HOME=/opt/java/openjdk
# Tue, 03 Oct 2023 08:16:45 GMT
ENV PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 03 Oct 2023 08:16:46 GMT
ENV LANG=en_US.UTF-8 LANGUAGE=en_US:en LC_ALL=en_US.UTF-8
# Tue, 03 Oct 2023 08:20:10 GMT
RUN apt-get update     && DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends tzdata curl wget ca-certificates fontconfig locales p11-kit binutils     && echo "en_US.UTF-8 UTF-8" >> /etc/locale.gen     && locale-gen en_US.UTF-8     && rm -rf /var/lib/apt/lists/*
# Tue, 03 Oct 2023 08:20:14 GMT
ENV JAVA_VERSION=jdk-17.0.8.1+1
# Tue, 03 Oct 2023 08:20:33 GMT
RUN set -eux;     ARCH="$(dpkg --print-architecture)";     case "${ARCH}" in        aarch64|arm64)          ESUM='eefd3cf3b3dd47ff269fa5b5c10b5e096b163f4e9c1810023abdbc00dc6cc304';          BINARY_URL='https://github.com/adoptium/temurin17-binaries/releases/download/jdk-17.0.8.1%2B1/OpenJDK17U-jdk_aarch64_linux_hotspot_17.0.8.1_1.tar.gz';          ;;        armhf|arm)          ESUM='b1f1d8b7fcb159a0a8029b6c3106d1d16207cecbb2047f9a4be2a64d29897da5';          BINARY_URL='https://github.com/adoptium/temurin17-binaries/releases/download/jdk-17.0.8.1%2B1/OpenJDK17U-jdk_arm_linux_hotspot_17.0.8.1_1.tar.gz';          ;;        ppc64el|powerpc:common64)          ESUM='00a4c07603d0218cd678461b5b3b7e25b3253102da4022d31fc35907f21a2efd';          BINARY_URL='https://github.com/adoptium/temurin17-binaries/releases/download/jdk-17.0.8.1%2B1/OpenJDK17U-jdk_ppc64le_linux_hotspot_17.0.8.1_1.tar.gz';          ;;        s390x|s390:64-bit)          ESUM='ffacba69c6843d7ca70d572489d6cc7ab7ae52c60f0852cedf4cf0d248b6fc37';          BINARY_URL='https://github.com/adoptium/temurin17-binaries/releases/download/jdk-17.0.8.1%2B1/OpenJDK17U-jdk_s390x_linux_hotspot_17.0.8.1_1.tar.gz';          ;;        amd64|i386:x86-64)          ESUM='c25dfbc334068a48c19c44ce39ad4b8427e309ae1cfa83f23c102e78b8a6dcc0';          BINARY_URL='https://github.com/adoptium/temurin17-binaries/releases/download/jdk-17.0.8.1%2B1/OpenJDK17U-jdk_x64_linux_hotspot_17.0.8.1_1.tar.gz';          ;;        *)          echo "Unsupported arch: ${ARCH}";          exit 1;          ;;     esac; 	  wget -O /tmp/openjdk.tar.gz ${BINARY_URL}; 	  echo "${ESUM} */tmp/openjdk.tar.gz" | sha256sum -c -; 	  mkdir -p "$JAVA_HOME"; 	  tar --extract 	      --file /tmp/openjdk.tar.gz 	      --directory "$JAVA_HOME" 	      --strip-components 1 	      --no-same-owner 	  ;     rm -f /tmp/openjdk.tar.gz ${JAVA_HOME}/lib/src.zip;     find "$JAVA_HOME/lib" -name '*.so' -exec dirname '{}' ';' | sort -u > /etc/ld.so.conf.d/docker-openjdk.conf;     ldconfig;     java -Xshare:dump;
# Tue, 03 Oct 2023 08:20:44 GMT
RUN echo Verifying install ...     && fileEncoding="$(echo 'System.out.println(System.getProperty("file.encoding"))' | jshell -s -)"; [ "$fileEncoding" = 'UTF-8' ]; rm -rf ~/.java     && echo javac --version && javac --version     && echo java --version && java --version     && echo Complete.
# Tue, 03 Oct 2023 08:20:44 GMT
COPY file:8b8864b3e02a33a579dc216fd51b28a6047bc8eeaa03045b258980fe0cf7fcb3 in /__cacert_entrypoint.sh 
# Tue, 03 Oct 2023 08:20:45 GMT
ENTRYPOINT ["/__cacert_entrypoint.sh"]
# Tue, 03 Oct 2023 08:20:45 GMT
CMD ["jshell"]
# Tue, 03 Oct 2023 11:12:02 GMT
CMD ["gradle"]
# Tue, 03 Oct 2023 11:12:03 GMT
ENV GRADLE_HOME=/opt/gradle
# Tue, 03 Oct 2023 11:12:05 GMT
RUN set -o errexit -o nounset     && echo "Adding gradle user and group"     && groupadd --system --gid 1000 gradle     && useradd --system --gid gradle --uid 1000 --shell /bin/bash --create-home gradle     && mkdir /home/gradle/.gradle     && chown --recursive gradle:gradle /home/gradle         && echo "Symlinking root Gradle cache to gradle Gradle cache"     && ln --symbolic /home/gradle/.gradle /root/.gradle
# Tue, 03 Oct 2023 11:12:06 GMT
VOLUME [/home/gradle/.gradle]
# Tue, 03 Oct 2023 11:12:07 GMT
WORKDIR /home/gradle
# Tue, 03 Oct 2023 11:12:55 GMT
RUN set -o errexit -o nounset     && apt-get update     && apt-get install --yes --no-install-recommends         unzip         wget                 bzr         git         git-lfs         mercurial         openssh-client         subversion     && rm --recursive --force /var/lib/apt/lists/*         && echo "Testing VCSes"     && which bzr     && which git     && which git-lfs     && which hg     && which svn
# Tue, 03 Oct 2023 11:12:59 GMT
ENV GRADLE_VERSION=8.3
# Tue, 03 Oct 2023 11:13:02 GMT
ARG GRADLE_DOWNLOAD_SHA256=591855b517fc635b9e04de1d05d5e76ada3f89f5fc76f87978d1b245b4f69225
# Tue, 03 Oct 2023 11:13:10 GMT
# ARGS: GRADLE_DOWNLOAD_SHA256=591855b517fc635b9e04de1d05d5e76ada3f89f5fc76f87978d1b245b4f69225
RUN set -o errexit -o nounset     && echo "Downloading Gradle"     && wget --no-verbose --output-document=gradle.zip "https://services.gradle.org/distributions/gradle-${GRADLE_VERSION}-bin.zip"         && echo "Checking Gradle download hash"     && echo "${GRADLE_DOWNLOAD_SHA256} *gradle.zip" | sha256sum --check -         && echo "Installing Gradle"     && unzip gradle.zip     && rm gradle.zip     && mv "gradle-${GRADLE_VERSION}" "${GRADLE_HOME}/"     && ln --symbolic "${GRADLE_HOME}/bin/gradle" /usr/bin/gradle
# Tue, 03 Oct 2023 11:13:13 GMT
USER gradle
# Tue, 03 Oct 2023 11:13:15 GMT
# ARGS: GRADLE_DOWNLOAD_SHA256=591855b517fc635b9e04de1d05d5e76ada3f89f5fc76f87978d1b245b4f69225
RUN set -o errexit -o nounset     && echo "Testing Gradle installation"     && gradle --version
# Tue, 03 Oct 2023 11:13:15 GMT
USER root
```

-	Layers:
	-	`sha256:8098558aeb0337452acaa8c74f02401dc8e9bc5a2c048e4c82c013b483a11f11`  
		Last Modified: Tue, 03 Oct 2023 07:57:52 GMT  
		Size: 35.7 MB (35702863 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c1a1a71044263240e812a6d7b84068cd0594360ef4157124e4c3783bf7297cfa`  
		Last Modified: Tue, 03 Oct 2023 08:24:00 GMT  
		Size: 18.7 MB (18728975 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3d725de9c6f916836b123cc2ea3b4ebecfb5c8388201eb76feae3cb3e6fafeb6`  
		Last Modified: Tue, 03 Oct 2023 08:24:14 GMT  
		Size: 144.5 MB (144496099 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d856cdd68f3bc215ba942b0fbfa954581c297d2ac0655a536fc081561d0ebd09`  
		Last Modified: Tue, 03 Oct 2023 08:23:54 GMT  
		Size: 174.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:342d7c29a897667460f0f83749bec15165419530c3036ba8a0668058ef08f9fa`  
		Last Modified: Tue, 03 Oct 2023 08:23:54 GMT  
		Size: 733.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:42364b30f2aaf598f28040787b0469f0b64dde7872e6a23d3dcc4529da2fd17a`  
		Last Modified: Tue, 03 Oct 2023 11:18:10 GMT  
		Size: 4.4 KB (4368 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9605a337630e3cc0277e38de59ce6c4dd10be560a70b2cfd59355ae948aec8d5`  
		Last Modified: Tue, 03 Oct 2023 11:18:26 GMT  
		Size: 55.7 MB (55697546 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:807ff58f9970ec194af96d19a2594404a5150e34ba19ea5bc87e7053d218fbc2`  
		Last Modified: Tue, 03 Oct 2023 11:18:22 GMT  
		Size: 130.7 MB (130667269 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4794d278d8c698a6d7ba447393b9775e5ddce3ae029e969894ccc57c22a3a53a`  
		Last Modified: Tue, 03 Oct 2023 11:18:11 GMT  
		Size: 170.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `gradle:jammy` - linux; s390x

```console
$ docker pull gradle@sha256:4dc7dbad8964b45786eb9ffd40a28b6cf34eb2bc72313230197c75410857a44f
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **362.1 MB (362080619 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e4cd05ed0c026cf5567b9a77d24413c35fea18516aab323594835e938ea46a0d`
-	Entrypoint: `["\/__cacert_entrypoint.sh"]`
-	Default Command: `["gradle"]`

```dockerfile
# Mon, 25 Sep 2023 10:17:26 GMT
ARG RELEASE
# Mon, 25 Sep 2023 10:17:26 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Mon, 25 Sep 2023 10:17:26 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Mon, 25 Sep 2023 10:17:26 GMT
LABEL org.opencontainers.image.version=22.04
# Mon, 25 Sep 2023 10:17:28 GMT
ADD file:78683f2464233172a7cd0d6adc4c7d9fb3ef05fa67ca22e6fbaca0325496a536 in / 
# Mon, 25 Sep 2023 10:17:28 GMT
CMD ["/bin/bash"]
# Tue, 03 Oct 2023 09:08:41 GMT
ENV JAVA_HOME=/opt/java/openjdk
# Tue, 03 Oct 2023 09:08:41 GMT
ENV PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 03 Oct 2023 09:08:41 GMT
ENV LANG=en_US.UTF-8 LANGUAGE=en_US:en LC_ALL=en_US.UTF-8
# Tue, 03 Oct 2023 09:10:18 GMT
RUN apt-get update     && DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends tzdata curl wget ca-certificates fontconfig locales p11-kit binutils     && echo "en_US.UTF-8 UTF-8" >> /etc/locale.gen     && locale-gen en_US.UTF-8     && rm -rf /var/lib/apt/lists/*
# Tue, 03 Oct 2023 09:10:20 GMT
ENV JAVA_VERSION=jdk-17.0.8.1+1
# Tue, 03 Oct 2023 09:10:31 GMT
RUN set -eux;     ARCH="$(dpkg --print-architecture)";     case "${ARCH}" in        aarch64|arm64)          ESUM='eefd3cf3b3dd47ff269fa5b5c10b5e096b163f4e9c1810023abdbc00dc6cc304';          BINARY_URL='https://github.com/adoptium/temurin17-binaries/releases/download/jdk-17.0.8.1%2B1/OpenJDK17U-jdk_aarch64_linux_hotspot_17.0.8.1_1.tar.gz';          ;;        armhf|arm)          ESUM='b1f1d8b7fcb159a0a8029b6c3106d1d16207cecbb2047f9a4be2a64d29897da5';          BINARY_URL='https://github.com/adoptium/temurin17-binaries/releases/download/jdk-17.0.8.1%2B1/OpenJDK17U-jdk_arm_linux_hotspot_17.0.8.1_1.tar.gz';          ;;        ppc64el|powerpc:common64)          ESUM='00a4c07603d0218cd678461b5b3b7e25b3253102da4022d31fc35907f21a2efd';          BINARY_URL='https://github.com/adoptium/temurin17-binaries/releases/download/jdk-17.0.8.1%2B1/OpenJDK17U-jdk_ppc64le_linux_hotspot_17.0.8.1_1.tar.gz';          ;;        s390x|s390:64-bit)          ESUM='ffacba69c6843d7ca70d572489d6cc7ab7ae52c60f0852cedf4cf0d248b6fc37';          BINARY_URL='https://github.com/adoptium/temurin17-binaries/releases/download/jdk-17.0.8.1%2B1/OpenJDK17U-jdk_s390x_linux_hotspot_17.0.8.1_1.tar.gz';          ;;        amd64|i386:x86-64)          ESUM='c25dfbc334068a48c19c44ce39ad4b8427e309ae1cfa83f23c102e78b8a6dcc0';          BINARY_URL='https://github.com/adoptium/temurin17-binaries/releases/download/jdk-17.0.8.1%2B1/OpenJDK17U-jdk_x64_linux_hotspot_17.0.8.1_1.tar.gz';          ;;        *)          echo "Unsupported arch: ${ARCH}";          exit 1;          ;;     esac; 	  wget -O /tmp/openjdk.tar.gz ${BINARY_URL}; 	  echo "${ESUM} */tmp/openjdk.tar.gz" | sha256sum -c -; 	  mkdir -p "$JAVA_HOME"; 	  tar --extract 	      --file /tmp/openjdk.tar.gz 	      --directory "$JAVA_HOME" 	      --strip-components 1 	      --no-same-owner 	  ;     rm -f /tmp/openjdk.tar.gz ${JAVA_HOME}/lib/src.zip;     find "$JAVA_HOME/lib" -name '*.so' -exec dirname '{}' ';' | sort -u > /etc/ld.so.conf.d/docker-openjdk.conf;     ldconfig;     java -Xshare:dump;
# Tue, 03 Oct 2023 09:10:39 GMT
RUN echo Verifying install ...     && fileEncoding="$(echo 'System.out.println(System.getProperty("file.encoding"))' | jshell -s -)"; [ "$fileEncoding" = 'UTF-8' ]; rm -rf ~/.java     && echo javac --version && javac --version     && echo java --version && java --version     && echo Complete.
# Tue, 03 Oct 2023 09:10:40 GMT
COPY file:8b8864b3e02a33a579dc216fd51b28a6047bc8eeaa03045b258980fe0cf7fcb3 in /__cacert_entrypoint.sh 
# Tue, 03 Oct 2023 09:10:40 GMT
ENTRYPOINT ["/__cacert_entrypoint.sh"]
# Tue, 03 Oct 2023 09:10:40 GMT
CMD ["jshell"]
# Tue, 03 Oct 2023 11:02:49 GMT
CMD ["gradle"]
# Tue, 03 Oct 2023 11:02:49 GMT
ENV GRADLE_HOME=/opt/gradle
# Tue, 03 Oct 2023 11:02:51 GMT
RUN set -o errexit -o nounset     && echo "Adding gradle user and group"     && groupadd --system --gid 1000 gradle     && useradd --system --gid gradle --uid 1000 --shell /bin/bash --create-home gradle     && mkdir /home/gradle/.gradle     && chown --recursive gradle:gradle /home/gradle         && echo "Symlinking root Gradle cache to gradle Gradle cache"     && ln --symbolic /home/gradle/.gradle /root/.gradle
# Tue, 03 Oct 2023 11:02:51 GMT
VOLUME [/home/gradle/.gradle]
# Tue, 03 Oct 2023 11:02:52 GMT
WORKDIR /home/gradle
# Tue, 03 Oct 2023 11:03:26 GMT
RUN set -o errexit -o nounset     && apt-get update     && apt-get install --yes --no-install-recommends         unzip         wget                 bzr         git         git-lfs         mercurial         openssh-client         subversion     && rm --recursive --force /var/lib/apt/lists/*         && echo "Testing VCSes"     && which bzr     && which git     && which git-lfs     && which hg     && which svn
# Tue, 03 Oct 2023 11:03:37 GMT
ENV GRADLE_VERSION=8.3
# Tue, 03 Oct 2023 11:03:37 GMT
ARG GRADLE_DOWNLOAD_SHA256=591855b517fc635b9e04de1d05d5e76ada3f89f5fc76f87978d1b245b4f69225
# Tue, 03 Oct 2023 11:03:57 GMT
# ARGS: GRADLE_DOWNLOAD_SHA256=591855b517fc635b9e04de1d05d5e76ada3f89f5fc76f87978d1b245b4f69225
RUN set -o errexit -o nounset     && echo "Downloading Gradle"     && wget --no-verbose --output-document=gradle.zip "https://services.gradle.org/distributions/gradle-${GRADLE_VERSION}-bin.zip"         && echo "Checking Gradle download hash"     && echo "${GRADLE_DOWNLOAD_SHA256} *gradle.zip" | sha256sum --check -         && echo "Installing Gradle"     && unzip gradle.zip     && rm gradle.zip     && mv "gradle-${GRADLE_VERSION}" "${GRADLE_HOME}/"     && ln --symbolic "${GRADLE_HOME}/bin/gradle" /usr/bin/gradle
# Tue, 03 Oct 2023 11:04:04 GMT
USER gradle
# Tue, 03 Oct 2023 11:04:05 GMT
# ARGS: GRADLE_DOWNLOAD_SHA256=591855b517fc635b9e04de1d05d5e76ada3f89f5fc76f87978d1b245b4f69225
RUN set -o errexit -o nounset     && echo "Testing Gradle installation"     && gradle --version
# Tue, 03 Oct 2023 11:04:06 GMT
USER root
```

-	Layers:
	-	`sha256:b6ba488997f9924c9473e547d56b3d4ae74495b1092ca3c613243185ee5d5151`  
		Last Modified: Tue, 03 Oct 2023 08:59:45 GMT  
		Size: 28.7 MB (28651983 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f54dc9f25198df234360ea82a24de7bf823b55e6000600bc0f095d05fc103b78`  
		Last Modified: Tue, 03 Oct 2023 09:13:17 GMT  
		Size: 17.3 MB (17254775 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:abe5a46c26186cc78210b95c057ee4a99f1f3a4e5b0b0821ffddfa0fb505b367`  
		Last Modified: Tue, 03 Oct 2023 09:13:26 GMT  
		Size: 134.2 MB (134217540 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0017d46d2028880f3e495629e9b1e9b32bc3e8334a057f52838dab2eb9f214f0`  
		Last Modified: Tue, 03 Oct 2023 09:13:20 GMT  
		Size: 174.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6be756ac3d82b87574c183d45db95b8ec1a7d188426c9ee2d4acdd87841a0d4a`  
		Last Modified: Tue, 03 Oct 2023 09:13:15 GMT  
		Size: 733.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:80b4a5559d95f3fc5782ea1383b766d62caac35066129fbfc8061cc10f1e6ffb`  
		Last Modified: Tue, 03 Oct 2023 11:09:38 GMT  
		Size: 4.4 KB (4370 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:eb54b979b64f219b962bc75eaeeba4a21d81e88e5c08f811a67164b4188728e8`  
		Last Modified: Tue, 03 Oct 2023 11:09:47 GMT  
		Size: 51.3 MB (51283570 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8efdf63ca06cab8be6ac1f03656e4527482b0850bd3a2c9105c355416228e995`  
		Last Modified: Tue, 03 Oct 2023 11:09:45 GMT  
		Size: 130.7 MB (130667305 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:73a11a67587fe22ddabfbf832a5c61b882aa6cbb9303d4ffd7b3880b3da2b66b`  
		Last Modified: Tue, 03 Oct 2023 11:09:38 GMT  
		Size: 169.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
