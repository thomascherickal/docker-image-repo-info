## `ibm-semeru-runtimes:open-11-jdk`

```console
$ docker pull ibm-semeru-runtimes@sha256:4a876942b13b4534d7e2a521e7df12d3d7185f222fc834b3f1a3cd6a5192dc17
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 3
	-	linux; amd64
	-	linux; arm64 variant v8
	-	linux; s390x

### `ibm-semeru-runtimes:open-11-jdk` - linux; amd64

```console
$ docker pull ibm-semeru-runtimes@sha256:6cf625961463b777167f337d8d85ec94ce2976688d3a8e77611c52b460adcebb
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **252.1 MB (252052843 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:9851ad8d3fd6dd2534bca78c1f794919d0194d52c266dc302d40470c1a09cc07`
-	Default Command: `["jshell"]`

```dockerfile
# Thu, 01 Sep 2022 23:46:35 GMT
ADD file:a7268f82a86219801950401c224cabbdd83ef510a7c71396b25f70c2639ae4fa in / 
# Thu, 01 Sep 2022 23:46:35 GMT
CMD ["bash"]
# Fri, 02 Sep 2022 20:20:13 GMT
ENV LANG=en_US.UTF-8 LANGUAGE=en_US:en LC_ALL=en_US.UTF-8
# Fri, 02 Sep 2022 20:20:37 GMT
RUN apt-get update     && DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends tzdata curl ca-certificates fontconfig locales     && echo "en_US.UTF-8 UTF-8" >> /etc/locale.gen     && locale-gen en_US.UTF-8     && rm -rf /var/lib/apt/lists/*
# Fri, 02 Sep 2022 20:22:33 GMT
ENV JAVA_VERSION=jdk-11.0.16.1+1_openj9-0.33.1
# Fri, 02 Sep 2022 20:22:47 GMT
RUN set -eux;     ARCH="$(dpkg --print-architecture)";     case "${ARCH}" in        aarch64|arm64)          ESUM='fad70f5bd615d08d9b3e6222ce738be713050eedc8dce4b57bdccc85747d9ff6';          BINARY_URL='https://github.com/ibmruntimes/semeru11-binaries/releases/download/jdk-11.0.16.1%2B1_openj9-0.33.1/ibm-semeru-open-jdk_aarch64_linux_11.0.16.1_1_openj9-0.33.1.tar.gz';          ;;        amd64|x86_64)          ESUM='4eb9dc86bf92e144d7a2c8d6c2a6beac28c17b7348f2f0524e715548f52fd8f1';          BINARY_URL='https://github.com/ibmruntimes/semeru11-binaries/releases/download/jdk-11.0.16.1%2B1_openj9-0.33.1/ibm-semeru-open-jdk_x64_linux_11.0.16.1_1_openj9-0.33.1.tar.gz';          ;;        ppc64el|ppc64le)          ESUM='d71e5d26b7240d0e8a80499221ab79e5eed30ab1d985a5316bcfd240148435f8';          BINARY_URL='https://github.com/ibmruntimes/semeru11-binaries/releases/download/jdk-11.0.16.1%2B1_openj9-0.33.1/ibm-semeru-open-jdk_ppc64le_linux_11.0.16.1_1_openj9-0.33.1.tar.gz';          ;;        s390x)          ESUM='df4b746a0fc51bbab38aa86822a5f8e5587ed2b997cdd764de1c349d8caaa784';          BINARY_URL='https://github.com/ibmruntimes/semeru11-binaries/releases/download/jdk-11.0.16.1%2B1_openj9-0.33.1/ibm-semeru-open-jdk_s390x_linux_11.0.16.1_1_openj9-0.33.1.tar.gz';          ;;        *)          echo "Unsupported arch: ${ARCH}";          exit 1;          ;;     esac;     curl -LfsSo /tmp/openjdk.tar.gz ${BINARY_URL};     echo "${ESUM} */tmp/openjdk.tar.gz" | sha256sum -c -;     mkdir -p /opt/java/openjdk;     cd /opt/java/openjdk;     tar -xf /tmp/openjdk.tar.gz --strip-components=1;     rm -rf /tmp/openjdk.tar.gz;
# Fri, 02 Sep 2022 20:22:47 GMT
ENV JAVA_HOME=/opt/java/openjdk PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Fri, 02 Sep 2022 20:22:48 GMT
ENV JAVA_TOOL_OPTIONS=-XX:+IgnoreUnrecognizedVMOptions -XX:+PortableSharedCache -XX:+IdleTuningGcOnIdle -Xshareclasses:name=openj9_system_scc,cacheDir=/opt/java/.scc,readonly,nonFatal
# Fri, 02 Sep 2022 20:23:23 GMT
RUN set -eux;     unset OPENJ9_JAVA_OPTIONS;     SCC_SIZE="50m";     DOWNLOAD_PATH_TOMCAT=/tmp/tomcat;     INSTALL_PATH_TOMCAT=/opt/tomcat-home;     TOMCAT_CHECKSUM="0db27185d9fc3174f2c670f814df3dda8a008b89d1a38a5d96cbbe119767ebfb1cf0bce956b27954aee9be19c4a7b91f2579d967932207976322033a86075f98";     TOMCAT_DWNLD_URL="https://archive.apache.org/dist/tomcat/tomcat-9/v9.0.35/bin/apache-tomcat-9.0.35.tar.gz";         mkdir -p "${DOWNLOAD_PATH_TOMCAT}" "${INSTALL_PATH_TOMCAT}";     curl -LfsSo "${DOWNLOAD_PATH_TOMCAT}"/tomcat.tar.gz "${TOMCAT_DWNLD_URL}";     echo "${TOMCAT_CHECKSUM} *${DOWNLOAD_PATH_TOMCAT}/tomcat.tar.gz" | sha512sum -c -;     tar -xf "${DOWNLOAD_PATH_TOMCAT}"/tomcat.tar.gz -C "${INSTALL_PATH_TOMCAT}" --strip-components=1;     rm -rf "${DOWNLOAD_PATH_TOMCAT}";         java -Xshareclasses:name=dry_run_scc,cacheDir=/opt/java/.scc,bootClassesOnly,nonFatal,createLayer -Xscmx$SCC_SIZE -version;     export OPENJ9_JAVA_OPTIONS="-Xshareclasses:name=dry_run_scc,cacheDir=/opt/java/.scc,bootClassesOnly,nonFatal";     "${INSTALL_PATH_TOMCAT}"/bin/startup.sh;     sleep 5;     "${INSTALL_PATH_TOMCAT}"/bin/shutdown.sh -force;     sleep 15;     FULL=$( (java -Xshareclasses:name=dry_run_scc,cacheDir=/opt/java/.scc,printallStats 2>&1 || true) | awk '/^Cache is [0-9.]*% .*full/ {print substr($3, 1, length($3)-1)}');     DST_CACHE=$(java -Xshareclasses:name=dry_run_scc,cacheDir=/opt/java/.scc,destroy 2>&1 || true);     SCC_SIZE=$(echo $SCC_SIZE | sed 's/.$//');     SCC_SIZE=$(awk "BEGIN {print int($SCC_SIZE * $FULL / 100.0)}");     [ "${SCC_SIZE}" -eq 0 ] && SCC_SIZE=1;     SCC_SIZE="${SCC_SIZE}m";     java -Xshareclasses:name=openj9_system_scc,cacheDir=/opt/java/.scc,bootClassesOnly,nonFatal,createLayer -Xscmx$SCC_SIZE -version;     unset OPENJ9_JAVA_OPTIONS;         export OPENJ9_JAVA_OPTIONS="-Xshareclasses:name=openj9_system_scc,cacheDir=/opt/java/.scc,bootClassesOnly,nonFatal";     "${INSTALL_PATH_TOMCAT}"/bin/startup.sh;     sleep 5;     "${INSTALL_PATH_TOMCAT}"/bin/shutdown.sh -force;     sleep 5;     FULL=$( (java -Xshareclasses:name=openj9_system_scc,cacheDir=/opt/java/.scc,printallStats 2>&1 || true) | awk '/^Cache is [0-9.]*% .*full/ {print substr($3, 1, length($3)-1)}');     echo "SCC layer is $FULL% full.";     rm -rf "${INSTALL_PATH_TOMCAT}";     if [ -d "/opt/java/.scc" ]; then           chmod -R 0777 /opt/java/.scc;     fi;         echo "SCC generation phase completed";
# Fri, 02 Sep 2022 20:23:23 GMT
CMD ["jshell"]
```

-	Layers:
	-	`sha256:2b55860d4c667a7200a0cb279aec26777df61e5d3530388f223ce7859d566e7a`  
		Last Modified: Tue, 16 Aug 2022 03:03:54 GMT  
		Size: 30.4 MB (30426706 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:324c05aec43f4753ae908eaf3403a3eaca6da3965505d673a6bf17e884ef8e24`  
		Last Modified: Fri, 02 Sep 2022 20:29:26 GMT  
		Size: 12.1 MB (12103651 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b9e828ec725b21b400958b648131a70538f3d53ab0572099e58ad40486dc1aaa`  
		Last Modified: Fri, 02 Sep 2022 20:30:16 GMT  
		Size: 204.4 MB (204414197 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e789deef0ee3d2313ccb0d1bbf6d7cf17ac0adfc72b2790003c20aff5494212c`  
		Last Modified: Fri, 02 Sep 2022 20:30:02 GMT  
		Size: 5.1 MB (5108289 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ibm-semeru-runtimes:open-11-jdk` - linux; arm64 variant v8

```console
$ docker pull ibm-semeru-runtimes@sha256:0797bf58b5953573327e16863ae5eb8771e8f3747ae02920cefb1b844298b55b
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **245.4 MB (245377380 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:2fc81a41fe0efc0eaaf395ed2102001487d41592bbe53c21db2289780172bf01`
-	Default Command: `["jshell"]`

```dockerfile
# Fri, 02 Sep 2022 00:57:51 GMT
ADD file:550e7da19f5f7cef52c6ea160a33daa482f44df086ddecffca8ec9be6385b848 in / 
# Fri, 02 Sep 2022 00:57:52 GMT
CMD ["bash"]
# Fri, 02 Sep 2022 20:40:16 GMT
ENV LANG=en_US.UTF-8 LANGUAGE=en_US:en LC_ALL=en_US.UTF-8
# Fri, 02 Sep 2022 20:40:33 GMT
RUN apt-get update     && DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends tzdata curl ca-certificates fontconfig locales     && echo "en_US.UTF-8 UTF-8" >> /etc/locale.gen     && locale-gen en_US.UTF-8     && rm -rf /var/lib/apt/lists/*
# Fri, 02 Sep 2022 20:42:39 GMT
ENV JAVA_VERSION=jdk-11.0.16.1+1_openj9-0.33.1
# Fri, 02 Sep 2022 20:42:56 GMT
RUN set -eux;     ARCH="$(dpkg --print-architecture)";     case "${ARCH}" in        aarch64|arm64)          ESUM='fad70f5bd615d08d9b3e6222ce738be713050eedc8dce4b57bdccc85747d9ff6';          BINARY_URL='https://github.com/ibmruntimes/semeru11-binaries/releases/download/jdk-11.0.16.1%2B1_openj9-0.33.1/ibm-semeru-open-jdk_aarch64_linux_11.0.16.1_1_openj9-0.33.1.tar.gz';          ;;        amd64|x86_64)          ESUM='4eb9dc86bf92e144d7a2c8d6c2a6beac28c17b7348f2f0524e715548f52fd8f1';          BINARY_URL='https://github.com/ibmruntimes/semeru11-binaries/releases/download/jdk-11.0.16.1%2B1_openj9-0.33.1/ibm-semeru-open-jdk_x64_linux_11.0.16.1_1_openj9-0.33.1.tar.gz';          ;;        ppc64el|ppc64le)          ESUM='d71e5d26b7240d0e8a80499221ab79e5eed30ab1d985a5316bcfd240148435f8';          BINARY_URL='https://github.com/ibmruntimes/semeru11-binaries/releases/download/jdk-11.0.16.1%2B1_openj9-0.33.1/ibm-semeru-open-jdk_ppc64le_linux_11.0.16.1_1_openj9-0.33.1.tar.gz';          ;;        s390x)          ESUM='df4b746a0fc51bbab38aa86822a5f8e5587ed2b997cdd764de1c349d8caaa784';          BINARY_URL='https://github.com/ibmruntimes/semeru11-binaries/releases/download/jdk-11.0.16.1%2B1_openj9-0.33.1/ibm-semeru-open-jdk_s390x_linux_11.0.16.1_1_openj9-0.33.1.tar.gz';          ;;        *)          echo "Unsupported arch: ${ARCH}";          exit 1;          ;;     esac;     curl -LfsSo /tmp/openjdk.tar.gz ${BINARY_URL};     echo "${ESUM} */tmp/openjdk.tar.gz" | sha256sum -c -;     mkdir -p /opt/java/openjdk;     cd /opt/java/openjdk;     tar -xf /tmp/openjdk.tar.gz --strip-components=1;     rm -rf /tmp/openjdk.tar.gz;
# Fri, 02 Sep 2022 20:42:57 GMT
ENV JAVA_HOME=/opt/java/openjdk PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Fri, 02 Sep 2022 20:42:57 GMT
ENV JAVA_TOOL_OPTIONS=-XX:+IgnoreUnrecognizedVMOptions -XX:+PortableSharedCache -XX:+IdleTuningGcOnIdle -Xshareclasses:name=openj9_system_scc,cacheDir=/opt/java/.scc,readonly,nonFatal
# Fri, 02 Sep 2022 20:43:32 GMT
RUN set -eux;     unset OPENJ9_JAVA_OPTIONS;     SCC_SIZE="50m";     DOWNLOAD_PATH_TOMCAT=/tmp/tomcat;     INSTALL_PATH_TOMCAT=/opt/tomcat-home;     TOMCAT_CHECKSUM="0db27185d9fc3174f2c670f814df3dda8a008b89d1a38a5d96cbbe119767ebfb1cf0bce956b27954aee9be19c4a7b91f2579d967932207976322033a86075f98";     TOMCAT_DWNLD_URL="https://archive.apache.org/dist/tomcat/tomcat-9/v9.0.35/bin/apache-tomcat-9.0.35.tar.gz";         mkdir -p "${DOWNLOAD_PATH_TOMCAT}" "${INSTALL_PATH_TOMCAT}";     curl -LfsSo "${DOWNLOAD_PATH_TOMCAT}"/tomcat.tar.gz "${TOMCAT_DWNLD_URL}";     echo "${TOMCAT_CHECKSUM} *${DOWNLOAD_PATH_TOMCAT}/tomcat.tar.gz" | sha512sum -c -;     tar -xf "${DOWNLOAD_PATH_TOMCAT}"/tomcat.tar.gz -C "${INSTALL_PATH_TOMCAT}" --strip-components=1;     rm -rf "${DOWNLOAD_PATH_TOMCAT}";         java -Xshareclasses:name=dry_run_scc,cacheDir=/opt/java/.scc,bootClassesOnly,nonFatal,createLayer -Xscmx$SCC_SIZE -version;     export OPENJ9_JAVA_OPTIONS="-Xshareclasses:name=dry_run_scc,cacheDir=/opt/java/.scc,bootClassesOnly,nonFatal";     "${INSTALL_PATH_TOMCAT}"/bin/startup.sh;     sleep 5;     "${INSTALL_PATH_TOMCAT}"/bin/shutdown.sh -force;     sleep 15;     FULL=$( (java -Xshareclasses:name=dry_run_scc,cacheDir=/opt/java/.scc,printallStats 2>&1 || true) | awk '/^Cache is [0-9.]*% .*full/ {print substr($3, 1, length($3)-1)}');     DST_CACHE=$(java -Xshareclasses:name=dry_run_scc,cacheDir=/opt/java/.scc,destroy 2>&1 || true);     SCC_SIZE=$(echo $SCC_SIZE | sed 's/.$//');     SCC_SIZE=$(awk "BEGIN {print int($SCC_SIZE * $FULL / 100.0)}");     [ "${SCC_SIZE}" -eq 0 ] && SCC_SIZE=1;     SCC_SIZE="${SCC_SIZE}m";     java -Xshareclasses:name=openj9_system_scc,cacheDir=/opt/java/.scc,bootClassesOnly,nonFatal,createLayer -Xscmx$SCC_SIZE -version;     unset OPENJ9_JAVA_OPTIONS;         export OPENJ9_JAVA_OPTIONS="-Xshareclasses:name=openj9_system_scc,cacheDir=/opt/java/.scc,bootClassesOnly,nonFatal";     "${INSTALL_PATH_TOMCAT}"/bin/startup.sh;     sleep 5;     "${INSTALL_PATH_TOMCAT}"/bin/shutdown.sh -force;     sleep 5;     FULL=$( (java -Xshareclasses:name=openj9_system_scc,cacheDir=/opt/java/.scc,printallStats 2>&1 || true) | awk '/^Cache is [0-9.]*% .*full/ {print substr($3, 1, length($3)-1)}');     echo "SCC layer is $FULL% full.";     rm -rf "${INSTALL_PATH_TOMCAT}";     if [ -d "/opt/java/.scc" ]; then           chmod -R 0777 /opt/java/.scc;     fi;         echo "SCC generation phase completed";
# Fri, 02 Sep 2022 20:43:33 GMT
CMD ["jshell"]
```

-	Layers:
	-	`sha256:00f50047d6061c27e70588a5aab89adada756e87d782a6c6bd08b4139eb8ea10`  
		Last Modified: Fri, 02 Sep 2022 00:59:40 GMT  
		Size: 28.4 MB (28381340 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d5f852001267437456455b5b653558e021beda1d08adc778f3427b4d6734c7c8`  
		Last Modified: Fri, 02 Sep 2022 20:51:25 GMT  
		Size: 12.1 MB (12063866 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1152c1bfc2d0e0a226d1de172825c85a8f363e4cb2f0ade4d98122f387f4a42f`  
		Last Modified: Fri, 02 Sep 2022 20:52:26 GMT  
		Size: 199.9 MB (199938693 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8f0c369afb314ccb4b745967beb9417664f1d85ef21940a2c85544f9ebda1d51`  
		Last Modified: Fri, 02 Sep 2022 20:52:08 GMT  
		Size: 5.0 MB (4993481 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ibm-semeru-runtimes:open-11-jdk` - linux; s390x

```console
$ docker pull ibm-semeru-runtimes@sha256:a642d767e6e5c5a852cde4b4cc6e2ef10c567eb5b3128e5831168529f7c3394a
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **249.1 MB (249094682 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:cade4a153ae71c036d881936a8a58a9c550309e519f602522bc61715aa595605`
-	Default Command: `["jshell"]`

```dockerfile
# Fri, 02 Sep 2022 01:03:25 GMT
ADD file:aabc057fd7b1b1f9b4b729222b6dc90e98f846a65bfee1ee57cc899b6cee5a10 in / 
# Fri, 02 Sep 2022 01:03:28 GMT
CMD ["bash"]
# Fri, 02 Sep 2022 20:42:05 GMT
ENV LANG=en_US.UTF-8 LANGUAGE=en_US:en LC_ALL=en_US.UTF-8
# Fri, 02 Sep 2022 20:42:27 GMT
RUN apt-get update     && DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends tzdata curl ca-certificates fontconfig locales     && echo "en_US.UTF-8 UTF-8" >> /etc/locale.gen     && locale-gen en_US.UTF-8     && rm -rf /var/lib/apt/lists/*
# Fri, 02 Sep 2022 20:44:31 GMT
ENV JAVA_VERSION=jdk-11.0.16.1+1_openj9-0.33.1
# Fri, 02 Sep 2022 20:44:49 GMT
RUN set -eux;     ARCH="$(dpkg --print-architecture)";     case "${ARCH}" in        aarch64|arm64)          ESUM='fad70f5bd615d08d9b3e6222ce738be713050eedc8dce4b57bdccc85747d9ff6';          BINARY_URL='https://github.com/ibmruntimes/semeru11-binaries/releases/download/jdk-11.0.16.1%2B1_openj9-0.33.1/ibm-semeru-open-jdk_aarch64_linux_11.0.16.1_1_openj9-0.33.1.tar.gz';          ;;        amd64|x86_64)          ESUM='4eb9dc86bf92e144d7a2c8d6c2a6beac28c17b7348f2f0524e715548f52fd8f1';          BINARY_URL='https://github.com/ibmruntimes/semeru11-binaries/releases/download/jdk-11.0.16.1%2B1_openj9-0.33.1/ibm-semeru-open-jdk_x64_linux_11.0.16.1_1_openj9-0.33.1.tar.gz';          ;;        ppc64el|ppc64le)          ESUM='d71e5d26b7240d0e8a80499221ab79e5eed30ab1d985a5316bcfd240148435f8';          BINARY_URL='https://github.com/ibmruntimes/semeru11-binaries/releases/download/jdk-11.0.16.1%2B1_openj9-0.33.1/ibm-semeru-open-jdk_ppc64le_linux_11.0.16.1_1_openj9-0.33.1.tar.gz';          ;;        s390x)          ESUM='df4b746a0fc51bbab38aa86822a5f8e5587ed2b997cdd764de1c349d8caaa784';          BINARY_URL='https://github.com/ibmruntimes/semeru11-binaries/releases/download/jdk-11.0.16.1%2B1_openj9-0.33.1/ibm-semeru-open-jdk_s390x_linux_11.0.16.1_1_openj9-0.33.1.tar.gz';          ;;        *)          echo "Unsupported arch: ${ARCH}";          exit 1;          ;;     esac;     curl -LfsSo /tmp/openjdk.tar.gz ${BINARY_URL};     echo "${ESUM} */tmp/openjdk.tar.gz" | sha256sum -c -;     mkdir -p /opt/java/openjdk;     cd /opt/java/openjdk;     tar -xf /tmp/openjdk.tar.gz --strip-components=1;     rm -rf /tmp/openjdk.tar.gz;
# Fri, 02 Sep 2022 20:45:01 GMT
ENV JAVA_HOME=/opt/java/openjdk PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Fri, 02 Sep 2022 20:45:01 GMT
ENV JAVA_TOOL_OPTIONS=-XX:+IgnoreUnrecognizedVMOptions -XX:+PortableSharedCache -XX:+IdleTuningGcOnIdle -Xshareclasses:name=openj9_system_scc,cacheDir=/opt/java/.scc,readonly,nonFatal
# Fri, 02 Sep 2022 20:45:36 GMT
RUN set -eux;     unset OPENJ9_JAVA_OPTIONS;     SCC_SIZE="50m";     DOWNLOAD_PATH_TOMCAT=/tmp/tomcat;     INSTALL_PATH_TOMCAT=/opt/tomcat-home;     TOMCAT_CHECKSUM="0db27185d9fc3174f2c670f814df3dda8a008b89d1a38a5d96cbbe119767ebfb1cf0bce956b27954aee9be19c4a7b91f2579d967932207976322033a86075f98";     TOMCAT_DWNLD_URL="https://archive.apache.org/dist/tomcat/tomcat-9/v9.0.35/bin/apache-tomcat-9.0.35.tar.gz";         mkdir -p "${DOWNLOAD_PATH_TOMCAT}" "${INSTALL_PATH_TOMCAT}";     curl -LfsSo "${DOWNLOAD_PATH_TOMCAT}"/tomcat.tar.gz "${TOMCAT_DWNLD_URL}";     echo "${TOMCAT_CHECKSUM} *${DOWNLOAD_PATH_TOMCAT}/tomcat.tar.gz" | sha512sum -c -;     tar -xf "${DOWNLOAD_PATH_TOMCAT}"/tomcat.tar.gz -C "${INSTALL_PATH_TOMCAT}" --strip-components=1;     rm -rf "${DOWNLOAD_PATH_TOMCAT}";         java -Xshareclasses:name=dry_run_scc,cacheDir=/opt/java/.scc,bootClassesOnly,nonFatal,createLayer -Xscmx$SCC_SIZE -version;     export OPENJ9_JAVA_OPTIONS="-Xshareclasses:name=dry_run_scc,cacheDir=/opt/java/.scc,bootClassesOnly,nonFatal";     "${INSTALL_PATH_TOMCAT}"/bin/startup.sh;     sleep 5;     "${INSTALL_PATH_TOMCAT}"/bin/shutdown.sh -force;     sleep 15;     FULL=$( (java -Xshareclasses:name=dry_run_scc,cacheDir=/opt/java/.scc,printallStats 2>&1 || true) | awk '/^Cache is [0-9.]*% .*full/ {print substr($3, 1, length($3)-1)}');     DST_CACHE=$(java -Xshareclasses:name=dry_run_scc,cacheDir=/opt/java/.scc,destroy 2>&1 || true);     SCC_SIZE=$(echo $SCC_SIZE | sed 's/.$//');     SCC_SIZE=$(awk "BEGIN {print int($SCC_SIZE * $FULL / 100.0)}");     [ "${SCC_SIZE}" -eq 0 ] && SCC_SIZE=1;     SCC_SIZE="${SCC_SIZE}m";     java -Xshareclasses:name=openj9_system_scc,cacheDir=/opt/java/.scc,bootClassesOnly,nonFatal,createLayer -Xscmx$SCC_SIZE -version;     unset OPENJ9_JAVA_OPTIONS;         export OPENJ9_JAVA_OPTIONS="-Xshareclasses:name=openj9_system_scc,cacheDir=/opt/java/.scc,bootClassesOnly,nonFatal";     "${INSTALL_PATH_TOMCAT}"/bin/startup.sh;     sleep 5;     "${INSTALL_PATH_TOMCAT}"/bin/shutdown.sh -force;     sleep 5;     FULL=$( (java -Xshareclasses:name=openj9_system_scc,cacheDir=/opt/java/.scc,printallStats 2>&1 || true) | awk '/^Cache is [0-9.]*% .*full/ {print substr($3, 1, length($3)-1)}');     echo "SCC layer is $FULL% full.";     rm -rf "${INSTALL_PATH_TOMCAT}";     if [ -d "/opt/java/.scc" ]; then           chmod -R 0777 /opt/java/.scc;     fi;         echo "SCC generation phase completed";
# Fri, 02 Sep 2022 20:45:37 GMT
CMD ["jshell"]
```

-	Layers:
	-	`sha256:a32e6a15a6635185097921b9d08997d505b6b6500b6c142ad8e718d87c45ffad`  
		Last Modified: Fri, 02 Sep 2022 01:05:01 GMT  
		Size: 28.6 MB (28643161 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:97b5cf75e6a192822ffe9728f595a19b7e0dc78cdf10b0a2b0e91f076bf45793`  
		Last Modified: Fri, 02 Sep 2022 20:53:42 GMT  
		Size: 12.1 MB (12146616 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0250612c46f3c8ff2873bbcad03db604a61613369c224d6e750e655b6cdc7e99`  
		Last Modified: Fri, 02 Sep 2022 20:54:29 GMT  
		Size: 202.9 MB (202931754 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4ccc07091b901e34e55f84649b69c35b49fa3a3ad96a1320666d8da7dbb0b03d`  
		Last Modified: Fri, 02 Sep 2022 20:54:15 GMT  
		Size: 5.4 MB (5373151 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
