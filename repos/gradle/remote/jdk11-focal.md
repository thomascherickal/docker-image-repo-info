## `gradle:jdk11-focal`

```console
$ docker pull gradle@sha256:c5111d86dd4f510a344be533f7935bf263cdaa5b21db121a00cfe627b1e3fb70
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
$ docker pull gradle@sha256:05f89543e954a8d3bb22d588f977afbf64e3a931a34c568c29cfe37d0f14180f
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **386.8 MB (386840047 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:2e2f21ee542635ff456dd39cf5abd0051fe777fafe176c2f634ac3314945ade0`
-	Entrypoint: `["\/__cacert_entrypoint.sh"]`
-	Default Command: `["gradle"]`

```dockerfile
# Tue, 03 Oct 2023 10:45:50 GMT
ARG RELEASE
# Tue, 03 Oct 2023 10:45:50 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Tue, 03 Oct 2023 10:45:50 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Tue, 03 Oct 2023 10:45:50 GMT
LABEL org.opencontainers.image.version=20.04
# Tue, 03 Oct 2023 10:45:51 GMT
ADD file:4809da414c2d478b4d991cbdaa2df457f2b3d07d0ff6cf673f09a66f90833e81 in / 
# Tue, 03 Oct 2023 10:45:52 GMT
CMD ["/bin/bash"]
# Fri, 13 Oct 2023 05:50:16 GMT
ENV JAVA_HOME=/opt/java/openjdk
# Fri, 13 Oct 2023 05:50:16 GMT
ENV PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Fri, 13 Oct 2023 05:50:16 GMT
ENV LANG=en_US.UTF-8 LANGUAGE=en_US:en LC_ALL=en_US.UTF-8
# Fri, 13 Oct 2023 05:50:53 GMT
RUN apt-get update     && DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends tzdata curl wget ca-certificates fontconfig locales p11-kit     && echo "en_US.UTF-8 UTF-8" >> /etc/locale.gen     && locale-gen en_US.UTF-8     && rm -rf /var/lib/apt/lists/*
# Fri, 13 Oct 2023 05:52:07 GMT
ENV JAVA_VERSION=jdk-11.0.20.1+1
# Fri, 13 Oct 2023 05:52:15 GMT
RUN set -eux;     ARCH="$(dpkg --print-architecture)";     case "${ARCH}" in        aarch64|arm64)          ESUM='69d39682c4a2fac294a9eaacbf62c26d3c8a2f9123f1b5d287498a5472c6b672';          BINARY_URL='https://github.com/adoptium/temurin11-binaries/releases/download/jdk-11.0.20.1%2B1/OpenJDK11U-jdk_aarch64_linux_hotspot_11.0.20.1_1.tar.gz';          ;;        armhf|arm)          ESUM='e83674aee238ebb5f359b9395b3c5e3fad5b645846095494662802d2f0fd01c9';          BINARY_URL='https://github.com/adoptium/temurin11-binaries/releases/download/jdk-11.0.20.1%2B1/OpenJDK11U-jdk_arm_linux_hotspot_11.0.20.1_1.tar.gz';          ;;        ppc64el|powerpc:common64)          ESUM='b806f4bb526161bf9b2ffb37be4e1b77f56b4e726dc4d52c7902130a79e7d710';          BINARY_URL='https://github.com/adoptium/temurin11-binaries/releases/download/jdk-11.0.20.1%2B1/OpenJDK11U-jdk_ppc64le_linux_hotspot_11.0.20.1_1.tar.gz';          ;;        s390x|s390:64-bit)          ESUM='a7efbe804a4616d38b6ac0def40cd9feacc04aee2bb89132191f4d33fc0a7c1e';          BINARY_URL='https://github.com/adoptium/temurin11-binaries/releases/download/jdk-11.0.20.1%2B1/OpenJDK11U-jdk_s390x_linux_hotspot_11.0.20.1_1.tar.gz';          ;;        amd64|i386:x86-64)          ESUM='398a64bff002f0e3b0c01ecd24a1a32c83cb72a5255344219e9757d4ddd9f857';          BINARY_URL='https://github.com/adoptium/temurin11-binaries/releases/download/jdk-11.0.20.1%2B1/OpenJDK11U-jdk_x64_linux_hotspot_11.0.20.1_1.tar.gz';          ;;        *)          echo "Unsupported arch: ${ARCH}";          exit 1;          ;;     esac; 	  wget -O /tmp/openjdk.tar.gz ${BINARY_URL}; 	  echo "${ESUM} */tmp/openjdk.tar.gz" | sha256sum -c -; 	  mkdir -p "$JAVA_HOME"; 	  tar --extract 	      --file /tmp/openjdk.tar.gz 	      --directory "$JAVA_HOME" 	      --strip-components 1 	      --no-same-owner 	  ;     rm -f /tmp/openjdk.tar.gz ${JAVA_HOME}/lib/src.zip;     find "$JAVA_HOME/lib" -name '*.so' -exec dirname '{}' ';' | sort -u > /etc/ld.so.conf.d/docker-openjdk.conf;     ldconfig;     java -Xshare:dump;
# Fri, 13 Oct 2023 05:52:17 GMT
RUN echo Verifying install ...     && fileEncoding="$(echo 'System.out.println(System.getProperty("file.encoding"))' | jshell -s -)"; [ "$fileEncoding" = 'UTF-8' ]; rm -rf ~/.java     && echo javac --version && javac --version     && echo java --version && java --version     && echo Complete.
# Fri, 13 Oct 2023 05:52:17 GMT
COPY file:8b8864b3e02a33a579dc216fd51b28a6047bc8eeaa03045b258980fe0cf7fcb3 in /__cacert_entrypoint.sh 
# Fri, 13 Oct 2023 05:52:17 GMT
ENTRYPOINT ["/__cacert_entrypoint.sh"]
# Fri, 13 Oct 2023 05:52:17 GMT
CMD ["jshell"]
# Fri, 13 Oct 2023 06:04:32 GMT
CMD ["gradle"]
# Fri, 13 Oct 2023 06:04:32 GMT
ENV GRADLE_HOME=/opt/gradle
# Fri, 13 Oct 2023 06:04:33 GMT
RUN set -o errexit -o nounset     && echo "Adding gradle user and group"     && groupadd --system --gid 1000 gradle     && useradd --system --gid gradle --uid 1000 --shell /bin/bash --create-home gradle     && mkdir /home/gradle/.gradle     && chown --recursive gradle:gradle /home/gradle         && echo "Symlinking root Gradle cache to gradle Gradle cache"     && ln --symbolic /home/gradle/.gradle /root/.gradle
# Fri, 13 Oct 2023 06:04:33 GMT
VOLUME [/home/gradle/.gradle]
# Fri, 13 Oct 2023 06:04:33 GMT
WORKDIR /home/gradle
# Fri, 13 Oct 2023 06:04:51 GMT
RUN set -o errexit -o nounset     && apt-get update     && apt-get install --yes --no-install-recommends         unzip         wget                 bzr         git         git-lfs         mercurial         openssh-client         subversion     && rm --recursive --force /var/lib/apt/lists/*         && echo "Testing VCSes"     && which bzr     && which git     && which git-lfs     && which hg     && which svn
# Fri, 13 Oct 2023 06:04:52 GMT
ENV GRADLE_VERSION=8.4
# Fri, 13 Oct 2023 06:04:52 GMT
ARG GRADLE_DOWNLOAD_SHA256=3e1af3ae886920c3ac87f7a91f816c0c7c436f276a6eefdb3da152100fef72ae
# Fri, 13 Oct 2023 06:04:56 GMT
# ARGS: GRADLE_DOWNLOAD_SHA256=3e1af3ae886920c3ac87f7a91f816c0c7c436f276a6eefdb3da152100fef72ae
RUN set -o errexit -o nounset     && echo "Downloading Gradle"     && wget --no-verbose --output-document=gradle.zip "https://services.gradle.org/distributions/gradle-${GRADLE_VERSION}-bin.zip"         && echo "Checking Gradle download hash"     && echo "${GRADLE_DOWNLOAD_SHA256} *gradle.zip" | sha256sum --check -         && echo "Installing Gradle"     && unzip gradle.zip     && rm gradle.zip     && mv "gradle-${GRADLE_VERSION}" "${GRADLE_HOME}/"     && ln --symbolic "${GRADLE_HOME}/bin/gradle" /usr/bin/gradle
# Fri, 13 Oct 2023 06:04:57 GMT
USER gradle
# Fri, 13 Oct 2023 06:04:58 GMT
# ARGS: GRADLE_DOWNLOAD_SHA256=3e1af3ae886920c3ac87f7a91f816c0c7c436f276a6eefdb3da152100fef72ae
RUN set -o errexit -o nounset     && echo "Testing Gradle installation"     && gradle --version
# Fri, 13 Oct 2023 06:04:58 GMT
USER root
```

