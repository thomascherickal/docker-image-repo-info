## `ibm-semeru-runtimes:open-11-jdk`

```console
$ docker pull ibm-semeru-runtimes@sha256:9f4cc9630bc582c8e75fb81f1fdc2ae49e227a26c3dfde28007650ae5128e672
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 3
	-	linux; amd64
	-	linux; arm64 variant v8
	-	linux; s390x

### `ibm-semeru-runtimes:open-11-jdk` - linux; amd64

```console
$ docker pull ibm-semeru-runtimes@sha256:0482cba588b7a19280576466f369dc3046c09b1bb50d3011513257a183c0099e
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **252.2 MB (252155510 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a2be38567b63e79a4cff9c571f430d10530086024d6d85f993845921f0b9a1e1`
-	Default Command: `["jshell"]`

```dockerfile
# Tue, 04 Oct 2022 23:35:20 GMT
ADD file:6cd2e13356aa5339c1f2abd3c210a52f6ed74fae05cd61aa09f37b6a4764f65c in / 
# Tue, 04 Oct 2022 23:35:20 GMT
CMD ["bash"]
# Wed, 05 Oct 2022 17:18:57 GMT
ENV LANG=en_US.UTF-8 LANGUAGE=en_US:en LC_ALL=en_US.UTF-8
# Wed, 05 Oct 2022 17:19:09 GMT
RUN apt-get update     && DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends tzdata curl ca-certificates fontconfig locales     && echo "en_US.UTF-8 UTF-8" >> /etc/locale.gen     && locale-gen en_US.UTF-8     && rm -rf /var/lib/apt/lists/*
# Wed, 05 Oct 2022 17:22:34 GMT
ENV JAVA_VERSION=jdk-11.0.16.1+1_openj9-0.33.1
# Wed, 05 Oct 2022 17:22:50 GMT
RUN set -eux;     ARCH="$(dpkg --print-architecture)";     case "${ARCH}" in        aarch64|arm64)          ESUM='fad70f5bd615d08d9b3e6222ce738be713050eedc8dce4b57bdccc85747d9ff6';          BINARY_URL='https://github.com/ibmruntimes/semeru11-binaries/releases/download/jdk-11.0.16.1%2B1_openj9-0.33.1/ibm-semeru-open-jdk_aarch64_linux_11.0.16.1_1_openj9-0.33.1.tar.gz';          ;;        amd64|x86_64)          ESUM='4eb9dc86bf92e144d7a2c8d6c2a6beac28c17b7348f2f0524e715548f52fd8f1';          BINARY_URL='https://github.com/ibmruntimes/semeru11-binaries/releases/download/jdk-11.0.16.1%2B1_openj9-0.33.1/ibm-semeru-open-jdk_x64_linux_11.0.16.1_1_openj9-0.33.1.tar.gz';          ;;        ppc64el|ppc64le)          ESUM='d71e5d26b7240d0e8a80499221ab79e5eed30ab1d985a5316bcfd240148435f8';          BINARY_URL='https://github.com/ibmruntimes/semeru11-binaries/releases/download/jdk-11.0.16.1%2B1_openj9-0.33.1/ibm-semeru-open-jdk_ppc64le_linux_11.0.16.1_1_openj9-0.33.1.tar.gz';          ;;        s390x)          ESUM='df4b746a0fc51bbab38aa86822a5f8e5587ed2b997cdd764de1c349d8caaa784';          BINARY_URL='https://github.com/ibmruntimes/semeru11-binaries/releases/download/jdk-11.0.16.1%2B1_openj9-0.33.1/ibm-semeru-open-jdk_s390x_linux_11.0.16.1_1_openj9-0.33.1.tar.gz';          ;;        *)          echo "Unsupported arch: ${ARCH}";          exit 1;          ;;     esac;     curl -LfsSo /tmp/openjdk.tar.gz ${BINARY_URL};     echo "${ESUM} */tmp/openjdk.tar.gz" | sha256sum -c -;     mkdir -p /opt/java/openjdk;     cd /opt/java/openjdk;     tar -xf /tmp/openjdk.tar.gz --strip-components=1;     rm -rf /tmp/openjdk.tar.gz;
# Wed, 05 Oct 2022 17:22:50 GMT
ENV JAVA_HOME=/opt/java/openjdk PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 05 Oct 2022 17:22:50 GMT
ENV JAVA_TOOL_OPTIONS=-XX:+IgnoreUnrecognizedVMOptions -XX:+PortableSharedCache -XX:+IdleTuningGcOnIdle -Xshareclasses:name=openj9_system_scc,cacheDir=/opt/java/.scc,readonly,nonFatal
# Wed, 05 Oct 2022 17:23:26 GMT
RUN set -eux;     unset OPENJ9_JAVA_OPTIONS;     SCC_SIZE="50m";     DOWNLOAD_PATH_TOMCAT=/tmp/tomcat;     INSTALL_PATH_TOMCAT=/opt/tomcat-home;     TOMCAT_CHECKSUM="0db27185d9fc3174f2c670f814df3dda8a008b89d1a38a5d96cbbe119767ebfb1cf0bce956b27954aee9be19c4a7b91f2579d967932207976322033a86075f98";     TOMCAT_DWNLD_URL="https://archive.apache.org/dist/tomcat/tomcat-9/v9.0.35/bin/apache-tomcat-9.0.35.tar.gz";         mkdir -p "${DOWNLOAD_PATH_TOMCAT}" "${INSTALL_PATH_TOMCAT}";     curl -LfsSo "${DOWNLOAD_PATH_TOMCAT}"/tomcat.tar.gz "${TOMCAT_DWNLD_URL}";     echo "${TOMCAT_CHECKSUM} *${DOWNLOAD_PATH_TOMCAT}/tomcat.tar.gz" | sha512sum -c -;     tar -xf "${DOWNLOAD_PATH_TOMCAT}"/tomcat.tar.gz -C "${INSTALL_PATH_TOMCAT}" --strip-components=1;     rm -rf "${DOWNLOAD_PATH_TOMCAT}";         java -Xshareclasses:name=dry_run_scc,cacheDir=/opt/java/.scc,bootClassesOnly,nonFatal,createLayer -Xscmx$SCC_SIZE -version;     export OPENJ9_JAVA_OPTIONS="-Xshareclasses:name=dry_run_scc,cacheDir=/opt/java/.scc,bootClassesOnly,nonFatal";     "${INSTALL_PATH_TOMCAT}"/bin/startup.sh;     sleep 5;     "${INSTALL_PATH_TOMCAT}"/bin/shutdown.sh -force;     sleep 15;     FULL=$( (java -Xshareclasses:name=dry_run_scc,cacheDir=/opt/java/.scc,printallStats 2>&1 || true) | awk '/^Cache is [0-9.]*% .*full/ {print substr($3, 1, length($3)-1)}');     DST_CACHE=$(java -Xshareclasses:name=dry_run_scc,cacheDir=/opt/java/.scc,destroy 2>&1 || true);     SCC_SIZE=$(echo $SCC_SIZE | sed 's/.$//');     SCC_SIZE=$(awk "BEGIN {print int($SCC_SIZE * $FULL / 100.0)}");     [ "${SCC_SIZE}" -eq 0 ] && SCC_SIZE=1;     SCC_SIZE="${SCC_SIZE}m";     java -Xshareclasses:name=openj9_system_scc,cacheDir=/opt/java/.scc,bootClassesOnly,nonFatal,createLayer -Xscmx$SCC_SIZE -version;     unset OPENJ9_JAVA_OPTIONS;         export OPENJ9_JAVA_OPTIONS="-Xshareclasses:name=openj9_system_scc,cacheDir=/opt/java/.scc,bootClassesOnly,nonFatal";     "${INSTALL_PATH_TOMCAT}"/bin/startup.sh;     sleep 5;     "${INSTALL_PATH_TOMCAT}"/bin/shutdown.sh -force;     sleep 5;     FULL=$( (java -Xshareclasses:name=openj9_system_scc,cacheDir=/opt/java/.scc,printallStats 2>&1 || true) | awk '/^Cache is [0-9.]*% .*full/ {print substr($3, 1, length($3)-1)}');     echo "SCC layer is $FULL% full.";     rm -rf "${INSTALL_PATH_TOMCAT}";     if [ -d "/opt/java/.scc" ]; then           chmod -R 0777 /opt/java/.scc;     fi;         echo "SCC generation phase completed";
# Wed, 05 Oct 2022 17:23:26 GMT
CMD ["jshell"]
```

-	Layers:
	-	`sha256:cf92e523b49ea3d1fae59f5f082437a5f96c244fda6697995920142ff31d59cf`  
		Last Modified: Tue, 04 Oct 2022 03:04:01 GMT  
		Size: 30.4 MB (30428928 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:223828f10a72de9358a21e0ea6f8da2f9fef1ed531e11a888a42e61b938994a3`  
		Last Modified: Wed, 05 Oct 2022 17:34:34 GMT  
		Size: 12.1 MB (12104036 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:312df89b483b09b39ae928774ad6832be26e23e29321a5680369ed847e03d16c`  
		Last Modified: Wed, 05 Oct 2022 17:36:07 GMT  
		Size: 204.4 MB (204414107 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0c1e28dfe005331cfe8e66ca0434ac5ad55216e7270b67561240aa1679e879c2`  
		Last Modified: Wed, 05 Oct 2022 17:35:52 GMT  
		Size: 5.2 MB (5208439 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ibm-semeru-runtimes:open-11-jdk` - linux; arm64 variant v8

```console
$ docker pull ibm-semeru-runtimes@sha256:5897b134dd26839998b26de47531b4fa3c958634b0c620fdecb840957ea81f9a
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **245.4 MB (245398636 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:223989b7c9c7b9289e3270024b588ef4520bf39a1ba4e7eb4ce26017c093d743`
-	Default Command: `["jshell"]`

```dockerfile
# Wed, 05 Oct 2022 00:02:19 GMT
ADD file:fd8103ca1472a4f51eeff3e22fbd1dfd61a3d22c34f16a61ef1ba016352e3629 in / 
# Wed, 05 Oct 2022 00:02:20 GMT
CMD ["bash"]
# Wed, 05 Oct 2022 16:30:26 GMT
ENV LANG=en_US.UTF-8 LANGUAGE=en_US:en LC_ALL=en_US.UTF-8
# Wed, 05 Oct 2022 16:30:43 GMT
RUN apt-get update     && DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends tzdata curl ca-certificates fontconfig locales     && echo "en_US.UTF-8 UTF-8" >> /etc/locale.gen     && locale-gen en_US.UTF-8     && rm -rf /var/lib/apt/lists/*
# Wed, 05 Oct 2022 16:34:24 GMT
ENV JAVA_VERSION=jdk-11.0.16.1+1_openj9-0.33.1
# Wed, 05 Oct 2022 16:34:31 GMT
RUN set -eux;     ARCH="$(dpkg --print-architecture)";     case "${ARCH}" in        aarch64|arm64)          ESUM='fad70f5bd615d08d9b3e6222ce738be713050eedc8dce4b57bdccc85747d9ff6';          BINARY_URL='https://github.com/ibmruntimes/semeru11-binaries/releases/download/jdk-11.0.16.1%2B1_openj9-0.33.1/ibm-semeru-open-jdk_aarch64_linux_11.0.16.1_1_openj9-0.33.1.tar.gz';          ;;        amd64|x86_64)          ESUM='4eb9dc86bf92e144d7a2c8d6c2a6beac28c17b7348f2f0524e715548f52fd8f1';          BINARY_URL='https://github.com/ibmruntimes/semeru11-binaries/releases/download/jdk-11.0.16.1%2B1_openj9-0.33.1/ibm-semeru-open-jdk_x64_linux_11.0.16.1_1_openj9-0.33.1.tar.gz';          ;;        ppc64el|ppc64le)          ESUM='d71e5d26b7240d0e8a80499221ab79e5eed30ab1d985a5316bcfd240148435f8';          BINARY_URL='https://github.com/ibmruntimes/semeru11-binaries/releases/download/jdk-11.0.16.1%2B1_openj9-0.33.1/ibm-semeru-open-jdk_ppc64le_linux_11.0.16.1_1_openj9-0.33.1.tar.gz';          ;;        s390x)          ESUM='df4b746a0fc51bbab38aa86822a5f8e5587ed2b997cdd764de1c349d8caaa784';          BINARY_URL='https://github.com/ibmruntimes/semeru11-binaries/releases/download/jdk-11.0.16.1%2B1_openj9-0.33.1/ibm-semeru-open-jdk_s390x_linux_11.0.16.1_1_openj9-0.33.1.tar.gz';          ;;        *)          echo "Unsupported arch: ${ARCH}";          exit 1;          ;;     esac;     curl -LfsSo /tmp/openjdk.tar.gz ${BINARY_URL};     echo "${ESUM} */tmp/openjdk.tar.gz" | sha256sum -c -;     mkdir -p /opt/java/openjdk;     cd /opt/java/openjdk;     tar -xf /tmp/openjdk.tar.gz --strip-components=1;     rm -rf /tmp/openjdk.tar.gz;
# Wed, 05 Oct 2022 16:34:32 GMT
ENV JAVA_HOME=/opt/java/openjdk PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 05 Oct 2022 16:34:32 GMT
ENV JAVA_TOOL_OPTIONS=-XX:+IgnoreUnrecognizedVMOptions -XX:+PortableSharedCache -XX:+IdleTuningGcOnIdle -Xshareclasses:name=openj9_system_scc,cacheDir=/opt/java/.scc,readonly,nonFatal
# Wed, 05 Oct 2022 16:35:07 GMT
RUN set -eux;     unset OPENJ9_JAVA_OPTIONS;     SCC_SIZE="50m";     DOWNLOAD_PATH_TOMCAT=/tmp/tomcat;     INSTALL_PATH_TOMCAT=/opt/tomcat-home;     TOMCAT_CHECKSUM="0db27185d9fc3174f2c670f814df3dda8a008b89d1a38a5d96cbbe119767ebfb1cf0bce956b27954aee9be19c4a7b91f2579d967932207976322033a86075f98";     TOMCAT_DWNLD_URL="https://archive.apache.org/dist/tomcat/tomcat-9/v9.0.35/bin/apache-tomcat-9.0.35.tar.gz";         mkdir -p "${DOWNLOAD_PATH_TOMCAT}" "${INSTALL_PATH_TOMCAT}";     curl -LfsSo "${DOWNLOAD_PATH_TOMCAT}"/tomcat.tar.gz "${TOMCAT_DWNLD_URL}";     echo "${TOMCAT_CHECKSUM} *${DOWNLOAD_PATH_TOMCAT}/tomcat.tar.gz" | sha512sum -c -;     tar -xf "${DOWNLOAD_PATH_TOMCAT}"/tomcat.tar.gz -C "${INSTALL_PATH_TOMCAT}" --strip-components=1;     rm -rf "${DOWNLOAD_PATH_TOMCAT}";         java -Xshareclasses:name=dry_run_scc,cacheDir=/opt/java/.scc,bootClassesOnly,nonFatal,createLayer -Xscmx$SCC_SIZE -version;     export OPENJ9_JAVA_OPTIONS="-Xshareclasses:name=dry_run_scc,cacheDir=/opt/java/.scc,bootClassesOnly,nonFatal";     "${INSTALL_PATH_TOMCAT}"/bin/startup.sh;     sleep 5;     "${INSTALL_PATH_TOMCAT}"/bin/shutdown.sh -force;     sleep 15;     FULL=$( (java -Xshareclasses:name=dry_run_scc,cacheDir=/opt/java/.scc,printallStats 2>&1 || true) | awk '/^Cache is [0-9.]*% .*full/ {print substr($3, 1, length($3)-1)}');     DST_CACHE=$(java -Xshareclasses:name=dry_run_scc,cacheDir=/opt/java/.scc,destroy 2>&1 || true);     SCC_SIZE=$(echo $SCC_SIZE | sed 's/.$//');     SCC_SIZE=$(awk "BEGIN {print int($SCC_SIZE * $FULL / 100.0)}");     [ "${SCC_SIZE}" -eq 0 ] && SCC_SIZE=1;     SCC_SIZE="${SCC_SIZE}m";     java -Xshareclasses:name=openj9_system_scc,cacheDir=/opt/java/.scc,bootClassesOnly,nonFatal,createLayer -Xscmx$SCC_SIZE -version;     unset OPENJ9_JAVA_OPTIONS;         export OPENJ9_JAVA_OPTIONS="-Xshareclasses:name=openj9_system_scc,cacheDir=/opt/java/.scc,bootClassesOnly,nonFatal";     "${INSTALL_PATH_TOMCAT}"/bin/startup.sh;     sleep 5;     "${INSTALL_PATH_TOMCAT}"/bin/shutdown.sh -force;     sleep 5;     FULL=$( (java -Xshareclasses:name=openj9_system_scc,cacheDir=/opt/java/.scc,printallStats 2>&1 || true) | awk '/^Cache is [0-9.]*% .*full/ {print substr($3, 1, length($3)-1)}');     echo "SCC layer is $FULL% full.";     rm -rf "${INSTALL_PATH_TOMCAT}";     if [ -d "/opt/java/.scc" ]; then           chmod -R 0777 /opt/java/.scc;     fi;         echo "SCC generation phase completed";
# Wed, 05 Oct 2022 16:35:08 GMT
CMD ["jshell"]
```

-	Layers:
	-	`sha256:d6cb415e2683249f7884ee5367306b023c72f907afeca2a30ca19c8de5f4f7d9`  
		Last Modified: Tue, 04 Oct 2022 15:08:22 GMT  
		Size: 28.4 MB (28382255 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d70f1e149a1b47a62ec60d4a4b409048e900d6f1fa93d0f7d83287fe79d4457c`  
		Last Modified: Wed, 05 Oct 2022 16:48:02 GMT  
		Size: 12.1 MB (12064123 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:418c56ba61a45ef788bad34afc45fdd12ba62a6a9759cbd98cbb75ad61b1cb66`  
		Last Modified: Wed, 05 Oct 2022 16:49:47 GMT  
		Size: 199.9 MB (199938620 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d588cc48ba604d734db623ed5562bedcabc03bc50bd06555dafbd833cbf87795`  
		Last Modified: Wed, 05 Oct 2022 16:49:31 GMT  
		Size: 5.0 MB (5013638 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ibm-semeru-runtimes:open-11-jdk` - linux; s390x

```console
$ docker pull ibm-semeru-runtimes@sha256:86a0fddfbaaf8daed4320b69bee0c71ab6cfe05fef0ef47cddd81d72ac0d0b41
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **249.1 MB (249069454 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ab94745dbbb14db90293c28767674bc240f25843bc98a5cdecafba9040b26ca7`
-	Default Command: `["jshell"]`

```dockerfile
# Tue, 04 Oct 2022 23:52:57 GMT
ADD file:b1fcc8690fce8195995c8eab6b853225d65017d69692537273760bf84bfb72ec in / 
# Tue, 04 Oct 2022 23:52:59 GMT
CMD ["bash"]
# Wed, 05 Oct 2022 07:15:22 GMT
ENV LANG=en_US.UTF-8 LANGUAGE=en_US:en LC_ALL=en_US.UTF-8
# Wed, 05 Oct 2022 07:15:44 GMT
RUN apt-get update     && DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends tzdata curl ca-certificates fontconfig locales     && echo "en_US.UTF-8 UTF-8" >> /etc/locale.gen     && locale-gen en_US.UTF-8     && rm -rf /var/lib/apt/lists/*
# Wed, 05 Oct 2022 07:19:27 GMT
ENV JAVA_VERSION=jdk-11.0.16.1+1_openj9-0.33.1
# Wed, 05 Oct 2022 07:19:42 GMT
RUN set -eux;     ARCH="$(dpkg --print-architecture)";     case "${ARCH}" in        aarch64|arm64)          ESUM='fad70f5bd615d08d9b3e6222ce738be713050eedc8dce4b57bdccc85747d9ff6';          BINARY_URL='https://github.com/ibmruntimes/semeru11-binaries/releases/download/jdk-11.0.16.1%2B1_openj9-0.33.1/ibm-semeru-open-jdk_aarch64_linux_11.0.16.1_1_openj9-0.33.1.tar.gz';          ;;        amd64|x86_64)          ESUM='4eb9dc86bf92e144d7a2c8d6c2a6beac28c17b7348f2f0524e715548f52fd8f1';          BINARY_URL='https://github.com/ibmruntimes/semeru11-binaries/releases/download/jdk-11.0.16.1%2B1_openj9-0.33.1/ibm-semeru-open-jdk_x64_linux_11.0.16.1_1_openj9-0.33.1.tar.gz';          ;;        ppc64el|ppc64le)          ESUM='d71e5d26b7240d0e8a80499221ab79e5eed30ab1d985a5316bcfd240148435f8';          BINARY_URL='https://github.com/ibmruntimes/semeru11-binaries/releases/download/jdk-11.0.16.1%2B1_openj9-0.33.1/ibm-semeru-open-jdk_ppc64le_linux_11.0.16.1_1_openj9-0.33.1.tar.gz';          ;;        s390x)          ESUM='df4b746a0fc51bbab38aa86822a5f8e5587ed2b997cdd764de1c349d8caaa784';          BINARY_URL='https://github.com/ibmruntimes/semeru11-binaries/releases/download/jdk-11.0.16.1%2B1_openj9-0.33.1/ibm-semeru-open-jdk_s390x_linux_11.0.16.1_1_openj9-0.33.1.tar.gz';          ;;        *)          echo "Unsupported arch: ${ARCH}";          exit 1;          ;;     esac;     curl -LfsSo /tmp/openjdk.tar.gz ${BINARY_URL};     echo "${ESUM} */tmp/openjdk.tar.gz" | sha256sum -c -;     mkdir -p /opt/java/openjdk;     cd /opt/java/openjdk;     tar -xf /tmp/openjdk.tar.gz --strip-components=1;     rm -rf /tmp/openjdk.tar.gz;
# Wed, 05 Oct 2022 07:19:47 GMT
ENV JAVA_HOME=/opt/java/openjdk PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 05 Oct 2022 07:19:47 GMT
ENV JAVA_TOOL_OPTIONS=-XX:+IgnoreUnrecognizedVMOptions -XX:+PortableSharedCache -XX:+IdleTuningGcOnIdle -Xshareclasses:name=openj9_system_scc,cacheDir=/opt/java/.scc,readonly,nonFatal
# Wed, 05 Oct 2022 07:20:20 GMT
RUN set -eux;     unset OPENJ9_JAVA_OPTIONS;     SCC_SIZE="50m";     DOWNLOAD_PATH_TOMCAT=/tmp/tomcat;     INSTALL_PATH_TOMCAT=/opt/tomcat-home;     TOMCAT_CHECKSUM="0db27185d9fc3174f2c670f814df3dda8a008b89d1a38a5d96cbbe119767ebfb1cf0bce956b27954aee9be19c4a7b91f2579d967932207976322033a86075f98";     TOMCAT_DWNLD_URL="https://archive.apache.org/dist/tomcat/tomcat-9/v9.0.35/bin/apache-tomcat-9.0.35.tar.gz";         mkdir -p "${DOWNLOAD_PATH_TOMCAT}" "${INSTALL_PATH_TOMCAT}";     curl -LfsSo "${DOWNLOAD_PATH_TOMCAT}"/tomcat.tar.gz "${TOMCAT_DWNLD_URL}";     echo "${TOMCAT_CHECKSUM} *${DOWNLOAD_PATH_TOMCAT}/tomcat.tar.gz" | sha512sum -c -;     tar -xf "${DOWNLOAD_PATH_TOMCAT}"/tomcat.tar.gz -C "${INSTALL_PATH_TOMCAT}" --strip-components=1;     rm -rf "${DOWNLOAD_PATH_TOMCAT}";         java -Xshareclasses:name=dry_run_scc,cacheDir=/opt/java/.scc,bootClassesOnly,nonFatal,createLayer -Xscmx$SCC_SIZE -version;     export OPENJ9_JAVA_OPTIONS="-Xshareclasses:name=dry_run_scc,cacheDir=/opt/java/.scc,bootClassesOnly,nonFatal";     "${INSTALL_PATH_TOMCAT}"/bin/startup.sh;     sleep 5;     "${INSTALL_PATH_TOMCAT}"/bin/shutdown.sh -force;     sleep 15;     FULL=$( (java -Xshareclasses:name=dry_run_scc,cacheDir=/opt/java/.scc,printallStats 2>&1 || true) | awk '/^Cache is [0-9.]*% .*full/ {print substr($3, 1, length($3)-1)}');     DST_CACHE=$(java -Xshareclasses:name=dry_run_scc,cacheDir=/opt/java/.scc,destroy 2>&1 || true);     SCC_SIZE=$(echo $SCC_SIZE | sed 's/.$//');     SCC_SIZE=$(awk "BEGIN {print int($SCC_SIZE * $FULL / 100.0)}");     [ "${SCC_SIZE}" -eq 0 ] && SCC_SIZE=1;     SCC_SIZE="${SCC_SIZE}m";     java -Xshareclasses:name=openj9_system_scc,cacheDir=/opt/java/.scc,bootClassesOnly,nonFatal,createLayer -Xscmx$SCC_SIZE -version;     unset OPENJ9_JAVA_OPTIONS;         export OPENJ9_JAVA_OPTIONS="-Xshareclasses:name=openj9_system_scc,cacheDir=/opt/java/.scc,bootClassesOnly,nonFatal";     "${INSTALL_PATH_TOMCAT}"/bin/startup.sh;     sleep 5;     "${INSTALL_PATH_TOMCAT}"/bin/shutdown.sh -force;     sleep 5;     FULL=$( (java -Xshareclasses:name=openj9_system_scc,cacheDir=/opt/java/.scc,printallStats 2>&1 || true) | awk '/^Cache is [0-9.]*% .*full/ {print substr($3, 1, length($3)-1)}');     echo "SCC layer is $FULL% full.";     rm -rf "${INSTALL_PATH_TOMCAT}";     if [ -d "/opt/java/.scc" ]; then           chmod -R 0777 /opt/java/.scc;     fi;         echo "SCC generation phase completed";
# Wed, 05 Oct 2022 07:20:20 GMT
CMD ["jshell"]
```

-	Layers:
	-	`sha256:29c30188ad5f0c76a8b336bfa488a1bdf199dc8127ed81e4051c1c71d4da8f87`  
		Last Modified: Tue, 04 Oct 2022 23:54:34 GMT  
		Size: 28.6 MB (28643466 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:12a8cc7473330bd6fbc22731594f4d1fd2b17b44ebdd2045c922739d6b0f83c7`  
		Last Modified: Wed, 05 Oct 2022 07:33:32 GMT  
		Size: 12.1 MB (12146856 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4bc9837c016dc337a0d2fe3c8b24616e16c4fece374bb26d59e66754cfa7f29a`  
		Last Modified: Wed, 05 Oct 2022 07:34:43 GMT  
		Size: 202.9 MB (202931756 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0281b9e24905dafeff006c4a1a0db22b65743f8a45eb0b6623d527d429bb2921`  
		Last Modified: Wed, 05 Oct 2022 07:34:31 GMT  
		Size: 5.3 MB (5347376 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
