## `ibm-semeru-runtimes:open-18-jdk-focal`

```console
$ docker pull ibm-semeru-runtimes@sha256:a3209131ab473bd8a249ee4ae26bf1020485594724712b4d3ed3bbbdbb6e9674
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 4
	-	linux; amd64
	-	linux; arm64 variant v8
	-	linux; ppc64le
	-	linux; s390x

### `ibm-semeru-runtimes:open-18-jdk-focal` - linux; amd64

```console
$ docker pull ibm-semeru-runtimes@sha256:d512e0c218a4e5022637327066db7fbe2d913d1aa1aece8eed436f4627369cbc
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **264.1 MB (264134412 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:827f436c74dda8ccba9ff33589121cb4afe21ac3cd549571f76f4258ec543bcc`
-	Default Command: `["jshell"]`

```dockerfile
# Fri, 29 Apr 2022 23:20:59 GMT
ADD file:7009ad0ee0bbe5ed7f381792e07347e260e6896aeee0d80597808065120fa96b in / 
# Fri, 29 Apr 2022 23:20:59 GMT
CMD ["bash"]
# Sat, 30 Apr 2022 00:22:32 GMT
ENV LANG=en_US.UTF-8 LANGUAGE=en_US:en LC_ALL=en_US.UTF-8
# Sat, 30 Apr 2022 00:24:13 GMT
RUN apt-get update     && DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends tzdata curl ca-certificates fontconfig locales binutils     && echo "en_US.UTF-8 UTF-8" >> /etc/locale.gen     && locale-gen en_US.UTF-8     && rm -rf /var/lib/apt/lists/*
# Sat, 30 Apr 2022 00:59:21 GMT
ENV JAVA_VERSION=jdk-18.0.1+10_openj9-0.32.0
# Sat, 30 Apr 2022 00:59:34 GMT
RUN set -eux;     ARCH="$(dpkg --print-architecture)";     case "${ARCH}" in        aarch64|arm64)          ESUM='fdbad7dbbdaf1b0b8c2e9eb483ab025ece0ea7222966b8ebc9bbd6c074189b88';          BINARY_URL='https://github.com/ibmruntimes/semeru18-binaries/releases/download/jdk-18.0.1%2B10_openj9-0.32.0/ibm-semeru-open-jdk_aarch64_linux_18.0.1_10_openj9-0.32.0.tar.gz';          ;;        ppc64el|ppc64le)          ESUM='d3195f1999026545ff783c0f0798e5ff06190e90eed2319459345d8f3de4fc95';          BINARY_URL='https://github.com/ibmruntimes/semeru18-binaries/releases/download/jdk-18.0.1%2B10_openj9-0.32.0/ibm-semeru-open-jdk_ppc64le_linux_18.0.1_10_openj9-0.32.0.tar.gz';          ;;        amd64|x86_64)          ESUM='6e146103169c4e3173c8ce32c549daa8a979c6389bfc3b0b9248f1ecaf37f5ea';          BINARY_URL='https://github.com/ibmruntimes/semeru18-binaries/releases/download/jdk-18.0.1%2B10_openj9-0.32.0/ibm-semeru-open-jdk_x64_linux_18.0.1_10_openj9-0.32.0.tar.gz';          ;;        s390x)          ESUM='2f730c5e8458b83c2372d35759ed87795986e65e4e50e61c6c1c6ca71180b437';          BINARY_URL='https://github.com/ibmruntimes/semeru18-binaries/releases/download/jdk-18.0.1%2B10_openj9-0.32.0/ibm-semeru-open-jdk_s390x_linux_18.0.1_10_openj9-0.32.0.tar.gz';          ;;        *)          echo "Unsupported arch: ${ARCH}";          exit 1;          ;;     esac;     curl -LfsSo /tmp/openjdk.tar.gz ${BINARY_URL};     echo "${ESUM} */tmp/openjdk.tar.gz" | sha256sum -c -;     mkdir -p /opt/java/openjdk;     cd /opt/java/openjdk;     tar -xf /tmp/openjdk.tar.gz --strip-components=1;     rm -rf /tmp/openjdk.tar.gz;
# Sat, 30 Apr 2022 00:59:35 GMT
ENV JAVA_HOME=/opt/java/openjdk PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Sat, 30 Apr 2022 00:59:35 GMT
ENV JAVA_TOOL_OPTIONS=-XX:+IgnoreUnrecognizedVMOptions -XX:+PortableSharedCache -XX:+IdleTuningGcOnIdle -Xshareclasses:name=openj9_system_scc,cacheDir=/opt/java/.scc,readonly,nonFatal
# Sat, 30 Apr 2022 01:00:10 GMT
RUN set -eux;     unset OPENJ9_JAVA_OPTIONS;     SCC_SIZE="50m";     DOWNLOAD_PATH_TOMCAT=/tmp/tomcat;     INSTALL_PATH_TOMCAT=/opt/tomcat-home;     TOMCAT_CHECKSUM="0db27185d9fc3174f2c670f814df3dda8a008b89d1a38a5d96cbbe119767ebfb1cf0bce956b27954aee9be19c4a7b91f2579d967932207976322033a86075f98";     TOMCAT_DWNLD_URL="https://archive.apache.org/dist/tomcat/tomcat-9/v9.0.35/bin/apache-tomcat-9.0.35.tar.gz";         mkdir -p "${DOWNLOAD_PATH_TOMCAT}" "${INSTALL_PATH_TOMCAT}";     curl -LfsSo "${DOWNLOAD_PATH_TOMCAT}"/tomcat.tar.gz "${TOMCAT_DWNLD_URL}";     echo "${TOMCAT_CHECKSUM} *${DOWNLOAD_PATH_TOMCAT}/tomcat.tar.gz" | sha512sum -c -;     tar -xf "${DOWNLOAD_PATH_TOMCAT}"/tomcat.tar.gz -C "${INSTALL_PATH_TOMCAT}" --strip-components=1;     rm -rf "${DOWNLOAD_PATH_TOMCAT}";         java -Xshareclasses:name=dry_run_scc,cacheDir=/opt/java/.scc,bootClassesOnly,nonFatal,createLayer -Xscmx$SCC_SIZE -version;     export OPENJ9_JAVA_OPTIONS="-Xshareclasses:name=dry_run_scc,cacheDir=/opt/java/.scc,bootClassesOnly,nonFatal";     "${INSTALL_PATH_TOMCAT}"/bin/startup.sh;     sleep 5;     "${INSTALL_PATH_TOMCAT}"/bin/shutdown.sh -force;     sleep 15;     FULL=$( (java -Xshareclasses:name=dry_run_scc,cacheDir=/opt/java/.scc,printallStats 2>&1 || true) | awk '/^Cache is [0-9.]*% .*full/ {print substr($3, 1, length($3)-1)}');     DST_CACHE=$(java -Xshareclasses:name=dry_run_scc,cacheDir=/opt/java/.scc,destroy 2>&1 || true);     SCC_SIZE=$(echo $SCC_SIZE | sed 's/.$//');     SCC_SIZE=$(awk "BEGIN {print int($SCC_SIZE * $FULL / 100.0)}");     [ "${SCC_SIZE}" -eq 0 ] && SCC_SIZE=1;     SCC_SIZE="${SCC_SIZE}m";     java -Xshareclasses:name=openj9_system_scc,cacheDir=/opt/java/.scc,bootClassesOnly,nonFatal,createLayer -Xscmx$SCC_SIZE -version;     unset OPENJ9_JAVA_OPTIONS;         export OPENJ9_JAVA_OPTIONS="-Xshareclasses:name=openj9_system_scc,cacheDir=/opt/java/.scc,bootClassesOnly,nonFatal";     "${INSTALL_PATH_TOMCAT}"/bin/startup.sh;     sleep 5;     "${INSTALL_PATH_TOMCAT}"/bin/shutdown.sh -force;     sleep 5;     FULL=$( (java -Xshareclasses:name=openj9_system_scc,cacheDir=/opt/java/.scc,printallStats 2>&1 || true) | awk '/^Cache is [0-9.]*% .*full/ {print substr($3, 1, length($3)-1)}');     echo "SCC layer is $FULL% full.";     rm -rf "${INSTALL_PATH_TOMCAT}";     if [ -d "/opt/java/.scc" ]; then           chmod -R 0777 /opt/java/.scc;     fi;         echo "SCC generation phase completed";
# Sat, 30 Apr 2022 01:00:10 GMT
CMD ["jshell"]
```

-	Layers:
	-	`sha256:d5fd17ec1767521cf97f61568096bfc9a7cd9c2d149576a7b43930c5a97062b0`  
		Last Modified: Thu, 28 Apr 2022 03:03:21 GMT  
		Size: 28.6 MB (28566230 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b5dc755b592da4b1124b1e234ecb462608d017290110a0193b350cec9a521e55`  
		Last Modified: Sat, 30 Apr 2022 00:27:40 GMT  
		Size: 19.8 MB (19772006 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:50437f011650db9fcb9f9792c1cba19ed48b0b4155040dc10f741793bd4fc6f3`  
		Last Modified: Sat, 30 Apr 2022 01:05:05 GMT  
		Size: 209.9 MB (209906755 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4133d0e7726f549f5982cfb9296f3d4ff9aeeb156d6d0cfddaa4a00bdf59e6e5`  
		Last Modified: Sat, 30 Apr 2022 01:04:51 GMT  
		Size: 5.9 MB (5889421 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ibm-semeru-runtimes:open-18-jdk-focal` - linux; arm64 variant v8

```console
$ docker pull ibm-semeru-runtimes@sha256:06f57e6a91dff89b61b77c0d65fb433ca2c499886ddb0bdb9e7f4c02957848b4
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **258.3 MB (258345516 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:9963a0949ff4d060e630b08a712d30f2bc8b48b32765dd943de3d0d47b342a38`
-	Default Command: `["jshell"]`

```dockerfile
# Fri, 29 Apr 2022 22:49:34 GMT
ADD file:ccdde790bb849fe101367f2b541f1062b3544d21f99a5acc535bf2b0884cc0eb in / 
# Fri, 29 Apr 2022 22:49:35 GMT
CMD ["bash"]
# Fri, 29 Apr 2022 23:28:34 GMT
ENV LANG=en_US.UTF-8 LANGUAGE=en_US:en LC_ALL=en_US.UTF-8
# Fri, 29 Apr 2022 23:30:47 GMT
RUN apt-get update     && DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends tzdata curl ca-certificates fontconfig locales binutils     && echo "en_US.UTF-8 UTF-8" >> /etc/locale.gen     && locale-gen en_US.UTF-8     && rm -rf /var/lib/apt/lists/*
# Tue, 31 May 2022 23:52:31 GMT
ENV JAVA_VERSION=jdk-18.0.1.1+2_openj9-0.32.0
# Tue, 31 May 2022 23:52:46 GMT
RUN set -eux;     ARCH="$(dpkg --print-architecture)";     case "${ARCH}" in        aarch64|arm64)          ESUM='c1ef383b12460857dcc358284bda8fb1632d62b614a81d8b115903b53d294cc1';          BINARY_URL='https://github.com/ibmruntimes/semeru18-binaries/releases/download/jdk-18.0.1.1%2B2_openj9-0.32.0/ibm-semeru-open-jdk_aarch64_linux_18.0.1.1_2_openj9-0.32.0.tar.gz';          ;;        ppc64el|ppc64le)          ESUM='355e54e53f1b6578f4168a83de663707b65cd2f47645b4da914a815cccbf41b6';          BINARY_URL='https://github.com/ibmruntimes/semeru18-binaries/releases/download/jdk-18.0.1.1%2B2_openj9-0.32.0/ibm-semeru-open-jdk_ppc64le_linux_18.0.1.1_2_openj9-0.32.0.tar.gz';          ;;        amd64|x86_64)          ESUM='708d7d7b5ac3c793f7fa9b045024276b54f973dcb833cccc0be697261884db4a';          BINARY_URL='https://github.com/ibmruntimes/semeru18-binaries/releases/download/jdk-18.0.1.1%2B2_openj9-0.32.0/ibm-semeru-open-jdk_x64_linux_18.0.1.1_2_openj9-0.32.0.tar.gz';          ;;        s390x)          ESUM='5f5c90c86d007fed3923898a293babe82933f12085c6c59b828606f7e83e7864';          BINARY_URL='https://github.com/ibmruntimes/semeru18-binaries/releases/download/jdk-18.0.1.1%2B2_openj9-0.32.0/ibm-semeru-open-jdk_s390x_linux_18.0.1.1_2_openj9-0.32.0.tar.gz';          ;;        *)          echo "Unsupported arch: ${ARCH}";          exit 1;          ;;     esac;     curl -LfsSo /tmp/openjdk.tar.gz ${BINARY_URL};     echo "${ESUM} */tmp/openjdk.tar.gz" | sha256sum -c -;     mkdir -p /opt/java/openjdk;     cd /opt/java/openjdk;     tar -xf /tmp/openjdk.tar.gz --strip-components=1;     rm -rf /tmp/openjdk.tar.gz;
# Tue, 31 May 2022 23:52:46 GMT
ENV JAVA_HOME=/opt/java/openjdk PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 31 May 2022 23:52:47 GMT
ENV JAVA_TOOL_OPTIONS=-XX:+IgnoreUnrecognizedVMOptions -XX:+PortableSharedCache -XX:+IdleTuningGcOnIdle -Xshareclasses:name=openj9_system_scc,cacheDir=/opt/java/.scc,readonly,nonFatal
# Tue, 31 May 2022 23:53:23 GMT
RUN set -eux;     unset OPENJ9_JAVA_OPTIONS;     SCC_SIZE="50m";     DOWNLOAD_PATH_TOMCAT=/tmp/tomcat;     INSTALL_PATH_TOMCAT=/opt/tomcat-home;     TOMCAT_CHECKSUM="0db27185d9fc3174f2c670f814df3dda8a008b89d1a38a5d96cbbe119767ebfb1cf0bce956b27954aee9be19c4a7b91f2579d967932207976322033a86075f98";     TOMCAT_DWNLD_URL="https://archive.apache.org/dist/tomcat/tomcat-9/v9.0.35/bin/apache-tomcat-9.0.35.tar.gz";         mkdir -p "${DOWNLOAD_PATH_TOMCAT}" "${INSTALL_PATH_TOMCAT}";     curl -LfsSo "${DOWNLOAD_PATH_TOMCAT}"/tomcat.tar.gz "${TOMCAT_DWNLD_URL}";     echo "${TOMCAT_CHECKSUM} *${DOWNLOAD_PATH_TOMCAT}/tomcat.tar.gz" | sha512sum -c -;     tar -xf "${DOWNLOAD_PATH_TOMCAT}"/tomcat.tar.gz -C "${INSTALL_PATH_TOMCAT}" --strip-components=1;     rm -rf "${DOWNLOAD_PATH_TOMCAT}";         java -Xshareclasses:name=dry_run_scc,cacheDir=/opt/java/.scc,bootClassesOnly,nonFatal,createLayer -Xscmx$SCC_SIZE -version;     export OPENJ9_JAVA_OPTIONS="-Xshareclasses:name=dry_run_scc,cacheDir=/opt/java/.scc,bootClassesOnly,nonFatal";     "${INSTALL_PATH_TOMCAT}"/bin/startup.sh;     sleep 5;     "${INSTALL_PATH_TOMCAT}"/bin/shutdown.sh -force;     sleep 15;     FULL=$( (java -Xshareclasses:name=dry_run_scc,cacheDir=/opt/java/.scc,printallStats 2>&1 || true) | awk '/^Cache is [0-9.]*% .*full/ {print substr($3, 1, length($3)-1)}');     DST_CACHE=$(java -Xshareclasses:name=dry_run_scc,cacheDir=/opt/java/.scc,destroy 2>&1 || true);     SCC_SIZE=$(echo $SCC_SIZE | sed 's/.$//');     SCC_SIZE=$(awk "BEGIN {print int($SCC_SIZE * $FULL / 100.0)}");     [ "${SCC_SIZE}" -eq 0 ] && SCC_SIZE=1;     SCC_SIZE="${SCC_SIZE}m";     java -Xshareclasses:name=openj9_system_scc,cacheDir=/opt/java/.scc,bootClassesOnly,nonFatal,createLayer -Xscmx$SCC_SIZE -version;     unset OPENJ9_JAVA_OPTIONS;         export OPENJ9_JAVA_OPTIONS="-Xshareclasses:name=openj9_system_scc,cacheDir=/opt/java/.scc,bootClassesOnly,nonFatal";     "${INSTALL_PATH_TOMCAT}"/bin/startup.sh;     sleep 5;     "${INSTALL_PATH_TOMCAT}"/bin/shutdown.sh -force;     sleep 5;     FULL=$( (java -Xshareclasses:name=openj9_system_scc,cacheDir=/opt/java/.scc,printallStats 2>&1 || true) | awk '/^Cache is [0-9.]*% .*full/ {print substr($3, 1, length($3)-1)}');     echo "SCC layer is $FULL% full.";     rm -rf "${INSTALL_PATH_TOMCAT}";     if [ -d "/opt/java/.scc" ]; then           chmod -R 0777 /opt/java/.scc;     fi;         echo "SCC generation phase completed";
# Tue, 31 May 2022 23:53:23 GMT
CMD ["jshell"]
```

-	Layers:
	-	`sha256:d4ba87bb7858f0dd4a60003f011338f3a58b87d0add985652856007fe5ca5034`  
		Last Modified: Fri, 29 Apr 2022 22:51:32 GMT  
		Size: 27.2 MB (27169388 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:11b467f4b58f0fff42ab91803fe1a7c56675eed1a58f67991e9e7b0e445b91c1`  
		Last Modified: Fri, 29 Apr 2022 23:35:19 GMT  
		Size: 20.5 MB (20499354 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:93e653167e842de1adf52ae89cc97deca89d6aa1660c0cef01b0c11716aad6ca`  
		Last Modified: Tue, 31 May 2022 23:58:17 GMT  
		Size: 205.1 MB (205052007 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9384f60cab55dddd0d346ccce1c156cfb5067aadb1be0428de31e576a28e1988`  
		Last Modified: Tue, 31 May 2022 23:57:59 GMT  
		Size: 5.6 MB (5624767 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ibm-semeru-runtimes:open-18-jdk-focal` - linux; ppc64le

```console
$ docker pull ibm-semeru-runtimes@sha256:92b09e202a0ab710b1b2bdc6607edcfe827d5194e5dd244d4950fb33ab2d8e1a
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **270.4 MB (270366329 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:67e50941b61c4fae4b7f477ed01bd7b133ecbe463d300de32681adc159ac08ad`
-	Default Command: `["jshell"]`

```dockerfile
# Fri, 29 Apr 2022 23:22:28 GMT
ADD file:55691ac7d76af0fcfafc39ebd1e5a4f2d7018147d6db6f89812db33fbaffc2f9 in / 
# Fri, 29 Apr 2022 23:22:33 GMT
CMD ["bash"]
# Sat, 30 Apr 2022 00:29:48 GMT
ENV LANG=en_US.UTF-8 LANGUAGE=en_US:en LC_ALL=en_US.UTF-8
# Sat, 30 Apr 2022 00:39:06 GMT
RUN apt-get update     && DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends tzdata curl ca-certificates fontconfig locales binutils     && echo "en_US.UTF-8 UTF-8" >> /etc/locale.gen     && locale-gen en_US.UTF-8     && rm -rf /var/lib/apt/lists/*
# Sat, 30 Apr 2022 01:38:37 GMT
ENV JAVA_VERSION=jdk-18.0.1+10_openj9-0.32.0
# Sat, 30 Apr 2022 01:38:57 GMT
RUN set -eux;     ARCH="$(dpkg --print-architecture)";     case "${ARCH}" in        aarch64|arm64)          ESUM='fdbad7dbbdaf1b0b8c2e9eb483ab025ece0ea7222966b8ebc9bbd6c074189b88';          BINARY_URL='https://github.com/ibmruntimes/semeru18-binaries/releases/download/jdk-18.0.1%2B10_openj9-0.32.0/ibm-semeru-open-jdk_aarch64_linux_18.0.1_10_openj9-0.32.0.tar.gz';          ;;        ppc64el|ppc64le)          ESUM='d3195f1999026545ff783c0f0798e5ff06190e90eed2319459345d8f3de4fc95';          BINARY_URL='https://github.com/ibmruntimes/semeru18-binaries/releases/download/jdk-18.0.1%2B10_openj9-0.32.0/ibm-semeru-open-jdk_ppc64le_linux_18.0.1_10_openj9-0.32.0.tar.gz';          ;;        amd64|x86_64)          ESUM='6e146103169c4e3173c8ce32c549daa8a979c6389bfc3b0b9248f1ecaf37f5ea';          BINARY_URL='https://github.com/ibmruntimes/semeru18-binaries/releases/download/jdk-18.0.1%2B10_openj9-0.32.0/ibm-semeru-open-jdk_x64_linux_18.0.1_10_openj9-0.32.0.tar.gz';          ;;        s390x)          ESUM='2f730c5e8458b83c2372d35759ed87795986e65e4e50e61c6c1c6ca71180b437';          BINARY_URL='https://github.com/ibmruntimes/semeru18-binaries/releases/download/jdk-18.0.1%2B10_openj9-0.32.0/ibm-semeru-open-jdk_s390x_linux_18.0.1_10_openj9-0.32.0.tar.gz';          ;;        *)          echo "Unsupported arch: ${ARCH}";          exit 1;          ;;     esac;     curl -LfsSo /tmp/openjdk.tar.gz ${BINARY_URL};     echo "${ESUM} */tmp/openjdk.tar.gz" | sha256sum -c -;     mkdir -p /opt/java/openjdk;     cd /opt/java/openjdk;     tar -xf /tmp/openjdk.tar.gz --strip-components=1;     rm -rf /tmp/openjdk.tar.gz;
# Sat, 30 Apr 2022 01:39:01 GMT
ENV JAVA_HOME=/opt/java/openjdk PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Sat, 30 Apr 2022 01:39:04 GMT
ENV JAVA_TOOL_OPTIONS=-XX:+IgnoreUnrecognizedVMOptions -XX:+PortableSharedCache -XX:+IdleTuningGcOnIdle -Xshareclasses:name=openj9_system_scc,cacheDir=/opt/java/.scc,readonly,nonFatal
# Sat, 30 Apr 2022 01:39:46 GMT
RUN set -eux;     unset OPENJ9_JAVA_OPTIONS;     SCC_SIZE="50m";     DOWNLOAD_PATH_TOMCAT=/tmp/tomcat;     INSTALL_PATH_TOMCAT=/opt/tomcat-home;     TOMCAT_CHECKSUM="0db27185d9fc3174f2c670f814df3dda8a008b89d1a38a5d96cbbe119767ebfb1cf0bce956b27954aee9be19c4a7b91f2579d967932207976322033a86075f98";     TOMCAT_DWNLD_URL="https://archive.apache.org/dist/tomcat/tomcat-9/v9.0.35/bin/apache-tomcat-9.0.35.tar.gz";         mkdir -p "${DOWNLOAD_PATH_TOMCAT}" "${INSTALL_PATH_TOMCAT}";     curl -LfsSo "${DOWNLOAD_PATH_TOMCAT}"/tomcat.tar.gz "${TOMCAT_DWNLD_URL}";     echo "${TOMCAT_CHECKSUM} *${DOWNLOAD_PATH_TOMCAT}/tomcat.tar.gz" | sha512sum -c -;     tar -xf "${DOWNLOAD_PATH_TOMCAT}"/tomcat.tar.gz -C "${INSTALL_PATH_TOMCAT}" --strip-components=1;     rm -rf "${DOWNLOAD_PATH_TOMCAT}";         java -Xshareclasses:name=dry_run_scc,cacheDir=/opt/java/.scc,bootClassesOnly,nonFatal,createLayer -Xscmx$SCC_SIZE -version;     export OPENJ9_JAVA_OPTIONS="-Xshareclasses:name=dry_run_scc,cacheDir=/opt/java/.scc,bootClassesOnly,nonFatal";     "${INSTALL_PATH_TOMCAT}"/bin/startup.sh;     sleep 5;     "${INSTALL_PATH_TOMCAT}"/bin/shutdown.sh -force;     sleep 15;     FULL=$( (java -Xshareclasses:name=dry_run_scc,cacheDir=/opt/java/.scc,printallStats 2>&1 || true) | awk '/^Cache is [0-9.]*% .*full/ {print substr($3, 1, length($3)-1)}');     DST_CACHE=$(java -Xshareclasses:name=dry_run_scc,cacheDir=/opt/java/.scc,destroy 2>&1 || true);     SCC_SIZE=$(echo $SCC_SIZE | sed 's/.$//');     SCC_SIZE=$(awk "BEGIN {print int($SCC_SIZE * $FULL / 100.0)}");     [ "${SCC_SIZE}" -eq 0 ] && SCC_SIZE=1;     SCC_SIZE="${SCC_SIZE}m";     java -Xshareclasses:name=openj9_system_scc,cacheDir=/opt/java/.scc,bootClassesOnly,nonFatal,createLayer -Xscmx$SCC_SIZE -version;     unset OPENJ9_JAVA_OPTIONS;         export OPENJ9_JAVA_OPTIONS="-Xshareclasses:name=openj9_system_scc,cacheDir=/opt/java/.scc,bootClassesOnly,nonFatal";     "${INSTALL_PATH_TOMCAT}"/bin/startup.sh;     sleep 5;     "${INSTALL_PATH_TOMCAT}"/bin/shutdown.sh -force;     sleep 5;     FULL=$( (java -Xshareclasses:name=openj9_system_scc,cacheDir=/opt/java/.scc,printallStats 2>&1 || true) | awk '/^Cache is [0-9.]*% .*full/ {print substr($3, 1, length($3)-1)}');     echo "SCC layer is $FULL% full.";     rm -rf "${INSTALL_PATH_TOMCAT}";     if [ -d "/opt/java/.scc" ]; then           chmod -R 0777 /opt/java/.scc;     fi;         echo "SCC generation phase completed";
# Sat, 30 Apr 2022 01:39:48 GMT
CMD ["jshell"]
```

-	Layers:
	-	`sha256:e9c0a77cb9f0f7330e3fc62254e4c8ae89ed4bba21209fdc1088195250f950b9`  
		Last Modified: Fri, 29 Apr 2022 23:25:23 GMT  
		Size: 33.3 MB (33290661 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:78469566e7f98d05da9b7bb014ec6ce7170e52dbf51ed022fc29dbb9212a0e38`  
		Last Modified: Sat, 30 Apr 2022 00:47:36 GMT  
		Size: 21.7 MB (21692524 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7d00e6f91e19cd25c56e244df2510dcdd197abbf0f7d41844d030db393207abb`  
		Last Modified: Sat, 30 Apr 2022 01:48:04 GMT  
		Size: 210.6 MB (210574666 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1924affbdb66461fefd76dc9b8c8f443172e1986996f09a2bc9ddd4a3bd686b7`  
		Last Modified: Sat, 30 Apr 2022 01:47:40 GMT  
		Size: 4.8 MB (4808478 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ibm-semeru-runtimes:open-18-jdk-focal` - linux; s390x

```console
$ docker pull ibm-semeru-runtimes@sha256:8cfdc67db2e2d9e6961d7410e890c83fae8e9740d634fe903d066e5072681506
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **258.5 MB (258516173 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:3446618146768cc12e191a674dcb5a444ab0bfa68ac8f1368d75e6ec6a72acf3`
-	Default Command: `["jshell"]`

```dockerfile
# Fri, 29 Apr 2022 22:50:05 GMT
ADD file:fdc1835c7f7eae641bd78a4c938c3d94746b95a0c151498d332a2b9878fd99d8 in / 
# Fri, 29 Apr 2022 22:50:07 GMT
CMD ["bash"]
# Fri, 29 Apr 2022 23:22:36 GMT
ENV LANG=en_US.UTF-8 LANGUAGE=en_US:en LC_ALL=en_US.UTF-8
# Fri, 29 Apr 2022 23:23:40 GMT
RUN apt-get update     && DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends tzdata curl ca-certificates fontconfig locales binutils     && echo "en_US.UTF-8 UTF-8" >> /etc/locale.gen     && locale-gen en_US.UTF-8     && rm -rf /var/lib/apt/lists/*
# Tue, 31 May 2022 23:48:20 GMT
ENV JAVA_VERSION=jdk-18.0.1.1+2_openj9-0.32.0
# Tue, 31 May 2022 23:48:32 GMT
RUN set -eux;     ARCH="$(dpkg --print-architecture)";     case "${ARCH}" in        aarch64|arm64)          ESUM='c1ef383b12460857dcc358284bda8fb1632d62b614a81d8b115903b53d294cc1';          BINARY_URL='https://github.com/ibmruntimes/semeru18-binaries/releases/download/jdk-18.0.1.1%2B2_openj9-0.32.0/ibm-semeru-open-jdk_aarch64_linux_18.0.1.1_2_openj9-0.32.0.tar.gz';          ;;        ppc64el|ppc64le)          ESUM='355e54e53f1b6578f4168a83de663707b65cd2f47645b4da914a815cccbf41b6';          BINARY_URL='https://github.com/ibmruntimes/semeru18-binaries/releases/download/jdk-18.0.1.1%2B2_openj9-0.32.0/ibm-semeru-open-jdk_ppc64le_linux_18.0.1.1_2_openj9-0.32.0.tar.gz';          ;;        amd64|x86_64)          ESUM='708d7d7b5ac3c793f7fa9b045024276b54f973dcb833cccc0be697261884db4a';          BINARY_URL='https://github.com/ibmruntimes/semeru18-binaries/releases/download/jdk-18.0.1.1%2B2_openj9-0.32.0/ibm-semeru-open-jdk_x64_linux_18.0.1.1_2_openj9-0.32.0.tar.gz';          ;;        s390x)          ESUM='5f5c90c86d007fed3923898a293babe82933f12085c6c59b828606f7e83e7864';          BINARY_URL='https://github.com/ibmruntimes/semeru18-binaries/releases/download/jdk-18.0.1.1%2B2_openj9-0.32.0/ibm-semeru-open-jdk_s390x_linux_18.0.1.1_2_openj9-0.32.0.tar.gz';          ;;        *)          echo "Unsupported arch: ${ARCH}";          exit 1;          ;;     esac;     curl -LfsSo /tmp/openjdk.tar.gz ${BINARY_URL};     echo "${ESUM} */tmp/openjdk.tar.gz" | sha256sum -c -;     mkdir -p /opt/java/openjdk;     cd /opt/java/openjdk;     tar -xf /tmp/openjdk.tar.gz --strip-components=1;     rm -rf /tmp/openjdk.tar.gz;
# Tue, 31 May 2022 23:48:37 GMT
ENV JAVA_HOME=/opt/java/openjdk PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 31 May 2022 23:48:37 GMT
ENV JAVA_TOOL_OPTIONS=-XX:+IgnoreUnrecognizedVMOptions -XX:+PortableSharedCache -XX:+IdleTuningGcOnIdle -Xshareclasses:name=openj9_system_scc,cacheDir=/opt/java/.scc,readonly,nonFatal
# Tue, 31 May 2022 23:49:10 GMT
RUN set -eux;     unset OPENJ9_JAVA_OPTIONS;     SCC_SIZE="50m";     DOWNLOAD_PATH_TOMCAT=/tmp/tomcat;     INSTALL_PATH_TOMCAT=/opt/tomcat-home;     TOMCAT_CHECKSUM="0db27185d9fc3174f2c670f814df3dda8a008b89d1a38a5d96cbbe119767ebfb1cf0bce956b27954aee9be19c4a7b91f2579d967932207976322033a86075f98";     TOMCAT_DWNLD_URL="https://archive.apache.org/dist/tomcat/tomcat-9/v9.0.35/bin/apache-tomcat-9.0.35.tar.gz";         mkdir -p "${DOWNLOAD_PATH_TOMCAT}" "${INSTALL_PATH_TOMCAT}";     curl -LfsSo "${DOWNLOAD_PATH_TOMCAT}"/tomcat.tar.gz "${TOMCAT_DWNLD_URL}";     echo "${TOMCAT_CHECKSUM} *${DOWNLOAD_PATH_TOMCAT}/tomcat.tar.gz" | sha512sum -c -;     tar -xf "${DOWNLOAD_PATH_TOMCAT}"/tomcat.tar.gz -C "${INSTALL_PATH_TOMCAT}" --strip-components=1;     rm -rf "${DOWNLOAD_PATH_TOMCAT}";         java -Xshareclasses:name=dry_run_scc,cacheDir=/opt/java/.scc,bootClassesOnly,nonFatal,createLayer -Xscmx$SCC_SIZE -version;     export OPENJ9_JAVA_OPTIONS="-Xshareclasses:name=dry_run_scc,cacheDir=/opt/java/.scc,bootClassesOnly,nonFatal";     "${INSTALL_PATH_TOMCAT}"/bin/startup.sh;     sleep 5;     "${INSTALL_PATH_TOMCAT}"/bin/shutdown.sh -force;     sleep 15;     FULL=$( (java -Xshareclasses:name=dry_run_scc,cacheDir=/opt/java/.scc,printallStats 2>&1 || true) | awk '/^Cache is [0-9.]*% .*full/ {print substr($3, 1, length($3)-1)}');     DST_CACHE=$(java -Xshareclasses:name=dry_run_scc,cacheDir=/opt/java/.scc,destroy 2>&1 || true);     SCC_SIZE=$(echo $SCC_SIZE | sed 's/.$//');     SCC_SIZE=$(awk "BEGIN {print int($SCC_SIZE * $FULL / 100.0)}");     [ "${SCC_SIZE}" -eq 0 ] && SCC_SIZE=1;     SCC_SIZE="${SCC_SIZE}m";     java -Xshareclasses:name=openj9_system_scc,cacheDir=/opt/java/.scc,bootClassesOnly,nonFatal,createLayer -Xscmx$SCC_SIZE -version;     unset OPENJ9_JAVA_OPTIONS;         export OPENJ9_JAVA_OPTIONS="-Xshareclasses:name=openj9_system_scc,cacheDir=/opt/java/.scc,bootClassesOnly,nonFatal";     "${INSTALL_PATH_TOMCAT}"/bin/startup.sh;     sleep 5;     "${INSTALL_PATH_TOMCAT}"/bin/shutdown.sh -force;     sleep 5;     FULL=$( (java -Xshareclasses:name=openj9_system_scc,cacheDir=/opt/java/.scc,printallStats 2>&1 || true) | awk '/^Cache is [0-9.]*% .*full/ {print substr($3, 1, length($3)-1)}');     echo "SCC layer is $FULL% full.";     rm -rf "${INSTALL_PATH_TOMCAT}";     if [ -d "/opt/java/.scc" ]; then           chmod -R 0777 /opt/java/.scc;     fi;         echo "SCC generation phase completed";
# Tue, 31 May 2022 23:49:10 GMT
CMD ["jshell"]
```

-	Layers:
	-	`sha256:6e0f1090807e81093e3637ffe3d350f58816de907201055908c3506a30c68993`  
		Last Modified: Fri, 29 Apr 2022 22:52:01 GMT  
		Size: 27.1 MB (27065417 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8061a8e3bb73503261725cfaf9256d8c5dc9ee8d357d1e40a4d6578ad8263162`  
		Last Modified: Fri, 29 Apr 2022 23:25:57 GMT  
		Size: 19.2 MB (19235277 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:de08d560db4b23aa2803e85843ca679c2c324f29125229fa0ca6602993af68d2`  
		Last Modified: Tue, 31 May 2022 23:51:48 GMT  
		Size: 206.2 MB (206216746 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cd95c39a71b854cec98e716d7dfec6a7e0ceadf3fae0839fdb60ec43019f23f1`  
		Last Modified: Tue, 31 May 2022 23:51:36 GMT  
		Size: 6.0 MB (5998733 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