-	Layers:
	-	`sha256:7a2c559011895d255fce249c00396abff5ae7e0c0a92931d0ed493e71de78e3a`  
		Last Modified: Tue, 03 Oct 2023 17:02:08 GMT  
		Size: 28.6 MB (28580681 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d58ba2f5735c673e4fce5f702cdf0e513d89a91adfffc4e42977eae7cd354a0a`  
		Last Modified: Fri, 13 Oct 2023 05:56:23 GMT  
		Size: 16.9 MB (16919575 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:30d677692c8a5373e6ee3b096be7076eae8d013ed651d83fc141c85527e81bb7`  
		Last Modified: Fri, 13 Oct 2023 05:57:46 GMT  
		Size: 144.8 MB (144837057 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:93e66e5ce18ead7c0d7d222c41523a820292790767d90035db6be25ee830d3e3`  
		Last Modified: Fri, 13 Oct 2023 05:57:34 GMT  
		Size: 175.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:be18422839b9d0ec1b9e1569bf52d1f1530a90ffda19f071b6e03bbda620b267`  
		Last Modified: Fri, 13 Oct 2023 05:57:34 GMT  
		Size: 734.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7fedd32a83f9ece0cb85edd85b4b6d2e8baa0a240805c3806f07ede98e809c8a`  
		Last Modified: Fri, 13 Oct 2023 06:12:07 GMT  
		Size: 4.4 KB (4358 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:258ad07957d813b969c62edd3e017ccf421e58d4e21fb771e6ff0faa09687252`  
		Last Modified: Fri, 13 Oct 2023 06:12:18 GMT  
		Size: 65.5 MB (65487567 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5546c3f1e96ed4e4ca25c6962f9d6262f8f62ea018ebd338d00650769501c740`  
		Last Modified: Fri, 13 Oct 2023 06:12:15 GMT  
		Size: 131.0 MB (131009729 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8d87495e134f62cce28525a1fffa34646b6c11fedf351c3a245f2d5c3a29594b`  
		Last Modified: Fri, 13 Oct 2023 06:12:07 GMT  
		Size: 171.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `gradle:jdk11-focal` - linux; arm variant v7

```console
$ docker pull gradle@sha256:c8e33d5ceba84b985ed0daf83d69ec8e68a6fdab64cce5137594184ba80236a3
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **368.8 MB (368763353 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:9b57c5030f4a2088624835b272447fc9cd17c497a7996b35c929c7743eb265ed`
-	Entrypoint: `["\/__cacert_entrypoint.sh"]`
-	Default Command: `["gradle"]`

```dockerfile
# Tue, 03 Oct 2023 10:47:59 GMT
ARG RELEASE
# Tue, 03 Oct 2023 10:47:59 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Tue, 03 Oct 2023 10:47:59 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Tue, 03 Oct 2023 10:47:59 GMT
LABEL org.opencontainers.image.version=20.04
# Tue, 03 Oct 2023 10:48:06 GMT
ADD file:8dffbfada6e0bebb2858525182aef87ac2cbd88c624f32696ec2cb947e71a4f3 in / 
# Tue, 03 Oct 2023 10:48:07 GMT
CMD ["/bin/bash"]
# Fri, 13 Oct 2023 01:15:08 GMT
ENV JAVA_HOME=/opt/java/openjdk
# Fri, 13 Oct 2023 01:15:08 GMT
ENV PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Fri, 13 Oct 2023 01:15:08 GMT
ENV LANG=en_US.UTF-8 LANGUAGE=en_US:en LC_ALL=en_US.UTF-8
# Fri, 13 Oct 2023 01:15:32 GMT
RUN apt-get update     && DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends tzdata curl wget ca-certificates fontconfig locales p11-kit     && echo "en_US.UTF-8 UTF-8" >> /etc/locale.gen     && locale-gen en_US.UTF-8     && rm -rf /var/lib/apt/lists/*
# Fri, 13 Oct 2023 01:16:59 GMT
ENV JAVA_VERSION=jdk-11.0.20.1+1
# Fri, 13 Oct 2023 01:17:12 GMT
RUN set -eux;     ARCH="$(dpkg --print-architecture)";     case "${ARCH}" in        aarch64|arm64)          ESUM='69d39682c4a2fac294a9eaacbf62c26d3c8a2f9123f1b5d287498a5472c6b672';          BINARY_URL='https://github.com/adoptium/temurin11-binaries/releases/download/jdk-11.0.20.1%2B1/OpenJDK11U-jdk_aarch64_linux_hotspot_11.0.20.1_1.tar.gz';          ;;        armhf|arm)          ESUM='e83674aee238ebb5f359b9395b3c5e3fad5b645846095494662802d2f0fd01c9';          BINARY_URL='https://github.com/adoptium/temurin11-binaries/releases/download/jdk-11.0.20.1%2B1/OpenJDK11U-jdk_arm_linux_hotspot_11.0.20.1_1.tar.gz';          ;;        ppc64el|powerpc:common64)          ESUM='b806f4bb526161bf9b2ffb37be4e1b77f56b4e726dc4d52c7902130a79e7d710';          BINARY_URL='https://github.com/adoptium/temurin11-binaries/releases/download/jdk-11.0.20.1%2B1/OpenJDK11U-jdk_ppc64le_linux_hotspot_11.0.20.1_1.tar.gz';          ;;        s390x|s390:64-bit)          ESUM='a7efbe804a4616d38b6ac0def40cd9feacc04aee2bb89132191f4d33fc0a7c1e';          BINARY_URL='https://github.com/adoptium/temurin11-binaries/releases/download/jdk-11.0.20.1%2B1/OpenJDK11U-jdk_s390x_linux_hotspot_11.0.20.1_1.tar.gz';          ;;        amd64|i386:x86-64)          ESUM='398a64bff002f0e3b0c01ecd24a1a32c83cb72a5255344219e9757d4ddd9f857';          BINARY_URL='https://github.com/adoptium/temurin11-binaries/releases/download/jdk-11.0.20.1%2B1/OpenJDK11U-jdk_x64_linux_hotspot_11.0.20.1_1.tar.gz';          ;;        *)          echo "Unsupported arch: ${ARCH}";          exit 1;          ;;     esac; 	  wget -O /tmp/openjdk.tar.gz ${BINARY_URL}; 	  echo "${ESUM} */tmp/openjdk.tar.gz" | sha256sum -c -; 	  mkdir -p "$JAVA_HOME"; 	  tar --extract 	      --file /tmp/openjdk.tar.gz 	      --directory "$JAVA_HOME" 	      --strip-components 1 	      --no-same-owner 	  ;     rm -f /tmp/openjdk.tar.gz ${JAVA_HOME}/lib/src.zip;     find "$JAVA_HOME/lib" -name '*.so' -exec dirname '{}' ';' | sort -u > /etc/ld.so.conf.d/docker-openjdk.conf;     ldconfig;     java -Xshare:dump;
# Fri, 13 Oct 2023 01:17:16 GMT
RUN echo Verifying install ...     && fileEncoding="$(echo 'System.out.println(System.getProperty("file.encoding"))' | jshell -s -)"; [ "$fileEncoding" = 'UTF-8' ]; rm -rf ~/.java     && echo javac --version && javac --version     && echo java --version && java --version     && echo Complete.
# Fri, 13 Oct 2023 01:17:16 GMT
COPY file:8b8864b3e02a33a579dc216fd51b28a6047bc8eeaa03045b258980fe0cf7fcb3 in /__cacert_entrypoint.sh 
# Fri, 13 Oct 2023 01:17:16 GMT
ENTRYPOINT ["/__cacert_entrypoint.sh"]
# Fri, 13 Oct 2023 01:17:17 GMT
CMD ["jshell"]
# Fri, 13 Oct 2023 04:06:14 GMT
CMD ["gradle"]
# Fri, 13 Oct 2023 04:06:15 GMT
ENV GRADLE_HOME=/opt/gradle
# Fri, 13 Oct 2023 04:06:15 GMT
RUN set -o errexit -o nounset     && echo "Adding gradle user and group"     && groupadd --system --gid 1000 gradle     && useradd --system --gid gradle --uid 1000 --shell /bin/bash --create-home gradle     && mkdir /home/gradle/.gradle     && chown --recursive gradle:gradle /home/gradle         && echo "Symlinking root Gradle cache to gradle Gradle cache"     && ln --symbolic /home/gradle/.gradle /root/.gradle
# Fri, 13 Oct 2023 04:06:15 GMT
VOLUME [/home/gradle/.gradle]
# Fri, 13 Oct 2023 04:06:15 GMT
WORKDIR /home/gradle
# Fri, 13 Oct 2023 04:06:33 GMT
RUN set -o errexit -o nounset     && apt-get update     && apt-get install --yes --no-install-recommends         unzip         wget                 bzr         git         git-lfs         mercurial         openssh-client         subversion     && rm --recursive --force /var/lib/apt/lists/*         && echo "Testing VCSes"     && which bzr     && which git     && which git-lfs     && which hg     && which svn
# Fri, 13 Oct 2023 04:06:34 GMT
ENV GRADLE_VERSION=8.4
# Fri, 13 Oct 2023 04:06:34 GMT
ARG GRADLE_DOWNLOAD_SHA256=3e1af3ae886920c3ac87f7a91f816c0c7c436f276a6eefdb3da152100fef72ae
# Fri, 13 Oct 2023 04:06:40 GMT
# ARGS: GRADLE_DOWNLOAD_SHA256=3e1af3ae886920c3ac87f7a91f816c0c7c436f276a6eefdb3da152100fef72ae
RUN set -o errexit -o nounset     && echo "Downloading Gradle"     && wget --no-verbose --output-document=gradle.zip "https://services.gradle.org/distributions/gradle-${GRADLE_VERSION}-bin.zip"         && echo "Checking Gradle download hash"     && echo "${GRADLE_DOWNLOAD_SHA256} *gradle.zip" | sha256sum --check -         && echo "Installing Gradle"     && unzip gradle.zip     && rm gradle.zip     && mv "gradle-${GRADLE_VERSION}" "${GRADLE_HOME}/"     && ln --symbolic "${GRADLE_HOME}/bin/gradle" /usr/bin/gradle
# Fri, 13 Oct 2023 04:06:40 GMT
USER gradle
# Fri, 13 Oct 2023 04:06:42 GMT
# ARGS: GRADLE_DOWNLOAD_SHA256=3e1af3ae886920c3ac87f7a91f816c0c7c436f276a6eefdb3da152100fef72ae
RUN set -o errexit -o nounset     && echo "Testing Gradle installation"     && gradle --version
# Fri, 13 Oct 2023 04:06:42 GMT
USER root
```

-	Layers:
	-	`sha256:3b5f1ba1b648ae0824ed6a95ab17335537f8e689df99917fd374af5dd34078eb`  
		Last Modified: Fri, 13 Oct 2023 01:11:42 GMT  
		Size: 24.6 MB (24592174 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2807e7ba722152aeebf6e73ef8d6ba6473d71ef34b3c32b67bc40d66aa1f4e07`  
		Last Modified: Fri, 13 Oct 2023 01:20:27 GMT  
		Size: 15.7 MB (15658676 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:83b6efebb864fae50ee8cd9b640876645c9645aef1d405d30d60904f0a505a6c`  
		Last Modified: Fri, 13 Oct 2023 01:22:00 GMT  
		Size: 137.4 MB (137403123 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:06cc3887cbd4c33a7efeb6e3d94c42ecdf48522b930e5b5db13144cfc1bd569d`  
		Last Modified: Fri, 13 Oct 2023 01:21:41 GMT  
		Size: 177.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:62624f29f7044452d9f46d81cf63c6d6716d22e65450f34e4fa3e149d2504bf4`  
		Last Modified: Fri, 13 Oct 2023 01:21:41 GMT  
		Size: 733.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:47bab0e1c9d546f03957fca57a189523f936a6066bc6a4087fd4032af201a232`  
		Last Modified: Fri, 13 Oct 2023 04:12:24 GMT  
		Size: 4.3 KB (4348 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d0f598e951da11937db2f170ecccd90d8b4e7aa144f1b41b81a154f0d00902df`  
		Last Modified: Fri, 13 Oct 2023 04:12:34 GMT  
		Size: 60.1 MB (60094225 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:756c81a63684234dbcf2b36381016b659b2518d961f716a1e1fccd8ea1130a67`  
		Last Modified: Fri, 13 Oct 2023 04:12:31 GMT  
		Size: 131.0 MB (131009726 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d79d82cb1d5d1d8d36b3cf0519a81d09d341c1c2072189c0268d1eaabea51f02`  
		Last Modified: Fri, 13 Oct 2023 04:12:23 GMT  
		Size: 171.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `gradle:jdk11-focal` - linux; arm64 variant v8

```console
$ docker pull gradle@sha256:98b368dadb6927f0203079ef7f0b83bdef8634158003b3a591df399a2c24f752
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **381.8 MB (381801178 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e9b9b8d86ca9a535a8a4e7f128aab24a60feadd4e940030500fd6670f5b6ca48`
-	Entrypoint: `["\/__cacert_entrypoint.sh"]`
-	Default Command: `["gradle"]`

```dockerfile
# Tue, 03 Oct 2023 11:04:09 GMT
ARG RELEASE
# Tue, 03 Oct 2023 11:04:09 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Tue, 03 Oct 2023 11:04:09 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Tue, 03 Oct 2023 11:04:10 GMT
LABEL org.opencontainers.image.version=20.04
# Tue, 03 Oct 2023 11:04:16 GMT
ADD file:f70cc2610ea8fcd25e6e9ae727eb9345d5b7198102f6a6d8e458ab8f99efefc3 in / 
# Tue, 03 Oct 2023 11:04:17 GMT
CMD ["/bin/bash"]
# Fri, 13 Oct 2023 02:46:03 GMT
ENV JAVA_HOME=/opt/java/openjdk
# Fri, 13 Oct 2023 02:46:03 GMT
ENV PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Fri, 13 Oct 2023 02:46:03 GMT
ENV LANG=en_US.UTF-8 LANGUAGE=en_US:en LC_ALL=en_US.UTF-8
# Fri, 13 Oct 2023 02:46:20 GMT
RUN apt-get update     && DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends tzdata curl wget ca-certificates fontconfig locales p11-kit     && echo "en_US.UTF-8 UTF-8" >> /etc/locale.gen     && locale-gen en_US.UTF-8     && rm -rf /var/lib/apt/lists/*
# Fri, 13 Oct 2023 02:47:16 GMT
ENV JAVA_VERSION=jdk-11.0.20.1+1
# Fri, 13 Oct 2023 02:47:25 GMT
RUN set -eux;     ARCH="$(dpkg --print-architecture)";     case "${ARCH}" in        aarch64|arm64)          ESUM='69d39682c4a2fac294a9eaacbf62c26d3c8a2f9123f1b5d287498a5472c6b672';          BINARY_URL='https://github.com/adoptium/temurin11-binaries/releases/download/jdk-11.0.20.1%2B1/OpenJDK11U-jdk_aarch64_linux_hotspot_11.0.20.1_1.tar.gz';          ;;        armhf|arm)          ESUM='e83674aee238ebb5f359b9395b3c5e3fad5b645846095494662802d2f0fd01c9';          BINARY_URL='https://github.com/adoptium/temurin11-binaries/releases/download/jdk-11.0.20.1%2B1/OpenJDK11U-jdk_arm_linux_hotspot_11.0.20.1_1.tar.gz';          ;;        ppc64el|powerpc:common64)          ESUM='b806f4bb526161bf9b2ffb37be4e1b77f56b4e726dc4d52c7902130a79e7d710';          BINARY_URL='https://github.com/adoptium/temurin11-binaries/releases/download/jdk-11.0.20.1%2B1/OpenJDK11U-jdk_ppc64le_linux_hotspot_11.0.20.1_1.tar.gz';          ;;        s390x|s390:64-bit)          ESUM='a7efbe804a4616d38b6ac0def40cd9feacc04aee2bb89132191f4d33fc0a7c1e';          BINARY_URL='https://github.com/adoptium/temurin11-binaries/releases/download/jdk-11.0.20.1%2B1/OpenJDK11U-jdk_s390x_linux_hotspot_11.0.20.1_1.tar.gz';          ;;        amd64|i386:x86-64)          ESUM='398a64bff002f0e3b0c01ecd24a1a32c83cb72a5255344219e9757d4ddd9f857';          BINARY_URL='https://github.com/adoptium/temurin11-binaries/releases/download/jdk-11.0.20.1%2B1/OpenJDK11U-jdk_x64_linux_hotspot_11.0.20.1_1.tar.gz';          ;;        *)          echo "Unsupported arch: ${ARCH}";          exit 1;          ;;     esac; 	  wget -O /tmp/openjdk.tar.gz ${BINARY_URL}; 	  echo "${ESUM} */tmp/openjdk.tar.gz" | sha256sum -c -; 	  mkdir -p "$JAVA_HOME"; 	  tar --extract 	      --file /tmp/openjdk.tar.gz 	      --directory "$JAVA_HOME" 	      --strip-components 1 	      --no-same-owner 	  ;     rm -f /tmp/openjdk.tar.gz ${JAVA_HOME}/lib/src.zip;     find "$JAVA_HOME/lib" -name '*.so' -exec dirname '{}' ';' | sort -u > /etc/ld.so.conf.d/docker-openjdk.conf;     ldconfig;     java -Xshare:dump;
# Fri, 13 Oct 2023 02:47:27 GMT
RUN echo Verifying install ...     && fileEncoding="$(echo 'System.out.println(System.getProperty("file.encoding"))' | jshell -s -)"; [ "$fileEncoding" = 'UTF-8' ]; rm -rf ~/.java     && echo javac --version && javac --version     && echo java --version && java --version     && echo Complete.
# Fri, 13 Oct 2023 02:47:28 GMT
COPY file:8b8864b3e02a33a579dc216fd51b28a6047bc8eeaa03045b258980fe0cf7fcb3 in /__cacert_entrypoint.sh 
# Fri, 13 Oct 2023 02:47:28 GMT
ENTRYPOINT ["/__cacert_entrypoint.sh"]
# Fri, 13 Oct 2023 02:47:28 GMT
CMD ["jshell"]
# Fri, 13 Oct 2023 03:38:10 GMT
CMD ["gradle"]
# Fri, 13 Oct 2023 03:38:11 GMT
ENV GRADLE_HOME=/opt/gradle
# Fri, 13 Oct 2023 03:38:11 GMT
RUN set -o errexit -o nounset     && echo "Adding gradle user and group"     && groupadd --system --gid 1000 gradle     && useradd --system --gid gradle --uid 1000 --shell /bin/bash --create-home gradle     && mkdir /home/gradle/.gradle     && chown --recursive gradle:gradle /home/gradle         && echo "Symlinking root Gradle cache to gradle Gradle cache"     && ln --symbolic /home/gradle/.gradle /root/.gradle
# Fri, 13 Oct 2023 03:38:11 GMT
VOLUME [/home/gradle/.gradle]
# Fri, 13 Oct 2023 03:38:11 GMT
WORKDIR /home/gradle
# Fri, 13 Oct 2023 03:38:26 GMT
RUN set -o errexit -o nounset     && apt-get update     && apt-get install --yes --no-install-recommends         unzip         wget                 bzr         git         git-lfs         mercurial         openssh-client         subversion     && rm --recursive --force /var/lib/apt/lists/*         && echo "Testing VCSes"     && which bzr     && which git     && which git-lfs     && which hg     && which svn
# Fri, 13 Oct 2023 03:38:27 GMT
ENV GRADLE_VERSION=8.4
# Fri, 13 Oct 2023 03:38:27 GMT
ARG GRADLE_DOWNLOAD_SHA256=3e1af3ae886920c3ac87f7a91f816c0c7c436f276a6eefdb3da152100fef72ae
# Fri, 13 Oct 2023 03:38:31 GMT
# ARGS: GRADLE_DOWNLOAD_SHA256=3e1af3ae886920c3ac87f7a91f816c0c7c436f276a6eefdb3da152100fef72ae
RUN set -o errexit -o nounset     && echo "Downloading Gradle"     && wget --no-verbose --output-document=gradle.zip "https://services.gradle.org/distributions/gradle-${GRADLE_VERSION}-bin.zip"         && echo "Checking Gradle download hash"     && echo "${GRADLE_DOWNLOAD_SHA256} *gradle.zip" | sha256sum --check -         && echo "Installing Gradle"     && unzip gradle.zip     && rm gradle.zip     && mv "gradle-${GRADLE_VERSION}" "${GRADLE_HOME}/"     && ln --symbolic "${GRADLE_HOME}/bin/gradle" /usr/bin/gradle
# Fri, 13 Oct 2023 03:38:31 GMT
USER gradle
# Fri, 13 Oct 2023 03:38:32 GMT
# ARGS: GRADLE_DOWNLOAD_SHA256=3e1af3ae886920c3ac87f7a91f816c0c7c436f276a6eefdb3da152100fef72ae
RUN set -o errexit -o nounset     && echo "Testing Gradle installation"     && gradle --version
# Fri, 13 Oct 2023 03:38:32 GMT
USER root
```

-	Layers:
	-	`sha256:6cba4020c0a193cd551ed8edf368670967e3546345b52c4ec66cb0931436e9b9`  
		Last Modified: Thu, 05 Oct 2023 12:12:17 GMT  
		Size: 27.2 MB (27199503 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b3a7fe5b0236efc346cd4debc4c5e5b3c24c2c34ab5913c1647b26219f2c53f7`  
		Last Modified: Fri, 13 Oct 2023 02:50:41 GMT  
		Size: 16.8 MB (16768291 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:84562ffe350fd123902a28225215826843d7983e543835f54b2af29c6e3ce992`  
		Last Modified: Fri, 13 Oct 2023 02:51:51 GMT  
		Size: 141.6 MB (141584461 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:49bd8ecdd6a33dcccec3d07709e6f8f48487b45cfb79709d88776ac6325faf6a`  
		Last Modified: Fri, 13 Oct 2023 02:51:42 GMT  
		Size: 176.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e0b93572998af73b5ca61b23f8a00ca5bf4b6fdbf25853fbc3a76cdff635f9ff`  
		Last Modified: Fri, 13 Oct 2023 02:51:42 GMT  
		Size: 733.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:34289c25f724c8d00ea4d165b1bd93f84a8554b8d2a10cf8e066387e19248da6`  
		Last Modified: Fri, 13 Oct 2023 03:44:34 GMT  
		Size: 4.4 KB (4362 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a62bc036caa8bf6caf094dbb60c7481b7db86a6574beb7437c694419d62ed320`  
		Last Modified: Fri, 13 Oct 2023 03:44:42 GMT  
		Size: 65.2 MB (65233754 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c0853e7ff14e74da6a087f673a1cbcd7351e70f98e5aa23faff6a606e2c2ead1`  
		Last Modified: Fri, 13 Oct 2023 03:44:40 GMT  
		Size: 131.0 MB (131009730 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7e9d074d7c230ce0530b717019949fafab3084d93f939e574b34ef9155b8f785`  
		Last Modified: Fri, 13 Oct 2023 03:44:34 GMT  
		Size: 168.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `gradle:jdk11-focal` - linux; ppc64le

```console
$ docker pull gradle@sha256:40b9f3975ea63cf43ada79f511b0f8e6dac138b8c2969bb578edfa8f8a1f3d7e
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **388.4 MB (388366389 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d126f13f1dcecbef2f1c3bbfca45e4328d505c880829986f3af1e1871508b5b5`
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
# Thu, 31 Aug 2023 20:16:56 GMT
ENV JAVA_VERSION=jdk-11.0.20.1+1
# Thu, 31 Aug 2023 20:17:12 GMT
RUN set -eux;     ARCH="$(dpkg --print-architecture)";     case "${ARCH}" in        aarch64|arm64)          ESUM='69d39682c4a2fac294a9eaacbf62c26d3c8a2f9123f1b5d287498a5472c6b672';          BINARY_URL='https://github.com/adoptium/temurin11-binaries/releases/download/jdk-11.0.20.1%2B1/OpenJDK11U-jdk_aarch64_linux_hotspot_11.0.20.1_1.tar.gz';          ;;        armhf|arm)          ESUM='e83674aee238ebb5f359b9395b3c5e3fad5b645846095494662802d2f0fd01c9';          BINARY_URL='https://github.com/adoptium/temurin11-binaries/releases/download/jdk-11.0.20.1%2B1/OpenJDK11U-jdk_arm_linux_hotspot_11.0.20.1_1.tar.gz';          ;;        ppc64el|powerpc:common64)          ESUM='b806f4bb526161bf9b2ffb37be4e1b77f56b4e726dc4d52c7902130a79e7d710';          BINARY_URL='https://github.com/adoptium/temurin11-binaries/releases/download/jdk-11.0.20.1%2B1/OpenJDK11U-jdk_ppc64le_linux_hotspot_11.0.20.1_1.tar.gz';          ;;        s390x|s390:64-bit)          ESUM='a7efbe804a4616d38b6ac0def40cd9feacc04aee2bb89132191f4d33fc0a7c1e';          BINARY_URL='https://github.com/adoptium/temurin11-binaries/releases/download/jdk-11.0.20.1%2B1/OpenJDK11U-jdk_s390x_linux_hotspot_11.0.20.1_1.tar.gz';          ;;        amd64|i386:x86-64)          ESUM='398a64bff002f0e3b0c01ecd24a1a32c83cb72a5255344219e9757d4ddd9f857';          BINARY_URL='https://github.com/adoptium/temurin11-binaries/releases/download/jdk-11.0.20.1%2B1/OpenJDK11U-jdk_x64_linux_hotspot_11.0.20.1_1.tar.gz';          ;;        *)          echo "Unsupported arch: ${ARCH}";          exit 1;          ;;     esac; 	  wget -O /tmp/openjdk.tar.gz ${BINARY_URL}; 	  echo "${ESUM} */tmp/openjdk.tar.gz" | sha256sum -c -; 	  mkdir -p "$JAVA_HOME"; 	  tar --extract 	      --file /tmp/openjdk.tar.gz 	      --directory "$JAVA_HOME" 	      --strip-components 1 	      --no-same-owner 	  ;     rm -f /tmp/openjdk.tar.gz ${JAVA_HOME}/lib/src.zip;     find "$JAVA_HOME/lib" -name '*.so' -exec dirname '{}' ';' | sort -u > /etc/ld.so.conf.d/docker-openjdk.conf;     ldconfig;     java -Xshare:dump;
# Thu, 31 Aug 2023 20:17:17 GMT
RUN echo Verifying install ...     && fileEncoding="$(echo 'System.out.println(System.getProperty("file.encoding"))' | jshell -s -)"; [ "$fileEncoding" = 'UTF-8' ]; rm -rf ~/.java     && echo javac --version && javac --version     && echo java --version && java --version     && echo Complete.
# Thu, 31 Aug 2023 20:17:18 GMT
COPY file:8b8864b3e02a33a579dc216fd51b28a6047bc8eeaa03045b258980fe0cf7fcb3 in /__cacert_entrypoint.sh 
# Thu, 31 Aug 2023 20:17:18 GMT
ENTRYPOINT ["/__cacert_entrypoint.sh"]
# Thu, 31 Aug 2023 20:17:18 GMT
CMD ["jshell"]
# Thu, 31 Aug 2023 20:48:26 GMT
CMD ["gradle"]
# Thu, 31 Aug 2023 20:48:27 GMT
ENV GRADLE_HOME=/opt/gradle
# Thu, 31 Aug 2023 20:48:28 GMT
RUN set -o errexit -o nounset     && echo "Adding gradle user and group"     && groupadd --system --gid 1000 gradle     && useradd --system --gid gradle --uid 1000 --shell /bin/bash --create-home gradle     && mkdir /home/gradle/.gradle     && chown --recursive gradle:gradle /home/gradle         && echo "Symlinking root Gradle cache to gradle Gradle cache"     && ln --symbolic /home/gradle/.gradle /root/.gradle
# Thu, 31 Aug 2023 20:48:29 GMT
VOLUME [/home/gradle/.gradle]
# Thu, 31 Aug 2023 20:48:29 GMT
WORKDIR /home/gradle
# Thu, 31 Aug 2023 20:49:53 GMT
RUN set -o errexit -o nounset     && apt-get update     && apt-get install --yes --no-install-recommends         unzip         wget                 bzr         git         git-lfs         mercurial         openssh-client         subversion     && rm --recursive --force /var/lib/apt/lists/*         && echo "Testing VCSes"     && which bzr     && which git     && which git-lfs     && which hg     && which svn
# Fri, 06 Oct 2023 01:30:10 GMT
ENV GRADLE_VERSION=8.4
# Fri, 06 Oct 2023 01:30:11 GMT
ARG GRADLE_DOWNLOAD_SHA256=3e1af3ae886920c3ac87f7a91f816c0c7c436f276a6eefdb3da152100fef72ae
# Fri, 06 Oct 2023 01:30:22 GMT
# ARGS: GRADLE_DOWNLOAD_SHA256=3e1af3ae886920c3ac87f7a91f816c0c7c436f276a6eefdb3da152100fef72ae
RUN set -o errexit -o nounset     && echo "Downloading Gradle"     && wget --no-verbose --output-document=gradle.zip "https://services.gradle.org/distributions/gradle-${GRADLE_VERSION}-bin.zip"         && echo "Checking Gradle download hash"     && echo "${GRADLE_DOWNLOAD_SHA256} *gradle.zip" | sha256sum --check -         && echo "Installing Gradle"     && unzip gradle.zip     && rm gradle.zip     && mv "gradle-${GRADLE_VERSION}" "${GRADLE_HOME}/"     && ln --symbolic "${GRADLE_HOME}/bin/gradle" /usr/bin/gradle
# Fri, 06 Oct 2023 01:30:24 GMT
USER gradle
# Fri, 06 Oct 2023 01:30:28 GMT
# ARGS: GRADLE_DOWNLOAD_SHA256=3e1af3ae886920c3ac87f7a91f816c0c7c436f276a6eefdb3da152100fef72ae
RUN set -o errexit -o nounset     && echo "Testing Gradle installation"     && gradle --version
# Fri, 06 Oct 2023 01:30:29 GMT
USER root
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
	-	`sha256:b30ee14fec73736695fb4cee6ac87933d7493e949d7832275ce84c2a36e09f66`  
		Last Modified: Thu, 31 Aug 2023 20:23:46 GMT  
		Size: 132.0 MB (131990919 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:89d52b03773fac76edc9e535fc9401fbed2d27792dcbd8979603609eab47cf1f`  
		Last Modified: Thu, 31 Aug 2023 20:23:27 GMT  
		Size: 176.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:861af085ad56c1f66ce64a251101f0b954e21e4496417bb90b99b699e470975b`  
		Last Modified: Thu, 31 Aug 2023 20:23:27 GMT  
		Size: 734.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:940cded88a7477b2de2ee9479b4e9cb103db353f56ef02573ed6d724b48564c8`  
		Last Modified: Thu, 31 Aug 2023 20:57:56 GMT  
		Size: 4.4 KB (4361 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3ec48c52229befb5077960ef52d8c6093e097ddf13769cd48002ccb8eebfd14b`  
		Last Modified: Thu, 31 Aug 2023 20:58:16 GMT  
		Size: 73.8 MB (73837923 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0a2e45d96c5f8d6b9b2f7e012d0f3f952bdfa3a32ddaf0e0365a5ef7d9f43803`  
		Last Modified: Fri, 06 Oct 2023 01:37:45 GMT  
		Size: 131.0 MB (131009765 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:07b3e4ba4e00909e044f2dbb93fc82198e045c00108996d93c9c36d8bee34eaf`  
		Last Modified: Fri, 06 Oct 2023 01:37:32 GMT  
		Size: 171.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `gradle:jdk11-focal` - linux; s390x

```console
$ docker pull gradle@sha256:dda841cd1209a23c294048068f9cad07a835dc4b5bc359f3d693d519c2f4adc2
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **364.6 MB (364606967 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:0d143a1ff56e0ebee642d9f86901c3a11ea9860beb6f27ec424543f65865b235`
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
# Thu, 31 Aug 2023 19:41:50 GMT
ENV JAVA_VERSION=jdk-11.0.20.1+1
# Thu, 31 Aug 2023 19:41:59 GMT
RUN set -eux;     ARCH="$(dpkg --print-architecture)";     case "${ARCH}" in        aarch64|arm64)          ESUM='69d39682c4a2fac294a9eaacbf62c26d3c8a2f9123f1b5d287498a5472c6b672';          BINARY_URL='https://github.com/adoptium/temurin11-binaries/releases/download/jdk-11.0.20.1%2B1/OpenJDK11U-jdk_aarch64_linux_hotspot_11.0.20.1_1.tar.gz';          ;;        armhf|arm)          ESUM='e83674aee238ebb5f359b9395b3c5e3fad5b645846095494662802d2f0fd01c9';          BINARY_URL='https://github.com/adoptium/temurin11-binaries/releases/download/jdk-11.0.20.1%2B1/OpenJDK11U-jdk_arm_linux_hotspot_11.0.20.1_1.tar.gz';          ;;        ppc64el|powerpc:common64)          ESUM='b806f4bb526161bf9b2ffb37be4e1b77f56b4e726dc4d52c7902130a79e7d710';          BINARY_URL='https://github.com/adoptium/temurin11-binaries/releases/download/jdk-11.0.20.1%2B1/OpenJDK11U-jdk_ppc64le_linux_hotspot_11.0.20.1_1.tar.gz';          ;;        s390x|s390:64-bit)          ESUM='a7efbe804a4616d38b6ac0def40cd9feacc04aee2bb89132191f4d33fc0a7c1e';          BINARY_URL='https://github.com/adoptium/temurin11-binaries/releases/download/jdk-11.0.20.1%2B1/OpenJDK11U-jdk_s390x_linux_hotspot_11.0.20.1_1.tar.gz';          ;;        amd64|i386:x86-64)          ESUM='398a64bff002f0e3b0c01ecd24a1a32c83cb72a5255344219e9757d4ddd9f857';          BINARY_URL='https://github.com/adoptium/temurin11-binaries/releases/download/jdk-11.0.20.1%2B1/OpenJDK11U-jdk_x64_linux_hotspot_11.0.20.1_1.tar.gz';          ;;        *)          echo "Unsupported arch: ${ARCH}";          exit 1;          ;;     esac; 	  wget -O /tmp/openjdk.tar.gz ${BINARY_URL}; 	  echo "${ESUM} */tmp/openjdk.tar.gz" | sha256sum -c -; 	  mkdir -p "$JAVA_HOME"; 	  tar --extract 	      --file /tmp/openjdk.tar.gz 	      --directory "$JAVA_HOME" 	      --strip-components 1 	      --no-same-owner 	  ;     rm -f /tmp/openjdk.tar.gz ${JAVA_HOME}/lib/src.zip;     find "$JAVA_HOME/lib" -name '*.so' -exec dirname '{}' ';' | sort -u > /etc/ld.so.conf.d/docker-openjdk.conf;     ldconfig;     java -Xshare:dump;
# Thu, 31 Aug 2023 19:42:04 GMT
RUN echo Verifying install ...     && fileEncoding="$(echo 'System.out.println(System.getProperty("file.encoding"))' | jshell -s -)"; [ "$fileEncoding" = 'UTF-8' ]; rm -rf ~/.java     && echo javac --version && javac --version     && echo java --version && java --version     && echo Complete.
# Thu, 31 Aug 2023 19:42:04 GMT
COPY file:8b8864b3e02a33a579dc216fd51b28a6047bc8eeaa03045b258980fe0cf7fcb3 in /__cacert_entrypoint.sh 
# Thu, 31 Aug 2023 19:42:05 GMT
ENTRYPOINT ["/__cacert_entrypoint.sh"]
# Thu, 31 Aug 2023 19:42:05 GMT
CMD ["jshell"]
# Thu, 31 Aug 2023 20:06:52 GMT
CMD ["gradle"]
# Thu, 31 Aug 2023 20:06:53 GMT
ENV GRADLE_HOME=/opt/gradle
# Thu, 31 Aug 2023 20:06:53 GMT
RUN set -o errexit -o nounset     && echo "Adding gradle user and group"     && groupadd --system --gid 1000 gradle     && useradd --system --gid gradle --uid 1000 --shell /bin/bash --create-home gradle     && mkdir /home/gradle/.gradle     && chown --recursive gradle:gradle /home/gradle         && echo "Symlinking root Gradle cache to gradle Gradle cache"     && ln --symbolic /home/gradle/.gradle /root/.gradle
# Thu, 31 Aug 2023 20:06:53 GMT
VOLUME [/home/gradle/.gradle]
# Thu, 31 Aug 2023 20:06:53 GMT
WORKDIR /home/gradle
# Thu, 31 Aug 2023 20:07:23 GMT
RUN set -o errexit -o nounset     && apt-get update     && apt-get install --yes --no-install-recommends         unzip         wget                 bzr         git         git-lfs         mercurial         openssh-client         subversion     && rm --recursive --force /var/lib/apt/lists/*         && echo "Testing VCSes"     && which bzr     && which git     && which git-lfs     && which hg     && which svn
# Mon, 09 Oct 2023 16:16:40 GMT
ENV GRADLE_VERSION=8.4
# Mon, 09 Oct 2023 16:16:40 GMT
ARG GRADLE_DOWNLOAD_SHA256=3e1af3ae886920c3ac87f7a91f816c0c7c436f276a6eefdb3da152100fef72ae
# Mon, 09 Oct 2023 16:16:57 GMT
# ARGS: GRADLE_DOWNLOAD_SHA256=3e1af3ae886920c3ac87f7a91f816c0c7c436f276a6eefdb3da152100fef72ae
RUN set -o errexit -o nounset     && echo "Downloading Gradle"     && wget --no-verbose --output-document=gradle.zip "https://services.gradle.org/distributions/gradle-${GRADLE_VERSION}-bin.zip"         && echo "Checking Gradle download hash"     && echo "${GRADLE_DOWNLOAD_SHA256} *gradle.zip" | sha256sum --check -         && echo "Installing Gradle"     && unzip gradle.zip     && rm gradle.zip     && mv "gradle-${GRADLE_VERSION}" "${GRADLE_HOME}/"     && ln --symbolic "${GRADLE_HOME}/bin/gradle" /usr/bin/gradle
# Mon, 09 Oct 2023 16:17:04 GMT
USER gradle
# Mon, 09 Oct 2023 16:17:06 GMT
# ARGS: GRADLE_DOWNLOAD_SHA256=3e1af3ae886920c3ac87f7a91f816c0c7c436f276a6eefdb3da152100fef72ae
RUN set -o errexit -o nounset     && echo "Testing Gradle installation"     && gradle --version
# Mon, 09 Oct 2023 16:17:07 GMT
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
	-	`sha256:f4ceb6d4bd82bee749389964ee37c845ed6da28e4d7f2a8aabd4d00cf6f3489d`  
		Last Modified: Thu, 31 Aug 2023 19:45:47 GMT  
		Size: 125.1 MB (125138877 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:eacda34edf30c34b8f5348c9de1e2ddb4cd3c0bd53f7705818ee69d54fabaeb0`  
		Last Modified: Thu, 31 Aug 2023 19:45:38 GMT  
		Size: 172.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f84bc164ff5724d74feecac879b58a1b8cfd76c6876563d54d58cbbfeca8356a`  
		Last Modified: Thu, 31 Aug 2023 19:45:38 GMT  
		Size: 732.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7c9788d2ac921d7fc0e72c94996263dc7b87bc0f9788d7566c0a2a1442b66255`  
		Last Modified: Thu, 31 Aug 2023 20:12:13 GMT  
		Size: 4.4 KB (4363 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7b3e7baf5d284b9f8ccdba531b43fd46d6e5d0135e1279259b9efac66a1976c6`  
		Last Modified: Thu, 31 Aug 2023 20:12:23 GMT  
		Size: 64.8 MB (64795232 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:74268f6714a50a5eb09837f38a3055aec2ca5708d83dbd193528712ab5900d9d`  
		Last Modified: Mon, 09 Oct 2023 16:22:23 GMT  
		Size: 131.0 MB (131009766 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9a3bb6f7f2058532285cf56dea76d1d8be34e2e14ca50ddc924608edd6bb76d3`  
		Last Modified: Mon, 09 Oct 2023 16:22:14 GMT  
		Size: 171.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
