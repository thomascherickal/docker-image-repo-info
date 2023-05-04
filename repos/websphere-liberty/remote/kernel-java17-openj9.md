## `websphere-liberty:kernel-java17-openj9`

```console
$ docker pull websphere-liberty@sha256:8687b6533b4073b6ade3919fb5ce13f946a4f799dd99d3a7878e68af1a942d7d
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 4
	-	linux; amd64
	-	linux; arm64 variant v8
	-	linux; ppc64le
	-	linux; s390x

### `websphere-liberty:kernel-java17-openj9` - linux; amd64

```console
$ docker pull websphere-liberty@sha256:4b572858f91a934aad652308c1085017530f7a0e96d0ff2cbfe89c77f8633c3c
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **114.8 MB (114805584 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:7c2f624d0ce112ce55fcb3ed6a068f10778c4a6f3e8c34b66559797a99290b6f`
-	Entrypoint: `["\/opt\/ibm\/helpers\/runtime\/docker-server.sh"]`
-	Default Command: `["\/opt\/ibm\/wlp\/bin\/server","run","defaultServer"]`

```dockerfile
# Thu, 13 Apr 2023 13:05:13 GMT
ARG RELEASE
# Thu, 13 Apr 2023 13:05:13 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Thu, 13 Apr 2023 13:05:13 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Thu, 13 Apr 2023 13:05:13 GMT
LABEL org.opencontainers.image.version=20.04
# Thu, 13 Apr 2023 13:05:15 GMT
ADD file:d05d1c0936b046937bd5755876db2f8da3ed8ccbcf464bb56c312fbc7ed78589 in / 
# Thu, 13 Apr 2023 13:05:15 GMT
CMD ["/bin/bash"]
# Tue, 18 Apr 2023 01:46:01 GMT
ENV LANG=en_US.UTF-8 LANGUAGE=en_US:en LC_ALL=en_US.UTF-8
# Tue, 18 Apr 2023 01:46:22 GMT
RUN apt-get update     && DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends tzdata curl ca-certificates fontconfig locales     && echo "en_US.UTF-8 UTF-8" >> /etc/locale.gen     && locale-gen en_US.UTF-8     && rm -rf /var/lib/apt/lists/*
# Tue, 18 Apr 2023 01:49:49 GMT
ENV JAVA_VERSION=jdk-17.0.6+10_openj9-0.36.0
# Tue, 18 Apr 2023 01:50:45 GMT
RUN set -eux;     ARCH="$(dpkg --print-architecture)";     case "${ARCH}" in        aarch64|arm64)          ESUM='492bd87e39fc0eb78218746e98c4c0f6730af9c998b872c1a175c0e907d11510';          BINARY_URL='https://github.com/ibmruntimes/semeru17-binaries/releases/download/jdk-17.0.6%2B10_openj9-0.36.0/ibm-semeru-open-jre_aarch64_linux_17.0.6_10_openj9-0.36.0.tar.gz';          ;;        ppc64el|ppc64le)          ESUM='f1342b0a8b472d2de6e882030d2797b9c37e1cd7a90e4cb0c3bd969d4cf8158c';          BINARY_URL='https://github.com/ibmruntimes/semeru17-binaries/releases/download/jdk-17.0.6%2B10_openj9-0.36.0/ibm-semeru-open-jre_ppc64le_linux_17.0.6_10_openj9-0.36.0.tar.gz';          ;;        amd64|x86_64)          ESUM='69ca1728f9aad7031908bd9a939b5a9a9c5e931d65bb5c72cbe6f599c7d00cc6';          BINARY_URL='https://github.com/ibmruntimes/semeru17-binaries/releases/download/jdk-17.0.6%2B10_openj9-0.36.0/ibm-semeru-open-jre_x64_linux_17.0.6_10_openj9-0.36.0.tar.gz';          ;;        s390x)          ESUM='542359aebfb91b6605c67db6523b2ce154bda63f7fa8a6c243944b2091f4eb2b';          BINARY_URL='https://github.com/ibmruntimes/semeru17-binaries/releases/download/jdk-17.0.6%2B10_openj9-0.36.0/ibm-semeru-open-jre_s390x_linux_17.0.6_10_openj9-0.36.0.tar.gz';          ;;        *)          echo "Unsupported arch: ${ARCH}";          exit 1;          ;;     esac;     curl -LfsSo /tmp/openjdk.tar.gz ${BINARY_URL};     echo "${ESUM} */tmp/openjdk.tar.gz" | sha256sum -c -;     mkdir -p /opt/java/openjdk;     cd /opt/java/openjdk;     tar -xf /tmp/openjdk.tar.gz --strip-components=1;     rm -rf /tmp/openjdk.tar.gz;
# Tue, 18 Apr 2023 01:50:45 GMT
ENV JAVA_HOME=/opt/java/openjdk PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 18 Apr 2023 01:50:45 GMT
ENV JAVA_TOOL_OPTIONS=-XX:+IgnoreUnrecognizedVMOptions -XX:+PortableSharedCache -XX:+IdleTuningGcOnIdle -Xshareclasses:name=openj9_system_scc,cacheDir=/opt/java/.scc,readonly,nonFatal
# Tue, 18 Apr 2023 01:51:21 GMT
RUN set -eux;     unset OPENJ9_JAVA_OPTIONS;     SCC_SIZE="50m";     DOWNLOAD_PATH_TOMCAT=/tmp/tomcat;     INSTALL_PATH_TOMCAT=/opt/tomcat-home;     TOMCAT_CHECKSUM="0db27185d9fc3174f2c670f814df3dda8a008b89d1a38a5d96cbbe119767ebfb1cf0bce956b27954aee9be19c4a7b91f2579d967932207976322033a86075f98";     TOMCAT_DWNLD_URL="https://archive.apache.org/dist/tomcat/tomcat-9/v9.0.35/bin/apache-tomcat-9.0.35.tar.gz";         mkdir -p "${DOWNLOAD_PATH_TOMCAT}" "${INSTALL_PATH_TOMCAT}";     curl -LfsSo "${DOWNLOAD_PATH_TOMCAT}"/tomcat.tar.gz "${TOMCAT_DWNLD_URL}";     echo "${TOMCAT_CHECKSUM} *${DOWNLOAD_PATH_TOMCAT}/tomcat.tar.gz" | sha512sum -c -;     tar -xf "${DOWNLOAD_PATH_TOMCAT}"/tomcat.tar.gz -C "${INSTALL_PATH_TOMCAT}" --strip-components=1;     rm -rf "${DOWNLOAD_PATH_TOMCAT}";         java -Xshareclasses:name=dry_run_scc,cacheDir=/opt/java/.scc,bootClassesOnly,nonFatal,createLayer -Xscmx$SCC_SIZE -version;     export OPENJ9_JAVA_OPTIONS="-Xshareclasses:name=dry_run_scc,cacheDir=/opt/java/.scc,bootClassesOnly,nonFatal";     "${INSTALL_PATH_TOMCAT}"/bin/startup.sh;     sleep 5;     "${INSTALL_PATH_TOMCAT}"/bin/shutdown.sh -force;     sleep 15;     FULL=$( (java -Xshareclasses:name=dry_run_scc,cacheDir=/opt/java/.scc,printallStats 2>&1 || true) | awk '/^Cache is [0-9.]*% .*full/ {print substr($3, 1, length($3)-1)}');     DST_CACHE=$(java -Xshareclasses:name=dry_run_scc,cacheDir=/opt/java/.scc,destroy 2>&1 || true);     SCC_SIZE=$(echo $SCC_SIZE | sed 's/.$//');     SCC_SIZE=$(awk "BEGIN {print int($SCC_SIZE * $FULL / 100.0)}");     [ "${SCC_SIZE}" -eq 0 ] && SCC_SIZE=1;     SCC_SIZE="${SCC_SIZE}m";     java -Xshareclasses:name=openj9_system_scc,cacheDir=/opt/java/.scc,bootClassesOnly,nonFatal,createLayer -Xscmx$SCC_SIZE -version;     unset OPENJ9_JAVA_OPTIONS;         export OPENJ9_JAVA_OPTIONS="-Xshareclasses:name=openj9_system_scc,cacheDir=/opt/java/.scc,bootClassesOnly,nonFatal";     "${INSTALL_PATH_TOMCAT}"/bin/startup.sh;     sleep 5;     "${INSTALL_PATH_TOMCAT}"/bin/shutdown.sh -force;     sleep 5;     FULL=$( (java -Xshareclasses:name=openj9_system_scc,cacheDir=/opt/java/.scc,printallStats 2>&1 || true) | awk '/^Cache is [0-9.]*% .*full/ {print substr($3, 1, length($3)-1)}');     echo "SCC layer is $FULL% full.";     rm -rf "${INSTALL_PATH_TOMCAT}";     if [ -d "/opt/java/.scc" ]; then           chmod -R 0777 /opt/java/.scc;     fi;         echo "SCC generation phase completed";
# Tue, 18 Apr 2023 06:56:20 GMT
ARG VERBOSE=false
# Tue, 18 Apr 2023 06:56:20 GMT
ARG OPENJ9_SCC=true
# Tue, 18 Apr 2023 06:56:20 GMT
ARG EN_SHA=366618db4b733337adc71ec30b1f33d36cf78a81858636360061036a926f373f
# Tue, 18 Apr 2023 06:56:20 GMT
ARG NON_IBM_SHA=d349f6ea3acd71910348904dd48f81940b86ca5f879737206ae37f858767ad0f
# Tue, 18 Apr 2023 06:56:21 GMT
ARG NOTICES_SHA=e7031658e09e2442279db72eed9238fb30d98c06dabb112fb21b8618b7e810ee
# Tue, 18 Apr 2023 06:56:21 GMT
LABEL org.opencontainers.image.authors=Chris Potter, Christy Jesuraj, Melissa Lee org.opencontainers.image.vendor=IBM org.opencontainers.image.url=http://wasdev.net org.opencontainers.image.documentation=https://www.ibm.com/support/knowledgecenter/SSAW57_liberty/com.ibm.websphere.wlp.nd.multiplatform.doc/ae/cwlp_about.html org.opencontainers.image.version=23.0.0.3 org.opencontainers.image.revision=cl230320230319-1900 org.opencontainers.image.description=This image contains the WebSphere Liberty runtime with IBM Semeru Runtime Open Edition OpenJDK with OpenJ9 and Ubuntu as the base OS.  For more information on this image please see https://github.com/WASdev/ci.docker#building-an-application-image org.opencontainers.image.title=IBM WebSphere Liberty
# Tue, 18 Apr 2023 06:56:21 GMT
ENV LIBERTY_VERSION=23.0.0_03
# Tue, 18 Apr 2023 06:56:21 GMT
ARG LIBERTY_URL
# Tue, 18 Apr 2023 06:56:21 GMT
ARG DOWNLOAD_OPTIONS=
# Tue, 18 Apr 2023 06:56:35 GMT
# ARGS: DOWNLOAD_OPTIONS= EN_SHA=366618db4b733337adc71ec30b1f33d36cf78a81858636360061036a926f373f NON_IBM_SHA=d349f6ea3acd71910348904dd48f81940b86ca5f879737206ae37f858767ad0f NOTICES_SHA=e7031658e09e2442279db72eed9238fb30d98c06dabb112fb21b8618b7e810ee OPENJ9_SCC=true VERBOSE=false
RUN apt-get update     && apt-get install -y --no-install-recommends unzip wget openssl     && rm -rf /var/lib/apt/lists/*     && mkdir -p /licenses/     && useradd -u 1001 -r -g 0 -s /usr/sbin/nologin default     && LIBERTY_URL=${LIBERTY_URL:-$(wget -q -O - https://public.dhe.ibm.com/ibmdl/export/pub/software/websphere/wasdev/downloads/wlp/index.yml  | grep $LIBERTY_VERSION -A 6 | sed -n 's/\s*kernel:\s//p' | tr -d '\r' )}      && wget $DOWNLOAD_OPTIONS $LIBERTY_URL -U UA-IBM-WebSphere-Liberty-Docker -O /tmp/wlp.zip     && unzip -q /tmp/wlp.zip -d /opt/ibm     && rm /tmp/wlp.zip     && chown -R 1001:0 /opt/ibm/wlp     && chmod -R g+rw /opt/ibm/wlp     && LICENSE_BASE=$(wget -q -O - https://public.dhe.ibm.com/ibmdl/export/pub/software/websphere/wasdev/downloads/wlp/index.yml  | grep $LIBERTY_VERSION -A 6 | sed -n 's/\s*license:\s//p' | sed 's/\(.*\)\/.*/\1\//' | tr -d '\r')     && wget ${LICENSE_BASE}en.html -U UA-IBM-WebSphere-Liberty-Docker -O /licenses/en.html     && wget ${LICENSE_BASE}non_ibm_license.html -U UA-IBM-WebSphere-Liberty-Docker -O /licenses/non_ibm_license.html     && wget ${LICENSE_BASE}notices.html -U UA-IBM-WebSphere-Liberty-Docker -O /licenses/notices.html     && echo "$EN_SHA /licenses/en.html" | sha256sum -c --strict --check     && echo "$NON_IBM_SHA /licenses/non_ibm_license.html" | sha256sum -c --strict --check     && echo "$NOTICES_SHA /licenses/notices.html" | sha256sum -c --strict --check     && apt-get purge --auto-remove -y unzip     && apt-get purge --auto-remove -y wget     && rm -rf /var/lib/apt/lists/*
# Tue, 18 Apr 2023 06:56:35 GMT
ENV PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/opt/ibm/wlp/bin:/opt/ibm/helpers/build
# Tue, 18 Apr 2023 06:56:35 GMT
LABEL ProductID=fbf6a96d49214c0abc6a3bc5da6e48cd ProductName=WebSphere Application Server Liberty ProductVersion=23.0.0.3 BuildLabel=cl230320230319-1900
# Tue, 18 Apr 2023 06:56:35 GMT
ENV LOG_DIR=/logs WLP_OUTPUT_DIR=/opt/ibm/wlp/output OPENJ9_SCC=true
# Tue, 18 Apr 2023 06:56:36 GMT
# ARGS: DOWNLOAD_OPTIONS= EN_SHA=366618db4b733337adc71ec30b1f33d36cf78a81858636360061036a926f373f NON_IBM_SHA=d349f6ea3acd71910348904dd48f81940b86ca5f879737206ae37f858767ad0f NOTICES_SHA=e7031658e09e2442279db72eed9238fb30d98c06dabb112fb21b8618b7e810ee VERBOSE=false
RUN /opt/ibm/wlp/bin/server create     && rm -rf $WLP_OUTPUT_DIR/.classCache /output/workarea
# Tue, 18 Apr 2023 06:56:36 GMT
COPY dir:0f3e336b1e5adb84a625050153035561e1c9802a57b7b90b5a17ebb82adba489 in /opt/ibm/helpers/ 
# Tue, 18 Apr 2023 06:56:36 GMT
COPY dir:1cf5cc2663c6235241a5228340a9c566587fe27b3e434a313debbf75dacd7a4b in /opt/ibm/fixes/ 
# Tue, 18 Apr 2023 06:56:37 GMT
# ARGS: DOWNLOAD_OPTIONS= EN_SHA=366618db4b733337adc71ec30b1f33d36cf78a81858636360061036a926f373f NON_IBM_SHA=d349f6ea3acd71910348904dd48f81940b86ca5f879737206ae37f858767ad0f NOTICES_SHA=e7031658e09e2442279db72eed9238fb30d98c06dabb112fb21b8618b7e810ee VERBOSE=false
RUN mkdir /logs     && mkdir /etc/wlp     && mkdir -p /opt/ibm/wlp/usr/shared/resources/lib.index.cache     && mkdir -p /home/default     && mkdir /output     && chmod -t /output     && rm -rf /output     && ln -s $WLP_OUTPUT_DIR/defaultServer /output     && ln -s /opt/ibm/wlp/usr/servers/defaultServer /config     && ln -s /opt/ibm /liberty     && ln -s /opt/ibm/wlp/usr/shared/resources/lib.index.cache /lib.index.cache     && mkdir -p /config/configDropins/defaults     && mkdir -p /config/configDropins/overrides     && chown -R 1001:0 /config     && chmod -R g+rw /config     && chown -R 1001:0 /opt/ibm/helpers     && chmod -R g+rwx /opt/ibm/helpers     && chown -R 1001:0 /opt/ibm/fixes     && chmod -R g+rwx /opt/ibm/fixes     && chown -R 1001:0 /opt/ibm/wlp/usr     && chmod -R g+rw /opt/ibm/wlp/usr     && chown -R 1001:0 /opt/ibm/wlp/output     && chmod -R g+rw /opt/ibm/wlp/output     && chown -R 1001:0 /logs     && chmod -R g+rw /logs     && chown -R 1001:0 /etc/wlp     && chmod -R g+rw /etc/wlp     && chown -R 1001:0 /home/default     && chmod -R g+rw /home/default
# Tue, 18 Apr 2023 06:56:43 GMT
# ARGS: DOWNLOAD_OPTIONS= EN_SHA=366618db4b733337adc71ec30b1f33d36cf78a81858636360061036a926f373f NON_IBM_SHA=d349f6ea3acd71910348904dd48f81940b86ca5f879737206ae37f858767ad0f NOTICES_SHA=e7031658e09e2442279db72eed9238fb30d98c06dabb112fb21b8618b7e810ee VERBOSE=false
RUN if [ "$OPENJ9_SCC" = "true" ]; then populate_scc.sh; fi     && rm -rf /output/messaging /output/resources/security /logs/* $WLP_OUTPUT_DIR/.classCache     && chown -R 1001:0 /opt/ibm/wlp/output     && chmod -R g+rwx /opt/ibm/wlp/output
# Tue, 18 Apr 2023 06:56:43 GMT
ENV RANDFILE=/tmp/.rnd OPENJ9_JAVA_OPTIONS=-XX:+IgnoreUnrecognizedVMOptions -XX:+IdleTuningGcOnIdle -Xshareclasses:name=openj9_system_scc,cacheDir=/opt/java/.scc,readonly,nonFatal -Dosgi.checkConfiguration=false
# Tue, 18 Apr 2023 06:56:43 GMT
USER 1001
# Tue, 18 Apr 2023 06:56:43 GMT
EXPOSE 9080 9443
# Tue, 18 Apr 2023 06:56:43 GMT
ENTRYPOINT ["/opt/ibm/helpers/runtime/docker-server.sh"]
# Tue, 18 Apr 2023 06:56:43 GMT
CMD ["/opt/ibm/wlp/bin/server" "run" "defaultServer"]
```

-	Layers:
	-	`sha256:99803d4b97f3db529ae9ca4174b0951afac6b309e7deaa8ec3214c584e02b3a8`  
		Last Modified: Thu, 13 Apr 2023 03:03:13 GMT  
		Size: 28.6 MB (28578563 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:59060db11c04ba6b24aa769f7968a1ff7e5c4029ff838bb2a0c95f83a0c318c2`  
		Last Modified: Tue, 18 Apr 2023 01:54:10 GMT  
		Size: 16.0 MB (16002795 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:54b69597426e81f23b8a8992f8d859f0723f65b1e2e137f9eb726f26d6f77147`  
		Last Modified: Tue, 18 Apr 2023 01:55:50 GMT  
		Size: 48.2 MB (48218475 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:be43806b8223fc6a690cd269fca157fa48e865925c5ca378aede4b0f4ea2dc93`  
		Last Modified: Tue, 18 Apr 2023 01:55:44 GMT  
		Size: 4.9 MB (4888324 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6d6f318471e416f3ce485f94c7d3e644fa45585facd1e63b56b92a5fa2fb67e7`  
		Last Modified: Tue, 18 Apr 2023 07:38:28 GMT  
		Size: 14.5 MB (14452469 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3a49ce11ae30bfde93a88ee868eb165c5b3964a424063477b0c29f1e73085ed6`  
		Last Modified: Tue, 18 Apr 2023 07:38:24 GMT  
		Size: 677.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0ddf222b06b40e13d454ffb6ca5834b4c76ec5b93937b2fdc3497516d6394226`  
		Last Modified: Tue, 18 Apr 2023 07:38:24 GMT  
		Size: 9.8 KB (9805 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f9d126caa6a2b2446e917cdd3dda88bb87ea3aeb639eaea49f61e0c57ab1d8d5`  
		Last Modified: Tue, 18 Apr 2023 07:38:24 GMT  
		Size: 270.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f7ea7677c1a46ee32d5bc4b6f60cdfc3f23fcce895f69287f6ff4b305821ec8d`  
		Last Modified: Tue, 18 Apr 2023 07:38:24 GMT  
		Size: 10.8 KB (10773 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:440d00998f38c344e81eff2479ef6973c756f2a6c3bb9be6010e779c60b2807a`  
		Last Modified: Tue, 18 Apr 2023 07:38:25 GMT  
		Size: 2.6 MB (2643433 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `websphere-liberty:kernel-java17-openj9` - linux; arm64 variant v8

```console
$ docker pull websphere-liberty@sha256:6fdd29ecb1af7e7a755db35f67f0653352ebd958767bb30aafbb85123ccb3e25
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **111.4 MB (111434621 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:eeb2a0e3a31c40382f0a7f1049aed20bf05be3945503a03d1882bb1b8f6e35c0`
-	Entrypoint: `["\/opt\/ibm\/helpers\/runtime\/docker-server.sh"]`
-	Default Command: `["\/opt\/ibm\/wlp\/bin\/server","run","defaultServer"]`

```dockerfile
# Thu, 13 Apr 2023 13:09:50 GMT
ARG RELEASE
# Thu, 13 Apr 2023 13:09:50 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Thu, 13 Apr 2023 13:09:50 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Thu, 13 Apr 2023 13:09:51 GMT
LABEL org.opencontainers.image.version=20.04
# Thu, 13 Apr 2023 13:09:59 GMT
ADD file:0150fa02321f8be160e90ff64583d263fe651b5d418ab65f05ba604449ab47c6 in / 
# Thu, 13 Apr 2023 13:10:00 GMT
CMD ["/bin/bash"]
# Tue, 18 Apr 2023 01:45:32 GMT
ENV LANG=en_US.UTF-8 LANGUAGE=en_US:en LC_ALL=en_US.UTF-8
# Tue, 18 Apr 2023 01:45:45 GMT
RUN apt-get update     && DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends tzdata curl ca-certificates fontconfig locales     && echo "en_US.UTF-8 UTF-8" >> /etc/locale.gen     && locale-gen en_US.UTF-8     && rm -rf /var/lib/apt/lists/*
# Tue, 18 Apr 2023 01:49:01 GMT
ENV JAVA_VERSION=jdk-17.0.6+10_openj9-0.36.0
# Tue, 18 Apr 2023 01:50:04 GMT
RUN set -eux;     ARCH="$(dpkg --print-architecture)";     case "${ARCH}" in        aarch64|arm64)          ESUM='492bd87e39fc0eb78218746e98c4c0f6730af9c998b872c1a175c0e907d11510';          BINARY_URL='https://github.com/ibmruntimes/semeru17-binaries/releases/download/jdk-17.0.6%2B10_openj9-0.36.0/ibm-semeru-open-jre_aarch64_linux_17.0.6_10_openj9-0.36.0.tar.gz';          ;;        ppc64el|ppc64le)          ESUM='f1342b0a8b472d2de6e882030d2797b9c37e1cd7a90e4cb0c3bd969d4cf8158c';          BINARY_URL='https://github.com/ibmruntimes/semeru17-binaries/releases/download/jdk-17.0.6%2B10_openj9-0.36.0/ibm-semeru-open-jre_ppc64le_linux_17.0.6_10_openj9-0.36.0.tar.gz';          ;;        amd64|x86_64)          ESUM='69ca1728f9aad7031908bd9a939b5a9a9c5e931d65bb5c72cbe6f599c7d00cc6';          BINARY_URL='https://github.com/ibmruntimes/semeru17-binaries/releases/download/jdk-17.0.6%2B10_openj9-0.36.0/ibm-semeru-open-jre_x64_linux_17.0.6_10_openj9-0.36.0.tar.gz';          ;;        s390x)          ESUM='542359aebfb91b6605c67db6523b2ce154bda63f7fa8a6c243944b2091f4eb2b';          BINARY_URL='https://github.com/ibmruntimes/semeru17-binaries/releases/download/jdk-17.0.6%2B10_openj9-0.36.0/ibm-semeru-open-jre_s390x_linux_17.0.6_10_openj9-0.36.0.tar.gz';          ;;        *)          echo "Unsupported arch: ${ARCH}";          exit 1;          ;;     esac;     curl -LfsSo /tmp/openjdk.tar.gz ${BINARY_URL};     echo "${ESUM} */tmp/openjdk.tar.gz" | sha256sum -c -;     mkdir -p /opt/java/openjdk;     cd /opt/java/openjdk;     tar -xf /tmp/openjdk.tar.gz --strip-components=1;     rm -rf /tmp/openjdk.tar.gz;
# Tue, 18 Apr 2023 01:50:04 GMT
ENV JAVA_HOME=/opt/java/openjdk PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 18 Apr 2023 01:50:05 GMT
ENV JAVA_TOOL_OPTIONS=-XX:+IgnoreUnrecognizedVMOptions -XX:+PortableSharedCache -XX:+IdleTuningGcOnIdle -Xshareclasses:name=openj9_system_scc,cacheDir=/opt/java/.scc,readonly,nonFatal
# Tue, 18 Apr 2023 01:50:39 GMT
RUN set -eux;     unset OPENJ9_JAVA_OPTIONS;     SCC_SIZE="50m";     DOWNLOAD_PATH_TOMCAT=/tmp/tomcat;     INSTALL_PATH_TOMCAT=/opt/tomcat-home;     TOMCAT_CHECKSUM="0db27185d9fc3174f2c670f814df3dda8a008b89d1a38a5d96cbbe119767ebfb1cf0bce956b27954aee9be19c4a7b91f2579d967932207976322033a86075f98";     TOMCAT_DWNLD_URL="https://archive.apache.org/dist/tomcat/tomcat-9/v9.0.35/bin/apache-tomcat-9.0.35.tar.gz";         mkdir -p "${DOWNLOAD_PATH_TOMCAT}" "${INSTALL_PATH_TOMCAT}";     curl -LfsSo "${DOWNLOAD_PATH_TOMCAT}"/tomcat.tar.gz "${TOMCAT_DWNLD_URL}";     echo "${TOMCAT_CHECKSUM} *${DOWNLOAD_PATH_TOMCAT}/tomcat.tar.gz" | sha512sum -c -;     tar -xf "${DOWNLOAD_PATH_TOMCAT}"/tomcat.tar.gz -C "${INSTALL_PATH_TOMCAT}" --strip-components=1;     rm -rf "${DOWNLOAD_PATH_TOMCAT}";         java -Xshareclasses:name=dry_run_scc,cacheDir=/opt/java/.scc,bootClassesOnly,nonFatal,createLayer -Xscmx$SCC_SIZE -version;     export OPENJ9_JAVA_OPTIONS="-Xshareclasses:name=dry_run_scc,cacheDir=/opt/java/.scc,bootClassesOnly,nonFatal";     "${INSTALL_PATH_TOMCAT}"/bin/startup.sh;     sleep 5;     "${INSTALL_PATH_TOMCAT}"/bin/shutdown.sh -force;     sleep 15;     FULL=$( (java -Xshareclasses:name=dry_run_scc,cacheDir=/opt/java/.scc,printallStats 2>&1 || true) | awk '/^Cache is [0-9.]*% .*full/ {print substr($3, 1, length($3)-1)}');     DST_CACHE=$(java -Xshareclasses:name=dry_run_scc,cacheDir=/opt/java/.scc,destroy 2>&1 || true);     SCC_SIZE=$(echo $SCC_SIZE | sed 's/.$//');     SCC_SIZE=$(awk "BEGIN {print int($SCC_SIZE * $FULL / 100.0)}");     [ "${SCC_SIZE}" -eq 0 ] && SCC_SIZE=1;     SCC_SIZE="${SCC_SIZE}m";     java -Xshareclasses:name=openj9_system_scc,cacheDir=/opt/java/.scc,bootClassesOnly,nonFatal,createLayer -Xscmx$SCC_SIZE -version;     unset OPENJ9_JAVA_OPTIONS;         export OPENJ9_JAVA_OPTIONS="-Xshareclasses:name=openj9_system_scc,cacheDir=/opt/java/.scc,bootClassesOnly,nonFatal";     "${INSTALL_PATH_TOMCAT}"/bin/startup.sh;     sleep 5;     "${INSTALL_PATH_TOMCAT}"/bin/shutdown.sh -force;     sleep 5;     FULL=$( (java -Xshareclasses:name=openj9_system_scc,cacheDir=/opt/java/.scc,printallStats 2>&1 || true) | awk '/^Cache is [0-9.]*% .*full/ {print substr($3, 1, length($3)-1)}');     echo "SCC layer is $FULL% full.";     rm -rf "${INSTALL_PATH_TOMCAT}";     if [ -d "/opt/java/.scc" ]; then           chmod -R 0777 /opt/java/.scc;     fi;         echo "SCC generation phase completed";
# Thu, 04 May 2023 09:01:06 GMT
ARG VERBOSE=false
# Thu, 04 May 2023 09:01:06 GMT
ARG OPENJ9_SCC=true
# Thu, 04 May 2023 09:01:06 GMT
ARG EN_SHA=d7580938d35387110e39c3c8b3bb5c1f8dc9f0418a2f77799dbcf69a2ab63093
# Thu, 04 May 2023 09:01:06 GMT
ARG NON_IBM_SHA=0d97a3e5cf5403a9b3be514509977f4e9be4a2ac4258e692ef8e64761910f4c0
# Thu, 04 May 2023 09:01:06 GMT
ARG NOTICES_SHA=71f58dc38b4c9b60beaec4459b97b0d08228ad8e5fe5e3a0f4fd7e7c66285925
# Thu, 04 May 2023 09:01:06 GMT
LABEL org.opencontainers.image.authors=Chris Potter, Christy Jesuraj, Melissa Lee org.opencontainers.image.vendor=IBM org.opencontainers.image.url=http://wasdev.net org.opencontainers.image.documentation=https://www.ibm.com/support/knowledgecenter/SSAW57_liberty/com.ibm.websphere.wlp.nd.multiplatform.doc/ae/cwlp_about.html org.opencontainers.image.version=23.0.0.4 org.opencontainers.image.revision=cl230420230418-0035 org.opencontainers.image.description=This image contains the WebSphere Liberty runtime with IBM Semeru Runtime Open Edition OpenJDK with OpenJ9 and Ubuntu as the base OS.  For more information on this image please see https://github.com/WASdev/ci.docker#building-an-application-image org.opencontainers.image.title=IBM WebSphere Liberty
# Thu, 04 May 2023 09:01:07 GMT
ENV LIBERTY_VERSION=23.0.0_04
# Thu, 04 May 2023 09:01:07 GMT
ARG LIBERTY_URL
# Thu, 04 May 2023 09:01:07 GMT
ARG DOWNLOAD_OPTIONS=
# Thu, 04 May 2023 09:01:19 GMT
# ARGS: DOWNLOAD_OPTIONS= EN_SHA=d7580938d35387110e39c3c8b3bb5c1f8dc9f0418a2f77799dbcf69a2ab63093 NON_IBM_SHA=0d97a3e5cf5403a9b3be514509977f4e9be4a2ac4258e692ef8e64761910f4c0 NOTICES_SHA=71f58dc38b4c9b60beaec4459b97b0d08228ad8e5fe5e3a0f4fd7e7c66285925 OPENJ9_SCC=true VERBOSE=false
RUN apt-get update     && apt-get install -y --no-install-recommends unzip wget openssl     && rm -rf /var/lib/apt/lists/*     && mkdir -p /licenses/     && useradd -u 1001 -r -g 0 -s /usr/sbin/nologin default     && LIBERTY_URL=${LIBERTY_URL:-$(wget -q -O - https://public.dhe.ibm.com/ibmdl/export/pub/software/websphere/wasdev/downloads/wlp/index.yml  | grep $LIBERTY_VERSION -A 6 | sed -n 's/\s*kernel:\s//p' | tr -d '\r' )}      && wget $DOWNLOAD_OPTIONS $LIBERTY_URL -U UA-IBM-WebSphere-Liberty-Docker -O /tmp/wlp.zip     && unzip -q /tmp/wlp.zip -d /opt/ibm     && rm /tmp/wlp.zip     && chown -R 1001:0 /opt/ibm/wlp     && chmod -R g+rw /opt/ibm/wlp     && LICENSE_BASE=$(wget -q -O - https://public.dhe.ibm.com/ibmdl/export/pub/software/websphere/wasdev/downloads/wlp/index.yml  | grep $LIBERTY_VERSION -A 6 | sed -n 's/\s*license:\s//p' | sed 's/\(.*\)\/.*/\1\//' | tr -d '\r')     && wget ${LICENSE_BASE}en.html -U UA-IBM-WebSphere-Liberty-Docker -O /licenses/en.html     && wget ${LICENSE_BASE}non_ibm_license.html -U UA-IBM-WebSphere-Liberty-Docker -O /licenses/non_ibm_license.html     && wget ${LICENSE_BASE}notices.html -U UA-IBM-WebSphere-Liberty-Docker -O /licenses/notices.html     && echo "$EN_SHA /licenses/en.html" | sha256sum -c --strict --check     && echo "$NON_IBM_SHA /licenses/non_ibm_license.html" | sha256sum -c --strict --check     && echo "$NOTICES_SHA /licenses/notices.html" | sha256sum -c --strict --check     && apt-get purge --auto-remove -y unzip     && apt-get purge --auto-remove -y wget     && rm -rf /var/lib/apt/lists/*
# Thu, 04 May 2023 09:01:19 GMT
ENV PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/opt/ibm/wlp/bin:/opt/ibm/helpers/build
# Thu, 04 May 2023 09:01:19 GMT
LABEL ProductID=fbf6a96d49214c0abc6a3bc5da6e48cd ProductName=WebSphere Application Server Liberty ProductVersion=23.0.0.4 BuildLabel=cl230420230418-0035
# Thu, 04 May 2023 09:01:19 GMT
ENV LOG_DIR=/logs WLP_OUTPUT_DIR=/opt/ibm/wlp/output OPENJ9_SCC=true
# Thu, 04 May 2023 09:01:19 GMT
# ARGS: DOWNLOAD_OPTIONS= EN_SHA=d7580938d35387110e39c3c8b3bb5c1f8dc9f0418a2f77799dbcf69a2ab63093 NON_IBM_SHA=0d97a3e5cf5403a9b3be514509977f4e9be4a2ac4258e692ef8e64761910f4c0 NOTICES_SHA=71f58dc38b4c9b60beaec4459b97b0d08228ad8e5fe5e3a0f4fd7e7c66285925 VERBOSE=false
RUN /opt/ibm/wlp/bin/server create     && rm -rf $WLP_OUTPUT_DIR/.classCache /output/workarea
# Thu, 04 May 2023 09:01:20 GMT
COPY dir:0f3e336b1e5adb84a625050153035561e1c9802a57b7b90b5a17ebb82adba489 in /opt/ibm/helpers/ 
# Thu, 04 May 2023 09:01:20 GMT
COPY dir:1cf5cc2663c6235241a5228340a9c566587fe27b3e434a313debbf75dacd7a4b in /opt/ibm/fixes/ 
# Thu, 04 May 2023 09:01:20 GMT
# ARGS: DOWNLOAD_OPTIONS= EN_SHA=d7580938d35387110e39c3c8b3bb5c1f8dc9f0418a2f77799dbcf69a2ab63093 NON_IBM_SHA=0d97a3e5cf5403a9b3be514509977f4e9be4a2ac4258e692ef8e64761910f4c0 NOTICES_SHA=71f58dc38b4c9b60beaec4459b97b0d08228ad8e5fe5e3a0f4fd7e7c66285925 VERBOSE=false
RUN mkdir /logs     && mkdir /etc/wlp     && mkdir -p /opt/ibm/wlp/usr/shared/resources/lib.index.cache     && mkdir -p /home/default     && mkdir /output     && chmod -t /output     && rm -rf /output     && ln -s $WLP_OUTPUT_DIR/defaultServer /output     && ln -s /opt/ibm/wlp/usr/servers/defaultServer /config     && ln -s /opt/ibm /liberty     && ln -s /opt/ibm/wlp/usr/shared/resources/lib.index.cache /lib.index.cache     && mkdir -p /config/configDropins/defaults     && mkdir -p /config/configDropins/overrides     && chown -R 1001:0 /config     && chmod -R g+rw /config     && chown -R 1001:0 /opt/ibm/helpers     && chmod -R g+rwx /opt/ibm/helpers     && chown -R 1001:0 /opt/ibm/fixes     && chmod -R g+rwx /opt/ibm/fixes     && chown -R 1001:0 /opt/ibm/wlp/usr     && chmod -R g+rw /opt/ibm/wlp/usr     && chown -R 1001:0 /opt/ibm/wlp/output     && chmod -R g+rw /opt/ibm/wlp/output     && chown -R 1001:0 /logs     && chmod -R g+rw /logs     && chown -R 1001:0 /etc/wlp     && chmod -R g+rw /etc/wlp     && chown -R 1001:0 /home/default     && chmod -R g+rw /home/default
# Thu, 04 May 2023 09:01:24 GMT
# ARGS: DOWNLOAD_OPTIONS= EN_SHA=d7580938d35387110e39c3c8b3bb5c1f8dc9f0418a2f77799dbcf69a2ab63093 NON_IBM_SHA=0d97a3e5cf5403a9b3be514509977f4e9be4a2ac4258e692ef8e64761910f4c0 NOTICES_SHA=71f58dc38b4c9b60beaec4459b97b0d08228ad8e5fe5e3a0f4fd7e7c66285925 VERBOSE=false
RUN if [ "$OPENJ9_SCC" = "true" ]; then populate_scc.sh; fi     && rm -rf /output/messaging /output/resources/security /logs/* $WLP_OUTPUT_DIR/.classCache     && chown -R 1001:0 /opt/ibm/wlp/output     && chmod -R g+rwx /opt/ibm/wlp/output
# Thu, 04 May 2023 09:01:25 GMT
ENV RANDFILE=/tmp/.rnd OPENJ9_JAVA_OPTIONS=-XX:+IgnoreUnrecognizedVMOptions -XX:+IdleTuningGcOnIdle -Xshareclasses:name=openj9_system_scc,cacheDir=/opt/java/.scc,readonly,nonFatal -Dosgi.checkConfiguration=false
# Thu, 04 May 2023 09:01:25 GMT
USER 1001
# Thu, 04 May 2023 09:01:25 GMT
EXPOSE 9080 9443
# Thu, 04 May 2023 09:01:25 GMT
ENTRYPOINT ["/opt/ibm/helpers/runtime/docker-server.sh"]
# Thu, 04 May 2023 09:01:25 GMT
CMD ["/opt/ibm/wlp/bin/server" "run" "defaultServer"]
```

-	Layers:
	-	`sha256:2378679266ac5157323158b6e52e7a884e559db5217037e57992e47a1667d525`  
		Last Modified: Fri, 14 Apr 2023 07:39:20 GMT  
		Size: 27.2 MB (27196396 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7751d4fbf2062d96159da55aa2a9331cd03b66d2d7a5bae5db82dd2693de8cb5`  
		Last Modified: Tue, 18 Apr 2023 01:53:16 GMT  
		Size: 15.9 MB (15865841 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:14cf99bcb696e2b3db477787e19cc4caba82db9c1e06c71d69bfda8bba8aa59a`  
		Last Modified: Tue, 18 Apr 2023 01:54:44 GMT  
		Size: 46.4 MB (46435138 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:450dadaefa25ce9d71bdc68815bd7473c5819574c61531ed7796c0aac8dd85a0`  
		Last Modified: Tue, 18 Apr 2023 01:54:39 GMT  
		Size: 4.6 MB (4576737 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0f33a03ff0fc6855e27d4aad8426841e3d3975b65f4b37645394edf462241f30`  
		Last Modified: Thu, 04 May 2023 09:59:48 GMT  
		Size: 14.7 MB (14749576 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e37eee167486d44d8824b6690f2765ff0ba0b006ca3f169cd6cc70c5dc131afe`  
		Last Modified: Thu, 04 May 2023 09:59:45 GMT  
		Size: 675.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e7511526f8105db7a339e2f0b61838746d72610aa9f0bdcd792feea98f021c06`  
		Last Modified: Thu, 04 May 2023 09:59:46 GMT  
		Size: 9.8 KB (9817 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:384b07c1fd643dd853357960f845ed52ade3e2c5806cc3394fa9d6d875894c21`  
		Last Modified: Thu, 04 May 2023 09:59:45 GMT  
		Size: 271.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1859c7ddb3e416e8040fb8140db1bbcded904d82071d6c6793ed98c54a19d6aa`  
		Last Modified: Thu, 04 May 2023 09:59:45 GMT  
		Size: 10.8 KB (10794 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:007348b41b44b52152cfbfb82a7e330a753574bbc8e5fd0edd372d2f25b70458`  
		Last Modified: Thu, 04 May 2023 09:59:46 GMT  
		Size: 2.6 MB (2589376 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `websphere-liberty:kernel-java17-openj9` - linux; ppc64le

```console
$ docker pull websphere-liberty@sha256:f765e7f85f742f2344ae64cb6ebaf649946fadfc2a39ca229ab8948f913a06c3
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **120.6 MB (120608970 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:8fdb443741798f66357db774b4e5543ef12785f25ed9188de98ce21bbe88d922`
-	Entrypoint: `["\/opt\/ibm\/helpers\/runtime\/docker-server.sh"]`
-	Default Command: `["\/opt\/ibm\/wlp\/bin\/server","run","defaultServer"]`

```dockerfile
# Thu, 13 Apr 2023 13:09:36 GMT
ARG RELEASE
# Thu, 13 Apr 2023 13:09:37 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Thu, 13 Apr 2023 13:09:37 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Thu, 13 Apr 2023 13:09:37 GMT
LABEL org.opencontainers.image.version=20.04
# Thu, 13 Apr 2023 13:09:40 GMT
ADD file:faba3891f58656ec753ba6ca4b63e7c1f27bcd236b665634b05d5bc1b1ceee0a in / 
# Thu, 13 Apr 2023 13:09:40 GMT
CMD ["/bin/bash"]
# Tue, 18 Apr 2023 01:24:54 GMT
ENV LANG=en_US.UTF-8 LANGUAGE=en_US:en LC_ALL=en_US.UTF-8
# Tue, 18 Apr 2023 01:25:21 GMT
RUN apt-get update     && DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends tzdata curl ca-certificates fontconfig locales     && echo "en_US.UTF-8 UTF-8" >> /etc/locale.gen     && locale-gen en_US.UTF-8     && rm -rf /var/lib/apt/lists/*
# Tue, 18 Apr 2023 01:29:26 GMT
ENV JAVA_VERSION=jdk-17.0.6+10_openj9-0.36.0
# Tue, 18 Apr 2023 01:30:46 GMT
RUN set -eux;     ARCH="$(dpkg --print-architecture)";     case "${ARCH}" in        aarch64|arm64)          ESUM='492bd87e39fc0eb78218746e98c4c0f6730af9c998b872c1a175c0e907d11510';          BINARY_URL='https://github.com/ibmruntimes/semeru17-binaries/releases/download/jdk-17.0.6%2B10_openj9-0.36.0/ibm-semeru-open-jre_aarch64_linux_17.0.6_10_openj9-0.36.0.tar.gz';          ;;        ppc64el|ppc64le)          ESUM='f1342b0a8b472d2de6e882030d2797b9c37e1cd7a90e4cb0c3bd969d4cf8158c';          BINARY_URL='https://github.com/ibmruntimes/semeru17-binaries/releases/download/jdk-17.0.6%2B10_openj9-0.36.0/ibm-semeru-open-jre_ppc64le_linux_17.0.6_10_openj9-0.36.0.tar.gz';          ;;        amd64|x86_64)          ESUM='69ca1728f9aad7031908bd9a939b5a9a9c5e931d65bb5c72cbe6f599c7d00cc6';          BINARY_URL='https://github.com/ibmruntimes/semeru17-binaries/releases/download/jdk-17.0.6%2B10_openj9-0.36.0/ibm-semeru-open-jre_x64_linux_17.0.6_10_openj9-0.36.0.tar.gz';          ;;        s390x)          ESUM='542359aebfb91b6605c67db6523b2ce154bda63f7fa8a6c243944b2091f4eb2b';          BINARY_URL='https://github.com/ibmruntimes/semeru17-binaries/releases/download/jdk-17.0.6%2B10_openj9-0.36.0/ibm-semeru-open-jre_s390x_linux_17.0.6_10_openj9-0.36.0.tar.gz';          ;;        *)          echo "Unsupported arch: ${ARCH}";          exit 1;          ;;     esac;     curl -LfsSo /tmp/openjdk.tar.gz ${BINARY_URL};     echo "${ESUM} */tmp/openjdk.tar.gz" | sha256sum -c -;     mkdir -p /opt/java/openjdk;     cd /opt/java/openjdk;     tar -xf /tmp/openjdk.tar.gz --strip-components=1;     rm -rf /tmp/openjdk.tar.gz;
# Tue, 18 Apr 2023 01:30:48 GMT
ENV JAVA_HOME=/opt/java/openjdk PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 18 Apr 2023 01:30:48 GMT
ENV JAVA_TOOL_OPTIONS=-XX:+IgnoreUnrecognizedVMOptions -XX:+PortableSharedCache -XX:+IdleTuningGcOnIdle -Xshareclasses:name=openj9_system_scc,cacheDir=/opt/java/.scc,readonly,nonFatal
# Tue, 18 Apr 2023 01:31:26 GMT
RUN set -eux;     unset OPENJ9_JAVA_OPTIONS;     SCC_SIZE="50m";     DOWNLOAD_PATH_TOMCAT=/tmp/tomcat;     INSTALL_PATH_TOMCAT=/opt/tomcat-home;     TOMCAT_CHECKSUM="0db27185d9fc3174f2c670f814df3dda8a008b89d1a38a5d96cbbe119767ebfb1cf0bce956b27954aee9be19c4a7b91f2579d967932207976322033a86075f98";     TOMCAT_DWNLD_URL="https://archive.apache.org/dist/tomcat/tomcat-9/v9.0.35/bin/apache-tomcat-9.0.35.tar.gz";         mkdir -p "${DOWNLOAD_PATH_TOMCAT}" "${INSTALL_PATH_TOMCAT}";     curl -LfsSo "${DOWNLOAD_PATH_TOMCAT}"/tomcat.tar.gz "${TOMCAT_DWNLD_URL}";     echo "${TOMCAT_CHECKSUM} *${DOWNLOAD_PATH_TOMCAT}/tomcat.tar.gz" | sha512sum -c -;     tar -xf "${DOWNLOAD_PATH_TOMCAT}"/tomcat.tar.gz -C "${INSTALL_PATH_TOMCAT}" --strip-components=1;     rm -rf "${DOWNLOAD_PATH_TOMCAT}";         java -Xshareclasses:name=dry_run_scc,cacheDir=/opt/java/.scc,bootClassesOnly,nonFatal,createLayer -Xscmx$SCC_SIZE -version;     export OPENJ9_JAVA_OPTIONS="-Xshareclasses:name=dry_run_scc,cacheDir=/opt/java/.scc,bootClassesOnly,nonFatal";     "${INSTALL_PATH_TOMCAT}"/bin/startup.sh;     sleep 5;     "${INSTALL_PATH_TOMCAT}"/bin/shutdown.sh -force;     sleep 15;     FULL=$( (java -Xshareclasses:name=dry_run_scc,cacheDir=/opt/java/.scc,printallStats 2>&1 || true) | awk '/^Cache is [0-9.]*% .*full/ {print substr($3, 1, length($3)-1)}');     DST_CACHE=$(java -Xshareclasses:name=dry_run_scc,cacheDir=/opt/java/.scc,destroy 2>&1 || true);     SCC_SIZE=$(echo $SCC_SIZE | sed 's/.$//');     SCC_SIZE=$(awk "BEGIN {print int($SCC_SIZE * $FULL / 100.0)}");     [ "${SCC_SIZE}" -eq 0 ] && SCC_SIZE=1;     SCC_SIZE="${SCC_SIZE}m";     java -Xshareclasses:name=openj9_system_scc,cacheDir=/opt/java/.scc,bootClassesOnly,nonFatal,createLayer -Xscmx$SCC_SIZE -version;     unset OPENJ9_JAVA_OPTIONS;         export OPENJ9_JAVA_OPTIONS="-Xshareclasses:name=openj9_system_scc,cacheDir=/opt/java/.scc,bootClassesOnly,nonFatal";     "${INSTALL_PATH_TOMCAT}"/bin/startup.sh;     sleep 5;     "${INSTALL_PATH_TOMCAT}"/bin/shutdown.sh -force;     sleep 5;     FULL=$( (java -Xshareclasses:name=openj9_system_scc,cacheDir=/opt/java/.scc,printallStats 2>&1 || true) | awk '/^Cache is [0-9.]*% .*full/ {print substr($3, 1, length($3)-1)}');     echo "SCC layer is $FULL% full.";     rm -rf "${INSTALL_PATH_TOMCAT}";     if [ -d "/opt/java/.scc" ]; then           chmod -R 0777 /opt/java/.scc;     fi;         echo "SCC generation phase completed";
# Tue, 18 Apr 2023 03:23:00 GMT
ARG VERBOSE=false
# Tue, 18 Apr 2023 03:23:00 GMT
ARG OPENJ9_SCC=true
# Tue, 18 Apr 2023 03:23:00 GMT
ARG EN_SHA=366618db4b733337adc71ec30b1f33d36cf78a81858636360061036a926f373f
# Tue, 18 Apr 2023 03:23:00 GMT
ARG NON_IBM_SHA=d349f6ea3acd71910348904dd48f81940b86ca5f879737206ae37f858767ad0f
# Tue, 18 Apr 2023 03:23:01 GMT
ARG NOTICES_SHA=e7031658e09e2442279db72eed9238fb30d98c06dabb112fb21b8618b7e810ee
# Tue, 18 Apr 2023 03:23:01 GMT
LABEL org.opencontainers.image.authors=Chris Potter, Christy Jesuraj, Melissa Lee org.opencontainers.image.vendor=IBM org.opencontainers.image.url=http://wasdev.net org.opencontainers.image.documentation=https://www.ibm.com/support/knowledgecenter/SSAW57_liberty/com.ibm.websphere.wlp.nd.multiplatform.doc/ae/cwlp_about.html org.opencontainers.image.version=23.0.0.3 org.opencontainers.image.revision=cl230320230319-1900 org.opencontainers.image.description=This image contains the WebSphere Liberty runtime with IBM Semeru Runtime Open Edition OpenJDK with OpenJ9 and Ubuntu as the base OS.  For more information on this image please see https://github.com/WASdev/ci.docker#building-an-application-image org.opencontainers.image.title=IBM WebSphere Liberty
# Tue, 18 Apr 2023 03:23:01 GMT
ENV LIBERTY_VERSION=23.0.0_03
# Tue, 18 Apr 2023 03:23:01 GMT
ARG LIBERTY_URL
# Tue, 18 Apr 2023 03:23:02 GMT
ARG DOWNLOAD_OPTIONS=
# Tue, 18 Apr 2023 03:23:40 GMT
# ARGS: DOWNLOAD_OPTIONS= EN_SHA=366618db4b733337adc71ec30b1f33d36cf78a81858636360061036a926f373f NON_IBM_SHA=d349f6ea3acd71910348904dd48f81940b86ca5f879737206ae37f858767ad0f NOTICES_SHA=e7031658e09e2442279db72eed9238fb30d98c06dabb112fb21b8618b7e810ee OPENJ9_SCC=true VERBOSE=false
RUN apt-get update     && apt-get install -y --no-install-recommends unzip wget openssl     && rm -rf /var/lib/apt/lists/*     && mkdir -p /licenses/     && useradd -u 1001 -r -g 0 -s /usr/sbin/nologin default     && LIBERTY_URL=${LIBERTY_URL:-$(wget -q -O - https://public.dhe.ibm.com/ibmdl/export/pub/software/websphere/wasdev/downloads/wlp/index.yml  | grep $LIBERTY_VERSION -A 6 | sed -n 's/\s*kernel:\s//p' | tr -d '\r' )}      && wget $DOWNLOAD_OPTIONS $LIBERTY_URL -U UA-IBM-WebSphere-Liberty-Docker -O /tmp/wlp.zip     && unzip -q /tmp/wlp.zip -d /opt/ibm     && rm /tmp/wlp.zip     && chown -R 1001:0 /opt/ibm/wlp     && chmod -R g+rw /opt/ibm/wlp     && LICENSE_BASE=$(wget -q -O - https://public.dhe.ibm.com/ibmdl/export/pub/software/websphere/wasdev/downloads/wlp/index.yml  | grep $LIBERTY_VERSION -A 6 | sed -n 's/\s*license:\s//p' | sed 's/\(.*\)\/.*/\1\//' | tr -d '\r')     && wget ${LICENSE_BASE}en.html -U UA-IBM-WebSphere-Liberty-Docker -O /licenses/en.html     && wget ${LICENSE_BASE}non_ibm_license.html -U UA-IBM-WebSphere-Liberty-Docker -O /licenses/non_ibm_license.html     && wget ${LICENSE_BASE}notices.html -U UA-IBM-WebSphere-Liberty-Docker -O /licenses/notices.html     && echo "$EN_SHA /licenses/en.html" | sha256sum -c --strict --check     && echo "$NON_IBM_SHA /licenses/non_ibm_license.html" | sha256sum -c --strict --check     && echo "$NOTICES_SHA /licenses/notices.html" | sha256sum -c --strict --check     && apt-get purge --auto-remove -y unzip     && apt-get purge --auto-remove -y wget     && rm -rf /var/lib/apt/lists/*
# Tue, 18 Apr 2023 03:23:40 GMT
ENV PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/opt/ibm/wlp/bin:/opt/ibm/helpers/build
# Tue, 18 Apr 2023 03:23:41 GMT
LABEL ProductID=fbf6a96d49214c0abc6a3bc5da6e48cd ProductName=WebSphere Application Server Liberty ProductVersion=23.0.0.3 BuildLabel=cl230320230319-1900
# Tue, 18 Apr 2023 03:23:41 GMT
ENV LOG_DIR=/logs WLP_OUTPUT_DIR=/opt/ibm/wlp/output OPENJ9_SCC=true
# Tue, 18 Apr 2023 03:23:42 GMT
# ARGS: DOWNLOAD_OPTIONS= EN_SHA=366618db4b733337adc71ec30b1f33d36cf78a81858636360061036a926f373f NON_IBM_SHA=d349f6ea3acd71910348904dd48f81940b86ca5f879737206ae37f858767ad0f NOTICES_SHA=e7031658e09e2442279db72eed9238fb30d98c06dabb112fb21b8618b7e810ee VERBOSE=false
RUN /opt/ibm/wlp/bin/server create     && rm -rf $WLP_OUTPUT_DIR/.classCache /output/workarea
# Tue, 18 Apr 2023 03:23:43 GMT
COPY dir:0f3e336b1e5adb84a625050153035561e1c9802a57b7b90b5a17ebb82adba489 in /opt/ibm/helpers/ 
# Tue, 18 Apr 2023 03:23:43 GMT
COPY dir:1cf5cc2663c6235241a5228340a9c566587fe27b3e434a313debbf75dacd7a4b in /opt/ibm/fixes/ 
# Tue, 18 Apr 2023 03:23:44 GMT
# ARGS: DOWNLOAD_OPTIONS= EN_SHA=366618db4b733337adc71ec30b1f33d36cf78a81858636360061036a926f373f NON_IBM_SHA=d349f6ea3acd71910348904dd48f81940b86ca5f879737206ae37f858767ad0f NOTICES_SHA=e7031658e09e2442279db72eed9238fb30d98c06dabb112fb21b8618b7e810ee VERBOSE=false
RUN mkdir /logs     && mkdir /etc/wlp     && mkdir -p /opt/ibm/wlp/usr/shared/resources/lib.index.cache     && mkdir -p /home/default     && mkdir /output     && chmod -t /output     && rm -rf /output     && ln -s $WLP_OUTPUT_DIR/defaultServer /output     && ln -s /opt/ibm/wlp/usr/servers/defaultServer /config     && ln -s /opt/ibm /liberty     && ln -s /opt/ibm/wlp/usr/shared/resources/lib.index.cache /lib.index.cache     && mkdir -p /config/configDropins/defaults     && mkdir -p /config/configDropins/overrides     && chown -R 1001:0 /config     && chmod -R g+rw /config     && chown -R 1001:0 /opt/ibm/helpers     && chmod -R g+rwx /opt/ibm/helpers     && chown -R 1001:0 /opt/ibm/fixes     && chmod -R g+rwx /opt/ibm/fixes     && chown -R 1001:0 /opt/ibm/wlp/usr     && chmod -R g+rw /opt/ibm/wlp/usr     && chown -R 1001:0 /opt/ibm/wlp/output     && chmod -R g+rw /opt/ibm/wlp/output     && chown -R 1001:0 /logs     && chmod -R g+rw /logs     && chown -R 1001:0 /etc/wlp     && chmod -R g+rw /etc/wlp     && chown -R 1001:0 /home/default     && chmod -R g+rw /home/default
# Tue, 18 Apr 2023 03:23:55 GMT
# ARGS: DOWNLOAD_OPTIONS= EN_SHA=366618db4b733337adc71ec30b1f33d36cf78a81858636360061036a926f373f NON_IBM_SHA=d349f6ea3acd71910348904dd48f81940b86ca5f879737206ae37f858767ad0f NOTICES_SHA=e7031658e09e2442279db72eed9238fb30d98c06dabb112fb21b8618b7e810ee VERBOSE=false
RUN if [ "$OPENJ9_SCC" = "true" ]; then populate_scc.sh; fi     && rm -rf /output/messaging /output/resources/security /logs/* $WLP_OUTPUT_DIR/.classCache     && chown -R 1001:0 /opt/ibm/wlp/output     && chmod -R g+rwx /opt/ibm/wlp/output
# Tue, 18 Apr 2023 03:23:56 GMT
ENV RANDFILE=/tmp/.rnd OPENJ9_JAVA_OPTIONS=-XX:+IgnoreUnrecognizedVMOptions -XX:+IdleTuningGcOnIdle -Xshareclasses:name=openj9_system_scc,cacheDir=/opt/java/.scc,readonly,nonFatal -Dosgi.checkConfiguration=false
# Tue, 18 Apr 2023 03:23:56 GMT
USER 1001
# Tue, 18 Apr 2023 03:23:56 GMT
EXPOSE 9080 9443
# Tue, 18 Apr 2023 03:23:57 GMT
ENTRYPOINT ["/opt/ibm/helpers/runtime/docker-server.sh"]
# Tue, 18 Apr 2023 03:23:57 GMT
CMD ["/opt/ibm/wlp/bin/server" "run" "defaultServer"]
```

-	Layers:
	-	`sha256:d276072145993a42aed3e2b3e8cd26b6e08aab266d9c9d792ee89b26150681da`  
		Last Modified: Fri, 14 Apr 2023 09:36:00 GMT  
		Size: 33.3 MB (33300980 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4a328f93092ceadb7a1b931cc278addf4dfae1321b9f8ced8d4ea73dc90facfb`  
		Last Modified: Tue, 18 Apr 2023 01:34:37 GMT  
		Size: 17.2 MB (17176898 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5cc4fe87f3e1ae2088dbb6c1d240f2210894fcfc5f16fc53893a903ceb8e8ca2`  
		Last Modified: Tue, 18 Apr 2023 01:37:05 GMT  
		Size: 49.3 MB (49325137 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:788f22ea43e560dcd86481b6db76e207091483f89d2d61dd6eacac91dda99a38`  
		Last Modified: Tue, 18 Apr 2023 01:36:53 GMT  
		Size: 3.8 MB (3761938 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c0076ae43b1a928ce2fbf5e2ab5f0d6fa23e0a76248ce35afd5cf92a820f1a73`  
		Last Modified: Tue, 18 Apr 2023 04:42:29 GMT  
		Size: 14.5 MB (14452994 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:87e5e5338fd3c72b3c1b02e0d4d669d4df8a6f0d3490b336653789e8eb863335`  
		Last Modified: Tue, 18 Apr 2023 04:42:25 GMT  
		Size: 680.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9747cf02540d0ebfcca5cab68c3394223598b896a79fe902754b86ce9bd4a320`  
		Last Modified: Tue, 18 Apr 2023 04:42:25 GMT  
		Size: 9.8 KB (9814 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a0c79ad9a26e8799140166d47c311ee5e49d7c8da779fc4ed61d5b8b091b91e3`  
		Last Modified: Tue, 18 Apr 2023 04:42:25 GMT  
		Size: 270.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e9fe478525312d95da159fc8e32c5482696c43361b99dbe24faaf540164917a7`  
		Last Modified: Tue, 18 Apr 2023 04:42:25 GMT  
		Size: 10.8 KB (10793 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:22e371444b713ac56889ba99cfa13d77574f6e89652e28c8af739e53bce084e9`  
		Last Modified: Tue, 18 Apr 2023 04:42:26 GMT  
		Size: 2.6 MB (2569466 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `websphere-liberty:kernel-java17-openj9` - linux; s390x

```console
$ docker pull websphere-liberty@sha256:d0709156ff697c9dc303da08232507d7d929369162f6b17d438436bf4d61f731
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **111.9 MB (111948168 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a7bd24ef1af89827f25aa4bd3a5a4e3d075c544543ae843c8882272af9007d76`
-	Entrypoint: `["\/opt\/ibm\/helpers\/runtime\/docker-server.sh"]`
-	Default Command: `["\/opt\/ibm\/wlp\/bin\/server","run","defaultServer"]`

```dockerfile
# Thu, 13 Apr 2023 13:09:35 GMT
ARG RELEASE
# Thu, 13 Apr 2023 13:09:35 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Thu, 13 Apr 2023 13:09:35 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Thu, 13 Apr 2023 13:09:35 GMT
LABEL org.opencontainers.image.version=20.04
# Thu, 13 Apr 2023 13:09:37 GMT
ADD file:44c66c03ba0afcc05de1b2078f83e8bfe04706b31491fcd3fdd93cfc88d5f06c in / 
# Thu, 13 Apr 2023 13:09:37 GMT
CMD ["/bin/bash"]
# Tue, 18 Apr 2023 01:20:33 GMT
ENV LANG=en_US.UTF-8 LANGUAGE=en_US:en LC_ALL=en_US.UTF-8
# Tue, 18 Apr 2023 01:20:42 GMT
RUN apt-get update     && DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends tzdata curl ca-certificates fontconfig locales     && echo "en_US.UTF-8 UTF-8" >> /etc/locale.gen     && locale-gen en_US.UTF-8     && rm -rf /var/lib/apt/lists/*
# Tue, 18 Apr 2023 01:24:46 GMT
ENV JAVA_VERSION=jdk-17.0.6+10_openj9-0.36.0
# Tue, 18 Apr 2023 01:25:51 GMT
RUN set -eux;     ARCH="$(dpkg --print-architecture)";     case "${ARCH}" in        aarch64|arm64)          ESUM='492bd87e39fc0eb78218746e98c4c0f6730af9c998b872c1a175c0e907d11510';          BINARY_URL='https://github.com/ibmruntimes/semeru17-binaries/releases/download/jdk-17.0.6%2B10_openj9-0.36.0/ibm-semeru-open-jre_aarch64_linux_17.0.6_10_openj9-0.36.0.tar.gz';          ;;        ppc64el|ppc64le)          ESUM='f1342b0a8b472d2de6e882030d2797b9c37e1cd7a90e4cb0c3bd969d4cf8158c';          BINARY_URL='https://github.com/ibmruntimes/semeru17-binaries/releases/download/jdk-17.0.6%2B10_openj9-0.36.0/ibm-semeru-open-jre_ppc64le_linux_17.0.6_10_openj9-0.36.0.tar.gz';          ;;        amd64|x86_64)          ESUM='69ca1728f9aad7031908bd9a939b5a9a9c5e931d65bb5c72cbe6f599c7d00cc6';          BINARY_URL='https://github.com/ibmruntimes/semeru17-binaries/releases/download/jdk-17.0.6%2B10_openj9-0.36.0/ibm-semeru-open-jre_x64_linux_17.0.6_10_openj9-0.36.0.tar.gz';          ;;        s390x)          ESUM='542359aebfb91b6605c67db6523b2ce154bda63f7fa8a6c243944b2091f4eb2b';          BINARY_URL='https://github.com/ibmruntimes/semeru17-binaries/releases/download/jdk-17.0.6%2B10_openj9-0.36.0/ibm-semeru-open-jre_s390x_linux_17.0.6_10_openj9-0.36.0.tar.gz';          ;;        *)          echo "Unsupported arch: ${ARCH}";          exit 1;          ;;     esac;     curl -LfsSo /tmp/openjdk.tar.gz ${BINARY_URL};     echo "${ESUM} */tmp/openjdk.tar.gz" | sha256sum -c -;     mkdir -p /opt/java/openjdk;     cd /opt/java/openjdk;     tar -xf /tmp/openjdk.tar.gz --strip-components=1;     rm -rf /tmp/openjdk.tar.gz;
# Tue, 18 Apr 2023 01:25:53 GMT
ENV JAVA_HOME=/opt/java/openjdk PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 18 Apr 2023 01:25:53 GMT
ENV JAVA_TOOL_OPTIONS=-XX:+IgnoreUnrecognizedVMOptions -XX:+PortableSharedCache -XX:+IdleTuningGcOnIdle -Xshareclasses:name=openj9_system_scc,cacheDir=/opt/java/.scc,readonly,nonFatal
# Tue, 18 Apr 2023 01:26:26 GMT
RUN set -eux;     unset OPENJ9_JAVA_OPTIONS;     SCC_SIZE="50m";     DOWNLOAD_PATH_TOMCAT=/tmp/tomcat;     INSTALL_PATH_TOMCAT=/opt/tomcat-home;     TOMCAT_CHECKSUM="0db27185d9fc3174f2c670f814df3dda8a008b89d1a38a5d96cbbe119767ebfb1cf0bce956b27954aee9be19c4a7b91f2579d967932207976322033a86075f98";     TOMCAT_DWNLD_URL="https://archive.apache.org/dist/tomcat/tomcat-9/v9.0.35/bin/apache-tomcat-9.0.35.tar.gz";         mkdir -p "${DOWNLOAD_PATH_TOMCAT}" "${INSTALL_PATH_TOMCAT}";     curl -LfsSo "${DOWNLOAD_PATH_TOMCAT}"/tomcat.tar.gz "${TOMCAT_DWNLD_URL}";     echo "${TOMCAT_CHECKSUM} *${DOWNLOAD_PATH_TOMCAT}/tomcat.tar.gz" | sha512sum -c -;     tar -xf "${DOWNLOAD_PATH_TOMCAT}"/tomcat.tar.gz -C "${INSTALL_PATH_TOMCAT}" --strip-components=1;     rm -rf "${DOWNLOAD_PATH_TOMCAT}";         java -Xshareclasses:name=dry_run_scc,cacheDir=/opt/java/.scc,bootClassesOnly,nonFatal,createLayer -Xscmx$SCC_SIZE -version;     export OPENJ9_JAVA_OPTIONS="-Xshareclasses:name=dry_run_scc,cacheDir=/opt/java/.scc,bootClassesOnly,nonFatal";     "${INSTALL_PATH_TOMCAT}"/bin/startup.sh;     sleep 5;     "${INSTALL_PATH_TOMCAT}"/bin/shutdown.sh -force;     sleep 15;     FULL=$( (java -Xshareclasses:name=dry_run_scc,cacheDir=/opt/java/.scc,printallStats 2>&1 || true) | awk '/^Cache is [0-9.]*% .*full/ {print substr($3, 1, length($3)-1)}');     DST_CACHE=$(java -Xshareclasses:name=dry_run_scc,cacheDir=/opt/java/.scc,destroy 2>&1 || true);     SCC_SIZE=$(echo $SCC_SIZE | sed 's/.$//');     SCC_SIZE=$(awk "BEGIN {print int($SCC_SIZE * $FULL / 100.0)}");     [ "${SCC_SIZE}" -eq 0 ] && SCC_SIZE=1;     SCC_SIZE="${SCC_SIZE}m";     java -Xshareclasses:name=openj9_system_scc,cacheDir=/opt/java/.scc,bootClassesOnly,nonFatal,createLayer -Xscmx$SCC_SIZE -version;     unset OPENJ9_JAVA_OPTIONS;         export OPENJ9_JAVA_OPTIONS="-Xshareclasses:name=openj9_system_scc,cacheDir=/opt/java/.scc,bootClassesOnly,nonFatal";     "${INSTALL_PATH_TOMCAT}"/bin/startup.sh;     sleep 5;     "${INSTALL_PATH_TOMCAT}"/bin/shutdown.sh -force;     sleep 5;     FULL=$( (java -Xshareclasses:name=openj9_system_scc,cacheDir=/opt/java/.scc,printallStats 2>&1 || true) | awk '/^Cache is [0-9.]*% .*full/ {print substr($3, 1, length($3)-1)}');     echo "SCC layer is $FULL% full.";     rm -rf "${INSTALL_PATH_TOMCAT}";     if [ -d "/opt/java/.scc" ]; then           chmod -R 0777 /opt/java/.scc;     fi;         echo "SCC generation phase completed";
# Tue, 18 Apr 2023 17:32:59 GMT
ARG VERBOSE=false
# Tue, 18 Apr 2023 17:32:59 GMT
ARG OPENJ9_SCC=true
# Tue, 18 Apr 2023 17:32:59 GMT
ARG EN_SHA=366618db4b733337adc71ec30b1f33d36cf78a81858636360061036a926f373f
# Tue, 18 Apr 2023 17:32:59 GMT
ARG NON_IBM_SHA=d349f6ea3acd71910348904dd48f81940b86ca5f879737206ae37f858767ad0f
# Tue, 18 Apr 2023 17:33:00 GMT
ARG NOTICES_SHA=e7031658e09e2442279db72eed9238fb30d98c06dabb112fb21b8618b7e810ee
# Tue, 18 Apr 2023 17:33:00 GMT
LABEL org.opencontainers.image.authors=Chris Potter, Christy Jesuraj, Melissa Lee org.opencontainers.image.vendor=IBM org.opencontainers.image.url=http://wasdev.net org.opencontainers.image.documentation=https://www.ibm.com/support/knowledgecenter/SSAW57_liberty/com.ibm.websphere.wlp.nd.multiplatform.doc/ae/cwlp_about.html org.opencontainers.image.version=23.0.0.3 org.opencontainers.image.revision=cl230320230319-1900 org.opencontainers.image.description=This image contains the WebSphere Liberty runtime with IBM Semeru Runtime Open Edition OpenJDK with OpenJ9 and Ubuntu as the base OS.  For more information on this image please see https://github.com/WASdev/ci.docker#building-an-application-image org.opencontainers.image.title=IBM WebSphere Liberty
# Tue, 18 Apr 2023 17:33:00 GMT
ENV LIBERTY_VERSION=23.0.0_03
# Tue, 18 Apr 2023 17:33:00 GMT
ARG LIBERTY_URL
# Tue, 18 Apr 2023 17:33:00 GMT
ARG DOWNLOAD_OPTIONS=
# Tue, 18 Apr 2023 17:33:11 GMT
# ARGS: DOWNLOAD_OPTIONS= EN_SHA=366618db4b733337adc71ec30b1f33d36cf78a81858636360061036a926f373f NON_IBM_SHA=d349f6ea3acd71910348904dd48f81940b86ca5f879737206ae37f858767ad0f NOTICES_SHA=e7031658e09e2442279db72eed9238fb30d98c06dabb112fb21b8618b7e810ee OPENJ9_SCC=true VERBOSE=false
RUN apt-get update     && apt-get install -y --no-install-recommends unzip wget openssl     && rm -rf /var/lib/apt/lists/*     && mkdir -p /licenses/     && useradd -u 1001 -r -g 0 -s /usr/sbin/nologin default     && LIBERTY_URL=${LIBERTY_URL:-$(wget -q -O - https://public.dhe.ibm.com/ibmdl/export/pub/software/websphere/wasdev/downloads/wlp/index.yml  | grep $LIBERTY_VERSION -A 6 | sed -n 's/\s*kernel:\s//p' | tr -d '\r' )}      && wget $DOWNLOAD_OPTIONS $LIBERTY_URL -U UA-IBM-WebSphere-Liberty-Docker -O /tmp/wlp.zip     && unzip -q /tmp/wlp.zip -d /opt/ibm     && rm /tmp/wlp.zip     && chown -R 1001:0 /opt/ibm/wlp     && chmod -R g+rw /opt/ibm/wlp     && LICENSE_BASE=$(wget -q -O - https://public.dhe.ibm.com/ibmdl/export/pub/software/websphere/wasdev/downloads/wlp/index.yml  | grep $LIBERTY_VERSION -A 6 | sed -n 's/\s*license:\s//p' | sed 's/\(.*\)\/.*/\1\//' | tr -d '\r')     && wget ${LICENSE_BASE}en.html -U UA-IBM-WebSphere-Liberty-Docker -O /licenses/en.html     && wget ${LICENSE_BASE}non_ibm_license.html -U UA-IBM-WebSphere-Liberty-Docker -O /licenses/non_ibm_license.html     && wget ${LICENSE_BASE}notices.html -U UA-IBM-WebSphere-Liberty-Docker -O /licenses/notices.html     && echo "$EN_SHA /licenses/en.html" | sha256sum -c --strict --check     && echo "$NON_IBM_SHA /licenses/non_ibm_license.html" | sha256sum -c --strict --check     && echo "$NOTICES_SHA /licenses/notices.html" | sha256sum -c --strict --check     && apt-get purge --auto-remove -y unzip     && apt-get purge --auto-remove -y wget     && rm -rf /var/lib/apt/lists/*
# Tue, 18 Apr 2023 17:33:11 GMT
ENV PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/opt/ibm/wlp/bin:/opt/ibm/helpers/build
# Tue, 18 Apr 2023 17:33:11 GMT
LABEL ProductID=fbf6a96d49214c0abc6a3bc5da6e48cd ProductName=WebSphere Application Server Liberty ProductVersion=23.0.0.3 BuildLabel=cl230320230319-1900
# Tue, 18 Apr 2023 17:33:11 GMT
ENV LOG_DIR=/logs WLP_OUTPUT_DIR=/opt/ibm/wlp/output OPENJ9_SCC=true
# Tue, 18 Apr 2023 17:33:12 GMT
# ARGS: DOWNLOAD_OPTIONS= EN_SHA=366618db4b733337adc71ec30b1f33d36cf78a81858636360061036a926f373f NON_IBM_SHA=d349f6ea3acd71910348904dd48f81940b86ca5f879737206ae37f858767ad0f NOTICES_SHA=e7031658e09e2442279db72eed9238fb30d98c06dabb112fb21b8618b7e810ee VERBOSE=false
RUN /opt/ibm/wlp/bin/server create     && rm -rf $WLP_OUTPUT_DIR/.classCache /output/workarea
# Tue, 18 Apr 2023 17:33:12 GMT
COPY dir:0f3e336b1e5adb84a625050153035561e1c9802a57b7b90b5a17ebb82adba489 in /opt/ibm/helpers/ 
# Tue, 18 Apr 2023 17:33:12 GMT
COPY dir:1cf5cc2663c6235241a5228340a9c566587fe27b3e434a313debbf75dacd7a4b in /opt/ibm/fixes/ 
# Tue, 18 Apr 2023 17:33:12 GMT
# ARGS: DOWNLOAD_OPTIONS= EN_SHA=366618db4b733337adc71ec30b1f33d36cf78a81858636360061036a926f373f NON_IBM_SHA=d349f6ea3acd71910348904dd48f81940b86ca5f879737206ae37f858767ad0f NOTICES_SHA=e7031658e09e2442279db72eed9238fb30d98c06dabb112fb21b8618b7e810ee VERBOSE=false
RUN mkdir /logs     && mkdir /etc/wlp     && mkdir -p /opt/ibm/wlp/usr/shared/resources/lib.index.cache     && mkdir -p /home/default     && mkdir /output     && chmod -t /output     && rm -rf /output     && ln -s $WLP_OUTPUT_DIR/defaultServer /output     && ln -s /opt/ibm/wlp/usr/servers/defaultServer /config     && ln -s /opt/ibm /liberty     && ln -s /opt/ibm/wlp/usr/shared/resources/lib.index.cache /lib.index.cache     && mkdir -p /config/configDropins/defaults     && mkdir -p /config/configDropins/overrides     && chown -R 1001:0 /config     && chmod -R g+rw /config     && chown -R 1001:0 /opt/ibm/helpers     && chmod -R g+rwx /opt/ibm/helpers     && chown -R 1001:0 /opt/ibm/fixes     && chmod -R g+rwx /opt/ibm/fixes     && chown -R 1001:0 /opt/ibm/wlp/usr     && chmod -R g+rw /opt/ibm/wlp/usr     && chown -R 1001:0 /opt/ibm/wlp/output     && chmod -R g+rw /opt/ibm/wlp/output     && chown -R 1001:0 /logs     && chmod -R g+rw /logs     && chown -R 1001:0 /etc/wlp     && chmod -R g+rw /etc/wlp     && chown -R 1001:0 /home/default     && chmod -R g+rw /home/default
# Tue, 18 Apr 2023 17:33:16 GMT
# ARGS: DOWNLOAD_OPTIONS= EN_SHA=366618db4b733337adc71ec30b1f33d36cf78a81858636360061036a926f373f NON_IBM_SHA=d349f6ea3acd71910348904dd48f81940b86ca5f879737206ae37f858767ad0f NOTICES_SHA=e7031658e09e2442279db72eed9238fb30d98c06dabb112fb21b8618b7e810ee VERBOSE=false
RUN if [ "$OPENJ9_SCC" = "true" ]; then populate_scc.sh; fi     && rm -rf /output/messaging /output/resources/security /logs/* $WLP_OUTPUT_DIR/.classCache     && chown -R 1001:0 /opt/ibm/wlp/output     && chmod -R g+rwx /opt/ibm/wlp/output
# Tue, 18 Apr 2023 17:33:16 GMT
ENV RANDFILE=/tmp/.rnd OPENJ9_JAVA_OPTIONS=-XX:+IgnoreUnrecognizedVMOptions -XX:+IdleTuningGcOnIdle -Xshareclasses:name=openj9_system_scc,cacheDir=/opt/java/.scc,readonly,nonFatal -Dosgi.checkConfiguration=false
# Tue, 18 Apr 2023 17:33:17 GMT
USER 1001
# Tue, 18 Apr 2023 17:33:17 GMT
EXPOSE 9080 9443
# Tue, 18 Apr 2023 17:33:17 GMT
ENTRYPOINT ["/opt/ibm/helpers/runtime/docker-server.sh"]
# Tue, 18 Apr 2023 17:33:17 GMT
CMD ["/opt/ibm/wlp/bin/server" "run" "defaultServer"]
```

-	Layers:
	-	`sha256:f11b609b1d63f2d37c0e3789823e7a7e62a078bddca7c46da8602655989c62d9`  
		Last Modified: Fri, 14 Apr 2023 09:38:39 GMT  
		Size: 27.0 MB (27016370 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:904a0c815c072ccdf47e2b629d60ff91ad3ae9a1485d39c406b7c5e846233b1c`  
		Last Modified: Tue, 18 Apr 2023 01:29:20 GMT  
		Size: 15.7 MB (15693377 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:08743e9ad8e97f800fc2153a06a0c2fd9236cda36ed15d44ff620a8c6dc2baab`  
		Last Modified: Tue, 18 Apr 2023 01:30:45 GMT  
		Size: 47.3 MB (47259354 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e7f1613454284e1afb2d3b27fbb20fac7d1d0dba8f76210a4c5f72c055a9719b`  
		Last Modified: Tue, 18 Apr 2023 01:30:40 GMT  
		Size: 4.9 MB (4886693 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d54b590615feb77dcde3da1803c72dc664283a3e66d6854365f89600a2a098c0`  
		Last Modified: Tue, 18 Apr 2023 18:34:55 GMT  
		Size: 14.5 MB (14452667 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:af239d3b333535836b106ec5d4dd6d7a85cdaa6196cacdd74872cdb9ef3c3dc8`  
		Last Modified: Tue, 18 Apr 2023 18:34:53 GMT  
		Size: 676.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:283661d6d74929be65bee02f3bba0f195683a70658bbcb17b61c9de5c93c5f88`  
		Last Modified: Tue, 18 Apr 2023 18:34:52 GMT  
		Size: 9.8 KB (9813 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dbc5518fe3ace1980bf183fdd0c06db7941c4485b6c73274c9369a1d7e52151a`  
		Last Modified: Tue, 18 Apr 2023 18:34:52 GMT  
		Size: 273.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b0623cbd2914d09adae32e6b6d4a4442fc74ba95f8c3c7c15f87763cac79d528`  
		Last Modified: Tue, 18 Apr 2023 18:34:52 GMT  
		Size: 10.8 KB (10783 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:770e00a421765c3fa8828e922fa4f31f47c65f7807c3f661e1871d7c40ceb221`  
		Last Modified: Tue, 18 Apr 2023 18:34:53 GMT  
		Size: 2.6 MB (2618162 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
