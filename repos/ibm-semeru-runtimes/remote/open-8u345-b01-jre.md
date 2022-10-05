## `ibm-semeru-runtimes:open-8u345-b01-jre`

```console
$ docker pull ibm-semeru-runtimes@sha256:7b0eed86cab5b75e729b48fba7e3f68d48eab8155189c6c8c78a04465ccba823
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 3
	-	linux; amd64
	-	linux; arm64 variant v8
	-	linux; s390x

### `ibm-semeru-runtimes:open-8u345-b01-jre` - linux; amd64

```console
$ docker pull ibm-semeru-runtimes@sha256:240f545a183fa1d8cc25c5cb88a24e5efa62b0b0a139355fd3939d0599f6910d
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **96.7 MB (96714593 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:3085e1fd950f5486e7b81a85096cdb0ec1697646d266fe0850250919e6812abf`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 04 Oct 2022 23:35:20 GMT
ADD file:6cd2e13356aa5339c1f2abd3c210a52f6ed74fae05cd61aa09f37b6a4764f65c in / 
# Tue, 04 Oct 2022 23:35:20 GMT
CMD ["bash"]
# Wed, 05 Oct 2022 17:18:57 GMT
ENV LANG=en_US.UTF-8 LANGUAGE=en_US:en LC_ALL=en_US.UTF-8
# Wed, 05 Oct 2022 17:19:09 GMT
RUN apt-get update     && DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends tzdata curl ca-certificates fontconfig locales     && echo "en_US.UTF-8 UTF-8" >> /etc/locale.gen     && locale-gen en_US.UTF-8     && rm -rf /var/lib/apt/lists/*
# Wed, 05 Oct 2022 17:19:10 GMT
ENV JAVA_VERSION=jdk8u345-b01_openj9-0.33.1
# Wed, 05 Oct 2022 17:20:50 GMT
RUN set -eux;     ARCH="$(dpkg --print-architecture)";     case "${ARCH}" in        aarch64|arm64)         ESUM='91479aa6163d196982f036bf5260e77f27085e5d65de50d68a3b9cb3903f6e15';          BINARY_URL='https://github.com/ibmruntimes/semeru8-binaries/releases/download/jdk8u345-b01_openj9-0.33.1/ibm-semeru-open-jre_aarch64_linux_8u345b01_openj9-0.33.1.tar.gz';          ;;        ppc64el|ppc64le)          ESUM='cb8772dfd613f89cd8a18067e38cf3dfa1feb4d0ecc579298a3d15f681602c88';          BINARY_URL='https://github.com/ibmruntimes/semeru8-binaries/releases/download/jdk8u345-b01_openj9-0.33.1/ibm-semeru-open-jre_ppc64le_linux_8u345b01_openj9-0.33.1.tar.gz';          ;;        amd64|x86_64)          ESUM='e8cbdfb677777544981d4c5290c19bef288d430978c2feb2dcf06e285f83a69a';          BINARY_URL='https://github.com/ibmruntimes/semeru8-binaries/releases/download/jdk8u345-b01_openj9-0.33.1/ibm-semeru-open-jre_x64_linux_8u345b01_openj9-0.33.1.tar.gz';          ;;        s390x)          ESUM='ad4adb78fc65b3740702569dd82bec743ec1715b297191f1ca3277f14eea88e0';          BINARY_URL='https://github.com/ibmruntimes/semeru8-binaries/releases/download/jdk8u345-b01_openj9-0.33.1/ibm-semeru-open-jre_s390x_linux_8u345b01_openj9-0.33.1.tar.gz';          ;;        *)          echo "Unsupported arch: ${ARCH}";          exit 1;          ;;     esac;     curl -LfsSo /tmp/openjdk.tar.gz ${BINARY_URL};     echo "${ESUM} */tmp/openjdk.tar.gz" | sha256sum -c -;     mkdir -p /opt/java/openjdk;     cd /opt/java/openjdk;     tar -xf /tmp/openjdk.tar.gz --strip-components=1;     rm -rf /tmp/openjdk.tar.gz;
# Wed, 05 Oct 2022 17:20:50 GMT
ENV JAVA_HOME=/opt/java/openjdk PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 05 Oct 2022 17:20:50 GMT
ENV JAVA_TOOL_OPTIONS=-XX:+IgnoreUnrecognizedVMOptions -XX:+PortableSharedCache -XX:+IdleTuningGcOnIdle -Xshareclasses:name=openj9_system_scc,cacheDir=/opt/java/.scc,readonly,nonFatal
# Wed, 05 Oct 2022 17:21:25 GMT
RUN set -eux;     unset OPENJ9_JAVA_OPTIONS;     SCC_SIZE="50m";     DOWNLOAD_PATH_TOMCAT=/tmp/tomcat;     INSTALL_PATH_TOMCAT=/opt/tomcat-home;     TOMCAT_CHECKSUM="0db27185d9fc3174f2c670f814df3dda8a008b89d1a38a5d96cbbe119767ebfb1cf0bce956b27954aee9be19c4a7b91f2579d967932207976322033a86075f98";     TOMCAT_DWNLD_URL="https://archive.apache.org/dist/tomcat/tomcat-9/v9.0.35/bin/apache-tomcat-9.0.35.tar.gz";         mkdir -p "${DOWNLOAD_PATH_TOMCAT}" "${INSTALL_PATH_TOMCAT}";     curl -LfsSo "${DOWNLOAD_PATH_TOMCAT}"/tomcat.tar.gz "${TOMCAT_DWNLD_URL}";     echo "${TOMCAT_CHECKSUM} *${DOWNLOAD_PATH_TOMCAT}/tomcat.tar.gz" | sha512sum -c -;     tar -xf "${DOWNLOAD_PATH_TOMCAT}"/tomcat.tar.gz -C "${INSTALL_PATH_TOMCAT}" --strip-components=1;     rm -rf "${DOWNLOAD_PATH_TOMCAT}";         java -Xshareclasses:name=dry_run_scc,cacheDir=/opt/java/.scc,bootClassesOnly,nonFatal,createLayer -Xscmx$SCC_SIZE -version;     export OPENJ9_JAVA_OPTIONS="-Xshareclasses:name=dry_run_scc,cacheDir=/opt/java/.scc,bootClassesOnly,nonFatal";     "${INSTALL_PATH_TOMCAT}"/bin/startup.sh;     sleep 5;     "${INSTALL_PATH_TOMCAT}"/bin/shutdown.sh -force;     sleep 15;     FULL=$( (java -Xshareclasses:name=dry_run_scc,cacheDir=/opt/java/.scc,printallStats 2>&1 || true) | awk '/^Cache is [0-9.]*% .*full/ {print substr($3, 1, length($3)-1)}');     DST_CACHE=$(java -Xshareclasses:name=dry_run_scc,cacheDir=/opt/java/.scc,destroy 2>&1 || true);     SCC_SIZE=$(echo $SCC_SIZE | sed 's/.$//');     SCC_SIZE=$(awk "BEGIN {print int($SCC_SIZE * $FULL / 100.0)}");     [ "${SCC_SIZE}" -eq 0 ] && SCC_SIZE=1;     SCC_SIZE="${SCC_SIZE}m";     java -Xshareclasses:name=openj9_system_scc,cacheDir=/opt/java/.scc,bootClassesOnly,nonFatal,createLayer -Xscmx$SCC_SIZE -version;     unset OPENJ9_JAVA_OPTIONS;         export OPENJ9_JAVA_OPTIONS="-Xshareclasses:name=openj9_system_scc,cacheDir=/opt/java/.scc,bootClassesOnly,nonFatal";     "${INSTALL_PATH_TOMCAT}"/bin/startup.sh;     sleep 5;     "${INSTALL_PATH_TOMCAT}"/bin/shutdown.sh -force;     sleep 5;     FULL=$( (java -Xshareclasses:name=openj9_system_scc,cacheDir=/opt/java/.scc,printallStats 2>&1 || true) | awk '/^Cache is [0-9.]*% .*full/ {print substr($3, 1, length($3)-1)}');     echo "SCC layer is $FULL% full.";     rm -rf "${INSTALL_PATH_TOMCAT}";     if [ -d "/opt/java/.scc" ]; then           chmod -R 0777 /opt/java/.scc;     fi;         echo "SCC generation phase completed";
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
	-	`sha256:766338647c24a223c166aa2b0a86bb79718db5d32871a6f5148387e37a4f38fd`  
		Last Modified: Wed, 05 Oct 2022 17:35:16 GMT  
		Size: 50.0 MB (50044150 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9ba6195866aff704b2ffde47bf776eb8873785559c4c59a7e524f3db1969dad1`  
		Last Modified: Wed, 05 Oct 2022 17:35:10 GMT  
		Size: 4.1 MB (4137479 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ibm-semeru-runtimes:open-8u345-b01-jre` - linux; arm64 variant v8

```console
$ docker pull ibm-semeru-runtimes@sha256:d8f7b8594c3dbacb1bee7c4c6887548a4d2d8c440e13ed3fea78ac6ab72af283
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **92.5 MB (92476360 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:12979333d042bef7f49adb6148b9de81be4c8057aa85a022be24aa9730e7e498`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 05 Oct 2022 00:02:19 GMT
ADD file:fd8103ca1472a4f51eeff3e22fbd1dfd61a3d22c34f16a61ef1ba016352e3629 in / 
# Wed, 05 Oct 2022 00:02:20 GMT
CMD ["bash"]
# Wed, 05 Oct 2022 16:30:26 GMT
ENV LANG=en_US.UTF-8 LANGUAGE=en_US:en LC_ALL=en_US.UTF-8
# Wed, 05 Oct 2022 16:30:43 GMT
RUN apt-get update     && DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends tzdata curl ca-certificates fontconfig locales     && echo "en_US.UTF-8 UTF-8" >> /etc/locale.gen     && locale-gen en_US.UTF-8     && rm -rf /var/lib/apt/lists/*
# Wed, 05 Oct 2022 16:30:43 GMT
ENV JAVA_VERSION=jdk8u345-b01_openj9-0.33.1
# Wed, 05 Oct 2022 16:32:37 GMT
RUN set -eux;     ARCH="$(dpkg --print-architecture)";     case "${ARCH}" in        aarch64|arm64)         ESUM='91479aa6163d196982f036bf5260e77f27085e5d65de50d68a3b9cb3903f6e15';          BINARY_URL='https://github.com/ibmruntimes/semeru8-binaries/releases/download/jdk8u345-b01_openj9-0.33.1/ibm-semeru-open-jre_aarch64_linux_8u345b01_openj9-0.33.1.tar.gz';          ;;        ppc64el|ppc64le)          ESUM='cb8772dfd613f89cd8a18067e38cf3dfa1feb4d0ecc579298a3d15f681602c88';          BINARY_URL='https://github.com/ibmruntimes/semeru8-binaries/releases/download/jdk8u345-b01_openj9-0.33.1/ibm-semeru-open-jre_ppc64le_linux_8u345b01_openj9-0.33.1.tar.gz';          ;;        amd64|x86_64)          ESUM='e8cbdfb677777544981d4c5290c19bef288d430978c2feb2dcf06e285f83a69a';          BINARY_URL='https://github.com/ibmruntimes/semeru8-binaries/releases/download/jdk8u345-b01_openj9-0.33.1/ibm-semeru-open-jre_x64_linux_8u345b01_openj9-0.33.1.tar.gz';          ;;        s390x)          ESUM='ad4adb78fc65b3740702569dd82bec743ec1715b297191f1ca3277f14eea88e0';          BINARY_URL='https://github.com/ibmruntimes/semeru8-binaries/releases/download/jdk8u345-b01_openj9-0.33.1/ibm-semeru-open-jre_s390x_linux_8u345b01_openj9-0.33.1.tar.gz';          ;;        *)          echo "Unsupported arch: ${ARCH}";          exit 1;          ;;     esac;     curl -LfsSo /tmp/openjdk.tar.gz ${BINARY_URL};     echo "${ESUM} */tmp/openjdk.tar.gz" | sha256sum -c -;     mkdir -p /opt/java/openjdk;     cd /opt/java/openjdk;     tar -xf /tmp/openjdk.tar.gz --strip-components=1;     rm -rf /tmp/openjdk.tar.gz;
# Wed, 05 Oct 2022 16:32:37 GMT
ENV JAVA_HOME=/opt/java/openjdk PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 05 Oct 2022 16:32:38 GMT
ENV JAVA_TOOL_OPTIONS=-XX:+IgnoreUnrecognizedVMOptions -XX:+PortableSharedCache -XX:+IdleTuningGcOnIdle -Xshareclasses:name=openj9_system_scc,cacheDir=/opt/java/.scc,readonly,nonFatal
# Wed, 05 Oct 2022 16:33:13 GMT
RUN set -eux;     unset OPENJ9_JAVA_OPTIONS;     SCC_SIZE="50m";     DOWNLOAD_PATH_TOMCAT=/tmp/tomcat;     INSTALL_PATH_TOMCAT=/opt/tomcat-home;     TOMCAT_CHECKSUM="0db27185d9fc3174f2c670f814df3dda8a008b89d1a38a5d96cbbe119767ebfb1cf0bce956b27954aee9be19c4a7b91f2579d967932207976322033a86075f98";     TOMCAT_DWNLD_URL="https://archive.apache.org/dist/tomcat/tomcat-9/v9.0.35/bin/apache-tomcat-9.0.35.tar.gz";         mkdir -p "${DOWNLOAD_PATH_TOMCAT}" "${INSTALL_PATH_TOMCAT}";     curl -LfsSo "${DOWNLOAD_PATH_TOMCAT}"/tomcat.tar.gz "${TOMCAT_DWNLD_URL}";     echo "${TOMCAT_CHECKSUM} *${DOWNLOAD_PATH_TOMCAT}/tomcat.tar.gz" | sha512sum -c -;     tar -xf "${DOWNLOAD_PATH_TOMCAT}"/tomcat.tar.gz -C "${INSTALL_PATH_TOMCAT}" --strip-components=1;     rm -rf "${DOWNLOAD_PATH_TOMCAT}";         java -Xshareclasses:name=dry_run_scc,cacheDir=/opt/java/.scc,bootClassesOnly,nonFatal,createLayer -Xscmx$SCC_SIZE -version;     export OPENJ9_JAVA_OPTIONS="-Xshareclasses:name=dry_run_scc,cacheDir=/opt/java/.scc,bootClassesOnly,nonFatal";     "${INSTALL_PATH_TOMCAT}"/bin/startup.sh;     sleep 5;     "${INSTALL_PATH_TOMCAT}"/bin/shutdown.sh -force;     sleep 15;     FULL=$( (java -Xshareclasses:name=dry_run_scc,cacheDir=/opt/java/.scc,printallStats 2>&1 || true) | awk '/^Cache is [0-9.]*% .*full/ {print substr($3, 1, length($3)-1)}');     DST_CACHE=$(java -Xshareclasses:name=dry_run_scc,cacheDir=/opt/java/.scc,destroy 2>&1 || true);     SCC_SIZE=$(echo $SCC_SIZE | sed 's/.$//');     SCC_SIZE=$(awk "BEGIN {print int($SCC_SIZE * $FULL / 100.0)}");     [ "${SCC_SIZE}" -eq 0 ] && SCC_SIZE=1;     SCC_SIZE="${SCC_SIZE}m";     java -Xshareclasses:name=openj9_system_scc,cacheDir=/opt/java/.scc,bootClassesOnly,nonFatal,createLayer -Xscmx$SCC_SIZE -version;     unset OPENJ9_JAVA_OPTIONS;         export OPENJ9_JAVA_OPTIONS="-Xshareclasses:name=openj9_system_scc,cacheDir=/opt/java/.scc,bootClassesOnly,nonFatal";     "${INSTALL_PATH_TOMCAT}"/bin/startup.sh;     sleep 5;     "${INSTALL_PATH_TOMCAT}"/bin/shutdown.sh -force;     sleep 5;     FULL=$( (java -Xshareclasses:name=openj9_system_scc,cacheDir=/opt/java/.scc,printallStats 2>&1 || true) | awk '/^Cache is [0-9.]*% .*full/ {print substr($3, 1, length($3)-1)}');     echo "SCC layer is $FULL% full.";     rm -rf "${INSTALL_PATH_TOMCAT}";     if [ -d "/opt/java/.scc" ]; then           chmod -R 0777 /opt/java/.scc;     fi;         echo "SCC generation phase completed";
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
	-	`sha256:4eaebefbfb342b7cad9b8b7f77845a22fdfe86483928f4334aafcfa837c89a75`  
		Last Modified: Wed, 05 Oct 2022 16:48:48 GMT  
		Size: 48.0 MB (47996719 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f23eb4d47acf1f33bedfdc93e35bf4c3784e819b611b3c31c7d5d86de4c7ae0b`  
		Last Modified: Wed, 05 Oct 2022 16:48:43 GMT  
		Size: 4.0 MB (4033263 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ibm-semeru-runtimes:open-8u345-b01-jre` - linux; s390x

```console
$ docker pull ibm-semeru-runtimes@sha256:2cc5e49e6fee7881604b1bc2aae2a61abb6db317b3362d6463688587264358f4
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **95.1 MB (95137304 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:7b8a68e1f5b680e4b3d3e16d41820d3832b14f35145a67bf7f2aef1baf0c77c7`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 04 Oct 2022 23:52:57 GMT
ADD file:b1fcc8690fce8195995c8eab6b853225d65017d69692537273760bf84bfb72ec in / 
# Tue, 04 Oct 2022 23:52:59 GMT
CMD ["bash"]
# Wed, 05 Oct 2022 07:15:22 GMT
ENV LANG=en_US.UTF-8 LANGUAGE=en_US:en LC_ALL=en_US.UTF-8
# Wed, 05 Oct 2022 07:15:44 GMT
RUN apt-get update     && DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends tzdata curl ca-certificates fontconfig locales     && echo "en_US.UTF-8 UTF-8" >> /etc/locale.gen     && locale-gen en_US.UTF-8     && rm -rf /var/lib/apt/lists/*
# Wed, 05 Oct 2022 07:15:45 GMT
ENV JAVA_VERSION=jdk8u345-b01_openj9-0.33.1
# Wed, 05 Oct 2022 07:17:34 GMT
RUN set -eux;     ARCH="$(dpkg --print-architecture)";     case "${ARCH}" in        aarch64|arm64)         ESUM='91479aa6163d196982f036bf5260e77f27085e5d65de50d68a3b9cb3903f6e15';          BINARY_URL='https://github.com/ibmruntimes/semeru8-binaries/releases/download/jdk8u345-b01_openj9-0.33.1/ibm-semeru-open-jre_aarch64_linux_8u345b01_openj9-0.33.1.tar.gz';          ;;        ppc64el|ppc64le)          ESUM='cb8772dfd613f89cd8a18067e38cf3dfa1feb4d0ecc579298a3d15f681602c88';          BINARY_URL='https://github.com/ibmruntimes/semeru8-binaries/releases/download/jdk8u345-b01_openj9-0.33.1/ibm-semeru-open-jre_ppc64le_linux_8u345b01_openj9-0.33.1.tar.gz';          ;;        amd64|x86_64)          ESUM='e8cbdfb677777544981d4c5290c19bef288d430978c2feb2dcf06e285f83a69a';          BINARY_URL='https://github.com/ibmruntimes/semeru8-binaries/releases/download/jdk8u345-b01_openj9-0.33.1/ibm-semeru-open-jre_x64_linux_8u345b01_openj9-0.33.1.tar.gz';          ;;        s390x)          ESUM='ad4adb78fc65b3740702569dd82bec743ec1715b297191f1ca3277f14eea88e0';          BINARY_URL='https://github.com/ibmruntimes/semeru8-binaries/releases/download/jdk8u345-b01_openj9-0.33.1/ibm-semeru-open-jre_s390x_linux_8u345b01_openj9-0.33.1.tar.gz';          ;;        *)          echo "Unsupported arch: ${ARCH}";          exit 1;          ;;     esac;     curl -LfsSo /tmp/openjdk.tar.gz ${BINARY_URL};     echo "${ESUM} */tmp/openjdk.tar.gz" | sha256sum -c -;     mkdir -p /opt/java/openjdk;     cd /opt/java/openjdk;     tar -xf /tmp/openjdk.tar.gz --strip-components=1;     rm -rf /tmp/openjdk.tar.gz;
# Wed, 05 Oct 2022 07:17:35 GMT
ENV JAVA_HOME=/opt/java/openjdk PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 05 Oct 2022 07:17:36 GMT
ENV JAVA_TOOL_OPTIONS=-XX:+IgnoreUnrecognizedVMOptions -XX:+PortableSharedCache -XX:+IdleTuningGcOnIdle -Xshareclasses:name=openj9_system_scc,cacheDir=/opt/java/.scc,readonly,nonFatal
# Wed, 05 Oct 2022 07:18:08 GMT
RUN set -eux;     unset OPENJ9_JAVA_OPTIONS;     SCC_SIZE="50m";     DOWNLOAD_PATH_TOMCAT=/tmp/tomcat;     INSTALL_PATH_TOMCAT=/opt/tomcat-home;     TOMCAT_CHECKSUM="0db27185d9fc3174f2c670f814df3dda8a008b89d1a38a5d96cbbe119767ebfb1cf0bce956b27954aee9be19c4a7b91f2579d967932207976322033a86075f98";     TOMCAT_DWNLD_URL="https://archive.apache.org/dist/tomcat/tomcat-9/v9.0.35/bin/apache-tomcat-9.0.35.tar.gz";         mkdir -p "${DOWNLOAD_PATH_TOMCAT}" "${INSTALL_PATH_TOMCAT}";     curl -LfsSo "${DOWNLOAD_PATH_TOMCAT}"/tomcat.tar.gz "${TOMCAT_DWNLD_URL}";     echo "${TOMCAT_CHECKSUM} *${DOWNLOAD_PATH_TOMCAT}/tomcat.tar.gz" | sha512sum -c -;     tar -xf "${DOWNLOAD_PATH_TOMCAT}"/tomcat.tar.gz -C "${INSTALL_PATH_TOMCAT}" --strip-components=1;     rm -rf "${DOWNLOAD_PATH_TOMCAT}";         java -Xshareclasses:name=dry_run_scc,cacheDir=/opt/java/.scc,bootClassesOnly,nonFatal,createLayer -Xscmx$SCC_SIZE -version;     export OPENJ9_JAVA_OPTIONS="-Xshareclasses:name=dry_run_scc,cacheDir=/opt/java/.scc,bootClassesOnly,nonFatal";     "${INSTALL_PATH_TOMCAT}"/bin/startup.sh;     sleep 5;     "${INSTALL_PATH_TOMCAT}"/bin/shutdown.sh -force;     sleep 15;     FULL=$( (java -Xshareclasses:name=dry_run_scc,cacheDir=/opt/java/.scc,printallStats 2>&1 || true) | awk '/^Cache is [0-9.]*% .*full/ {print substr($3, 1, length($3)-1)}');     DST_CACHE=$(java -Xshareclasses:name=dry_run_scc,cacheDir=/opt/java/.scc,destroy 2>&1 || true);     SCC_SIZE=$(echo $SCC_SIZE | sed 's/.$//');     SCC_SIZE=$(awk "BEGIN {print int($SCC_SIZE * $FULL / 100.0)}");     [ "${SCC_SIZE}" -eq 0 ] && SCC_SIZE=1;     SCC_SIZE="${SCC_SIZE}m";     java -Xshareclasses:name=openj9_system_scc,cacheDir=/opt/java/.scc,bootClassesOnly,nonFatal,createLayer -Xscmx$SCC_SIZE -version;     unset OPENJ9_JAVA_OPTIONS;         export OPENJ9_JAVA_OPTIONS="-Xshareclasses:name=openj9_system_scc,cacheDir=/opt/java/.scc,bootClassesOnly,nonFatal";     "${INSTALL_PATH_TOMCAT}"/bin/startup.sh;     sleep 5;     "${INSTALL_PATH_TOMCAT}"/bin/shutdown.sh -force;     sleep 5;     FULL=$( (java -Xshareclasses:name=openj9_system_scc,cacheDir=/opt/java/.scc,printallStats 2>&1 || true) | awk '/^Cache is [0-9.]*% .*full/ {print substr($3, 1, length($3)-1)}');     echo "SCC layer is $FULL% full.";     rm -rf "${INSTALL_PATH_TOMCAT}";     if [ -d "/opt/java/.scc" ]; then           chmod -R 0777 /opt/java/.scc;     fi;         echo "SCC generation phase completed";
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
	-	`sha256:1b28f32cafb0edb4b23413fca275fd1964daaa3072ec96c5a670353ec8209140`  
		Last Modified: Wed, 05 Oct 2022 07:34:04 GMT  
		Size: 50.0 MB (49974583 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4d37652a24ca6db4113efe01722601c922f27856ccff3f5d66cbe1d2d6badd2a`  
		Last Modified: Wed, 05 Oct 2022 07:33:59 GMT  
		Size: 4.4 MB (4372399 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
