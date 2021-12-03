## `gradle:7-jdk`

```console
$ docker pull gradle@sha256:9b0e1dc2a5ea94d14ee38b0aadfbec2d8c977c2ed732a7ef63a1f4e5d22b6608
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 5
	-	linux; amd64
	-	linux; arm variant v7
	-	linux; arm64 variant v8
	-	linux; ppc64le
	-	linux; s390x

### `gradle:7-jdk` - linux; amd64

```console
$ docker pull gradle@sha256:927dbceddf461859d025212e0bf9bd9cddfea742239c999cc1e219c7e1413aff
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **422.7 MB (422741256 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c87bed1d9fdd9b492854a070f8ee845de292c1c41bcd26ab0247d39c226975dd`
-	Default Command: `["gradle"]`

```dockerfile
# Sat, 16 Oct 2021 00:37:47 GMT
ADD file:5d68d27cc15a80653c93d3a0b262a28112d47a46326ff5fc2dfbf7fa3b9a0ce8 in / 
# Sat, 16 Oct 2021 00:37:47 GMT
CMD ["bash"]
# Sat, 16 Oct 2021 02:44:06 GMT
ENV LANG=en_US.UTF-8 LANGUAGE=en_US:en LC_ALL=en_US.UTF-8
# Mon, 29 Nov 2021 20:23:15 GMT
RUN apt-get update     && DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends tzdata curl ca-certificates fontconfig locales python-is-python3 binutils     && echo "en_US.UTF-8 UTF-8" >> /etc/locale.gen     && locale-gen en_US.UTF-8     && rm -rf /var/lib/apt/lists/*
# Mon, 29 Nov 2021 20:24:07 GMT
ENV JAVA_VERSION=jdk-17.0.1+12
# Mon, 29 Nov 2021 20:24:17 GMT
RUN set -eux;     ARCH="$(dpkg --print-architecture)";     case "${ARCH}" in        aarch64|arm64)          ESUM='f23d482b2b4ada08166201d1a0e299e3e371fdca5cd7288dcbd81ae82f3a75e3';          BINARY_URL='https://github.com/adoptium/temurin17-binaries/releases/download/jdk-17.0.1%2B12/OpenJDK17U-jdk_aarch64_linux_hotspot_17.0.1_12.tar.gz';          ;;        armhf|arm)          ESUM='f5945a39929384235e7cb1c57df071b8c7e49274632e2a54e54b2bad05de21a5';          BINARY_URL='https://github.com/adoptium/temurin17-binaries/releases/download/jdk-17.0.1%2B12/OpenJDK17U-jdk_arm_linux_hotspot_17.0.1_12.tar.gz';          ;;        ppc64el|powerpc:common64)          ESUM='bd65d4e8ecc4236924ae34d2075b956799abca594021e1b40c36aa08a0d610b0';          BINARY_URL='https://github.com/adoptium/temurin17-binaries/releases/download/jdk-17.0.1%2B12/OpenJDK17U-jdk_ppc64le_linux_hotspot_17.0.1_12.tar.gz';          ;;        s390x|s390:64-bit)          ESUM='dcc17e6ef28984656e997b6b8a6a31c89f45aff87a56b5d3819137c8f1050bef';          BINARY_URL='https://github.com/adoptium/temurin17-binaries/releases/download/jdk-17.0.1%2B12/OpenJDK17U-jdk_s390x_linux_hotspot_17.0.1_12.tar.gz';          ;;        amd64|i386:x86-64)          ESUM='6ea18c276dcbb8522feeebcfc3a4b5cb7c7e7368ba8590d3326c6c3efc5448b6';          BINARY_URL='https://github.com/adoptium/temurin17-binaries/releases/download/jdk-17.0.1%2B12/OpenJDK17U-jdk_x64_linux_hotspot_17.0.1_12.tar.gz';          ;;        *)          echo "Unsupported arch: ${ARCH}";          exit 1;          ;;     esac;     curl -LfsSo /tmp/openjdk.tar.gz ${BINARY_URL};     echo "${ESUM} */tmp/openjdk.tar.gz" | sha256sum -c -;     mkdir -p /opt/java/openjdk;     cd /opt/java/openjdk;     tar -xf /tmp/openjdk.tar.gz --strip-components=1;     rm -rf /tmp/openjdk.tar.gz;
# Mon, 29 Nov 2021 20:24:18 GMT
ENV JAVA_HOME=/opt/java/openjdk PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Mon, 29 Nov 2021 20:24:19 GMT
RUN echo Verifying install ...     && echo javac --version && javac --version     && echo java --version && java --version     && echo Complete.
# Mon, 29 Nov 2021 20:24:19 GMT
CMD ["jshell"]
# Tue, 30 Nov 2021 00:57:48 GMT
CMD ["gradle"]
# Tue, 30 Nov 2021 00:57:48 GMT
ENV GRADLE_HOME=/opt/gradle
# Tue, 30 Nov 2021 00:57:49 GMT
RUN set -o errexit -o nounset     && echo "Adding gradle user and group"     && groupadd --system --gid 1000 gradle     && useradd --system --gid gradle --uid 1000 --shell /bin/bash --create-home gradle     && mkdir /home/gradle/.gradle     && chown --recursive gradle:gradle /home/gradle         && echo "Symlinking root Gradle cache to gradle Gradle cache"     && ln --symbolic /home/gradle/.gradle /root/.gradle
# Tue, 30 Nov 2021 00:57:49 GMT
VOLUME [/home/gradle/.gradle]
# Tue, 30 Nov 2021 00:57:49 GMT
WORKDIR /home/gradle
# Tue, 30 Nov 2021 00:58:07 GMT
RUN set -o errexit -o nounset     && apt-get update     && apt-get install --yes --no-install-recommends         unzip         wget                 bzr         git         git-lfs         mercurial         openssh-client         subversion     && rm --recursive --force /var/lib/apt/lists/*         && echo "Testing VCSes"     && which bzr     && which git     && which git-lfs     && which hg     && which svn
# Tue, 30 Nov 2021 00:58:08 GMT
ENV GRADLE_VERSION=7.3
# Tue, 30 Nov 2021 00:58:08 GMT
ARG GRADLE_DOWNLOAD_SHA256=de8f52ad49bdc759164f72439a3bf56ddb1589c4cde802d3cec7d6ad0e0ee410
# Tue, 30 Nov 2021 00:58:14 GMT
# ARGS: GRADLE_DOWNLOAD_SHA256=de8f52ad49bdc759164f72439a3bf56ddb1589c4cde802d3cec7d6ad0e0ee410
RUN set -o errexit -o nounset     && echo "Downloading Gradle"     && wget --no-verbose --output-document=gradle.zip "https://services.gradle.org/distributions/gradle-${GRADLE_VERSION}-bin.zip"         && echo "Checking download hash"     && echo "${GRADLE_DOWNLOAD_SHA256} *gradle.zip" | sha256sum --check -         && echo "Installing Gradle"     && unzip gradle.zip     && rm gradle.zip     && mv "gradle-${GRADLE_VERSION}" "${GRADLE_HOME}/"     && ln --symbolic "${GRADLE_HOME}/bin/gradle" /usr/bin/gradle         && echo "Testing Gradle installation"     && gradle --version
```

-	Layers:
	-	`sha256:7b1a6ab2e44dbac178598dabe7cff59bd67233dba0b27e4fbd1f9d4b3c877a54`  
		Last Modified: Thu, 07 Oct 2021 23:44:23 GMT  
		Size: 28.6 MB (28567101 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8329695590e84b5300263017fbf5b303ea7b92c02e4805724cae67d76d617245`  
		Last Modified: Mon, 29 Nov 2021 20:26:59 GMT  
		Size: 28.6 MB (28563394 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9bd6da4468dba5d21638b5f59eac728f437dd482e8e439d64563176621dd576a`  
		Last Modified: Mon, 29 Nov 2021 20:27:40 GMT  
		Size: 192.9 MB (192948648 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8e07f21656cb7fda578ab5bfc2f4e302a9a0de2e0268746e56d5a5e5fd83af1b`  
		Last Modified: Mon, 29 Nov 2021 20:27:25 GMT  
		Size: 160.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ca055f63c6124f2685f4b6d4dee42c9c4994b01c478598f897f46d1535294d0a`  
		Last Modified: Tue, 30 Nov 2021 01:01:52 GMT  
		Size: 4.4 KB (4364 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8327f35ed409d7ecff475696d5257f34c10dd3a191d73755113cff0671a5dccb`  
		Last Modified: Tue, 30 Nov 2021 01:02:04 GMT  
		Size: 56.9 MB (56876562 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ef642c3463814c1f85f5706b342fd6600c1bb9a4704628463736eb7e0fe76889`  
		Last Modified: Tue, 30 Nov 2021 01:02:00 GMT  
		Size: 115.8 MB (115781027 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `gradle:7-jdk` - linux; arm variant v7

```console
$ docker pull gradle@sha256:76868f63be769387d7db07e591c8164f7b49fef87850edafed4adf75c1bbedf1
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **409.1 MB (409090170 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:7071f94a241baef304257e8f653a87b41a1246a08347f0653be9e2cf3f80f806`
-	Default Command: `["gradle"]`

```dockerfile
# Sat, 16 Oct 2021 01:12:00 GMT
ADD file:625e3906181f4bd86e59a0e9748f67fcb1391a2e65e36c729e71353381a49757 in / 
# Sat, 16 Oct 2021 01:12:00 GMT
CMD ["bash"]
# Sat, 16 Oct 2021 02:38:37 GMT
ENV LANG=en_US.UTF-8 LANGUAGE=en_US:en LC_ALL=en_US.UTF-8
# Mon, 29 Nov 2021 20:02:03 GMT
RUN apt-get update     && DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends tzdata curl ca-certificates fontconfig locales python-is-python3 binutils     && echo "en_US.UTF-8 UTF-8" >> /etc/locale.gen     && locale-gen en_US.UTF-8     && rm -rf /var/lib/apt/lists/*
# Mon, 29 Nov 2021 20:02:46 GMT
ENV JAVA_VERSION=jdk-17.0.1+12
# Mon, 29 Nov 2021 20:03:11 GMT
RUN set -eux;     ARCH="$(dpkg --print-architecture)";     case "${ARCH}" in        aarch64|arm64)          ESUM='f23d482b2b4ada08166201d1a0e299e3e371fdca5cd7288dcbd81ae82f3a75e3';          BINARY_URL='https://github.com/adoptium/temurin17-binaries/releases/download/jdk-17.0.1%2B12/OpenJDK17U-jdk_aarch64_linux_hotspot_17.0.1_12.tar.gz';          ;;        armhf|arm)          ESUM='f5945a39929384235e7cb1c57df071b8c7e49274632e2a54e54b2bad05de21a5';          BINARY_URL='https://github.com/adoptium/temurin17-binaries/releases/download/jdk-17.0.1%2B12/OpenJDK17U-jdk_arm_linux_hotspot_17.0.1_12.tar.gz';          ;;        ppc64el|powerpc:common64)          ESUM='bd65d4e8ecc4236924ae34d2075b956799abca594021e1b40c36aa08a0d610b0';          BINARY_URL='https://github.com/adoptium/temurin17-binaries/releases/download/jdk-17.0.1%2B12/OpenJDK17U-jdk_ppc64le_linux_hotspot_17.0.1_12.tar.gz';          ;;        s390x|s390:64-bit)          ESUM='dcc17e6ef28984656e997b6b8a6a31c89f45aff87a56b5d3819137c8f1050bef';          BINARY_URL='https://github.com/adoptium/temurin17-binaries/releases/download/jdk-17.0.1%2B12/OpenJDK17U-jdk_s390x_linux_hotspot_17.0.1_12.tar.gz';          ;;        amd64|i386:x86-64)          ESUM='6ea18c276dcbb8522feeebcfc3a4b5cb7c7e7368ba8590d3326c6c3efc5448b6';          BINARY_URL='https://github.com/adoptium/temurin17-binaries/releases/download/jdk-17.0.1%2B12/OpenJDK17U-jdk_x64_linux_hotspot_17.0.1_12.tar.gz';          ;;        *)          echo "Unsupported arch: ${ARCH}";          exit 1;          ;;     esac;     curl -LfsSo /tmp/openjdk.tar.gz ${BINARY_URL};     echo "${ESUM} */tmp/openjdk.tar.gz" | sha256sum -c -;     mkdir -p /opt/java/openjdk;     cd /opt/java/openjdk;     tar -xf /tmp/openjdk.tar.gz --strip-components=1;     rm -rf /tmp/openjdk.tar.gz;
# Mon, 29 Nov 2021 20:03:12 GMT
ENV JAVA_HOME=/opt/java/openjdk PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Mon, 29 Nov 2021 20:03:14 GMT
RUN echo Verifying install ...     && echo javac --version && javac --version     && echo java --version && java --version     && echo Complete.
# Mon, 29 Nov 2021 20:03:15 GMT
CMD ["jshell"]
# Mon, 29 Nov 2021 22:54:17 GMT
CMD ["gradle"]
# Mon, 29 Nov 2021 22:54:18 GMT
ENV GRADLE_HOME=/opt/gradle
# Mon, 29 Nov 2021 22:54:19 GMT
RUN set -o errexit -o nounset     && echo "Adding gradle user and group"     && groupadd --system --gid 1000 gradle     && useradd --system --gid gradle --uid 1000 --shell /bin/bash --create-home gradle     && mkdir /home/gradle/.gradle     && chown --recursive gradle:gradle /home/gradle         && echo "Symlinking root Gradle cache to gradle Gradle cache"     && ln --symbolic /home/gradle/.gradle /root/.gradle
# Mon, 29 Nov 2021 22:54:20 GMT
VOLUME [/home/gradle/.gradle]
# Mon, 29 Nov 2021 22:54:20 GMT
WORKDIR /home/gradle
# Mon, 29 Nov 2021 22:55:04 GMT
RUN set -o errexit -o nounset     && apt-get update     && apt-get install --yes --no-install-recommends         unzip         wget                 bzr         git         git-lfs         mercurial         openssh-client         subversion     && rm --recursive --force /var/lib/apt/lists/*         && echo "Testing VCSes"     && which bzr     && which git     && which git-lfs     && which hg     && which svn
# Mon, 29 Nov 2021 22:55:05 GMT
ENV GRADLE_VERSION=7.3
# Mon, 29 Nov 2021 22:55:05 GMT
ARG GRADLE_DOWNLOAD_SHA256=de8f52ad49bdc759164f72439a3bf56ddb1589c4cde802d3cec7d6ad0e0ee410
# Mon, 29 Nov 2021 22:55:18 GMT
# ARGS: GRADLE_DOWNLOAD_SHA256=de8f52ad49bdc759164f72439a3bf56ddb1589c4cde802d3cec7d6ad0e0ee410
RUN set -o errexit -o nounset     && echo "Downloading Gradle"     && wget --no-verbose --output-document=gradle.zip "https://services.gradle.org/distributions/gradle-${GRADLE_VERSION}-bin.zip"         && echo "Checking download hash"     && echo "${GRADLE_DOWNLOAD_SHA256} *gradle.zip" | sha256sum --check -         && echo "Installing Gradle"     && unzip gradle.zip     && rm gradle.zip     && mv "gradle-${GRADLE_VERSION}" "${GRADLE_HOME}/"     && ln --symbolic "${GRADLE_HOME}/bin/gradle" /usr/bin/gradle         && echo "Testing Gradle installation"     && gradle --version
```

-	Layers:
	-	`sha256:8795d4da4abd6abcafe7285749aa85d3a164999e84720a3845f764e56e306771`  
		Last Modified: Sat, 16 Oct 2021 01:15:01 GMT  
		Size: 24.1 MB (24064451 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b01ac063d17e84c31998292290d215bdc4fac4ff250c6809c5fde3571256b123`  
		Last Modified: Mon, 29 Nov 2021 20:09:29 GMT  
		Size: 27.4 MB (27369751 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a36fd1c4c8d6897c78d7d70bf2ab9fba49808f14c44c092a78307840b8e2dba8`  
		Last Modified: Mon, 29 Nov 2021 20:11:51 GMT  
		Size: 190.0 MB (189974990 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:091e34fd451454ce296353582cd1eee9119a4502276acefe2275f3ddeeef3add`  
		Last Modified: Mon, 29 Nov 2021 20:10:39 GMT  
		Size: 160.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:72de0b2d2ba2141054daec5a39c50b7a8a07046a702363cbc6278bd1a1309ac3`  
		Last Modified: Mon, 29 Nov 2021 23:01:32 GMT  
		Size: 4.3 KB (4350 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7f655a3c5567d1eccbc3aece92e4bb104bc1feb4fb0ce60ca29a2439e1db0466`  
		Last Modified: Mon, 29 Nov 2021 23:02:09 GMT  
		Size: 51.9 MB (51895389 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5de96262831353d15803ef12d2426a7cff43f8636ff709913bee5ca4d31e1278`  
		Last Modified: Mon, 29 Nov 2021 23:02:04 GMT  
		Size: 115.8 MB (115781079 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `gradle:7-jdk` - linux; arm64 variant v8

```console
$ docker pull gradle@sha256:c04db9d18cfbdb8ef0d398e2e97204705de002c9244b3d417116d330caf72613
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **418.7 MB (418694029 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b60d2a4ba1bef9fb8c643711175ced1eade484a0cbef5f1ce57c719b527d3901`
-	Default Command: `["gradle"]`

```dockerfile
# Sat, 16 Oct 2021 01:47:45 GMT
ADD file:ff4909f2124325dac58d43c617132325934ed48a5ab4c534d05f931fcf700a2f in / 
# Sat, 16 Oct 2021 01:47:45 GMT
CMD ["bash"]
# Sat, 16 Oct 2021 03:25:20 GMT
ENV LANG=en_US.UTF-8 LANGUAGE=en_US:en LC_ALL=en_US.UTF-8
# Mon, 29 Nov 2021 19:41:49 GMT
RUN apt-get update     && DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends tzdata curl ca-certificates fontconfig locales python-is-python3 binutils     && echo "en_US.UTF-8 UTF-8" >> /etc/locale.gen     && locale-gen en_US.UTF-8     && rm -rf /var/lib/apt/lists/*
# Mon, 29 Nov 2021 19:42:22 GMT
ENV JAVA_VERSION=jdk-17.0.1+12
# Mon, 29 Nov 2021 19:42:32 GMT
RUN set -eux;     ARCH="$(dpkg --print-architecture)";     case "${ARCH}" in        aarch64|arm64)          ESUM='f23d482b2b4ada08166201d1a0e299e3e371fdca5cd7288dcbd81ae82f3a75e3';          BINARY_URL='https://github.com/adoptium/temurin17-binaries/releases/download/jdk-17.0.1%2B12/OpenJDK17U-jdk_aarch64_linux_hotspot_17.0.1_12.tar.gz';          ;;        armhf|arm)          ESUM='f5945a39929384235e7cb1c57df071b8c7e49274632e2a54e54b2bad05de21a5';          BINARY_URL='https://github.com/adoptium/temurin17-binaries/releases/download/jdk-17.0.1%2B12/OpenJDK17U-jdk_arm_linux_hotspot_17.0.1_12.tar.gz';          ;;        ppc64el|powerpc:common64)          ESUM='bd65d4e8ecc4236924ae34d2075b956799abca594021e1b40c36aa08a0d610b0';          BINARY_URL='https://github.com/adoptium/temurin17-binaries/releases/download/jdk-17.0.1%2B12/OpenJDK17U-jdk_ppc64le_linux_hotspot_17.0.1_12.tar.gz';          ;;        s390x|s390:64-bit)          ESUM='dcc17e6ef28984656e997b6b8a6a31c89f45aff87a56b5d3819137c8f1050bef';          BINARY_URL='https://github.com/adoptium/temurin17-binaries/releases/download/jdk-17.0.1%2B12/OpenJDK17U-jdk_s390x_linux_hotspot_17.0.1_12.tar.gz';          ;;        amd64|i386:x86-64)          ESUM='6ea18c276dcbb8522feeebcfc3a4b5cb7c7e7368ba8590d3326c6c3efc5448b6';          BINARY_URL='https://github.com/adoptium/temurin17-binaries/releases/download/jdk-17.0.1%2B12/OpenJDK17U-jdk_x64_linux_hotspot_17.0.1_12.tar.gz';          ;;        *)          echo "Unsupported arch: ${ARCH}";          exit 1;          ;;     esac;     curl -LfsSo /tmp/openjdk.tar.gz ${BINARY_URL};     echo "${ESUM} */tmp/openjdk.tar.gz" | sha256sum -c -;     mkdir -p /opt/java/openjdk;     cd /opt/java/openjdk;     tar -xf /tmp/openjdk.tar.gz --strip-components=1;     rm -rf /tmp/openjdk.tar.gz;
# Mon, 29 Nov 2021 19:42:33 GMT
ENV JAVA_HOME=/opt/java/openjdk PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Mon, 29 Nov 2021 19:42:35 GMT
RUN echo Verifying install ...     && echo javac --version && javac --version     && echo java --version && java --version     && echo Complete.
# Mon, 29 Nov 2021 19:42:35 GMT
CMD ["jshell"]
# Mon, 29 Nov 2021 22:11:08 GMT
CMD ["gradle"]
# Mon, 29 Nov 2021 22:11:09 GMT
ENV GRADLE_HOME=/opt/gradle
# Mon, 29 Nov 2021 22:11:10 GMT
RUN set -o errexit -o nounset     && echo "Adding gradle user and group"     && groupadd --system --gid 1000 gradle     && useradd --system --gid gradle --uid 1000 --shell /bin/bash --create-home gradle     && mkdir /home/gradle/.gradle     && chown --recursive gradle:gradle /home/gradle         && echo "Symlinking root Gradle cache to gradle Gradle cache"     && ln --symbolic /home/gradle/.gradle /root/.gradle
# Mon, 29 Nov 2021 22:11:11 GMT
VOLUME [/home/gradle/.gradle]
# Mon, 29 Nov 2021 22:11:12 GMT
WORKDIR /home/gradle
# Mon, 29 Nov 2021 22:11:33 GMT
RUN set -o errexit -o nounset     && apt-get update     && apt-get install --yes --no-install-recommends         unzip         wget                 bzr         git         git-lfs         mercurial         openssh-client         subversion     && rm --recursive --force /var/lib/apt/lists/*         && echo "Testing VCSes"     && which bzr     && which git     && which git-lfs     && which hg     && which svn
# Fri, 03 Dec 2021 16:30:21 GMT
ENV GRADLE_VERSION=7.3.1
# Fri, 03 Dec 2021 16:30:21 GMT
ARG GRADLE_DOWNLOAD_SHA256=9afb3ca688fc12c761a0e9e4321e4d24e977a4a8916c8a768b1fe05ddb4d6b66
# Fri, 03 Dec 2021 16:30:28 GMT
# ARGS: GRADLE_DOWNLOAD_SHA256=9afb3ca688fc12c761a0e9e4321e4d24e977a4a8916c8a768b1fe05ddb4d6b66
RUN set -o errexit -o nounset     && echo "Downloading Gradle"     && wget --no-verbose --output-document=gradle.zip "https://services.gradle.org/distributions/gradle-${GRADLE_VERSION}-bin.zip"         && echo "Checking download hash"     && echo "${GRADLE_DOWNLOAD_SHA256} *gradle.zip" | sha256sum --check -         && echo "Installing Gradle"     && unzip gradle.zip     && rm gradle.zip     && mv "gradle-${GRADLE_VERSION}" "${GRADLE_HOME}/"     && ln --symbolic "${GRADLE_HOME}/bin/gradle" /usr/bin/gradle         && echo "Testing Gradle installation"     && gradle --version
```

-	Layers:
	-	`sha256:a39c84e173f038958d338f55a9e8ee64bb6643e8ac6ae98e08ca65146e668d86`  
		Last Modified: Sat, 09 Oct 2021 15:32:18 GMT  
		Size: 27.2 MB (27170900 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e4bc7e92316b9d4dee98cf60f4fcb0995823e001fcc5448df92e5fb76485370a`  
		Last Modified: Mon, 29 Nov 2021 19:45:52 GMT  
		Size: 29.4 MB (29377186 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:95d180b2dc1c1c285d6e2b151165c27dfd9d9be3b7b441f2e63cebd618fb21cd`  
		Last Modified: Mon, 29 Nov 2021 19:46:39 GMT  
		Size: 189.9 MB (189863189 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:eba9302b1d1d2223c79e74b1bc37844906cf1abe5d734079f9344f3db9d462ba`  
		Last Modified: Mon, 29 Nov 2021 19:46:21 GMT  
		Size: 128.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9cdd1388c163bb1b0d99d3a3f8b55fe5972f4facf74af6e506a7ab7135a80ff8`  
		Last Modified: Mon, 29 Nov 2021 22:14:28 GMT  
		Size: 4.3 KB (4313 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a9909b6491f7912220c96600f10a2236d29168a6291a52e66f9f7eb303ea0f76`  
		Last Modified: Mon, 29 Nov 2021 22:14:38 GMT  
		Size: 56.5 MB (56495513 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c532aa2081b8db7d99ba624d58157dae5131de7e5b96fad4f9531b9c8c83b3bd`  
		Last Modified: Fri, 03 Dec 2021 16:32:58 GMT  
		Size: 115.8 MB (115782800 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `gradle:7-jdk` - linux; ppc64le

```console
$ docker pull gradle@sha256:22325bb57377d09401f5c213a9e02e636c2a7db4ee6efba284eba9306b7a2f26
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **433.4 MB (433359569 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:2cb7cf69e54fb38d32602f1c8f16327f2bfa3ed904df913c3d4ec99ee5d700a1`
-	Default Command: `["gradle"]`

```dockerfile
# Sat, 16 Oct 2021 00:36:38 GMT
ADD file:9246bf887411af1b286de95d779c11581dcef3c0d5a29e434162f0c085a7ce85 in / 
# Sat, 16 Oct 2021 00:36:44 GMT
CMD ["bash"]
# Sat, 16 Oct 2021 00:54:47 GMT
ENV LANG=en_US.UTF-8 LANGUAGE=en_US:en LC_ALL=en_US.UTF-8
# Mon, 29 Nov 2021 20:22:29 GMT
RUN apt-get update     && DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends tzdata curl ca-certificates fontconfig locales python-is-python3 binutils     && echo "en_US.UTF-8 UTF-8" >> /etc/locale.gen     && locale-gen en_US.UTF-8     && rm -rf /var/lib/apt/lists/*
# Mon, 29 Nov 2021 20:23:23 GMT
ENV JAVA_VERSION=jdk-17.0.1+12
# Mon, 29 Nov 2021 20:23:42 GMT
RUN set -eux;     ARCH="$(dpkg --print-architecture)";     case "${ARCH}" in        aarch64|arm64)          ESUM='f23d482b2b4ada08166201d1a0e299e3e371fdca5cd7288dcbd81ae82f3a75e3';          BINARY_URL='https://github.com/adoptium/temurin17-binaries/releases/download/jdk-17.0.1%2B12/OpenJDK17U-jdk_aarch64_linux_hotspot_17.0.1_12.tar.gz';          ;;        armhf|arm)          ESUM='f5945a39929384235e7cb1c57df071b8c7e49274632e2a54e54b2bad05de21a5';          BINARY_URL='https://github.com/adoptium/temurin17-binaries/releases/download/jdk-17.0.1%2B12/OpenJDK17U-jdk_arm_linux_hotspot_17.0.1_12.tar.gz';          ;;        ppc64el|powerpc:common64)          ESUM='bd65d4e8ecc4236924ae34d2075b956799abca594021e1b40c36aa08a0d610b0';          BINARY_URL='https://github.com/adoptium/temurin17-binaries/releases/download/jdk-17.0.1%2B12/OpenJDK17U-jdk_ppc64le_linux_hotspot_17.0.1_12.tar.gz';          ;;        s390x|s390:64-bit)          ESUM='dcc17e6ef28984656e997b6b8a6a31c89f45aff87a56b5d3819137c8f1050bef';          BINARY_URL='https://github.com/adoptium/temurin17-binaries/releases/download/jdk-17.0.1%2B12/OpenJDK17U-jdk_s390x_linux_hotspot_17.0.1_12.tar.gz';          ;;        amd64|i386:x86-64)          ESUM='6ea18c276dcbb8522feeebcfc3a4b5cb7c7e7368ba8590d3326c6c3efc5448b6';          BINARY_URL='https://github.com/adoptium/temurin17-binaries/releases/download/jdk-17.0.1%2B12/OpenJDK17U-jdk_x64_linux_hotspot_17.0.1_12.tar.gz';          ;;        *)          echo "Unsupported arch: ${ARCH}";          exit 1;          ;;     esac;     curl -LfsSo /tmp/openjdk.tar.gz ${BINARY_URL};     echo "${ESUM} */tmp/openjdk.tar.gz" | sha256sum -c -;     mkdir -p /opt/java/openjdk;     cd /opt/java/openjdk;     tar -xf /tmp/openjdk.tar.gz --strip-components=1;     rm -rf /tmp/openjdk.tar.gz;
# Mon, 29 Nov 2021 20:23:48 GMT
ENV JAVA_HOME=/opt/java/openjdk PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Mon, 29 Nov 2021 20:23:52 GMT
RUN echo Verifying install ...     && echo javac --version && javac --version     && echo java --version && java --version     && echo Complete.
# Mon, 29 Nov 2021 20:23:53 GMT
CMD ["jshell"]
# Mon, 29 Nov 2021 21:37:21 GMT
CMD ["gradle"]
# Mon, 29 Nov 2021 21:37:23 GMT
ENV GRADLE_HOME=/opt/gradle
# Mon, 29 Nov 2021 21:37:27 GMT
RUN set -o errexit -o nounset     && echo "Adding gradle user and group"     && groupadd --system --gid 1000 gradle     && useradd --system --gid gradle --uid 1000 --shell /bin/bash --create-home gradle     && mkdir /home/gradle/.gradle     && chown --recursive gradle:gradle /home/gradle         && echo "Symlinking root Gradle cache to gradle Gradle cache"     && ln --symbolic /home/gradle/.gradle /root/.gradle
# Mon, 29 Nov 2021 21:37:28 GMT
VOLUME [/home/gradle/.gradle]
# Mon, 29 Nov 2021 21:37:32 GMT
WORKDIR /home/gradle
# Mon, 29 Nov 2021 21:38:38 GMT
RUN set -o errexit -o nounset     && apt-get update     && apt-get install --yes --no-install-recommends         unzip         wget                 bzr         git         git-lfs         mercurial         openssh-client         subversion     && rm --recursive --force /var/lib/apt/lists/*         && echo "Testing VCSes"     && which bzr     && which git     && which git-lfs     && which hg     && which svn
# Fri, 03 Dec 2021 17:42:20 GMT
ENV GRADLE_VERSION=7.3.1
# Fri, 03 Dec 2021 17:42:22 GMT
ARG GRADLE_DOWNLOAD_SHA256=9afb3ca688fc12c761a0e9e4321e4d24e977a4a8916c8a768b1fe05ddb4d6b66
# Fri, 03 Dec 2021 17:42:47 GMT
# ARGS: GRADLE_DOWNLOAD_SHA256=9afb3ca688fc12c761a0e9e4321e4d24e977a4a8916c8a768b1fe05ddb4d6b66
RUN set -o errexit -o nounset     && echo "Downloading Gradle"     && wget --no-verbose --output-document=gradle.zip "https://services.gradle.org/distributions/gradle-${GRADLE_VERSION}-bin.zip"         && echo "Checking download hash"     && echo "${GRADLE_DOWNLOAD_SHA256} *gradle.zip" | sha256sum --check -         && echo "Installing Gradle"     && unzip gradle.zip     && rm gradle.zip     && mv "gradle-${GRADLE_VERSION}" "${GRADLE_HOME}/"     && ln --symbolic "${GRADLE_HOME}/bin/gradle" /usr/bin/gradle         && echo "Testing Gradle installation"     && gradle --version
```

-	Layers:
	-	`sha256:77ba7971d651af68e20e7cbb6603a3f7acd8ef2893066767a93db104723556f2`  
		Last Modified: Sat, 16 Oct 2021 00:38:38 GMT  
		Size: 33.3 MB (33287238 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7d71f328d69a3848141b8b31ebd2a2657d78fcb95dfdd3400c8ed3202aa0a24b`  
		Last Modified: Mon, 29 Nov 2021 20:27:29 GMT  
		Size: 31.1 MB (31132613 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:977f5b7339ae1bacc07ae3b1f72ad5481f428e62aac60c7dbbb47a45269c3c4e`  
		Last Modified: Mon, 29 Nov 2021 20:28:24 GMT  
		Size: 188.6 MB (188569216 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bfde010f261760bd3f21ceabcc01e64755b546d235e600542be123cd6c5954e8`  
		Last Modified: Mon, 29 Nov 2021 20:28:00 GMT  
		Size: 160.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:def4fe1e112b6d4a66180b60396cd8ab7228d09493338c34514df6ed523a3732`  
		Last Modified: Mon, 29 Nov 2021 21:42:37 GMT  
		Size: 4.4 KB (4360 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6892a4d708b9ebfbdb2cabaa484337dc6de18eef56c9ee7957e2971a5b2133f2`  
		Last Modified: Mon, 29 Nov 2021 21:42:52 GMT  
		Size: 64.6 MB (64583067 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7305e81274ae8533f181df251a3527cc857852f7c9a08ff1737c546da1507d6b`  
		Last Modified: Fri, 03 Dec 2021 17:45:48 GMT  
		Size: 115.8 MB (115782915 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `gradle:7-jdk` - linux; s390x

```console
$ docker pull gradle@sha256:51b3a448bc9b910194f770f25612c7f95c794c1638a2a6b3797bf8c364ce1038
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **407.4 MB (407374484 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:6a526b08f49e7ee5d5dd3c8f9d2cfbcc27f4d35a52de3807bc8dac24e7c7dd2a`
-	Default Command: `["gradle"]`

```dockerfile
# Sat, 16 Oct 2021 00:41:46 GMT
ADD file:cf3b6f9c395392eaf2c629969f59c48cde60ae1c74c3dbb13886481999a7a4d5 in / 
# Sat, 16 Oct 2021 00:41:48 GMT
CMD ["bash"]
# Sat, 16 Oct 2021 00:58:42 GMT
ENV LANG=en_US.UTF-8 LANGUAGE=en_US:en LC_ALL=en_US.UTF-8
# Mon, 29 Nov 2021 19:45:24 GMT
RUN apt-get update     && DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends tzdata curl ca-certificates fontconfig locales python-is-python3 binutils     && echo "en_US.UTF-8 UTF-8" >> /etc/locale.gen     && locale-gen en_US.UTF-8     && rm -rf /var/lib/apt/lists/*
# Mon, 29 Nov 2021 19:45:46 GMT
ENV JAVA_VERSION=jdk-17.0.1+12
# Mon, 29 Nov 2021 19:45:54 GMT
RUN set -eux;     ARCH="$(dpkg --print-architecture)";     case "${ARCH}" in        aarch64|arm64)          ESUM='f23d482b2b4ada08166201d1a0e299e3e371fdca5cd7288dcbd81ae82f3a75e3';          BINARY_URL='https://github.com/adoptium/temurin17-binaries/releases/download/jdk-17.0.1%2B12/OpenJDK17U-jdk_aarch64_linux_hotspot_17.0.1_12.tar.gz';          ;;        armhf|arm)          ESUM='f5945a39929384235e7cb1c57df071b8c7e49274632e2a54e54b2bad05de21a5';          BINARY_URL='https://github.com/adoptium/temurin17-binaries/releases/download/jdk-17.0.1%2B12/OpenJDK17U-jdk_arm_linux_hotspot_17.0.1_12.tar.gz';          ;;        ppc64el|powerpc:common64)          ESUM='bd65d4e8ecc4236924ae34d2075b956799abca594021e1b40c36aa08a0d610b0';          BINARY_URL='https://github.com/adoptium/temurin17-binaries/releases/download/jdk-17.0.1%2B12/OpenJDK17U-jdk_ppc64le_linux_hotspot_17.0.1_12.tar.gz';          ;;        s390x|s390:64-bit)          ESUM='dcc17e6ef28984656e997b6b8a6a31c89f45aff87a56b5d3819137c8f1050bef';          BINARY_URL='https://github.com/adoptium/temurin17-binaries/releases/download/jdk-17.0.1%2B12/OpenJDK17U-jdk_s390x_linux_hotspot_17.0.1_12.tar.gz';          ;;        amd64|i386:x86-64)          ESUM='6ea18c276dcbb8522feeebcfc3a4b5cb7c7e7368ba8590d3326c6c3efc5448b6';          BINARY_URL='https://github.com/adoptium/temurin17-binaries/releases/download/jdk-17.0.1%2B12/OpenJDK17U-jdk_x64_linux_hotspot_17.0.1_12.tar.gz';          ;;        *)          echo "Unsupported arch: ${ARCH}";          exit 1;          ;;     esac;     curl -LfsSo /tmp/openjdk.tar.gz ${BINARY_URL};     echo "${ESUM} */tmp/openjdk.tar.gz" | sha256sum -c -;     mkdir -p /opt/java/openjdk;     cd /opt/java/openjdk;     tar -xf /tmp/openjdk.tar.gz --strip-components=1;     rm -rf /tmp/openjdk.tar.gz;
# Mon, 29 Nov 2021 19:45:57 GMT
ENV JAVA_HOME=/opt/java/openjdk PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Mon, 29 Nov 2021 19:45:58 GMT
RUN echo Verifying install ...     && echo javac --version && javac --version     && echo java --version && java --version     && echo Complete.
# Mon, 29 Nov 2021 19:45:58 GMT
CMD ["jshell"]
# Mon, 29 Nov 2021 20:40:04 GMT
CMD ["gradle"]
# Mon, 29 Nov 2021 20:40:04 GMT
ENV GRADLE_HOME=/opt/gradle
# Mon, 29 Nov 2021 20:40:05 GMT
RUN set -o errexit -o nounset     && echo "Adding gradle user and group"     && groupadd --system --gid 1000 gradle     && useradd --system --gid gradle --uid 1000 --shell /bin/bash --create-home gradle     && mkdir /home/gradle/.gradle     && chown --recursive gradle:gradle /home/gradle         && echo "Symlinking root Gradle cache to gradle Gradle cache"     && ln --symbolic /home/gradle/.gradle /root/.gradle
# Mon, 29 Nov 2021 20:40:05 GMT
VOLUME [/home/gradle/.gradle]
# Mon, 29 Nov 2021 20:40:05 GMT
WORKDIR /home/gradle
# Mon, 29 Nov 2021 20:40:21 GMT
RUN set -o errexit -o nounset     && apt-get update     && apt-get install --yes --no-install-recommends         unzip         wget                 bzr         git         git-lfs         mercurial         openssh-client         subversion     && rm --recursive --force /var/lib/apt/lists/*         && echo "Testing VCSes"     && which bzr     && which git     && which git-lfs     && which hg     && which svn
# Fri, 03 Dec 2021 01:20:24 GMT
ENV GRADLE_VERSION=7.3.1
# Fri, 03 Dec 2021 01:20:24 GMT
ARG GRADLE_DOWNLOAD_SHA256=9afb3ca688fc12c761a0e9e4321e4d24e977a4a8916c8a768b1fe05ddb4d6b66
# Fri, 03 Dec 2021 01:20:31 GMT
# ARGS: GRADLE_DOWNLOAD_SHA256=9afb3ca688fc12c761a0e9e4321e4d24e977a4a8916c8a768b1fe05ddb4d6b66
RUN set -o errexit -o nounset     && echo "Downloading Gradle"     && wget --no-verbose --output-document=gradle.zip "https://services.gradle.org/distributions/gradle-${GRADLE_VERSION}-bin.zip"         && echo "Checking download hash"     && echo "${GRADLE_DOWNLOAD_SHA256} *gradle.zip" | sha256sum --check -         && echo "Installing Gradle"     && unzip gradle.zip     && rm gradle.zip     && mv "gradle-${GRADLE_VERSION}" "${GRADLE_HOME}/"     && ln --symbolic "${GRADLE_HOME}/bin/gradle" /usr/bin/gradle         && echo "Testing Gradle installation"     && gradle --version
```

-	Layers:
	-	`sha256:1f0267805ccac7499fadaabf65e52d4564add2bc20ed25bcf77df24d8debb103`  
		Last Modified: Sat, 16 Oct 2021 00:42:57 GMT  
		Size: 27.1 MB (27120856 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:06dd1b67c19cd65073e039ddb0ad0478e4ebeff4ccfb02e00bde920aefe11b4b`  
		Last Modified: Mon, 29 Nov 2021 19:47:48 GMT  
		Size: 27.9 MB (27940770 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3564f1f4aa560c08eb901fe777d34220aed6913c442b7b14e94e2ed9bbf5e4d9`  
		Last Modified: Mon, 29 Nov 2021 19:48:18 GMT  
		Size: 180.4 MB (180365429 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e63e5594c887f1de34e7a6518cb7c4c336269ff428a1b4bed0409ca5fcffbb4c`  
		Last Modified: Mon, 29 Nov 2021 19:48:06 GMT  
		Size: 160.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5adfa879631a67ac19a8fd9f5fbb6ab6ad6f11cc628d599e266e5810dd22b176`  
		Last Modified: Mon, 29 Nov 2021 20:42:42 GMT  
		Size: 4.4 KB (4368 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:102264c876643a8ae46f980975faa2b401015ce1641705630c22d1d1a8bd38b0`  
		Last Modified: Mon, 29 Nov 2021 20:42:51 GMT  
		Size: 56.2 MB (56159994 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:36d5e2e45a7c4e6732bffbedd033c498b46e5730880632bb7c19d50d305fe9ad`  
		Last Modified: Fri, 03 Dec 2021 01:22:28 GMT  
		Size: 115.8 MB (115782907 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
