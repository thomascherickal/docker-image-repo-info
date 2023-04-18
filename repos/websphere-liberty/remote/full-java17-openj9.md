## `websphere-liberty:full-java17-openj9`

```console
$ docker pull websphere-liberty@sha256:db9f336f9ee7e91e5f491d49037cba187299fd600a232aa5849914a873a6bd38
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 3
	-	linux; amd64
	-	linux; ppc64le
	-	linux; s390x

### `websphere-liberty:full-java17-openj9` - linux; amd64

```console
$ docker pull websphere-liberty@sha256:08c39f7e618e8a5a39159abda087215829f9c328401c55f6da9e9f57aa975c99
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **488.8 MB (488770319 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:64256be5e6df849004703782add7ec28487dc523e349d9bff414b8512106c1df`
-	Entrypoint: `["\/opt\/ibm\/helpers\/runtime\/docker-server.sh"]`
-	Default Command: `["\/opt\/ibm\/wlp\/bin\/server","run","defaultServer"]`

```dockerfile
# Wed, 08 Mar 2023 04:41:24 GMT
ARG RELEASE
# Wed, 08 Mar 2023 04:41:24 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Wed, 08 Mar 2023 04:41:24 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Wed, 08 Mar 2023 04:41:24 GMT
LABEL org.opencontainers.image.version=20.04
# Wed, 08 Mar 2023 04:41:26 GMT
ADD file:20f2ff22b9a8ca9bec5178036c9ebc525a12cd4312daf5d14a9a631a30be20e1 in / 
# Wed, 08 Mar 2023 04:41:27 GMT
CMD ["/bin/bash"]
# Thu, 16 Mar 2023 03:15:07 GMT
ENV LANG=en_US.UTF-8 LANGUAGE=en_US:en LC_ALL=en_US.UTF-8
# Thu, 16 Mar 2023 03:15:21 GMT
RUN apt-get update     && DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends tzdata curl ca-certificates fontconfig locales     && echo "en_US.UTF-8 UTF-8" >> /etc/locale.gen     && locale-gen en_US.UTF-8     && rm -rf /var/lib/apt/lists/*
# Thu, 16 Mar 2023 03:22:37 GMT
ENV JAVA_VERSION=jdk-17.0.6+10_openj9-0.36.0
# Thu, 16 Mar 2023 03:24:22 GMT
RUN set -eux;     ARCH="$(dpkg --print-architecture)";     case "${ARCH}" in        aarch64|arm64)          ESUM='492bd87e39fc0eb78218746e98c4c0f6730af9c998b872c1a175c0e907d11510';          BINARY_URL='https://github.com/ibmruntimes/semeru17-binaries/releases/download/jdk-17.0.6%2B10_openj9-0.36.0/ibm-semeru-open-jre_aarch64_linux_17.0.6_10_openj9-0.36.0.tar.gz';          ;;        ppc64el|ppc64le)          ESUM='f1342b0a8b472d2de6e882030d2797b9c37e1cd7a90e4cb0c3bd969d4cf8158c';          BINARY_URL='https://github.com/ibmruntimes/semeru17-binaries/releases/download/jdk-17.0.6%2B10_openj9-0.36.0/ibm-semeru-open-jre_ppc64le_linux_17.0.6_10_openj9-0.36.0.tar.gz';          ;;        amd64|x86_64)          ESUM='69ca1728f9aad7031908bd9a939b5a9a9c5e931d65bb5c72cbe6f599c7d00cc6';          BINARY_URL='https://github.com/ibmruntimes/semeru17-binaries/releases/download/jdk-17.0.6%2B10_openj9-0.36.0/ibm-semeru-open-jre_x64_linux_17.0.6_10_openj9-0.36.0.tar.gz';          ;;        s390x)          ESUM='542359aebfb91b6605c67db6523b2ce154bda63f7fa8a6c243944b2091f4eb2b';          BINARY_URL='https://github.com/ibmruntimes/semeru17-binaries/releases/download/jdk-17.0.6%2B10_openj9-0.36.0/ibm-semeru-open-jre_s390x_linux_17.0.6_10_openj9-0.36.0.tar.gz';          ;;        *)          echo "Unsupported arch: ${ARCH}";          exit 1;          ;;     esac;     curl -LfsSo /tmp/openjdk.tar.gz ${BINARY_URL};     echo "${ESUM} */tmp/openjdk.tar.gz" | sha256sum -c -;     mkdir -p /opt/java/openjdk;     cd /opt/java/openjdk;     tar -xf /tmp/openjdk.tar.gz --strip-components=1;     rm -rf /tmp/openjdk.tar.gz;
# Thu, 16 Mar 2023 03:24:22 GMT
ENV JAVA_HOME=/opt/java/openjdk PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 16 Mar 2023 03:24:22 GMT
ENV JAVA_TOOL_OPTIONS=-XX:+IgnoreUnrecognizedVMOptions -XX:+PortableSharedCache -XX:+IdleTuningGcOnIdle -Xshareclasses:name=openj9_system_scc,cacheDir=/opt/java/.scc,readonly,nonFatal
# Thu, 16 Mar 2023 03:24:57 GMT
RUN set -eux;     unset OPENJ9_JAVA_OPTIONS;     SCC_SIZE="50m";     DOWNLOAD_PATH_TOMCAT=/tmp/tomcat;     INSTALL_PATH_TOMCAT=/opt/tomcat-home;     TOMCAT_CHECKSUM="0db27185d9fc3174f2c670f814df3dda8a008b89d1a38a5d96cbbe119767ebfb1cf0bce956b27954aee9be19c4a7b91f2579d967932207976322033a86075f98";     TOMCAT_DWNLD_URL="https://archive.apache.org/dist/tomcat/tomcat-9/v9.0.35/bin/apache-tomcat-9.0.35.tar.gz";         mkdir -p "${DOWNLOAD_PATH_TOMCAT}" "${INSTALL_PATH_TOMCAT}";     curl -LfsSo "${DOWNLOAD_PATH_TOMCAT}"/tomcat.tar.gz "${TOMCAT_DWNLD_URL}";     echo "${TOMCAT_CHECKSUM} *${DOWNLOAD_PATH_TOMCAT}/tomcat.tar.gz" | sha512sum -c -;     tar -xf "${DOWNLOAD_PATH_TOMCAT}"/tomcat.tar.gz -C "${INSTALL_PATH_TOMCAT}" --strip-components=1;     rm -rf "${DOWNLOAD_PATH_TOMCAT}";         java -Xshareclasses:name=dry_run_scc,cacheDir=/opt/java/.scc,bootClassesOnly,nonFatal,createLayer -Xscmx$SCC_SIZE -version;     export OPENJ9_JAVA_OPTIONS="-Xshareclasses:name=dry_run_scc,cacheDir=/opt/java/.scc,bootClassesOnly,nonFatal";     "${INSTALL_PATH_TOMCAT}"/bin/startup.sh;     sleep 5;     "${INSTALL_PATH_TOMCAT}"/bin/shutdown.sh -force;     sleep 15;     FULL=$( (java -Xshareclasses:name=dry_run_scc,cacheDir=/opt/java/.scc,printallStats 2>&1 || true) | awk '/^Cache is [0-9.]*% .*full/ {print substr($3, 1, length($3)-1)}');     DST_CACHE=$(java -Xshareclasses:name=dry_run_scc,cacheDir=/opt/java/.scc,destroy 2>&1 || true);     SCC_SIZE=$(echo $SCC_SIZE | sed 's/.$//');     SCC_SIZE=$(awk "BEGIN {print int($SCC_SIZE * $FULL / 100.0)}");     [ "${SCC_SIZE}" -eq 0 ] && SCC_SIZE=1;     SCC_SIZE="${SCC_SIZE}m";     java -Xshareclasses:name=openj9_system_scc,cacheDir=/opt/java/.scc,bootClassesOnly,nonFatal,createLayer -Xscmx$SCC_SIZE -version;     unset OPENJ9_JAVA_OPTIONS;         export OPENJ9_JAVA_OPTIONS="-Xshareclasses:name=openj9_system_scc,cacheDir=/opt/java/.scc,bootClassesOnly,nonFatal";     "${INSTALL_PATH_TOMCAT}"/bin/startup.sh;     sleep 5;     "${INSTALL_PATH_TOMCAT}"/bin/shutdown.sh -force;     sleep 5;     FULL=$( (java -Xshareclasses:name=openj9_system_scc,cacheDir=/opt/java/.scc,printallStats 2>&1 || true) | awk '/^Cache is [0-9.]*% .*full/ {print substr($3, 1, length($3)-1)}');     echo "SCC layer is $FULL% full.";     rm -rf "${INSTALL_PATH_TOMCAT}";     if [ -d "/opt/java/.scc" ]; then           chmod -R 0777 /opt/java/.scc;     fi;         echo "SCC generation phase completed";
# Thu, 16 Mar 2023 09:37:21 GMT
ARG VERBOSE=false
# Thu, 16 Mar 2023 09:37:21 GMT
ARG OPENJ9_SCC=true
# Tue, 11 Apr 2023 22:30:30 GMT
ARG EN_SHA=366618db4b733337adc71ec30b1f33d36cf78a81858636360061036a926f373f
# Tue, 11 Apr 2023 22:30:30 GMT
ARG NON_IBM_SHA=d349f6ea3acd71910348904dd48f81940b86ca5f879737206ae37f858767ad0f
# Tue, 11 Apr 2023 22:30:30 GMT
ARG NOTICES_SHA=e7031658e09e2442279db72eed9238fb30d98c06dabb112fb21b8618b7e810ee
# Tue, 11 Apr 2023 22:30:30 GMT
LABEL org.opencontainers.image.authors=Chris Potter, Christy Jesuraj, Melissa Lee org.opencontainers.image.vendor=IBM org.opencontainers.image.url=http://wasdev.net org.opencontainers.image.documentation=https://www.ibm.com/support/knowledgecenter/SSAW57_liberty/com.ibm.websphere.wlp.nd.multiplatform.doc/ae/cwlp_about.html org.opencontainers.image.version=23.0.0.3 org.opencontainers.image.revision=cl230320230319-1900 org.opencontainers.image.description=This image contains the WebSphere Liberty runtime with IBM Semeru Runtime Open Edition OpenJDK with OpenJ9 and Ubuntu as the base OS.  For more information on this image please see https://github.com/WASdev/ci.docker#building-an-application-image org.opencontainers.image.title=IBM WebSphere Liberty
# Tue, 11 Apr 2023 22:30:30 GMT
ENV LIBERTY_VERSION=23.0.0_03
# Tue, 11 Apr 2023 22:30:30 GMT
ARG LIBERTY_URL
# Tue, 11 Apr 2023 22:30:30 GMT
ARG DOWNLOAD_OPTIONS=
# Tue, 11 Apr 2023 22:30:43 GMT
# ARGS: DOWNLOAD_OPTIONS= EN_SHA=366618db4b733337adc71ec30b1f33d36cf78a81858636360061036a926f373f NON_IBM_SHA=d349f6ea3acd71910348904dd48f81940b86ca5f879737206ae37f858767ad0f NOTICES_SHA=e7031658e09e2442279db72eed9238fb30d98c06dabb112fb21b8618b7e810ee OPENJ9_SCC=true VERBOSE=false
RUN apt-get update     && apt-get install -y --no-install-recommends unzip wget openssl     && rm -rf /var/lib/apt/lists/*     && mkdir -p /licenses/     && useradd -u 1001 -r -g 0 -s /usr/sbin/nologin default     && LIBERTY_URL=${LIBERTY_URL:-$(wget -q -O - https://public.dhe.ibm.com/ibmdl/export/pub/software/websphere/wasdev/downloads/wlp/index.yml  | grep $LIBERTY_VERSION -A 6 | sed -n 's/\s*kernel:\s//p' | tr -d '\r' )}      && wget $DOWNLOAD_OPTIONS $LIBERTY_URL -U UA-IBM-WebSphere-Liberty-Docker -O /tmp/wlp.zip     && unzip -q /tmp/wlp.zip -d /opt/ibm     && rm /tmp/wlp.zip     && chown -R 1001:0 /opt/ibm/wlp     && chmod -R g+rw /opt/ibm/wlp     && LICENSE_BASE=$(wget -q -O - https://public.dhe.ibm.com/ibmdl/export/pub/software/websphere/wasdev/downloads/wlp/index.yml  | grep $LIBERTY_VERSION -A 6 | sed -n 's/\s*license:\s//p' | sed 's/\(.*\)\/.*/\1\//' | tr -d '\r')     && wget ${LICENSE_BASE}en.html -U UA-IBM-WebSphere-Liberty-Docker -O /licenses/en.html     && wget ${LICENSE_BASE}non_ibm_license.html -U UA-IBM-WebSphere-Liberty-Docker -O /licenses/non_ibm_license.html     && wget ${LICENSE_BASE}notices.html -U UA-IBM-WebSphere-Liberty-Docker -O /licenses/notices.html     && echo "$EN_SHA /licenses/en.html" | sha256sum -c --strict --check     && echo "$NON_IBM_SHA /licenses/non_ibm_license.html" | sha256sum -c --strict --check     && echo "$NOTICES_SHA /licenses/notices.html" | sha256sum -c --strict --check     && apt-get purge --auto-remove -y unzip     && apt-get purge --auto-remove -y wget     && rm -rf /var/lib/apt/lists/*
# Tue, 11 Apr 2023 22:30:43 GMT
ENV PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/opt/ibm/wlp/bin:/opt/ibm/helpers/build
# Tue, 11 Apr 2023 22:30:44 GMT
LABEL ProductID=fbf6a96d49214c0abc6a3bc5da6e48cd ProductName=WebSphere Application Server Liberty ProductVersion=23.0.0.3 BuildLabel=cl230320230319-1900
# Tue, 11 Apr 2023 22:30:44 GMT
ENV LOG_DIR=/logs WLP_OUTPUT_DIR=/opt/ibm/wlp/output OPENJ9_SCC=true
# Tue, 11 Apr 2023 22:30:44 GMT
# ARGS: DOWNLOAD_OPTIONS= EN_SHA=366618db4b733337adc71ec30b1f33d36cf78a81858636360061036a926f373f NON_IBM_SHA=d349f6ea3acd71910348904dd48f81940b86ca5f879737206ae37f858767ad0f NOTICES_SHA=e7031658e09e2442279db72eed9238fb30d98c06dabb112fb21b8618b7e810ee VERBOSE=false
RUN /opt/ibm/wlp/bin/server create     && rm -rf $WLP_OUTPUT_DIR/.classCache /output/workarea
# Tue, 11 Apr 2023 22:30:44 GMT
COPY dir:0f3e336b1e5adb84a625050153035561e1c9802a57b7b90b5a17ebb82adba489 in /opt/ibm/helpers/ 
# Tue, 11 Apr 2023 22:30:45 GMT
COPY dir:1cf5cc2663c6235241a5228340a9c566587fe27b3e434a313debbf75dacd7a4b in /opt/ibm/fixes/ 
# Tue, 11 Apr 2023 22:30:45 GMT
# ARGS: DOWNLOAD_OPTIONS= EN_SHA=366618db4b733337adc71ec30b1f33d36cf78a81858636360061036a926f373f NON_IBM_SHA=d349f6ea3acd71910348904dd48f81940b86ca5f879737206ae37f858767ad0f NOTICES_SHA=e7031658e09e2442279db72eed9238fb30d98c06dabb112fb21b8618b7e810ee VERBOSE=false
RUN mkdir /logs     && mkdir /etc/wlp     && mkdir -p /opt/ibm/wlp/usr/shared/resources/lib.index.cache     && mkdir -p /home/default     && mkdir /output     && chmod -t /output     && rm -rf /output     && ln -s $WLP_OUTPUT_DIR/defaultServer /output     && ln -s /opt/ibm/wlp/usr/servers/defaultServer /config     && ln -s /opt/ibm /liberty     && ln -s /opt/ibm/wlp/usr/shared/resources/lib.index.cache /lib.index.cache     && mkdir -p /config/configDropins/defaults     && mkdir -p /config/configDropins/overrides     && chown -R 1001:0 /config     && chmod -R g+rw /config     && chown -R 1001:0 /opt/ibm/helpers     && chmod -R g+rwx /opt/ibm/helpers     && chown -R 1001:0 /opt/ibm/fixes     && chmod -R g+rwx /opt/ibm/fixes     && chown -R 1001:0 /opt/ibm/wlp/usr     && chmod -R g+rw /opt/ibm/wlp/usr     && chown -R 1001:0 /opt/ibm/wlp/output     && chmod -R g+rw /opt/ibm/wlp/output     && chown -R 1001:0 /logs     && chmod -R g+rw /logs     && chown -R 1001:0 /etc/wlp     && chmod -R g+rw /etc/wlp     && chown -R 1001:0 /home/default     && chmod -R g+rw /home/default
# Tue, 11 Apr 2023 22:30:51 GMT
# ARGS: DOWNLOAD_OPTIONS= EN_SHA=366618db4b733337adc71ec30b1f33d36cf78a81858636360061036a926f373f NON_IBM_SHA=d349f6ea3acd71910348904dd48f81940b86ca5f879737206ae37f858767ad0f NOTICES_SHA=e7031658e09e2442279db72eed9238fb30d98c06dabb112fb21b8618b7e810ee VERBOSE=false
RUN if [ "$OPENJ9_SCC" = "true" ]; then populate_scc.sh; fi     && rm -rf /output/messaging /output/resources/security /logs/* $WLP_OUTPUT_DIR/.classCache     && chown -R 1001:0 /opt/ibm/wlp/output     && chmod -R g+rwx /opt/ibm/wlp/output
# Tue, 11 Apr 2023 22:30:51 GMT
ENV RANDFILE=/tmp/.rnd OPENJ9_JAVA_OPTIONS=-XX:+IgnoreUnrecognizedVMOptions -XX:+IdleTuningGcOnIdle -Xshareclasses:name=openj9_system_scc,cacheDir=/opt/java/.scc,readonly,nonFatal -Dosgi.checkConfiguration=false
# Tue, 11 Apr 2023 22:30:51 GMT
USER 1001
# Tue, 11 Apr 2023 22:30:51 GMT
EXPOSE 9080 9443
# Tue, 11 Apr 2023 22:30:51 GMT
ENTRYPOINT ["/opt/ibm/helpers/runtime/docker-server.sh"]
# Tue, 11 Apr 2023 22:30:51 GMT
CMD ["/opt/ibm/wlp/bin/server" "run" "defaultServer"]
# Tue, 11 Apr 2023 22:51:55 GMT
ARG VERBOSE=false
# Tue, 11 Apr 2023 22:51:55 GMT
ARG REPOSITORIES_PROPERTIES=
# Tue, 11 Apr 2023 23:01:42 GMT
# ARGS: REPOSITORIES_PROPERTIES= VERBOSE=false
RUN if [ ! -z $REPOSITORIES_PROPERTIES ]; then mkdir /opt/ibm/wlp/etc/   && echo $REPOSITORIES_PROPERTIES > /opt/ibm/wlp/etc/repositories.properties; fi   && installUtility install --acceptLicense baseBundle   && if [ ! -z $REPOSITORIES_PROPERTIES ]; then rm /opt/ibm/wlp/etc/repositories.properties; fi   && rm -rf /output/workarea /output/logs   && find /opt/ibm/wlp ! -perm -g=rw -print0 | xargs -r -0 chmod g+rw
# Tue, 11 Apr 2023 23:01:43 GMT
COPY --chown=1001:0file:f212cc38605f508baa0f75a07632700533ad28792dd9761a792209e709b00f23 in /config/ 
# Tue, 11 Apr 2023 23:02:12 GMT
# ARGS: REPOSITORIES_PROPERTIES= VERBOSE=false
RUN if [ "$OPENJ9_SCC" = "true" ]; then populate_scc.sh; fi     && rm -rf /output/messaging /output/resources/security /logs/* $WLP_OUTPUT_DIR/.classCache     && find /opt/ibm/wlp/output ! -perm -g=rwx -print0 | xargs -0 -r chmod g+rwx
```

-	Layers:
	-	`sha256:5544ebdc0c7b82aa6901eae124b1d220914d2629a9bde25396d7ee9cfd273a8f`  
		Last Modified: Wed, 08 Mar 2023 09:02:58 GMT  
		Size: 28.6 MB (28578068 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:88ee649a107970a9b268a804786d7d72435836f4aefdd600745ee7122da67b92`  
		Last Modified: Thu, 16 Mar 2023 03:30:59 GMT  
		Size: 16.0 MB (15997519 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c6bd151aa61a3377b40d5e65e20832ce5888fbc0529bad5043f5aaf8142e9fa8`  
		Last Modified: Thu, 16 Mar 2023 03:34:18 GMT  
		Size: 48.2 MB (48218507 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4d1a71c60fb1d4cd3223f40eb94986e48674871564a62b81e8425e04df971c3f`  
		Last Modified: Thu, 16 Mar 2023 03:34:12 GMT  
		Size: 4.8 MB (4756441 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:76bb86e980d223a82cc01a47060d4168f99e6c94809b6c73d660c0e9e454502e`  
		Last Modified: Tue, 11 Apr 2023 23:03:14 GMT  
		Size: 14.5 MB (14452454 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:12e110f910c448fb2a44e47dcd70e0c31785173044bb404ca961d3ad2bfa8166`  
		Last Modified: Tue, 11 Apr 2023 23:03:11 GMT  
		Size: 677.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:78934507e290da42aeb7fa7fc9acf831917837c88bb721b7c7a299b7f4e61764`  
		Last Modified: Tue, 11 Apr 2023 23:03:11 GMT  
		Size: 9.8 KB (9811 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5eb6f94b81406988a217e0f173cb5dc2d327cd939ea12b3b6919cab8732852cb`  
		Last Modified: Tue, 11 Apr 2023 23:03:11 GMT  
		Size: 272.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:74591995fa0ec19a44e6ed5515767473a17449fd44d6bd95072e85a9ddb9b187`  
		Last Modified: Tue, 11 Apr 2023 23:03:11 GMT  
		Size: 10.8 KB (10789 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dc87c3dfe17c9922750965ecc083fbe33780fb83da55a6d105190786e6cba174`  
		Last Modified: Tue, 11 Apr 2023 23:03:12 GMT  
		Size: 2.7 MB (2696609 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a67e7c03d36d723857d7b632c4b4a75831ac1f05346e7ba4beb8cdce343a4e1f`  
		Last Modified: Tue, 11 Apr 2023 23:04:25 GMT  
		Size: 359.0 MB (359033512 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:908a3b2dca1dd05a1b63cee3584c4cc021a29fee5d385e63e8f3094d407c1bf7`  
		Last Modified: Tue, 11 Apr 2023 23:04:08 GMT  
		Size: 945.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8f12924f9225eae68bffa80813bf2a464f02ff22264ff9fc38de70a4f6d581e6`  
		Last Modified: Tue, 11 Apr 2023 23:04:10 GMT  
		Size: 15.0 MB (15014715 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `websphere-liberty:full-java17-openj9` - linux; ppc64le

```console
$ docker pull websphere-liberty@sha256:667a0aea24a8b92d396b912c8d9fe57011ed02c81226c20b33c10063b4ee7865
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **492.6 MB (492567734 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:88decc9aa0251255df3bd8bfcda00f0b7ce4723ff16f9e32eddc1890c978cc37`
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
# Tue, 18 Apr 2023 03:43:39 GMT
ARG VERBOSE=false
# Tue, 18 Apr 2023 03:43:39 GMT
ARG REPOSITORIES_PROPERTIES=
# Tue, 18 Apr 2023 04:02:59 GMT
# ARGS: REPOSITORIES_PROPERTIES= VERBOSE=false
RUN if [ ! -z $REPOSITORIES_PROPERTIES ]; then mkdir /opt/ibm/wlp/etc/   && echo $REPOSITORIES_PROPERTIES > /opt/ibm/wlp/etc/repositories.properties; fi   && installUtility install --acceptLicense baseBundle   && if [ ! -z $REPOSITORIES_PROPERTIES ]; then rm /opt/ibm/wlp/etc/repositories.properties; fi   && rm -rf /output/workarea /output/logs   && find /opt/ibm/wlp ! -perm -g=rw -print0 | xargs -r -0 chmod g+rw
# Tue, 18 Apr 2023 04:03:04 GMT
COPY --chown=1001:0file:f212cc38605f508baa0f75a07632700533ad28792dd9761a792209e709b00f23 in /config/ 
# Tue, 18 Apr 2023 04:03:59 GMT
# ARGS: REPOSITORIES_PROPERTIES= VERBOSE=false
RUN if [ "$OPENJ9_SCC" = "true" ]; then populate_scc.sh; fi     && rm -rf /output/messaging /output/resources/security /logs/* $WLP_OUTPUT_DIR/.classCache     && find /opt/ibm/wlp/output ! -perm -g=rwx -print0 | xargs -0 -r chmod g+rwx
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
	-	`sha256:e4e70c46ab7720ba4533492cad526752683858fff007595901681161423c8e63`  
		Last Modified: Tue, 18 Apr 2023 04:43:47 GMT  
		Size: 359.0 MB (359034556 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d399fd1271c4b34c84815b22d7519f104277657837c9394c77b260914a395470`  
		Last Modified: Tue, 18 Apr 2023 04:43:17 GMT  
		Size: 944.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:61ccbdf2283ee35bfcbad4a4929cf1db65f265b5541fff9bf7f45eebe5c2608a`  
		Last Modified: Tue, 18 Apr 2023 04:43:19 GMT  
		Size: 12.9 MB (12923264 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `websphere-liberty:full-java17-openj9` - linux; s390x

```console
$ docker pull websphere-liberty@sha256:d906602f2821b9b1c5ed1741b3dce9069004764f4d458241524917f1a11d858c
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **486.4 MB (486432150 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:235049ff40e84e660ab65dd379b7f73acef9b2c4f64fd5659e64939bad7834ae`
-	Entrypoint: `["\/opt\/ibm\/helpers\/runtime\/docker-server.sh"]`
-	Default Command: `["\/opt\/ibm\/wlp\/bin\/server","run","defaultServer"]`

```dockerfile
# Wed, 08 Mar 2023 04:41:58 GMT
ARG RELEASE
# Wed, 08 Mar 2023 04:41:58 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Wed, 08 Mar 2023 04:41:58 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Wed, 08 Mar 2023 04:41:58 GMT
LABEL org.opencontainers.image.version=20.04
# Wed, 08 Mar 2023 04:42:00 GMT
ADD file:4463dafd3352de8c5ff87090e2f30be9bdffc3fa9d84e27b13e2364d856f82e9 in / 
# Wed, 08 Mar 2023 04:42:00 GMT
CMD ["/bin/bash"]
# Thu, 16 Mar 2023 02:16:22 GMT
ENV LANG=en_US.UTF-8 LANGUAGE=en_US:en LC_ALL=en_US.UTF-8
# Thu, 16 Mar 2023 02:16:33 GMT
RUN apt-get update     && DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends tzdata curl ca-certificates fontconfig locales     && echo "en_US.UTF-8 UTF-8" >> /etc/locale.gen     && locale-gen en_US.UTF-8     && rm -rf /var/lib/apt/lists/*
# Thu, 16 Mar 2023 02:24:03 GMT
ENV JAVA_VERSION=jdk-17.0.6+10_openj9-0.36.0
# Thu, 16 Mar 2023 02:26:13 GMT
RUN set -eux;     ARCH="$(dpkg --print-architecture)";     case "${ARCH}" in        aarch64|arm64)          ESUM='492bd87e39fc0eb78218746e98c4c0f6730af9c998b872c1a175c0e907d11510';          BINARY_URL='https://github.com/ibmruntimes/semeru17-binaries/releases/download/jdk-17.0.6%2B10_openj9-0.36.0/ibm-semeru-open-jre_aarch64_linux_17.0.6_10_openj9-0.36.0.tar.gz';          ;;        ppc64el|ppc64le)          ESUM='f1342b0a8b472d2de6e882030d2797b9c37e1cd7a90e4cb0c3bd969d4cf8158c';          BINARY_URL='https://github.com/ibmruntimes/semeru17-binaries/releases/download/jdk-17.0.6%2B10_openj9-0.36.0/ibm-semeru-open-jre_ppc64le_linux_17.0.6_10_openj9-0.36.0.tar.gz';          ;;        amd64|x86_64)          ESUM='69ca1728f9aad7031908bd9a939b5a9a9c5e931d65bb5c72cbe6f599c7d00cc6';          BINARY_URL='https://github.com/ibmruntimes/semeru17-binaries/releases/download/jdk-17.0.6%2B10_openj9-0.36.0/ibm-semeru-open-jre_x64_linux_17.0.6_10_openj9-0.36.0.tar.gz';          ;;        s390x)          ESUM='542359aebfb91b6605c67db6523b2ce154bda63f7fa8a6c243944b2091f4eb2b';          BINARY_URL='https://github.com/ibmruntimes/semeru17-binaries/releases/download/jdk-17.0.6%2B10_openj9-0.36.0/ibm-semeru-open-jre_s390x_linux_17.0.6_10_openj9-0.36.0.tar.gz';          ;;        *)          echo "Unsupported arch: ${ARCH}";          exit 1;          ;;     esac;     curl -LfsSo /tmp/openjdk.tar.gz ${BINARY_URL};     echo "${ESUM} */tmp/openjdk.tar.gz" | sha256sum -c -;     mkdir -p /opt/java/openjdk;     cd /opt/java/openjdk;     tar -xf /tmp/openjdk.tar.gz --strip-components=1;     rm -rf /tmp/openjdk.tar.gz;
# Thu, 16 Mar 2023 02:26:16 GMT
ENV JAVA_HOME=/opt/java/openjdk PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 16 Mar 2023 02:26:16 GMT
ENV JAVA_TOOL_OPTIONS=-XX:+IgnoreUnrecognizedVMOptions -XX:+PortableSharedCache -XX:+IdleTuningGcOnIdle -Xshareclasses:name=openj9_system_scc,cacheDir=/opt/java/.scc,readonly,nonFatal
# Thu, 16 Mar 2023 02:26:55 GMT
RUN set -eux;     unset OPENJ9_JAVA_OPTIONS;     SCC_SIZE="50m";     DOWNLOAD_PATH_TOMCAT=/tmp/tomcat;     INSTALL_PATH_TOMCAT=/opt/tomcat-home;     TOMCAT_CHECKSUM="0db27185d9fc3174f2c670f814df3dda8a008b89d1a38a5d96cbbe119767ebfb1cf0bce956b27954aee9be19c4a7b91f2579d967932207976322033a86075f98";     TOMCAT_DWNLD_URL="https://archive.apache.org/dist/tomcat/tomcat-9/v9.0.35/bin/apache-tomcat-9.0.35.tar.gz";         mkdir -p "${DOWNLOAD_PATH_TOMCAT}" "${INSTALL_PATH_TOMCAT}";     curl -LfsSo "${DOWNLOAD_PATH_TOMCAT}"/tomcat.tar.gz "${TOMCAT_DWNLD_URL}";     echo "${TOMCAT_CHECKSUM} *${DOWNLOAD_PATH_TOMCAT}/tomcat.tar.gz" | sha512sum -c -;     tar -xf "${DOWNLOAD_PATH_TOMCAT}"/tomcat.tar.gz -C "${INSTALL_PATH_TOMCAT}" --strip-components=1;     rm -rf "${DOWNLOAD_PATH_TOMCAT}";         java -Xshareclasses:name=dry_run_scc,cacheDir=/opt/java/.scc,bootClassesOnly,nonFatal,createLayer -Xscmx$SCC_SIZE -version;     export OPENJ9_JAVA_OPTIONS="-Xshareclasses:name=dry_run_scc,cacheDir=/opt/java/.scc,bootClassesOnly,nonFatal";     "${INSTALL_PATH_TOMCAT}"/bin/startup.sh;     sleep 5;     "${INSTALL_PATH_TOMCAT}"/bin/shutdown.sh -force;     sleep 15;     FULL=$( (java -Xshareclasses:name=dry_run_scc,cacheDir=/opt/java/.scc,printallStats 2>&1 || true) | awk '/^Cache is [0-9.]*% .*full/ {print substr($3, 1, length($3)-1)}');     DST_CACHE=$(java -Xshareclasses:name=dry_run_scc,cacheDir=/opt/java/.scc,destroy 2>&1 || true);     SCC_SIZE=$(echo $SCC_SIZE | sed 's/.$//');     SCC_SIZE=$(awk "BEGIN {print int($SCC_SIZE * $FULL / 100.0)}");     [ "${SCC_SIZE}" -eq 0 ] && SCC_SIZE=1;     SCC_SIZE="${SCC_SIZE}m";     java -Xshareclasses:name=openj9_system_scc,cacheDir=/opt/java/.scc,bootClassesOnly,nonFatal,createLayer -Xscmx$SCC_SIZE -version;     unset OPENJ9_JAVA_OPTIONS;         export OPENJ9_JAVA_OPTIONS="-Xshareclasses:name=openj9_system_scc,cacheDir=/opt/java/.scc,bootClassesOnly,nonFatal";     "${INSTALL_PATH_TOMCAT}"/bin/startup.sh;     sleep 5;     "${INSTALL_PATH_TOMCAT}"/bin/shutdown.sh -force;     sleep 5;     FULL=$( (java -Xshareclasses:name=openj9_system_scc,cacheDir=/opt/java/.scc,printallStats 2>&1 || true) | awk '/^Cache is [0-9.]*% .*full/ {print substr($3, 1, length($3)-1)}');     echo "SCC layer is $FULL% full.";     rm -rf "${INSTALL_PATH_TOMCAT}";     if [ -d "/opt/java/.scc" ]; then           chmod -R 0777 /opt/java/.scc;     fi;         echo "SCC generation phase completed";
# Thu, 16 Mar 2023 19:35:51 GMT
ARG VERBOSE=false
# Thu, 16 Mar 2023 19:35:51 GMT
ARG OPENJ9_SCC=true
# Tue, 11 Apr 2023 22:54:54 GMT
ARG EN_SHA=366618db4b733337adc71ec30b1f33d36cf78a81858636360061036a926f373f
# Tue, 11 Apr 2023 22:54:54 GMT
ARG NON_IBM_SHA=d349f6ea3acd71910348904dd48f81940b86ca5f879737206ae37f858767ad0f
# Tue, 11 Apr 2023 22:54:54 GMT
ARG NOTICES_SHA=e7031658e09e2442279db72eed9238fb30d98c06dabb112fb21b8618b7e810ee
# Tue, 11 Apr 2023 22:54:54 GMT
LABEL org.opencontainers.image.authors=Chris Potter, Christy Jesuraj, Melissa Lee org.opencontainers.image.vendor=IBM org.opencontainers.image.url=http://wasdev.net org.opencontainers.image.documentation=https://www.ibm.com/support/knowledgecenter/SSAW57_liberty/com.ibm.websphere.wlp.nd.multiplatform.doc/ae/cwlp_about.html org.opencontainers.image.version=23.0.0.3 org.opencontainers.image.revision=cl230320230319-1900 org.opencontainers.image.description=This image contains the WebSphere Liberty runtime with IBM Semeru Runtime Open Edition OpenJDK with OpenJ9 and Ubuntu as the base OS.  For more information on this image please see https://github.com/WASdev/ci.docker#building-an-application-image org.opencontainers.image.title=IBM WebSphere Liberty
# Tue, 11 Apr 2023 22:54:54 GMT
ENV LIBERTY_VERSION=23.0.0_03
# Tue, 11 Apr 2023 22:54:54 GMT
ARG LIBERTY_URL
# Tue, 11 Apr 2023 22:54:55 GMT
ARG DOWNLOAD_OPTIONS=
# Tue, 11 Apr 2023 22:55:10 GMT
# ARGS: DOWNLOAD_OPTIONS= EN_SHA=366618db4b733337adc71ec30b1f33d36cf78a81858636360061036a926f373f NON_IBM_SHA=d349f6ea3acd71910348904dd48f81940b86ca5f879737206ae37f858767ad0f NOTICES_SHA=e7031658e09e2442279db72eed9238fb30d98c06dabb112fb21b8618b7e810ee OPENJ9_SCC=true VERBOSE=false
RUN apt-get update     && apt-get install -y --no-install-recommends unzip wget openssl     && rm -rf /var/lib/apt/lists/*     && mkdir -p /licenses/     && useradd -u 1001 -r -g 0 -s /usr/sbin/nologin default     && LIBERTY_URL=${LIBERTY_URL:-$(wget -q -O - https://public.dhe.ibm.com/ibmdl/export/pub/software/websphere/wasdev/downloads/wlp/index.yml  | grep $LIBERTY_VERSION -A 6 | sed -n 's/\s*kernel:\s//p' | tr -d '\r' )}      && wget $DOWNLOAD_OPTIONS $LIBERTY_URL -U UA-IBM-WebSphere-Liberty-Docker -O /tmp/wlp.zip     && unzip -q /tmp/wlp.zip -d /opt/ibm     && rm /tmp/wlp.zip     && chown -R 1001:0 /opt/ibm/wlp     && chmod -R g+rw /opt/ibm/wlp     && LICENSE_BASE=$(wget -q -O - https://public.dhe.ibm.com/ibmdl/export/pub/software/websphere/wasdev/downloads/wlp/index.yml  | grep $LIBERTY_VERSION -A 6 | sed -n 's/\s*license:\s//p' | sed 's/\(.*\)\/.*/\1\//' | tr -d '\r')     && wget ${LICENSE_BASE}en.html -U UA-IBM-WebSphere-Liberty-Docker -O /licenses/en.html     && wget ${LICENSE_BASE}non_ibm_license.html -U UA-IBM-WebSphere-Liberty-Docker -O /licenses/non_ibm_license.html     && wget ${LICENSE_BASE}notices.html -U UA-IBM-WebSphere-Liberty-Docker -O /licenses/notices.html     && echo "$EN_SHA /licenses/en.html" | sha256sum -c --strict --check     && echo "$NON_IBM_SHA /licenses/non_ibm_license.html" | sha256sum -c --strict --check     && echo "$NOTICES_SHA /licenses/notices.html" | sha256sum -c --strict --check     && apt-get purge --auto-remove -y unzip     && apt-get purge --auto-remove -y wget     && rm -rf /var/lib/apt/lists/*
# Tue, 11 Apr 2023 22:55:11 GMT
ENV PATH=/opt/java/openjdk/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/opt/ibm/wlp/bin:/opt/ibm/helpers/build
# Tue, 11 Apr 2023 22:55:11 GMT
LABEL ProductID=fbf6a96d49214c0abc6a3bc5da6e48cd ProductName=WebSphere Application Server Liberty ProductVersion=23.0.0.3 BuildLabel=cl230320230319-1900
# Tue, 11 Apr 2023 22:55:11 GMT
ENV LOG_DIR=/logs WLP_OUTPUT_DIR=/opt/ibm/wlp/output OPENJ9_SCC=true
# Tue, 11 Apr 2023 22:55:12 GMT
# ARGS: DOWNLOAD_OPTIONS= EN_SHA=366618db4b733337adc71ec30b1f33d36cf78a81858636360061036a926f373f NON_IBM_SHA=d349f6ea3acd71910348904dd48f81940b86ca5f879737206ae37f858767ad0f NOTICES_SHA=e7031658e09e2442279db72eed9238fb30d98c06dabb112fb21b8618b7e810ee VERBOSE=false
RUN /opt/ibm/wlp/bin/server create     && rm -rf $WLP_OUTPUT_DIR/.classCache /output/workarea
# Tue, 11 Apr 2023 22:55:12 GMT
COPY dir:0f3e336b1e5adb84a625050153035561e1c9802a57b7b90b5a17ebb82adba489 in /opt/ibm/helpers/ 
# Tue, 11 Apr 2023 22:55:12 GMT
COPY dir:1cf5cc2663c6235241a5228340a9c566587fe27b3e434a313debbf75dacd7a4b in /opt/ibm/fixes/ 
# Tue, 11 Apr 2023 22:55:12 GMT
# ARGS: DOWNLOAD_OPTIONS= EN_SHA=366618db4b733337adc71ec30b1f33d36cf78a81858636360061036a926f373f NON_IBM_SHA=d349f6ea3acd71910348904dd48f81940b86ca5f879737206ae37f858767ad0f NOTICES_SHA=e7031658e09e2442279db72eed9238fb30d98c06dabb112fb21b8618b7e810ee VERBOSE=false
RUN mkdir /logs     && mkdir /etc/wlp     && mkdir -p /opt/ibm/wlp/usr/shared/resources/lib.index.cache     && mkdir -p /home/default     && mkdir /output     && chmod -t /output     && rm -rf /output     && ln -s $WLP_OUTPUT_DIR/defaultServer /output     && ln -s /opt/ibm/wlp/usr/servers/defaultServer /config     && ln -s /opt/ibm /liberty     && ln -s /opt/ibm/wlp/usr/shared/resources/lib.index.cache /lib.index.cache     && mkdir -p /config/configDropins/defaults     && mkdir -p /config/configDropins/overrides     && chown -R 1001:0 /config     && chmod -R g+rw /config     && chown -R 1001:0 /opt/ibm/helpers     && chmod -R g+rwx /opt/ibm/helpers     && chown -R 1001:0 /opt/ibm/fixes     && chmod -R g+rwx /opt/ibm/fixes     && chown -R 1001:0 /opt/ibm/wlp/usr     && chmod -R g+rw /opt/ibm/wlp/usr     && chown -R 1001:0 /opt/ibm/wlp/output     && chmod -R g+rw /opt/ibm/wlp/output     && chown -R 1001:0 /logs     && chmod -R g+rw /logs     && chown -R 1001:0 /etc/wlp     && chmod -R g+rw /etc/wlp     && chown -R 1001:0 /home/default     && chmod -R g+rw /home/default
# Tue, 11 Apr 2023 22:55:16 GMT
# ARGS: DOWNLOAD_OPTIONS= EN_SHA=366618db4b733337adc71ec30b1f33d36cf78a81858636360061036a926f373f NON_IBM_SHA=d349f6ea3acd71910348904dd48f81940b86ca5f879737206ae37f858767ad0f NOTICES_SHA=e7031658e09e2442279db72eed9238fb30d98c06dabb112fb21b8618b7e810ee VERBOSE=false
RUN if [ "$OPENJ9_SCC" = "true" ]; then populate_scc.sh; fi     && rm -rf /output/messaging /output/resources/security /logs/* $WLP_OUTPUT_DIR/.classCache     && chown -R 1001:0 /opt/ibm/wlp/output     && chmod -R g+rwx /opt/ibm/wlp/output
# Tue, 11 Apr 2023 22:55:17 GMT
ENV RANDFILE=/tmp/.rnd OPENJ9_JAVA_OPTIONS=-XX:+IgnoreUnrecognizedVMOptions -XX:+IdleTuningGcOnIdle -Xshareclasses:name=openj9_system_scc,cacheDir=/opt/java/.scc,readonly,nonFatal -Dosgi.checkConfiguration=false
# Tue, 11 Apr 2023 22:55:17 GMT
USER 1001
# Tue, 11 Apr 2023 22:55:17 GMT
EXPOSE 9080 9443
# Tue, 11 Apr 2023 22:55:17 GMT
ENTRYPOINT ["/opt/ibm/helpers/runtime/docker-server.sh"]
# Tue, 11 Apr 2023 22:55:17 GMT
CMD ["/opt/ibm/wlp/bin/server" "run" "defaultServer"]
# Tue, 11 Apr 2023 23:25:53 GMT
ARG VERBOSE=false
# Tue, 11 Apr 2023 23:25:54 GMT
ARG REPOSITORIES_PROPERTIES=
# Tue, 11 Apr 2023 23:36:18 GMT
# ARGS: REPOSITORIES_PROPERTIES= VERBOSE=false
RUN if [ ! -z $REPOSITORIES_PROPERTIES ]; then mkdir /opt/ibm/wlp/etc/   && echo $REPOSITORIES_PROPERTIES > /opt/ibm/wlp/etc/repositories.properties; fi   && installUtility install --acceptLicense baseBundle   && if [ ! -z $REPOSITORIES_PROPERTIES ]; then rm /opt/ibm/wlp/etc/repositories.properties; fi   && rm -rf /output/workarea /output/logs   && find /opt/ibm/wlp ! -perm -g=rw -print0 | xargs -r -0 chmod g+rw
# Tue, 11 Apr 2023 23:36:25 GMT
COPY --chown=1001:0file:f212cc38605f508baa0f75a07632700533ad28792dd9761a792209e709b00f23 in /config/ 
# Tue, 11 Apr 2023 23:36:50 GMT
# ARGS: REPOSITORIES_PROPERTIES= VERBOSE=false
RUN if [ "$OPENJ9_SCC" = "true" ]; then populate_scc.sh; fi     && rm -rf /output/messaging /output/resources/security /logs/* $WLP_OUTPUT_DIR/.classCache     && find /opt/ibm/wlp/output ! -perm -g=rwx -print0 | xargs -0 -r chmod g+rwx
```

-	Layers:
	-	`sha256:422c367cdac1ee2f6bd9ea546c8e5a643af0847a822d04ba202af409973273ad`  
		Last Modified: Thu, 16 Mar 2023 01:40:19 GMT  
		Size: 27.0 MB (27016120 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:56386641fb30606093401c5d6c9ba0f0a777400ddc5894b90d60fc8ac2e6ebf1`  
		Last Modified: Thu, 16 Mar 2023 02:33:20 GMT  
		Size: 15.7 MB (15688892 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:af777ee93c03b4bb0a7b17a7b3e4dafa480fa1bd93177ad2bd62fda54c3aa08b`  
		Last Modified: Thu, 16 Mar 2023 02:36:13 GMT  
		Size: 47.3 MB (47259355 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:120be55e583f77e4b939ce30ad129133e60848f31c50f943da04bc3c554d19c0`  
		Last Modified: Thu, 16 Mar 2023 02:36:07 GMT  
		Size: 4.9 MB (4869052 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4d567210b70d0518fc70b359038d9afdad41580dc434d415a352b19cf7ca8022`  
		Last Modified: Tue, 11 Apr 2023 23:38:32 GMT  
		Size: 14.5 MB (14452611 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:728df2be40ef844f8d5349f11cc327bc020a6a9d52a454da2862ea4ba035ef74`  
		Last Modified: Tue, 11 Apr 2023 23:38:29 GMT  
		Size: 677.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:77af7fdcc6b2cb1d56bb91479dc444d59c1c6fa485cdaac9a377aee0642ae29d`  
		Last Modified: Tue, 11 Apr 2023 23:38:29 GMT  
		Size: 9.8 KB (9812 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:abb6f5fde2a2d2443ed4c81fb938aee2c9339c50f4173d6d3975f60b92d8cb9c`  
		Last Modified: Tue, 11 Apr 2023 23:38:29 GMT  
		Size: 272.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:977891bbc4b9169668fd5b227381f9d2859ede9a56d37b9a512c010d1b554a2f`  
		Last Modified: Tue, 11 Apr 2023 23:38:29 GMT  
		Size: 10.8 KB (10795 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ab9d28529bb3c8579f146b2232b73953f030164ed4a2a0900740982ecc7b88d9`  
		Last Modified: Tue, 11 Apr 2023 23:38:30 GMT  
		Size: 2.6 MB (2612563 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bb7bfc62477ea93ef48dfcc6addf532475184359884fbcd61d92102af83f23df`  
		Last Modified: Tue, 11 Apr 2023 23:39:36 GMT  
		Size: 359.0 MB (359033702 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:33fc31e89f453508e964711a32aa1b5a0ab483db52d8dede2c156cc22c35398c`  
		Last Modified: Tue, 11 Apr 2023 23:39:20 GMT  
		Size: 947.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1b881614860d0a73de5644a2f857c78c4cd8c99a3fca9dcbcb1f94d7b7b79040`  
		Last Modified: Tue, 11 Apr 2023 23:39:22 GMT  
		Size: 15.5 MB (15477352 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
