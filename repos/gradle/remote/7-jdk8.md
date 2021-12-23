## `gradle:7-jdk8`

```console
$ docker pull gradle@sha256:4bad60518f086a5a864766e62d0204f0fe12c328fc4bdb7179d8fa8fb31e28ce
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 4
	-	linux; amd64
	-	linux; arm variant v7
	-	linux; arm64 variant v8
	-	linux; ppc64le

### `gradle:7-jdk8` - linux; amd64

```console
$ docker pull gradle@sha256:00d18603fd86210afdf9488f8a027f4e196c7eee4d72613bd03008faa78ce8fd
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **329.6 MB (329647828 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:4af204e8f4cab91da64c5f39698db2e1d09261e9c1c5a047757ef236d0e112cf`
-	Default Command: `["gradle"]`

```dockerfile
# Sat, 16 Oct 2021 00:37:47 GMT
ADD file:5d68d27cc15a80653c93d3a0b262a28112d47a46326ff5fc2dfbf7fa3b9a0ce8 in / 
# Sat, 16 Oct 2021 00:37:47 GMT
CMD ["bash"]
# Sat, 16 Oct 2021 02:44:06 GMT
ENV LANG=en_US.UTF-8 LANGUAGE=en_US:en LC_ALL=en_US.UTF-8
# Mon, 29 Nov 2021 20:21:51 GMT
RUN apt-get update     && DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends tzdata curl ca-certificates fontconfig locales python-is-python3     && echo "en_US.UTF-8 UTF-8" >> /etc/locale.gen     && locale-gen en_US.UTF-8     && rm -rf /var/lib/apt/lists/*
# Mon, 29 Nov 2021 20:21:51 GMT
ENV JAVA_VERSION=jdk8u312-b07
# Mon, 29 Nov 2021 20:21:58 GMT
RUN set -eux;     ARCH="$(dpkg --print-architecture)";     case "${ARCH}" in        aarch64|arm64)          ESUM='87ff502eba3008cac71edeb9595398a73dc14883fe3072d152e731bf0877897e';          BINARY_URL='https://github.com/adoptium/temurin8-binaries/releases/download/jdk8u312-b07/OpenJDK8U-jdk_aarch64_linux_hotspot_8u312b07.tar.gz';          ;;        armhf|arm)          ESUM='5a9e72c6c20373aa380554a6d7191a258540d2a0399d842223b8d5eb0f74b298';          BINARY_URL='https://github.com/adoptium/temurin8-binaries/releases/download/jdk8u312-b07/OpenJDK8U-jdk_arm_linux_hotspot_8u312b07.tar.gz';          apt-get update          && DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends libatomic1          && rm -rf /var/lib/apt/lists/*          ;;        ppc64el|powerpc:common64)          ESUM='ddce3f067eab6fd98bb2a8ea3d18de6b09ea41d10382c76ad22bd3e7895951cf';          BINARY_URL='https://github.com/adoptium/temurin8-binaries/releases/download/jdk8u312-b07/OpenJDK8U-jdk_ppc64le_linux_hotspot_8u312b07.tar.gz';          ;;        amd64|i386:x86-64)          ESUM='699981083983b60a7eeb511ad640fae3ae4b879de5a3980fe837e8ade9c34a08';          BINARY_URL='https://github.com/adoptium/temurin8-binaries/releases/download/jdk8u312-b07/OpenJDK8U-jdk_x64_linux_hotspot_8u312b07.tar.gz';          ;;        *)          echo "Unsupported arch: ${ARCH}";          exit 1;          ;;     esac;     curl -LfsSo /tmp/openjdk.tar.gz ${BINARY_URL};     echo "${ESUM} */tmp/openjdk.tar.gz" | sha256sum -c -;     mkdir -p /opt/java/openjdk;     cd /opt/java/openjdk;     tar -xf /tmp/openjdk.tar.gz --strip-components=1;     rm -rf /tmp/openjdk.tar.gz;
# Mon, 29 Nov 2021 20:21:58 GMT
ENV JAVA_HOME=/opt/java/openjdk PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Mon, 29 Nov 2021 20:21:59 GMT
RUN echo Verifying install ...     && echo javac -version && javac -version     && echo java -version && java -version     && echo Complete.
# Tue, 30 Nov 2021 00:55:05 GMT
CMD ["gradle"]
# Tue, 30 Nov 2021 00:55:05 GMT
ENV GRADLE_HOME=/opt/gradle
# Tue, 30 Nov 2021 00:55:07 GMT
RUN set -o errexit -o nounset     && echo "Adding gradle user and group"     && groupadd --system --gid 1000 gradle     && useradd --system --gid gradle --uid 1000 --shell /bin/bash --create-home gradle     && mkdir /home/gradle/.gradle     && chown --recursive gradle:gradle /home/gradle         && echo "Symlinking root Gradle cache to gradle Gradle cache"     && ln --symbolic /home/gradle/.gradle /root/.gradle
# Tue, 30 Nov 2021 00:55:08 GMT
VOLUME [/home/gradle/.gradle]
# Tue, 30 Nov 2021 00:55:08 GMT
WORKDIR /home/gradle
# Tue, 30 Nov 2021 00:56:50 GMT
RUN set -o errexit -o nounset     && apt-get update     && apt-get install --yes --no-install-recommends         unzip         wget                 bzr         git         git-lfs         mercurial         openssh-client         subversion     && rm --recursive --force /var/lib/apt/lists/*         && echo "Testing VCSes"     && which bzr     && which git     && which git-lfs     && which hg     && which svn
# Wed, 22 Dec 2021 18:24:12 GMT
ENV GRADLE_VERSION=7.3.3
# Wed, 22 Dec 2021 18:24:12 GMT
ARG GRADLE_DOWNLOAD_SHA256=b586e04868a22fd817c8971330fec37e298f3242eb85c374181b12d637f80302
# Wed, 22 Dec 2021 18:24:18 GMT
# ARGS: GRADLE_DOWNLOAD_SHA256=b586e04868a22fd817c8971330fec37e298f3242eb85c374181b12d637f80302
RUN set -o errexit -o nounset     && echo "Downloading Gradle"     && wget --no-verbose --output-document=gradle.zip "https://services.gradle.org/distributions/gradle-${GRADLE_VERSION}-bin.zip"         && echo "Checking download hash"     && echo "${GRADLE_DOWNLOAD_SHA256} *gradle.zip" | sha256sum --check -         && echo "Installing Gradle"     && unzip gradle.zip     && rm gradle.zip     && mv "gradle-${GRADLE_VERSION}" "${GRADLE_HOME}/"     && ln --symbolic "${GRADLE_HOME}/bin/gradle" /usr/bin/gradle         && echo "Testing Gradle installation"     && gradle --version
```

-	Layers:
	-	`sha256:7b1a6ab2e44dbac178598dabe7cff59bd67233dba0b27e4fbd1f9d4b3c877a54`  
		Last Modified: Thu, 07 Oct 2021 23:44:23 GMT  
		Size: 28.6 MB (28567101 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5c122ee837fa892e5fdd4f7c857600f80a7b8fa855d2475bb325372d55eaff04`  
		Last Modified: Mon, 29 Nov 2021 20:25:31 GMT  
		Size: 24.8 MB (24814948 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2d17ed067016237a1002f776049c937fb67f102c9b479ab08fc1f38a66a10dc5`  
		Last Modified: Mon, 29 Nov 2021 20:25:36 GMT  
		Size: 103.6 MB (103602675 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:89aa7ee48d2c07dc1e91c77e52b708506e59c6f77c5ac335e0c79c1a34e9cceb`  
		Last Modified: Mon, 29 Nov 2021 20:25:27 GMT  
		Size: 160.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:be121367973f284edf4192fa1416240fc76489346c65c35a5b99afc4745575ca`  
		Last Modified: Tue, 30 Nov 2021 01:00:50 GMT  
		Size: 4.4 KB (4363 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9062319e972fbb9a79a6ec6f22473dbf23efdacc241ece055dd3b34ea24379fa`  
		Last Modified: Tue, 30 Nov 2021 01:01:06 GMT  
		Size: 56.9 MB (56873550 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ed11c964fa7346d709390ae4729c4ddf6378627dfc785e5a830ddba29bb1cc3a`  
		Last Modified: Wed, 22 Dec 2021 18:26:44 GMT  
		Size: 115.8 MB (115785031 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `gradle:7-jdk8` - linux; arm variant v7

```console
$ docker pull gradle@sha256:0628db447dcfe943a2c5e3571bc58144ac31f6ce87000c46897826d8ded2140f
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **314.1 MB (314091189 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:7d4482b978a685fd2c73b6dd0de93706dfc4d06d05ba95cccbeee4ae8d638be7`
-	Default Command: `["gradle"]`

```dockerfile
# Sat, 16 Oct 2021 01:12:00 GMT
ADD file:625e3906181f4bd86e59a0e9748f67fcb1391a2e65e36c729e71353381a49757 in / 
# Sat, 16 Oct 2021 01:12:00 GMT
CMD ["bash"]
# Sat, 16 Oct 2021 02:38:37 GMT
ENV LANG=en_US.UTF-8 LANGUAGE=en_US:en LC_ALL=en_US.UTF-8
# Mon, 29 Nov 2021 19:58:37 GMT
RUN apt-get update     && DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends tzdata curl ca-certificates fontconfig locales python-is-python3     && echo "en_US.UTF-8 UTF-8" >> /etc/locale.gen     && locale-gen en_US.UTF-8     && rm -rf /var/lib/apt/lists/*
# Mon, 29 Nov 2021 19:58:38 GMT
ENV JAVA_VERSION=jdk8u312-b07
# Mon, 29 Nov 2021 19:59:03 GMT
RUN set -eux;     ARCH="$(dpkg --print-architecture)";     case "${ARCH}" in        aarch64|arm64)          ESUM='87ff502eba3008cac71edeb9595398a73dc14883fe3072d152e731bf0877897e';          BINARY_URL='https://github.com/adoptium/temurin8-binaries/releases/download/jdk8u312-b07/OpenJDK8U-jdk_aarch64_linux_hotspot_8u312b07.tar.gz';          ;;        armhf|arm)          ESUM='5a9e72c6c20373aa380554a6d7191a258540d2a0399d842223b8d5eb0f74b298';          BINARY_URL='https://github.com/adoptium/temurin8-binaries/releases/download/jdk8u312-b07/OpenJDK8U-jdk_arm_linux_hotspot_8u312b07.tar.gz';          apt-get update          && DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends libatomic1          && rm -rf /var/lib/apt/lists/*          ;;        ppc64el|powerpc:common64)          ESUM='ddce3f067eab6fd98bb2a8ea3d18de6b09ea41d10382c76ad22bd3e7895951cf';          BINARY_URL='https://github.com/adoptium/temurin8-binaries/releases/download/jdk8u312-b07/OpenJDK8U-jdk_ppc64le_linux_hotspot_8u312b07.tar.gz';          ;;        amd64|i386:x86-64)          ESUM='699981083983b60a7eeb511ad640fae3ae4b879de5a3980fe837e8ade9c34a08';          BINARY_URL='https://github.com/adoptium/temurin8-binaries/releases/download/jdk8u312-b07/OpenJDK8U-jdk_x64_linux_hotspot_8u312b07.tar.gz';          ;;        *)          echo "Unsupported arch: ${ARCH}";          exit 1;          ;;     esac;     curl -LfsSo /tmp/openjdk.tar.gz ${BINARY_URL};     echo "${ESUM} */tmp/openjdk.tar.gz" | sha256sum -c -;     mkdir -p /opt/java/openjdk;     cd /opt/java/openjdk;     tar -xf /tmp/openjdk.tar.gz --strip-components=1;     rm -rf /tmp/openjdk.tar.gz;
# Mon, 29 Nov 2021 19:59:04 GMT
ENV JAVA_HOME=/opt/java/openjdk PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Mon, 29 Nov 2021 19:59:06 GMT
RUN echo Verifying install ...     && echo javac -version && javac -version     && echo java -version && java -version     && echo Complete.
# Mon, 29 Nov 2021 22:51:37 GMT
CMD ["gradle"]
# Mon, 29 Nov 2021 22:51:37 GMT
ENV GRADLE_HOME=/opt/gradle
# Mon, 29 Nov 2021 22:51:39 GMT
RUN set -o errexit -o nounset     && echo "Adding gradle user and group"     && groupadd --system --gid 1000 gradle     && useradd --system --gid gradle --uid 1000 --shell /bin/bash --create-home gradle     && mkdir /home/gradle/.gradle     && chown --recursive gradle:gradle /home/gradle         && echo "Symlinking root Gradle cache to gradle Gradle cache"     && ln --symbolic /home/gradle/.gradle /root/.gradle
# Mon, 29 Nov 2021 22:51:40 GMT
VOLUME [/home/gradle/.gradle]
# Mon, 29 Nov 2021 22:51:40 GMT
WORKDIR /home/gradle
# Mon, 29 Nov 2021 22:52:23 GMT
RUN set -o errexit -o nounset     && apt-get update     && apt-get install --yes --no-install-recommends         unzip         wget                 bzr         git         git-lfs         mercurial         openssh-client         subversion     && rm --recursive --force /var/lib/apt/lists/*         && echo "Testing VCSes"     && which bzr     && which git     && which git-lfs     && which hg     && which svn
# Thu, 23 Dec 2021 04:12:47 GMT
ENV GRADLE_VERSION=7.3.3
# Thu, 23 Dec 2021 04:12:48 GMT
ARG GRADLE_DOWNLOAD_SHA256=b586e04868a22fd817c8971330fec37e298f3242eb85c374181b12d637f80302
# Thu, 23 Dec 2021 04:13:00 GMT
# ARGS: GRADLE_DOWNLOAD_SHA256=b586e04868a22fd817c8971330fec37e298f3242eb85c374181b12d637f80302
RUN set -o errexit -o nounset     && echo "Downloading Gradle"     && wget --no-verbose --output-document=gradle.zip "https://services.gradle.org/distributions/gradle-${GRADLE_VERSION}-bin.zip"         && echo "Checking download hash"     && echo "${GRADLE_DOWNLOAD_SHA256} *gradle.zip" | sha256sum --check -         && echo "Installing Gradle"     && unzip gradle.zip     && rm gradle.zip     && mv "gradle-${GRADLE_VERSION}" "${GRADLE_HOME}/"     && ln --symbolic "${GRADLE_HOME}/bin/gradle" /usr/bin/gradle         && echo "Testing Gradle installation"     && gradle --version
```

-	Layers:
	-	`sha256:8795d4da4abd6abcafe7285749aa85d3a164999e84720a3845f764e56e306771`  
		Last Modified: Sat, 16 Oct 2021 01:15:01 GMT  
		Size: 24.1 MB (24064451 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5f49a73fe087725ab5b9956d86afb7a1ca7735fe7eb993e92d61d1d780acba64`  
		Last Modified: Mon, 29 Nov 2021 20:05:51 GMT  
		Size: 23.1 MB (23068723 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5c3a3a8c5177609c904ac5f3ade897ce11d2cfbeb33b39d5ad35478f991c135f`  
		Last Modified: Mon, 29 Nov 2021 20:06:17 GMT  
		Size: 99.3 MB (99274869 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5e927ab3c7e0d15a3d77ed50fad49172601ee50cee3503afb7cfa220f25ec4f4`  
		Last Modified: Mon, 29 Nov 2021 20:05:35 GMT  
		Size: 160.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a038d880c83158ff4de132fb634b4db68695fe4a7767ea7a775e4f422f4e5091`  
		Last Modified: Mon, 29 Nov 2021 22:59:34 GMT  
		Size: 4.3 KB (4348 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:de4500020d5632831f9009f2f92741644df8dda52e4ae20a9fa9883631d9a254`  
		Last Modified: Mon, 29 Nov 2021 23:00:11 GMT  
		Size: 51.9 MB (51893650 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8ba046066de8b327490abe903a6dee65af55112a7ccc8e3268f8e9ab2090161f`  
		Last Modified: Thu, 23 Dec 2021 04:18:42 GMT  
		Size: 115.8 MB (115784988 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `gradle:7-jdk8` - linux; arm64 variant v8

```console
$ docker pull gradle@sha256:35a25da3579692aececf86ef42e263f31264072695fe36a6082b459ed66efabe
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **326.9 MB (326944783 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:779d482712a75e8180230fd3bbdd959eb96b815a6f268f6b235c035057b9dfcc`
-	Default Command: `["gradle"]`

```dockerfile
# Sat, 16 Oct 2021 01:47:45 GMT
ADD file:ff4909f2124325dac58d43c617132325934ed48a5ab4c534d05f931fcf700a2f in / 
# Sat, 16 Oct 2021 01:47:45 GMT
CMD ["bash"]
# Sat, 16 Oct 2021 03:25:20 GMT
ENV LANG=en_US.UTF-8 LANGUAGE=en_US:en LC_ALL=en_US.UTF-8
# Mon, 29 Nov 2021 19:40:01 GMT
RUN apt-get update     && DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends tzdata curl ca-certificates fontconfig locales python-is-python3     && echo "en_US.UTF-8 UTF-8" >> /etc/locale.gen     && locale-gen en_US.UTF-8     && rm -rf /var/lib/apt/lists/*
# Mon, 29 Nov 2021 19:40:02 GMT
ENV JAVA_VERSION=jdk8u312-b07
# Mon, 29 Nov 2021 19:40:10 GMT
RUN set -eux;     ARCH="$(dpkg --print-architecture)";     case "${ARCH}" in        aarch64|arm64)          ESUM='87ff502eba3008cac71edeb9595398a73dc14883fe3072d152e731bf0877897e';          BINARY_URL='https://github.com/adoptium/temurin8-binaries/releases/download/jdk8u312-b07/OpenJDK8U-jdk_aarch64_linux_hotspot_8u312b07.tar.gz';          ;;        armhf|arm)          ESUM='5a9e72c6c20373aa380554a6d7191a258540d2a0399d842223b8d5eb0f74b298';          BINARY_URL='https://github.com/adoptium/temurin8-binaries/releases/download/jdk8u312-b07/OpenJDK8U-jdk_arm_linux_hotspot_8u312b07.tar.gz';          apt-get update          && DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends libatomic1          && rm -rf /var/lib/apt/lists/*          ;;        ppc64el|powerpc:common64)          ESUM='ddce3f067eab6fd98bb2a8ea3d18de6b09ea41d10382c76ad22bd3e7895951cf';          BINARY_URL='https://github.com/adoptium/temurin8-binaries/releases/download/jdk8u312-b07/OpenJDK8U-jdk_ppc64le_linux_hotspot_8u312b07.tar.gz';          ;;        amd64|i386:x86-64)          ESUM='699981083983b60a7eeb511ad640fae3ae4b879de5a3980fe837e8ade9c34a08';          BINARY_URL='https://github.com/adoptium/temurin8-binaries/releases/download/jdk8u312-b07/OpenJDK8U-jdk_x64_linux_hotspot_8u312b07.tar.gz';          ;;        *)          echo "Unsupported arch: ${ARCH}";          exit 1;          ;;     esac;     curl -LfsSo /tmp/openjdk.tar.gz ${BINARY_URL};     echo "${ESUM} */tmp/openjdk.tar.gz" | sha256sum -c -;     mkdir -p /opt/java/openjdk;     cd /opt/java/openjdk;     tar -xf /tmp/openjdk.tar.gz --strip-components=1;     rm -rf /tmp/openjdk.tar.gz;
# Mon, 29 Nov 2021 19:40:11 GMT
ENV JAVA_HOME=/opt/java/openjdk PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Mon, 29 Nov 2021 19:40:13 GMT
RUN echo Verifying install ...     && echo javac -version && javac -version     && echo java -version && java -version     && echo Complete.
# Mon, 29 Nov 2021 22:09:46 GMT
CMD ["gradle"]
# Mon, 29 Nov 2021 22:09:47 GMT
ENV GRADLE_HOME=/opt/gradle
# Mon, 29 Nov 2021 22:09:48 GMT
RUN set -o errexit -o nounset     && echo "Adding gradle user and group"     && groupadd --system --gid 1000 gradle     && useradd --system --gid gradle --uid 1000 --shell /bin/bash --create-home gradle     && mkdir /home/gradle/.gradle     && chown --recursive gradle:gradle /home/gradle         && echo "Symlinking root Gradle cache to gradle Gradle cache"     && ln --symbolic /home/gradle/.gradle /root/.gradle
# Mon, 29 Nov 2021 22:09:49 GMT
VOLUME [/home/gradle/.gradle]
# Mon, 29 Nov 2021 22:09:50 GMT
WORKDIR /home/gradle
# Mon, 29 Nov 2021 22:10:12 GMT
RUN set -o errexit -o nounset     && apt-get update     && apt-get install --yes --no-install-recommends         unzip         wget                 bzr         git         git-lfs         mercurial         openssh-client         subversion     && rm --recursive --force /var/lib/apt/lists/*         && echo "Testing VCSes"     && which bzr     && which git     && which git-lfs     && which hg     && which svn
# Wed, 22 Dec 2021 19:24:26 GMT
ENV GRADLE_VERSION=7.3.3
# Wed, 22 Dec 2021 19:24:26 GMT
ARG GRADLE_DOWNLOAD_SHA256=b586e04868a22fd817c8971330fec37e298f3242eb85c374181b12d637f80302
# Wed, 22 Dec 2021 19:24:33 GMT
# ARGS: GRADLE_DOWNLOAD_SHA256=b586e04868a22fd817c8971330fec37e298f3242eb85c374181b12d637f80302
RUN set -o errexit -o nounset     && echo "Downloading Gradle"     && wget --no-verbose --output-document=gradle.zip "https://services.gradle.org/distributions/gradle-${GRADLE_VERSION}-bin.zip"         && echo "Checking download hash"     && echo "${GRADLE_DOWNLOAD_SHA256} *gradle.zip" | sha256sum --check -         && echo "Installing Gradle"     && unzip gradle.zip     && rm gradle.zip     && mv "gradle-${GRADLE_VERSION}" "${GRADLE_HOME}/"     && ln --symbolic "${GRADLE_HOME}/bin/gradle" /usr/bin/gradle         && echo "Testing Gradle installation"     && gradle --version
```

-	Layers:
	-	`sha256:a39c84e173f038958d338f55a9e8ee64bb6643e8ac6ae98e08ca65146e668d86`  
		Last Modified: Sat, 09 Oct 2021 15:32:18 GMT  
		Size: 27.2 MB (27170900 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7fa42563dc02061b51ce62bff7340de9cea06ea720e8658d2a7693902aa8f700`  
		Last Modified: Mon, 29 Nov 2021 19:44:11 GMT  
		Size: 24.8 MB (24763049 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:343dd1f534fdf1b2da680fddc088c67d53fe32f7fd576b0f6be005126354cdf7`  
		Last Modified: Mon, 29 Nov 2021 19:44:17 GMT  
		Size: 102.7 MB (102728946 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5b923b78169a827f6588a2eeffba72af636d621c7523caa0ef1a430da82a5c6a`  
		Last Modified: Mon, 29 Nov 2021 19:44:06 GMT  
		Size: 128.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ac71010cfbc1b04836d4b9e4e43f290982c20b02a907f2fad042035a1f1a0b98`  
		Last Modified: Mon, 29 Nov 2021 22:13:32 GMT  
		Size: 4.3 KB (4312 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b7f957c6279b1687e4660b0cfca7e6478301a7f46b1212b2f85dfe2f3c402818`  
		Last Modified: Mon, 29 Nov 2021 22:13:42 GMT  
		Size: 56.5 MB (56492733 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8cb65ebe5dcbcc2f66605e327074ca555628475cdc9daaa1a5e5b5ad3597956c`  
		Last Modified: Wed, 22 Dec 2021 19:26:32 GMT  
		Size: 115.8 MB (115784715 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `gradle:7-jdk8` - linux; ppc64le

```console
$ docker pull gradle@sha256:06b59c72764e07eca9988800cfd047df0b4c811e905c8b68e31ecaa13bcefe64
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **341.4 MB (341396374 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:4341c51c767c1282adac0679f8798aa7dc00e4207aef32d2bfd3d13eed23e004`
-	Default Command: `["gradle"]`

```dockerfile
# Sat, 16 Oct 2021 00:36:38 GMT
ADD file:9246bf887411af1b286de95d779c11581dcef3c0d5a29e434162f0c085a7ce85 in / 
# Sat, 16 Oct 2021 00:36:44 GMT
CMD ["bash"]
# Sat, 16 Oct 2021 00:54:47 GMT
ENV LANG=en_US.UTF-8 LANGUAGE=en_US:en LC_ALL=en_US.UTF-8
# Mon, 29 Nov 2021 20:18:28 GMT
RUN apt-get update     && DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends tzdata curl ca-certificates fontconfig locales python-is-python3     && echo "en_US.UTF-8 UTF-8" >> /etc/locale.gen     && locale-gen en_US.UTF-8     && rm -rf /var/lib/apt/lists/*
# Mon, 29 Nov 2021 20:18:32 GMT
ENV JAVA_VERSION=jdk8u312-b07
# Mon, 29 Nov 2021 20:18:45 GMT
RUN set -eux;     ARCH="$(dpkg --print-architecture)";     case "${ARCH}" in        aarch64|arm64)          ESUM='87ff502eba3008cac71edeb9595398a73dc14883fe3072d152e731bf0877897e';          BINARY_URL='https://github.com/adoptium/temurin8-binaries/releases/download/jdk8u312-b07/OpenJDK8U-jdk_aarch64_linux_hotspot_8u312b07.tar.gz';          ;;        armhf|arm)          ESUM='5a9e72c6c20373aa380554a6d7191a258540d2a0399d842223b8d5eb0f74b298';          BINARY_URL='https://github.com/adoptium/temurin8-binaries/releases/download/jdk8u312-b07/OpenJDK8U-jdk_arm_linux_hotspot_8u312b07.tar.gz';          apt-get update          && DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends libatomic1          && rm -rf /var/lib/apt/lists/*          ;;        ppc64el|powerpc:common64)          ESUM='ddce3f067eab6fd98bb2a8ea3d18de6b09ea41d10382c76ad22bd3e7895951cf';          BINARY_URL='https://github.com/adoptium/temurin8-binaries/releases/download/jdk8u312-b07/OpenJDK8U-jdk_ppc64le_linux_hotspot_8u312b07.tar.gz';          ;;        amd64|i386:x86-64)          ESUM='699981083983b60a7eeb511ad640fae3ae4b879de5a3980fe837e8ade9c34a08';          BINARY_URL='https://github.com/adoptium/temurin8-binaries/releases/download/jdk8u312-b07/OpenJDK8U-jdk_x64_linux_hotspot_8u312b07.tar.gz';          ;;        *)          echo "Unsupported arch: ${ARCH}";          exit 1;          ;;     esac;     curl -LfsSo /tmp/openjdk.tar.gz ${BINARY_URL};     echo "${ESUM} */tmp/openjdk.tar.gz" | sha256sum -c -;     mkdir -p /opt/java/openjdk;     cd /opt/java/openjdk;     tar -xf /tmp/openjdk.tar.gz --strip-components=1;     rm -rf /tmp/openjdk.tar.gz;
# Mon, 29 Nov 2021 20:18:49 GMT
ENV JAVA_HOME=/opt/java/openjdk PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Mon, 29 Nov 2021 20:18:53 GMT
RUN echo Verifying install ...     && echo javac -version && javac -version     && echo java -version && java -version     && echo Complete.
# Mon, 29 Nov 2021 21:33:15 GMT
CMD ["gradle"]
# Mon, 29 Nov 2021 21:33:16 GMT
ENV GRADLE_HOME=/opt/gradle
# Mon, 29 Nov 2021 21:33:23 GMT
RUN set -o errexit -o nounset     && echo "Adding gradle user and group"     && groupadd --system --gid 1000 gradle     && useradd --system --gid gradle --uid 1000 --shell /bin/bash --create-home gradle     && mkdir /home/gradle/.gradle     && chown --recursive gradle:gradle /home/gradle         && echo "Symlinking root Gradle cache to gradle Gradle cache"     && ln --symbolic /home/gradle/.gradle /root/.gradle
# Mon, 29 Nov 2021 21:33:26 GMT
VOLUME [/home/gradle/.gradle]
# Mon, 29 Nov 2021 21:33:27 GMT
WORKDIR /home/gradle
# Mon, 29 Nov 2021 21:34:36 GMT
RUN set -o errexit -o nounset     && apt-get update     && apt-get install --yes --no-install-recommends         unzip         wget                 bzr         git         git-lfs         mercurial         openssh-client         subversion     && rm --recursive --force /var/lib/apt/lists/*         && echo "Testing VCSes"     && which bzr     && which git     && which git-lfs     && which hg     && which svn
# Wed, 22 Dec 2021 20:41:49 GMT
ENV GRADLE_VERSION=7.3.3
# Wed, 22 Dec 2021 20:41:50 GMT
ARG GRADLE_DOWNLOAD_SHA256=b586e04868a22fd817c8971330fec37e298f3242eb85c374181b12d637f80302
# Wed, 22 Dec 2021 20:42:04 GMT
# ARGS: GRADLE_DOWNLOAD_SHA256=b586e04868a22fd817c8971330fec37e298f3242eb85c374181b12d637f80302
RUN set -o errexit -o nounset     && echo "Downloading Gradle"     && wget --no-verbose --output-document=gradle.zip "https://services.gradle.org/distributions/gradle-${GRADLE_VERSION}-bin.zip"         && echo "Checking download hash"     && echo "${GRADLE_DOWNLOAD_SHA256} *gradle.zip" | sha256sum --check -         && echo "Installing Gradle"     && unzip gradle.zip     && rm gradle.zip     && mv "gradle-${GRADLE_VERSION}" "${GRADLE_HOME}/"     && ln --symbolic "${GRADLE_HOME}/bin/gradle" /usr/bin/gradle         && echo "Testing Gradle installation"     && gradle --version
```

-	Layers:
	-	`sha256:77ba7971d651af68e20e7cbb6603a3f7acd8ef2893066767a93db104723556f2`  
		Last Modified: Sat, 16 Oct 2021 00:38:38 GMT  
		Size: 33.3 MB (33287238 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4ce46da97c533978caacb28d5a66ed1f0b6374622ee6806ebe49cc2fa004597f`  
		Last Modified: Mon, 29 Nov 2021 20:25:42 GMT  
		Size: 26.6 MB (26647174 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2fc8ccd6cd9a35678f6f5196c114212c1b3ca78f5215402e7e565db899453b1e`  
		Last Modified: Mon, 29 Nov 2021 20:25:50 GMT  
		Size: 101.1 MB (101091939 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4fbe9312d48d242a8d6c73ff3231c06ef6b81af73780926567f62efe49685adf`  
		Last Modified: Mon, 29 Nov 2021 20:25:37 GMT  
		Size: 162.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2f54c6c94f1bb38d28386741c78c2de0ee2d5e390329fdf873d97830f2527293`  
		Last Modified: Mon, 29 Nov 2021 21:41:34 GMT  
		Size: 4.4 KB (4367 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:050811d0fd3ab362e5cc98787a41c6c7a6be980514e029ff62762bf5b9bda3f1`  
		Last Modified: Mon, 29 Nov 2021 21:41:47 GMT  
		Size: 64.6 MB (64580508 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:797856786a8817e288d525945dfd7182f05a2bfe9e0bb2d217c277cc78d55b9a`  
		Last Modified: Wed, 22 Dec 2021 20:44:43 GMT  
		Size: 115.8 MB (115784986 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
