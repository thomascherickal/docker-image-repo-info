## `ibm-semeru-runtimes:open-8-jdk-focal`

```console
$ docker pull ibm-semeru-runtimes@sha256:19df907d29d760a2b35ffbffd9758ef80b3ca2a39ecda015c12f999d89395466
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 4
	-	linux; amd64
	-	linux; arm64 variant v8
	-	linux; ppc64le
	-	linux; s390x

### `ibm-semeru-runtimes:open-8-jdk-focal` - linux; amd64

```console
$ docker pull ibm-semeru-runtimes@sha256:8f61877fdfe2c95021d2b5536e3ba271d527edcc90abedf85b0fa5071fe247aa
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **165.7 MB (165710470 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:5f5c7f25448ff6c3811d37402eb90b0abee6c7bfe43e5e3f62c60451ed616d2a`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Tue, 28 Nov 2023 05:17:39 GMT
ARG RELEASE
# Tue, 28 Nov 2023 05:17:39 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Tue, 28 Nov 2023 05:17:39 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Tue, 28 Nov 2023 05:17:39 GMT
LABEL org.opencontainers.image.version=20.04
# Tue, 28 Nov 2023 05:17:41 GMT
ADD file:9169bb1d6ef21313aed17e924538fee03d858460ae6b05e01968457dfc043bd7 in / 
# Tue, 28 Nov 2023 05:17:41 GMT
CMD ["/bin/bash"]
# Sat, 02 Dec 2023 02:22:48 GMT
ENV LANG=en_US.UTF-8 LANGUAGE=en_US:en LC_ALL=en_US.UTF-8
# Sat, 02 Dec 2023 02:23:10 GMT
RUN apt-get update     && DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends tzdata curl ca-certificates fontconfig locales     && echo "en_US.UTF-8 UTF-8" >> /etc/locale.gen     && locale-gen en_US.UTF-8     && rm -rf /var/lib/apt/lists/*
# Sat, 02 Dec 2023 02:23:10 GMT
ENV JAVA_VERSION=jdk8u392-b08_openj9-0.41.0
# Sat, 02 Dec 2023 02:23:16 GMT
RUN set -eux;     ARCH="$(dpkg --print-architecture)";     case "${ARCH}" in        aarch64|arm64)          ESUM='a804e9ecec05eb4565482f8d1716c176819de8a7521945b0b0eb2aa863f63c41';          BINARY_URL='https://github.com/ibmruntimes/semeru8-binaries/releases/download/jdk8u392-b08_openj9-0.41.0/ibm-semeru-open-jdk_aarch64_linux_8u392b08_openj9-0.41.0.tar.gz';          ;;        ppc64el|ppc64le)          ESUM='4a2e57b49089f88f345ed0362efb85dd31a76e1ab97345a529e5c386e93691b4';          BINARY_URL='https://github.com/ibmruntimes/semeru8-binaries/releases/download/jdk8u392-b08_openj9-0.41.0/ibm-semeru-open-jdk_ppc64le_linux_8u392b08_openj9-0.41.0.tar.gz';          ;;        amd64|x86_64)          ESUM='3ea78d9e4f5dce48a83507b273d17d59055de7ccb9d008f51365082bc543dbe6';          BINARY_URL='https://github.com/ibmruntimes/semeru8-binaries/releases/download/jdk8u392-b08_openj9-0.41.0/ibm-semeru-open-jdk_x64_linux_8u392b08_openj9-0.41.0.tar.gz';          ;;        s390x)          ESUM='db0b6afe4c5d5cdaea872562fb802c56f08e90f7e7b5e9e6cad7bbf040badede';          BINARY_URL='https://github.com/ibmruntimes/semeru8-binaries/releases/download/jdk8u392-b08_openj9-0.41.0/ibm-semeru-open-jdk_s390x_linux_8u392b08_openj9-0.41.0.tar.gz';          ;;        *)          echo "Unsupported arch: ${ARCH}";          exit 1;          ;;     esac;     curl -LfsSo /tmp/openjdk.tar.gz ${BINARY_URL};     echo "${ESUM} */tmp/openjdk.tar.gz" | sha256sum -c -;     mkdir -p /opt/java/openjdk;     cd /opt/java/openjdk;     tar -xf /tmp/openjdk.tar.gz --strip-components=1;     rm -rf /tmp/openjdk.tar.gz;
# Sat, 02 Dec 2023 02:23:17 GMT
ENV JAVA_HOME=/opt/java/openjdk PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Sat, 02 Dec 2023 02:23:17 GMT
ENV JAVA_TOOL_OPTIONS=-XX:+IgnoreUnrecognizedVMOptions -XX:+PortableSharedCache -XX:+IdleTuningGcOnIdle -Xshareclasses:name=openj9_system_scc,cacheDir=/opt/java/.scc,readonly,nonFatal
# Sat, 02 Dec 2023 02:23:52 GMT
RUN set -eux;     unset OPENJ9_JAVA_OPTIONS;     SCC_SIZE="50m";     DOWNLOAD_PATH_TOMCAT=/tmp/tomcat;     INSTALL_PATH_TOMCAT=/opt/tomcat-home;     TOMCAT_CHECKSUM="0db27185d9fc3174f2c670f814df3dda8a008b89d1a38a5d96cbbe119767ebfb1cf0bce956b27954aee9be19c4a7b91f2579d967932207976322033a86075f98";     TOMCAT_DWNLD_URL="https://archive.apache.org/dist/tomcat/tomcat-9/v9.0.35/bin/apache-tomcat-9.0.35.tar.gz";         mkdir -p "${DOWNLOAD_PATH_TOMCAT}" "${INSTALL_PATH_TOMCAT}";     curl -LfsSo "${DOWNLOAD_PATH_TOMCAT}"/tomcat.tar.gz "${TOMCAT_DWNLD_URL}";     echo "${TOMCAT_CHECKSUM} *${DOWNLOAD_PATH_TOMCAT}/tomcat.tar.gz" | sha512sum -c -;     tar -xf "${DOWNLOAD_PATH_TOMCAT}"/tomcat.tar.gz -C "${INSTALL_PATH_TOMCAT}" --strip-components=1;     rm -rf "${DOWNLOAD_PATH_TOMCAT}";         java -Xshareclasses:name=dry_run_scc,cacheDir=/opt/java/.scc,bootClassesOnly,nonFatal,createLayer -Xscmx$SCC_SIZE -version;     export OPENJ9_JAVA_OPTIONS="-Xshareclasses:name=dry_run_scc,cacheDir=/opt/java/.scc,bootClassesOnly,nonFatal";     "${INSTALL_PATH_TOMCAT}"/bin/startup.sh;     sleep 5;     "${INSTALL_PATH_TOMCAT}"/bin/shutdown.sh -force;     sleep 15;     FULL=$( (java -Xshareclasses:name=dry_run_scc,cacheDir=/opt/java/.scc,printallStats 2>&1 || true) | awk '/^Cache is [0-9.]*% .*full/ {print substr($3, 1, length($3)-1)}');     DST_CACHE=$(java -Xshareclasses:name=dry_run_scc,cacheDir=/opt/java/.scc,destroy 2>&1 || true);     SCC_SIZE=$(echo $SCC_SIZE | sed 's/.$//');     SCC_SIZE=$(awk "BEGIN {print int($SCC_SIZE * $FULL / 100.0)}");     [ "${SCC_SIZE}" -eq 0 ] && SCC_SIZE=1;     SCC_SIZE="${SCC_SIZE}m";     java -Xshareclasses:name=openj9_system_scc,cacheDir=/opt/java/.scc,bootClassesOnly,nonFatal,createLayer -Xscmx$SCC_SIZE -version;     unset OPENJ9_JAVA_OPTIONS;         export OPENJ9_JAVA_OPTIONS="-Xshareclasses:name=openj9_system_scc,cacheDir=/opt/java/.scc,bootClassesOnly,nonFatal";     "${INSTALL_PATH_TOMCAT}"/bin/startup.sh;     sleep 5;     "${INSTALL_PATH_TOMCAT}"/bin/shutdown.sh -force;     sleep 5;     FULL=$( (java -Xshareclasses:name=openj9_system_scc,cacheDir=/opt/java/.scc,printallStats 2>&1 || true) | awk '/^Cache is [0-9.]*% .*full/ {print substr($3, 1, length($3)-1)}');     echo "SCC layer is $FULL% full.";     rm -rf "${INSTALL_PATH_TOMCAT}";     if [ -d "/opt/java/.scc" ]; then           chmod -R 0777 /opt/java/.scc;     fi;         echo "SCC generation phase completed";
```

-	Layers:
	-	`sha256:30ecab32a3b65c6ec04c63a65b90e627b49d1297d8793896ed50b656377d8a06`  
		Last Modified: Tue, 28 Nov 2023 10:11:56 GMT  
		Size: 28.6 MB (28584029 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f109746680b20397ed4ef68a3988028ee9fc824b184f43e7a4aca170d9ee5874`  
		Last Modified: Sat, 02 Dec 2023 02:37:30 GMT  
		Size: 16.1 MB (16058015 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:812cbce909fa875cd2d65bd34908e47e4f52fe12518980316ef234021b259f7d`  
		Last Modified: Sat, 02 Dec 2023 02:37:37 GMT  
		Size: 116.8 MB (116844615 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d190941ec2b62369585c9ebba72a12e16a81cedf555f5aeff3340f5335ed448f`  
		Last Modified: Sat, 02 Dec 2023 02:37:28 GMT  
		Size: 4.2 MB (4223811 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ibm-semeru-runtimes:open-8-jdk-focal` - linux; arm64 variant v8

```console
$ docker pull ibm-semeru-runtimes@sha256:23372a30d0e946e7246bd29a0c4ffa35b6e70b59ca49def9c27bb518246d0680
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **162.9 MB (162906826 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f26f70aec6219132005da96bdf03175c4d06f302cca4b92cfb4fb5da6f711e63`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Tue, 28 Nov 2023 05:25:16 GMT
ARG RELEASE
# Tue, 28 Nov 2023 05:25:16 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Tue, 28 Nov 2023 05:25:16 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Tue, 28 Nov 2023 05:25:16 GMT
LABEL org.opencontainers.image.version=20.04
# Tue, 28 Nov 2023 05:25:23 GMT
ADD file:f80c582e6edb1f05fc0cefc201be3c47d4b4c6ceb20889c434c9fdef0291cbbf in / 
# Tue, 28 Nov 2023 05:25:23 GMT
CMD ["/bin/bash"]
# Sat, 02 Dec 2023 07:19:22 GMT
ENV LANG=en_US.UTF-8 LANGUAGE=en_US:en LC_ALL=en_US.UTF-8
# Sat, 02 Dec 2023 07:20:14 GMT
RUN apt-get update     && DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends tzdata curl ca-certificates fontconfig locales     && echo "en_US.UTF-8 UTF-8" >> /etc/locale.gen     && locale-gen en_US.UTF-8     && rm -rf /var/lib/apt/lists/*
# Sat, 02 Dec 2023 07:20:15 GMT
ENV JAVA_VERSION=jdk8u392-b08_openj9-0.41.0
# Sat, 02 Dec 2023 07:20:20 GMT
RUN set -eux;     ARCH="$(dpkg --print-architecture)";     case "${ARCH}" in        aarch64|arm64)          ESUM='a804e9ecec05eb4565482f8d1716c176819de8a7521945b0b0eb2aa863f63c41';          BINARY_URL='https://github.com/ibmruntimes/semeru8-binaries/releases/download/jdk8u392-b08_openj9-0.41.0/ibm-semeru-open-jdk_aarch64_linux_8u392b08_openj9-0.41.0.tar.gz';          ;;        ppc64el|ppc64le)          ESUM='4a2e57b49089f88f345ed0362efb85dd31a76e1ab97345a529e5c386e93691b4';          BINARY_URL='https://github.com/ibmruntimes/semeru8-binaries/releases/download/jdk8u392-b08_openj9-0.41.0/ibm-semeru-open-jdk_ppc64le_linux_8u392b08_openj9-0.41.0.tar.gz';          ;;        amd64|x86_64)          ESUM='3ea78d9e4f5dce48a83507b273d17d59055de7ccb9d008f51365082bc543dbe6';          BINARY_URL='https://github.com/ibmruntimes/semeru8-binaries/releases/download/jdk8u392-b08_openj9-0.41.0/ibm-semeru-open-jdk_x64_linux_8u392b08_openj9-0.41.0.tar.gz';          ;;        s390x)          ESUM='db0b6afe4c5d5cdaea872562fb802c56f08e90f7e7b5e9e6cad7bbf040badede';          BINARY_URL='https://github.com/ibmruntimes/semeru8-binaries/releases/download/jdk8u392-b08_openj9-0.41.0/ibm-semeru-open-jdk_s390x_linux_8u392b08_openj9-0.41.0.tar.gz';          ;;        *)          echo "Unsupported arch: ${ARCH}";          exit 1;          ;;     esac;     curl -LfsSo /tmp/openjdk.tar.gz ${BINARY_URL};     echo "${ESUM} */tmp/openjdk.tar.gz" | sha256sum -c -;     mkdir -p /opt/java/openjdk;     cd /opt/java/openjdk;     tar -xf /tmp/openjdk.tar.gz --strip-components=1;     rm -rf /tmp/openjdk.tar.gz;
# Sat, 02 Dec 2023 07:20:21 GMT
ENV JAVA_HOME=/opt/java/openjdk PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Sat, 02 Dec 2023 07:20:21 GMT
ENV JAVA_TOOL_OPTIONS=-XX:+IgnoreUnrecognizedVMOptions -XX:+PortableSharedCache -XX:+IdleTuningGcOnIdle -Xshareclasses:name=openj9_system_scc,cacheDir=/opt/java/.scc,readonly,nonFatal
# Sat, 02 Dec 2023 07:20:56 GMT
RUN set -eux;     unset OPENJ9_JAVA_OPTIONS;     SCC_SIZE="50m";     DOWNLOAD_PATH_TOMCAT=/tmp/tomcat;     INSTALL_PATH_TOMCAT=/opt/tomcat-home;     TOMCAT_CHECKSUM="0db27185d9fc3174f2c670f814df3dda8a008b89d1a38a5d96cbbe119767ebfb1cf0bce956b27954aee9be19c4a7b91f2579d967932207976322033a86075f98";     TOMCAT_DWNLD_URL="https://archive.apache.org/dist/tomcat/tomcat-9/v9.0.35/bin/apache-tomcat-9.0.35.tar.gz";         mkdir -p "${DOWNLOAD_PATH_TOMCAT}" "${INSTALL_PATH_TOMCAT}";     curl -LfsSo "${DOWNLOAD_PATH_TOMCAT}"/tomcat.tar.gz "${TOMCAT_DWNLD_URL}";     echo "${TOMCAT_CHECKSUM} *${DOWNLOAD_PATH_TOMCAT}/tomcat.tar.gz" | sha512sum -c -;     tar -xf "${DOWNLOAD_PATH_TOMCAT}"/tomcat.tar.gz -C "${INSTALL_PATH_TOMCAT}" --strip-components=1;     rm -rf "${DOWNLOAD_PATH_TOMCAT}";         java -Xshareclasses:name=dry_run_scc,cacheDir=/opt/java/.scc,bootClassesOnly,nonFatal,createLayer -Xscmx$SCC_SIZE -version;     export OPENJ9_JAVA_OPTIONS="-Xshareclasses:name=dry_run_scc,cacheDir=/opt/java/.scc,bootClassesOnly,nonFatal";     "${INSTALL_PATH_TOMCAT}"/bin/startup.sh;     sleep 5;     "${INSTALL_PATH_TOMCAT}"/bin/shutdown.sh -force;     sleep 15;     FULL=$( (java -Xshareclasses:name=dry_run_scc,cacheDir=/opt/java/.scc,printallStats 2>&1 || true) | awk '/^Cache is [0-9.]*% .*full/ {print substr($3, 1, length($3)-1)}');     DST_CACHE=$(java -Xshareclasses:name=dry_run_scc,cacheDir=/opt/java/.scc,destroy 2>&1 || true);     SCC_SIZE=$(echo $SCC_SIZE | sed 's/.$//');     SCC_SIZE=$(awk "BEGIN {print int($SCC_SIZE * $FULL / 100.0)}");     [ "${SCC_SIZE}" -eq 0 ] && SCC_SIZE=1;     SCC_SIZE="${SCC_SIZE}m";     java -Xshareclasses:name=openj9_system_scc,cacheDir=/opt/java/.scc,bootClassesOnly,nonFatal,createLayer -Xscmx$SCC_SIZE -version;     unset OPENJ9_JAVA_OPTIONS;         export OPENJ9_JAVA_OPTIONS="-Xshareclasses:name=openj9_system_scc,cacheDir=/opt/java/.scc,bootClassesOnly,nonFatal";     "${INSTALL_PATH_TOMCAT}"/bin/startup.sh;     sleep 5;     "${INSTALL_PATH_TOMCAT}"/bin/shutdown.sh -force;     sleep 5;     FULL=$( (java -Xshareclasses:name=openj9_system_scc,cacheDir=/opt/java/.scc,printallStats 2>&1 || true) | awk '/^Cache is [0-9.]*% .*full/ {print substr($3, 1, length($3)-1)}');     echo "SCC layer is $FULL% full.";     rm -rf "${INSTALL_PATH_TOMCAT}";     if [ -d "/opt/java/.scc" ]; then           chmod -R 0777 /opt/java/.scc;     fi;         echo "SCC generation phase completed";
```

-	Layers:
	-	`sha256:5d2acf9ee7cfde47b6ce997317767b8fa9bf8d93b8297016db9e093d06aa913d`  
		Last Modified: Wed, 29 Nov 2023 17:47:09 GMT  
		Size: 27.2 MB (27203865 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7f3c8605cdb414099746de21259d24e908c9e6c6587b3e6af1cc8212b94402ee`  
		Last Modified: Sat, 02 Dec 2023 07:33:45 GMT  
		Size: 15.9 MB (15925597 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9764ddd359413de6a5d2495cfc487488c3fce8d7eade7a486985420af5f8d72d`  
		Last Modified: Sat, 02 Dec 2023 07:33:50 GMT  
		Size: 115.7 MB (115705654 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:db617d06586b20217a4551cfc57fc408b2871e0b319e42c9839994208d90077f`  
		Last Modified: Sat, 02 Dec 2023 07:33:43 GMT  
		Size: 4.1 MB (4071710 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ibm-semeru-runtimes:open-8-jdk-focal` - linux; ppc64le

```console
$ docker pull ibm-semeru-runtimes@sha256:2013554fee8fb4e8fb3a3ecc33cfd26b09cc25a26f4b7ee35072b042e0a4da95
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **170.9 MB (170933160 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:291a0d612c4543a5fb2c6d23f0e1ecc76da3af59b8478523a3a1bf263df7ee05`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Tue, 28 Nov 2023 05:22:52 GMT
ARG RELEASE
# Tue, 28 Nov 2023 05:22:53 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Tue, 28 Nov 2023 05:22:53 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Tue, 28 Nov 2023 05:22:53 GMT
LABEL org.opencontainers.image.version=20.04
# Tue, 28 Nov 2023 05:22:55 GMT
ADD file:a576e9688b14486d4fbbb0e868434fe4c3cbd4d24ddeaca6f6242b7f3e5420dc in / 
# Tue, 28 Nov 2023 05:22:56 GMT
CMD ["/bin/bash"]
# Sat, 02 Dec 2023 05:41:15 GMT
ENV LANG=en_US.UTF-8 LANGUAGE=en_US:en LC_ALL=en_US.UTF-8
# Sat, 02 Dec 2023 05:42:18 GMT
RUN apt-get update     && DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends tzdata curl ca-certificates fontconfig locales     && echo "en_US.UTF-8 UTF-8" >> /etc/locale.gen     && locale-gen en_US.UTF-8     && rm -rf /var/lib/apt/lists/*
# Sat, 02 Dec 2023 05:42:22 GMT
ENV JAVA_VERSION=jdk8u392-b08_openj9-0.41.0
# Sat, 02 Dec 2023 05:42:32 GMT
RUN set -eux;     ARCH="$(dpkg --print-architecture)";     case "${ARCH}" in        aarch64|arm64)          ESUM='a804e9ecec05eb4565482f8d1716c176819de8a7521945b0b0eb2aa863f63c41';          BINARY_URL='https://github.com/ibmruntimes/semeru8-binaries/releases/download/jdk8u392-b08_openj9-0.41.0/ibm-semeru-open-jdk_aarch64_linux_8u392b08_openj9-0.41.0.tar.gz';          ;;        ppc64el|ppc64le)          ESUM='4a2e57b49089f88f345ed0362efb85dd31a76e1ab97345a529e5c386e93691b4';          BINARY_URL='https://github.com/ibmruntimes/semeru8-binaries/releases/download/jdk8u392-b08_openj9-0.41.0/ibm-semeru-open-jdk_ppc64le_linux_8u392b08_openj9-0.41.0.tar.gz';          ;;        amd64|x86_64)          ESUM='3ea78d9e4f5dce48a83507b273d17d59055de7ccb9d008f51365082bc543dbe6';          BINARY_URL='https://github.com/ibmruntimes/semeru8-binaries/releases/download/jdk8u392-b08_openj9-0.41.0/ibm-semeru-open-jdk_x64_linux_8u392b08_openj9-0.41.0.tar.gz';          ;;        s390x)          ESUM='db0b6afe4c5d5cdaea872562fb802c56f08e90f7e7b5e9e6cad7bbf040badede';          BINARY_URL='https://github.com/ibmruntimes/semeru8-binaries/releases/download/jdk8u392-b08_openj9-0.41.0/ibm-semeru-open-jdk_s390x_linux_8u392b08_openj9-0.41.0.tar.gz';          ;;        *)          echo "Unsupported arch: ${ARCH}";          exit 1;          ;;     esac;     curl -LfsSo /tmp/openjdk.tar.gz ${BINARY_URL};     echo "${ESUM} */tmp/openjdk.tar.gz" | sha256sum -c -;     mkdir -p /opt/java/openjdk;     cd /opt/java/openjdk;     tar -xf /tmp/openjdk.tar.gz --strip-components=1;     rm -rf /tmp/openjdk.tar.gz;
# Sat, 02 Dec 2023 05:42:34 GMT
ENV JAVA_HOME=/opt/java/openjdk PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Sat, 02 Dec 2023 05:42:35 GMT
ENV JAVA_TOOL_OPTIONS=-XX:+IgnoreUnrecognizedVMOptions -XX:+PortableSharedCache -XX:+IdleTuningGcOnIdle -Xshareclasses:name=openj9_system_scc,cacheDir=/opt/java/.scc,readonly,nonFatal
# Sat, 02 Dec 2023 05:43:11 GMT
RUN set -eux;     unset OPENJ9_JAVA_OPTIONS;     SCC_SIZE="50m";     DOWNLOAD_PATH_TOMCAT=/tmp/tomcat;     INSTALL_PATH_TOMCAT=/opt/tomcat-home;     TOMCAT_CHECKSUM="0db27185d9fc3174f2c670f814df3dda8a008b89d1a38a5d96cbbe119767ebfb1cf0bce956b27954aee9be19c4a7b91f2579d967932207976322033a86075f98";     TOMCAT_DWNLD_URL="https://archive.apache.org/dist/tomcat/tomcat-9/v9.0.35/bin/apache-tomcat-9.0.35.tar.gz";         mkdir -p "${DOWNLOAD_PATH_TOMCAT}" "${INSTALL_PATH_TOMCAT}";     curl -LfsSo "${DOWNLOAD_PATH_TOMCAT}"/tomcat.tar.gz "${TOMCAT_DWNLD_URL}";     echo "${TOMCAT_CHECKSUM} *${DOWNLOAD_PATH_TOMCAT}/tomcat.tar.gz" | sha512sum -c -;     tar -xf "${DOWNLOAD_PATH_TOMCAT}"/tomcat.tar.gz -C "${INSTALL_PATH_TOMCAT}" --strip-components=1;     rm -rf "${DOWNLOAD_PATH_TOMCAT}";         java -Xshareclasses:name=dry_run_scc,cacheDir=/opt/java/.scc,bootClassesOnly,nonFatal,createLayer -Xscmx$SCC_SIZE -version;     export OPENJ9_JAVA_OPTIONS="-Xshareclasses:name=dry_run_scc,cacheDir=/opt/java/.scc,bootClassesOnly,nonFatal";     "${INSTALL_PATH_TOMCAT}"/bin/startup.sh;     sleep 5;     "${INSTALL_PATH_TOMCAT}"/bin/shutdown.sh -force;     sleep 15;     FULL=$( (java -Xshareclasses:name=dry_run_scc,cacheDir=/opt/java/.scc,printallStats 2>&1 || true) | awk '/^Cache is [0-9.]*% .*full/ {print substr($3, 1, length($3)-1)}');     DST_CACHE=$(java -Xshareclasses:name=dry_run_scc,cacheDir=/opt/java/.scc,destroy 2>&1 || true);     SCC_SIZE=$(echo $SCC_SIZE | sed 's/.$//');     SCC_SIZE=$(awk "BEGIN {print int($SCC_SIZE * $FULL / 100.0)}");     [ "${SCC_SIZE}" -eq 0 ] && SCC_SIZE=1;     SCC_SIZE="${SCC_SIZE}m";     java -Xshareclasses:name=openj9_system_scc,cacheDir=/opt/java/.scc,bootClassesOnly,nonFatal,createLayer -Xscmx$SCC_SIZE -version;     unset OPENJ9_JAVA_OPTIONS;         export OPENJ9_JAVA_OPTIONS="-Xshareclasses:name=openj9_system_scc,cacheDir=/opt/java/.scc,bootClassesOnly,nonFatal";     "${INSTALL_PATH_TOMCAT}"/bin/startup.sh;     sleep 5;     "${INSTALL_PATH_TOMCAT}"/bin/shutdown.sh -force;     sleep 5;     FULL=$( (java -Xshareclasses:name=openj9_system_scc,cacheDir=/opt/java/.scc,printallStats 2>&1 || true) | awk '/^Cache is [0-9.]*% .*full/ {print substr($3, 1, length($3)-1)}');     echo "SCC layer is $FULL% full.";     rm -rf "${INSTALL_PATH_TOMCAT}";     if [ -d "/opt/java/.scc" ]; then           chmod -R 0777 /opt/java/.scc;     fi;         echo "SCC generation phase completed";
```

-	Layers:
	-	`sha256:94be7103524649944e1375e5e1f8d6bd17dfa2bb7ecf5aa6fbe80eee27f0c30e`  
		Last Modified: Sat, 02 Dec 2023 04:48:00 GMT  
		Size: 33.3 MB (33313750 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5b559299d9ce9693a4c8513d94551a6ea63779536f7abe29c13d9959ccba62ea`  
		Last Modified: Sat, 02 Dec 2023 05:58:54 GMT  
		Size: 17.2 MB (17232945 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e37b96a2ce1dc66f0bb88cce13d87431e05c7df1f4d823d1a2084ae25b47526f`  
		Last Modified: Sat, 02 Dec 2023 05:59:01 GMT  
		Size: 116.9 MB (116919033 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d216ccd7e521b0a9740f4d3ebe0d1a16a6b113a8fcc3151fc14f699ed9bd74c8`  
		Last Modified: Sat, 02 Dec 2023 05:58:52 GMT  
		Size: 3.5 MB (3467432 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ibm-semeru-runtimes:open-8-jdk-focal` - linux; s390x

```console
$ docker pull ibm-semeru-runtimes@sha256:a71e9519a307b17f0bb4cc6ca40122c48165e508e1674189dfddd73b6b8f31d1
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **163.2 MB (163238859 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a54e379a850252ee1e63aa7d6edb8c7ca1c29ebd1926288d9ac142bd5949d7e7`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Wed, 13 Dec 2023 10:31:17 GMT
ARG RELEASE
# Wed, 13 Dec 2023 10:31:17 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Wed, 13 Dec 2023 10:31:17 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Wed, 13 Dec 2023 10:31:17 GMT
LABEL org.opencontainers.image.version=20.04
# Wed, 13 Dec 2023 10:31:19 GMT
ADD file:acb39119899edf16a81c2953b282eebb13d32feac981d3f40b60bdfc13ad7bb5 in / 
# Wed, 13 Dec 2023 10:31:20 GMT
CMD ["/bin/bash"]
# Sat, 16 Dec 2023 07:55:25 GMT
ENV LANG=en_US.UTF-8 LANGUAGE=en_US:en LC_ALL=en_US.UTF-8
# Sat, 16 Dec 2023 07:55:38 GMT
RUN apt-get update     && DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends tzdata curl ca-certificates fontconfig locales     && echo "en_US.UTF-8 UTF-8" >> /etc/locale.gen     && locale-gen en_US.UTF-8     && rm -rf /var/lib/apt/lists/*
# Sat, 16 Dec 2023 07:55:40 GMT
ENV JAVA_VERSION=jdk8u392-b08_openj9-0.41.0
# Sat, 16 Dec 2023 07:55:49 GMT
RUN set -eux;     ARCH="$(dpkg --print-architecture)";     case "${ARCH}" in        aarch64|arm64)          ESUM='a804e9ecec05eb4565482f8d1716c176819de8a7521945b0b0eb2aa863f63c41';          BINARY_URL='https://github.com/ibmruntimes/semeru8-binaries/releases/download/jdk8u392-b08_openj9-0.41.0/ibm-semeru-open-jdk_aarch64_linux_8u392b08_openj9-0.41.0.tar.gz';          ;;        ppc64el|ppc64le)          ESUM='4a2e57b49089f88f345ed0362efb85dd31a76e1ab97345a529e5c386e93691b4';          BINARY_URL='https://github.com/ibmruntimes/semeru8-binaries/releases/download/jdk8u392-b08_openj9-0.41.0/ibm-semeru-open-jdk_ppc64le_linux_8u392b08_openj9-0.41.0.tar.gz';          ;;        amd64|x86_64)          ESUM='3ea78d9e4f5dce48a83507b273d17d59055de7ccb9d008f51365082bc543dbe6';          BINARY_URL='https://github.com/ibmruntimes/semeru8-binaries/releases/download/jdk8u392-b08_openj9-0.41.0/ibm-semeru-open-jdk_x64_linux_8u392b08_openj9-0.41.0.tar.gz';          ;;        s390x)          ESUM='db0b6afe4c5d5cdaea872562fb802c56f08e90f7e7b5e9e6cad7bbf040badede';          BINARY_URL='https://github.com/ibmruntimes/semeru8-binaries/releases/download/jdk8u392-b08_openj9-0.41.0/ibm-semeru-open-jdk_s390x_linux_8u392b08_openj9-0.41.0.tar.gz';          ;;        *)          echo "Unsupported arch: ${ARCH}";          exit 1;          ;;     esac;     curl -LfsSo /tmp/openjdk.tar.gz ${BINARY_URL};     echo "${ESUM} */tmp/openjdk.tar.gz" | sha256sum -c -;     mkdir -p /opt/java/openjdk;     cd /opt/java/openjdk;     tar -xf /tmp/openjdk.tar.gz --strip-components=1;     rm -rf /tmp/openjdk.tar.gz;
# Sat, 16 Dec 2023 07:55:54 GMT
ENV JAVA_HOME=/opt/java/openjdk PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Sat, 16 Dec 2023 07:55:54 GMT
ENV JAVA_TOOL_OPTIONS=-XX:+IgnoreUnrecognizedVMOptions -XX:+PortableSharedCache -XX:+IdleTuningGcOnIdle -Xshareclasses:name=openj9_system_scc,cacheDir=/opt/java/.scc,readonly,nonFatal
# Sat, 16 Dec 2023 07:56:27 GMT
RUN set -eux;     unset OPENJ9_JAVA_OPTIONS;     SCC_SIZE="50m";     DOWNLOAD_PATH_TOMCAT=/tmp/tomcat;     INSTALL_PATH_TOMCAT=/opt/tomcat-home;     TOMCAT_CHECKSUM="0db27185d9fc3174f2c670f814df3dda8a008b89d1a38a5d96cbbe119767ebfb1cf0bce956b27954aee9be19c4a7b91f2579d967932207976322033a86075f98";     TOMCAT_DWNLD_URL="https://archive.apache.org/dist/tomcat/tomcat-9/v9.0.35/bin/apache-tomcat-9.0.35.tar.gz";         mkdir -p "${DOWNLOAD_PATH_TOMCAT}" "${INSTALL_PATH_TOMCAT}";     curl -LfsSo "${DOWNLOAD_PATH_TOMCAT}"/tomcat.tar.gz "${TOMCAT_DWNLD_URL}";     echo "${TOMCAT_CHECKSUM} *${DOWNLOAD_PATH_TOMCAT}/tomcat.tar.gz" | sha512sum -c -;     tar -xf "${DOWNLOAD_PATH_TOMCAT}"/tomcat.tar.gz -C "${INSTALL_PATH_TOMCAT}" --strip-components=1;     rm -rf "${DOWNLOAD_PATH_TOMCAT}";         java -Xshareclasses:name=dry_run_scc,cacheDir=/opt/java/.scc,bootClassesOnly,nonFatal,createLayer -Xscmx$SCC_SIZE -version;     export OPENJ9_JAVA_OPTIONS="-Xshareclasses:name=dry_run_scc,cacheDir=/opt/java/.scc,bootClassesOnly,nonFatal";     "${INSTALL_PATH_TOMCAT}"/bin/startup.sh;     sleep 5;     "${INSTALL_PATH_TOMCAT}"/bin/shutdown.sh -force;     sleep 15;     FULL=$( (java -Xshareclasses:name=dry_run_scc,cacheDir=/opt/java/.scc,printallStats 2>&1 || true) | awk '/^Cache is [0-9.]*% .*full/ {print substr($3, 1, length($3)-1)}');     DST_CACHE=$(java -Xshareclasses:name=dry_run_scc,cacheDir=/opt/java/.scc,destroy 2>&1 || true);     SCC_SIZE=$(echo $SCC_SIZE | sed 's/.$//');     SCC_SIZE=$(awk "BEGIN {print int($SCC_SIZE * $FULL / 100.0)}");     [ "${SCC_SIZE}" -eq 0 ] && SCC_SIZE=1;     SCC_SIZE="${SCC_SIZE}m";     java -Xshareclasses:name=openj9_system_scc,cacheDir=/opt/java/.scc,bootClassesOnly,nonFatal,createLayer -Xscmx$SCC_SIZE -version;     unset OPENJ9_JAVA_OPTIONS;         export OPENJ9_JAVA_OPTIONS="-Xshareclasses:name=openj9_system_scc,cacheDir=/opt/java/.scc,bootClassesOnly,nonFatal";     "${INSTALL_PATH_TOMCAT}"/bin/startup.sh;     sleep 5;     "${INSTALL_PATH_TOMCAT}"/bin/shutdown.sh -force;     sleep 5;     FULL=$( (java -Xshareclasses:name=openj9_system_scc,cacheDir=/opt/java/.scc,printallStats 2>&1 || true) | awk '/^Cache is [0-9.]*% .*full/ {print substr($3, 1, length($3)-1)}');     echo "SCC layer is $FULL% full.";     rm -rf "${INSTALL_PATH_TOMCAT}";     if [ -d "/opt/java/.scc" ]; then           chmod -R 0777 /opt/java/.scc;     fi;         echo "SCC generation phase completed";
```

-	Layers:
	-	`sha256:b17df547765b88177f27d934075b822d3ec46e7f985d1f46b83d63a5b1b34f48`  
		Last Modified: Sat, 16 Dec 2023 07:41:56 GMT  
		Size: 27.0 MB (27015634 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:df8140ee27d18b2b703f14d361460b999d78ace7bc9fdd8f6f45e2323fae2975`  
		Last Modified: Sat, 16 Dec 2023 08:13:26 GMT  
		Size: 15.8 MB (15754376 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b50ee6d24bb7a4473911e2819e01aa8696fa3b2cb18286d9a40bdc50babe0a82`  
		Last Modified: Sat, 16 Dec 2023 08:13:32 GMT  
		Size: 116.1 MB (116119060 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9c1a9865e8e8b327fe2a61df25ae5fb49985813533388ba061e810f4d6cfa286`  
		Last Modified: Sat, 16 Dec 2023 08:13:24 GMT  
		Size: 4.3 MB (4349789 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
